# Comparing `tmp/chempy-0.8.3.tar.gz` & `tmp/chempy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chempy-0.8.3.tar", last modified: Sun Jul 16 10:14:30 2023, max compression
+gzip compressed data, was "chempy-0.9.0.tar", last modified: Wed Apr 24 16:24:28 2024, max compression
```

## Comparing `chempy-0.8.3.tar` & `chempy-0.9.0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.113779 chempy-0.8.3/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       38 2020-12-30 14:27:24.000000 chempy-0.8.3/AUTHORS
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7814 2023-07-16 09:59:36.000000 chempy-0.8.3/CHANGES.rst
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1303 2020-12-30 14:27:24.000000 chempy-0.8.3/LICENSE
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       71 2020-12-30 14:27:24.000000 chempy-0.8.3/MANIFEST.in
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18489 2023-07-16 10:14:30.113779 chempy-0.8.3/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    17504 2023-07-16 09:59:31.000000 chempy-0.8.3/README.rst
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.037778 chempy-0.8.3/chempy/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      709 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9477 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/_eqsys.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2475 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/_equilibrium.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       22 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy/_release.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5990 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       45 2020-12-30 14:27:24.000000 chempy-0.8.3/chempy/_url.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2437 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/_util.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      321 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    53293 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/chemistry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      386 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/debye_huckel.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1091 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/einstein_smoluchowski.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.041778 chempy-0.8.3/chempy/electrochemistry/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       24 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1379 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/nernst.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.041778 chempy-0.8.3/chempy/electrochemistry/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/electrochemistry/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1068 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/electrochemistry/tests/test_nernst.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7778 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/electrolytes.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    16931 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/equilibria.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      258 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3595 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/henry.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.049778 chempy-0.8.3/chempy/kinetics/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      199 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6516 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/_native.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      710 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/_rates.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4942 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/analysis.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8362 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5966 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/kinetics/eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     7550 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/integrated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    28053 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/kinetics/ode.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11341 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/rates.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.053778 chempy-0.8.3/chempy/kinetics/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/kinetics/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     9361 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test__native.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10553 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/kinetics/tests/test__rates.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1612 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_arrhenius.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1007 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_eyring.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1549 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_integrated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    41283 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/kinetics/tests/test_ode.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15162 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/kinetics/tests/test_rates.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.061778 chempy-0.8.3/chempy/printing/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      325 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3895 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/printing/js.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6194 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/numbers.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      807 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/pretty.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2350 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/printing/printer.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3283 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/printing/string.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1272 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4306 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/printing/tables.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.065778 chempy-0.8.3/chempy/printing/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/printing/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2198 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_numbers.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      432 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_str.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      610 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tests/test_table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      630 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/tex.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2714 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/printing/web.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.069778 chempy-0.8.3/chempy/properties/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      145 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1551 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/debye_huckel_radii.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3204 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/gas_sol_electrolytes_schumpe_1993.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5576 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/sulfuric_acid_density_myhre_1998.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.073778 chempy-0.8.3/chempy/properties/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/properties/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      403 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_gas_sol_electrolytes_schumpe_1993.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      835 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1349 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_density_tanaka_2001.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1297 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_diffusivity_holz_2000.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      946 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1471 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/tests/test_water_viscosity_korson_1969.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2804 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/water_density_tanaka_2001.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2775 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/properties/water_diffusivity_holz_2000.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3096 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/water_permittivity_bradley_pitzer_1979.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1566 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/properties/water_viscosity_korson_1969.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    31994 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/reactionsystem.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      472 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/symbolic.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.085778 chempy-0.8.3/chempy/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2487 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/ammonical_cupric_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1570 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test__equilibrium.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20777 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/tests/test_chemistry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       84 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_core.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1294 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_einstein_smoluchowski.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1531 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_electrolytes.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4491 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/tests/test_equilibria.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1206 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_henry.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15621 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_reactionsystem.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2018 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_solution.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    15995 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/tests/test_units.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      430 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/tests/test_util.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.089778 chempy-0.8.3/chempy/thermodynamics/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)       77 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/thermodynamics/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1814 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/thermodynamics/expressions.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.089778 chempy-0.8.3/chempy/thermodynamics/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/thermodynamics/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3438 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/thermodynamics/tests/test_expressions.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    22736 2023-07-16 09:59:31.000000 chempy-0.8.3/chempy/units.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.101779 chempy-0.8.3/chempy/util/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      147 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2233 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/_aqueous.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      795 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/_dimensionality.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    25887 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_expr.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4153 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_expr_deprecated.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5910 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_julia.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2295 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/_quantities.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4652 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/arithmeticdict.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6776 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/bkh.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4940 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/deprecation.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     5114 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/graph.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1062 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/numutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20195 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/parsing.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     6753 2021-10-29 07:48:12.000000 chempy-0.8.3/chempy/util/periodic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     8881 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/pyutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    11947 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/regression.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      890 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/rendering.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2792 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/stoich.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    10550 2023-07-16 08:39:56.000000 chempy-0.8.3/chempy/util/table.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4079 2021-09-18 21:19:30.000000 chempy-0.8.3/chempy/util/terminal.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2015 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/testing.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.109779 chempy-0.8.3/chempy/util/tests/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        0 2020-11-23 23:38:22.000000 chempy-0.8.3/chempy/util/tests/__init__.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     4058 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_arithmeticdict.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18801 2021-10-29 07:48:12.000000 chempy-0.8.3/chempy/util/tests/test_expr.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1631 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_graph.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      462 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_numutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    20501 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/util/tests/test_parsing.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2250 2022-03-29 16:41:58.000000 chempy-0.8.3/chempy/util/tests/test_periodic.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1850 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_pyutil.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      783 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_regression.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      726 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_rendering.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     2987 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_stoich.py
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     1459 2021-09-18 15:16:38.000000 chempy-0.8.3/chempy/util/tests/test_table.py
-drwxrwxr-x   0 bjorn     (1000) bjorn     (1000)        0 2023-07-16 10:14:30.037778 chempy-0.8.3/chempy.egg-info/
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)    18489 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/PKG-INFO
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)     3961 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/SOURCES.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        1 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/dependency_links.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      703 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/requires.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)        7 2023-07-16 10:14:29.000000 chempy-0.8.3/chempy.egg-info/top_level.txt
--rw-rw-r--   0 bjorn     (1000) bjorn     (1000)      884 2023-07-16 10:14:30.113779 chempy-0.8.3/setup.cfg
--rwxrwxr-x   0 bjorn     (1000) bjorn     (1000)     4994 2023-07-16 08:39:56.000000 chempy-0.8.3/setup.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.333497 chempy-0.9.0/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       38 2024-03-29 20:38:25.000000 chempy-0.9.0/AUTHORS
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     8307 2024-04-23 12:29:23.000000 chempy-0.9.0/CHANGES.rst
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1303 2024-03-29 20:38:25.000000 chempy-0.9.0/LICENSE
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       71 2024-03-29 20:38:25.000000 chempy-0.9.0/MANIFEST.in
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    18111 2024-04-24 16:24:28.333497 chempy-0.9.0/PKG-INFO
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    17146 2024-04-24 16:24:07.000000 chempy-0.9.0/README.rst
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      709 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     9477 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/_eqsys.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2475 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/_equilibrium.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       22 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy/_release.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     5990 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/_solution.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       45 2024-03-29 20:38:25.000000 chempy-0.9.0/chempy/_url.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2437 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/_util.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      321 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/arrhenius.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    53655 2024-04-23 12:29:23.000000 chempy-0.9.0/chempy/chemistry.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      386 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/debye_huckel.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1091 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/einstein_smoluchowski.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/electrochemistry/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       24 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/electrochemistry/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1379 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/electrochemistry/nernst.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/electrochemistry/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/electrochemistry/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1068 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/electrochemistry/tests/test_nernst.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     7778 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/electrolytes.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    16931 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/equilibria.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      258 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/eyring.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3595 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/henry.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/kinetics/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      199 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     6516 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/_native.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      710 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/_rates.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4942 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/analysis.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     8362 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/arrhenius.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     5966 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/eyring.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     7550 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/integrated.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    28053 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/ode.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    11341 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/rates.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/kinetics/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/kinetics/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     9361 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test__native.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    10553 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test__rates.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1612 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test_arrhenius.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1007 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test_eyring.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1549 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test_integrated.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    41283 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test_ode.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    15162 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/kinetics/tests/test_rates.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/printing/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      325 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3895 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/js.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     6194 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/numbers.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      807 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/pretty.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2350 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/printer.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3283 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/string.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1272 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/table.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4306 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/tables.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy/printing/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/printing/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2198 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/tests/test_numbers.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      432 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/tests/test_str.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      610 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/tests/test_table.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      630 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/tex.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2714 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/printing/web.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/properties/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      145 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1551 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/debye_huckel_radii.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3204 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/gas_sol_electrolytes_schumpe_1993.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     5576 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/sulfuric_acid_density_myhre_1998.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/properties/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/properties/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      403 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_gas_sol_electrolytes_schumpe_1993.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      835 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1349 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_water_density_tanaka_2001.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1297 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_water_diffusivity_holz_2000.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      946 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1471 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/tests/test_water_viscosity_korson_1969.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2804 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/water_density_tanaka_2001.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2775 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/water_diffusivity_holz_2000.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3096 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/water_permittivity_bradley_pitzer_1979.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1566 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/properties/water_viscosity_korson_1969.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    31994 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/reactionsystem.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      472 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/symbolic.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2487 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/ammonical_cupric_solution.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1570 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test__equilibrium.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    21772 2024-04-23 12:29:23.000000 chempy-0.9.0/chempy/tests/test_chemistry.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       84 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_core.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1294 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_einstein_smoluchowski.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1531 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_electrolytes.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4491 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_equilibria.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1206 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_henry.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    15621 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_reactionsystem.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2018 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_solution.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    15995 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_units.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      430 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/tests/test_util.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/thermodynamics/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)       77 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/thermodynamics/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1814 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/thermodynamics/expressions.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/thermodynamics/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/thermodynamics/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3438 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/thermodynamics/tests/test_expressions.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    22736 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/units.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.329497 chempy-0.9.0/chempy/util/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      147 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2233 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_aqueous.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      795 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_dimensionality.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    25887 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_expr.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4153 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_expr_deprecated.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     5910 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_julia.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2295 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/_quantities.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4652 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/arithmeticdict.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     6776 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/bkh.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4940 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/deprecation.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     5114 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/graph.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1062 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/numutil.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    20504 2024-04-23 11:20:25.000000 chempy-0.9.0/chempy/util/parsing.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     6753 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/periodic.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     8881 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/pyutil.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    11947 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/regression.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      890 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/rendering.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2792 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/stoich.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    10550 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/table.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4079 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/terminal.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2015 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/testing.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.333497 chempy-0.9.0/chempy/util/tests/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        0 2023-05-06 19:27:27.000000 chempy-0.9.0/chempy/util/tests/__init__.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     4058 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_arithmeticdict.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    18801 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_expr.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1641 2024-04-24 16:24:07.000000 chempy-0.9.0/chempy/util/tests/test_graph.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      462 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_numutil.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    22117 2024-04-23 11:20:25.000000 chempy-0.9.0/chempy/util/tests/test_parsing.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2250 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_periodic.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1850 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_pyutil.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      783 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_regression.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      726 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_rendering.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     2987 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_stoich.py
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     1459 2024-04-22 06:07:55.000000 chempy-0.9.0/chempy/util/tests/test_table.py
+drwxr-xr-x   0 bjorn     (1000) bjorn     (1000)        0 2024-04-24 16:24:28.325497 chempy-0.9.0/chempy.egg-info/
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)    18111 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy.egg-info/PKG-INFO
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)     3961 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy.egg-info/SOURCES.txt
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        1 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy.egg-info/dependency_links.txt
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      703 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy.egg-info/requires.txt
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)        7 2024-04-24 16:24:28.000000 chempy-0.9.0/chempy.egg-info/top_level.txt
+-rw-r--r--   0 bjorn     (1000) bjorn     (1000)      910 2024-04-24 16:24:28.333497 chempy-0.9.0/setup.cfg
+-rwxr-xr-x   0 bjorn     (1000) bjorn     (1000)     4994 2024-04-24 16:24:07.000000 chempy-0.9.0/setup.py
```

### Comparing `chempy-0.8.3/CHANGES.rst` & `chempy-0.9.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v0.9.0
+======
+- Fractional stoichiometries are now officially supported in parser (e.g. Fe2O3.14)
+- Complexes/crystal water should now be delimited with '..' (fix by @jeremyagray)
+- Unicode printing of subscript decimal point should now work (gh-223, fix by @jeremyagray)
+- Substance class now has a __hash__ function (fix by @DNIIBOY)
+- Unit per100eV now has correct repr (fix by @daankoning)
+- Passing results from balance_stoichiometry into Reaction now works (gh-218, thanks @montmorill)
+
 v0.8.3
 ======
 - Fixes for latest version of quantities.
 - Build python wheel as part of release script.
 
 v0.8.2
 ======
```

### Comparing `chempy-0.8.3/LICENSE` & `chempy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/PKG-INFO` & `chempy-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: chempy
-Version: 0.8.3
+Version: 0.9.0
 Summary: ChemPy is a Python package useful for solving problems in chemistry.
 Home-page: https://github.com/bjodah/chempy
 Author: Bjoern I. Dahlgren
 Author-email: bjodah@gmail.com
 License: BSD
 Keywords: chemistry,water properties,physical chemistry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -29,21 +28,21 @@
 License-File: AUTHORS
 
 ChemPy
 ======
 
 .. image:: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml/badge.svg
    :target: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml
-   :alt: Build status
+   :alt: Github Actions CI status
+.. image:: https://hackspett.bjodah.se/api/badges/1/status.svg
+   :target: https://hackspett.bjodah.se/repos/1
+   :alt: Woodpecker CI status
 .. image:: https://img.shields.io/pypi/v/chempy.svg
    :target: https://pypi.python.org/pypi/chempy
    :alt: PyPI version
-.. image:: https://img.shields.io/badge/python-3.8,3.9-blue.svg
-   :target: https://www.python.org/
-   :alt: Python version
 .. image:: https://img.shields.io/pypi/l/chempy.svg
    :target: https://github.com/bjodah/chempy/blob/master/LICENSE
    :alt: License
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
@@ -133,21 +132,21 @@
 `Dockerfile <scripts/environment/Dockerfile>`_.
 
 Using Docker
 ~~~~~~~~~~~~
 If you have `Docker <https://www.docker.com>`_ installed, you may use it to host a jupyter
 notebook server::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 8888
+  $ ./scripts/host-env.sh host-notebook --port 8888
 
 the first time you run the command, some dependencies will be downloaded. When the installation
 is complete there will be a link visible which you can open in your browser. You can also run
 the test suite using the same docker-image::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 0
+  $ ./scripts/host-env.sh run-tests
 
 there will be a few skipped test (due to some dependencies not being installed by default) and
 quite a few warnings.
 
 
 Examples
 --------
@@ -400,36 +399,26 @@
    ...     print('[H2O] = %.2f M (at %d °C)' % (to_unitless(concentration_H2O, u.molar), T_C))
    ...
    [H2O] = 55.46 M (at 15 °C)
    [H2O] = 55.35 M (at 25 °C)
    [H2O] = 55.18 M (at 35 °C)
 
 
-Run notebooks using binder
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-Using only a web-browser (and an internet connection) it is possible to explore the
-notebooks here: (by the courtesy of the people behind mybinder)
-
-.. image:: http://mybinder.org/badge.svg
-   :target: https://mybinder.org/v2/gh/bjodah/chempy/f5f2546e79e165ba8fb258fc87d83a7fbdcbad64?filepath=index.ipynb
-   :alt: Binder
-
-
 Citing
 ------
 If you make use of ChemPy in e.g. academic work you may cite the following peer-reviewed publication:
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
 Depending on what underlying solver you are using you should also cite the appropriate paper
 (you can look at the list of references in the JOSS article). If you need to reference,
 in addition to the paper, a specific point version of ChemPy (for e.g. reproducibility)
-you can get per-version DOIs from the zendodo archive:
+you can get per-version DOIs from the zenodo archive:
 
 .. image:: https://zenodo.org/badge/8840/bjodah/chempy.svg
    :target: https://zenodo.org/badge/latestdoi/8840/bjodah/chempy
    :alt: Zenodo DOI
 
 Licensing
 ---------
@@ -450,9 +439,7 @@
 (see further details `here <CONTRIBUTING.rst>`_).
 
 
 Author
 ------
 Björn I. Dahlgren, contact:
  - gmail address: bjodah
-
-
```

### Comparing `chempy-0.8.3/README.rst` & `chempy-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ChemPy
 ======
 
 .. image:: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml/badge.svg
    :target: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml
-   :alt: Build status
+   :alt: Github Actions CI status
+.. image:: https://hackspett.bjodah.se/api/badges/1/status.svg
+   :target: https://hackspett.bjodah.se/repos/1
+   :alt: Woodpecker CI status
 .. image:: https://img.shields.io/pypi/v/chempy.svg
    :target: https://pypi.python.org/pypi/chempy
    :alt: PyPI version
-.. image:: https://img.shields.io/badge/python-3.8,3.9-blue.svg
-   :target: https://www.python.org/
-   :alt: Python version
 .. image:: https://img.shields.io/pypi/l/chempy.svg
    :target: https://github.com/bjodah/chempy/blob/master/LICENSE
    :alt: License
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
@@ -103,21 +103,21 @@
 `Dockerfile <scripts/environment/Dockerfile>`_.
 
 Using Docker
 ~~~~~~~~~~~~
 If you have `Docker <https://www.docker.com>`_ installed, you may use it to host a jupyter
 notebook server::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 8888
+  $ ./scripts/host-env.sh host-notebook --port 8888
 
 the first time you run the command, some dependencies will be downloaded. When the installation
 is complete there will be a link visible which you can open in your browser. You can also run
 the test suite using the same docker-image::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 0
+  $ ./scripts/host-env.sh run-tests
 
 there will be a few skipped test (due to some dependencies not being installed by default) and
 quite a few warnings.
 
 
 Examples
 --------
@@ -370,36 +370,26 @@
    ...     print('[H2O] = %.2f M (at %d °C)' % (to_unitless(concentration_H2O, u.molar), T_C))
    ...
    [H2O] = 55.46 M (at 15 °C)
    [H2O] = 55.35 M (at 25 °C)
    [H2O] = 55.18 M (at 35 °C)
 
 
-Run notebooks using binder
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-Using only a web-browser (and an internet connection) it is possible to explore the
-notebooks here: (by the courtesy of the people behind mybinder)
-
-.. image:: http://mybinder.org/badge.svg
-   :target: https://mybinder.org/v2/gh/bjodah/chempy/f5f2546e79e165ba8fb258fc87d83a7fbdcbad64?filepath=index.ipynb
-   :alt: Binder
-
-
 Citing
 ------
 If you make use of ChemPy in e.g. academic work you may cite the following peer-reviewed publication:
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
 Depending on what underlying solver you are using you should also cite the appropriate paper
 (you can look at the list of references in the JOSS article). If you need to reference,
 in addition to the paper, a specific point version of ChemPy (for e.g. reproducibility)
-you can get per-version DOIs from the zendodo archive:
+you can get per-version DOIs from the zenodo archive:
 
 .. image:: https://zenodo.org/badge/8840/bjodah/chempy.svg
    :target: https://zenodo.org/badge/latestdoi/8840/bjodah/chempy
    :alt: Zenodo DOI
 
 Licensing
 ---------
```

### Comparing `chempy-0.8.3/chempy/__init__.py` & `chempy-0.9.0/chempy/__init__.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/_eqsys.py` & `chempy-0.9.0/chempy/_eqsys.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/_equilibrium.py` & `chempy-0.9.0/chempy/_equilibrium.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/_solution.py` & `chempy-0.9.0/chempy/_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/_util.py` & `chempy-0.9.0/chempy/_util.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/chemistry.py` & `chempy-0.9.0/chempy/chemistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,24 @@
 
     def __eq__(self, other):
         for attr in self.attrs:
             if getattr(self, attr) != getattr(other, attr):
                 return False
         return True
 
+    def __hash__(self) -> int:
+        hashed_values = []
+        for key in self.attrs:
+            value = getattr(self, key)
+            if isinstance(value, dict):
+                hashed_values.append(hash(tuple(sorted(value.items()))))
+            else:
+                hashed_values.append(hash(value))
+        return sum(hashed_values)
+
     @property
     def charge(self):
         """Convenience property for accessing ``composition[0]``"""
         return self.composition.get(0, 0)  # electron (net) deficiency
 
     @property
     def mass(self):
@@ -442,17 +452,16 @@
     default_checks = {"any_effect", "all_positive", "all_integral", "consistent_units"}
 
     @staticmethod
     def _init_stoich(container):
         if isinstance(container, set):
             container = {k: 1 for k in container}
         container = container or {}
-        if (
-            type(container) == dict
-        ):  # we don't want isinstance here in case of OrderedDict
+        if type(container) == dict:  # noqa
+            # we don't want isinstance here in case of OrderedDict
             container = OrderedDict(sorted(container.items(), key=lambda kv: kv[0]))
         return container
 
     def __init__(
         self,
         reac,
         prod,
@@ -570,15 +579,15 @@
     def check_all_integral(self, throw=False):
         """Checks if all stoichiometric coefficients are integers"""
         for nam, cont in [
             (nam, getattr(self, nam))
             for nam in "reac prod inact_reac inact_prod".split()
         ]:
             for k, v in cont.items():
-                if v != type(v)(int(v)):
+                if v != int(v) and v != type(v)(int(v)):
                     if throw:
                         raise ValueError(
                             "Found a non-integer stoichiometric coefficient for %s in %s."
                             % (k, nam)
                         )
                     else:
                         return False
@@ -1442,19 +1451,18 @@
         substances = OrderedDict(
             [(k, substance_factory(k)) for k in chain(reactants, products)]
         )
     if isinstance(substances, str):
         substances = OrderedDict(
             [(k, substance_factory(k)) for k in substances.split()]
         )
-    if (
-        type(reactants) == set
-    ):  # we don't want isinstance since it might be "OrderedSet"
+    if type(reactants) == set:  # noqa
+        # we don't want isinstance since it might be "OrderedSet"
         reactants = sorted(reactants)
-    if type(products) == set:
+    if type(products) == set:  # noqa
         products = sorted(products)
     subst_keys = list(reactants) + list(products)
 
     cks = Substance.composition_keys(substances.values())
 
     if parametric_symbols is None:
         parametric_symbols = numbered_symbols("x", start=1, integer=True, positive=True)
```

### Comparing `chempy-0.8.3/chempy/einstein_smoluchowski.py` & `chempy-0.9.0/chempy/einstein_smoluchowski.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/electrochemistry/nernst.py` & `chempy-0.9.0/chempy/electrochemistry/nernst.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/electrochemistry/tests/test_nernst.py` & `chempy-0.9.0/chempy/electrochemistry/tests/test_nernst.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/electrolytes.py` & `chempy-0.9.0/chempy/electrolytes.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/equilibria.py` & `chempy-0.9.0/chempy/equilibria.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/henry.py` & `chempy-0.9.0/chempy/henry.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/_native.py` & `chempy-0.9.0/chempy/kinetics/_native.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/_rates.py` & `chempy-0.9.0/chempy/kinetics/_rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/analysis.py` & `chempy-0.9.0/chempy/kinetics/analysis.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/arrhenius.py` & `chempy-0.9.0/chempy/kinetics/arrhenius.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/eyring.py` & `chempy-0.9.0/chempy/kinetics/eyring.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/integrated.py` & `chempy-0.9.0/chempy/kinetics/integrated.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/ode.py` & `chempy-0.9.0/chempy/kinetics/ode.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/rates.py` & `chempy-0.9.0/chempy/kinetics/rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test__native.py` & `chempy-0.9.0/chempy/kinetics/tests/test__native.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test__rates.py` & `chempy-0.9.0/chempy/kinetics/tests/test__rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test_arrhenius.py` & `chempy-0.9.0/chempy/kinetics/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test_eyring.py` & `chempy-0.9.0/chempy/kinetics/tests/test_eyring.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test_integrated.py` & `chempy-0.9.0/chempy/kinetics/tests/test_integrated.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test_ode.py` & `chempy-0.9.0/chempy/kinetics/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/kinetics/tests/test_rates.py` & `chempy-0.9.0/chempy/kinetics/tests/test_rates.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/js.py` & `chempy-0.9.0/chempy/printing/js.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/numbers.py` & `chempy-0.9.0/chempy/printing/numbers.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/pretty.py` & `chempy-0.9.0/chempy/printing/pretty.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/printer.py` & `chempy-0.9.0/chempy/printing/printer.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/string.py` & `chempy-0.9.0/chempy/printing/string.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/table.py` & `chempy-0.9.0/chempy/printing/table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/tables.py` & `chempy-0.9.0/chempy/printing/tables.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/tests/test_numbers.py` & `chempy-0.9.0/chempy/printing/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/tests/test_table.py` & `chempy-0.9.0/chempy/printing/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/tex.py` & `chempy-0.9.0/chempy/printing/tex.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/printing/web.py` & `chempy-0.9.0/chempy/printing/web.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/debye_huckel_radii.py` & `chempy-0.9.0/chempy/properties/debye_huckel_radii.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/gas_sol_electrolytes_schumpe_1993.py` & `chempy-0.9.0/chempy/properties/gas_sol_electrolytes_schumpe_1993.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/sulfuric_acid_density_myhre_1998.py` & `chempy-0.9.0/chempy/properties/sulfuric_acid_density_myhre_1998.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py` & `chempy-0.9.0/chempy/properties/tests/test_sulfuric_acid_density_myhre_1998.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/tests/test_water_density_tanaka_2001.py` & `chempy-0.9.0/chempy/properties/tests/test_water_density_tanaka_2001.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/tests/test_water_diffusivity_holz_2000.py` & `chempy-0.9.0/chempy/properties/tests/test_water_diffusivity_holz_2000.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py` & `chempy-0.9.0/chempy/properties/tests/test_water_permittivity_bradley_pitzer_1979.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/tests/test_water_viscosity_korson_1969.py` & `chempy-0.9.0/chempy/properties/tests/test_water_viscosity_korson_1969.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/water_density_tanaka_2001.py` & `chempy-0.9.0/chempy/properties/water_density_tanaka_2001.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/water_diffusivity_holz_2000.py` & `chempy-0.9.0/chempy/properties/water_diffusivity_holz_2000.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/water_permittivity_bradley_pitzer_1979.py` & `chempy-0.9.0/chempy/properties/water_permittivity_bradley_pitzer_1979.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/properties/water_viscosity_korson_1969.py` & `chempy-0.9.0/chempy/properties/water_viscosity_korson_1969.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/reactionsystem.py` & `chempy-0.9.0/chempy/reactionsystem.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/ammonical_cupric_solution.py` & `chempy-0.9.0/chempy/tests/ammonical_cupric_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test__equilibrium.py` & `chempy-0.9.0/chempy/tests/test__equilibrium.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_chemistry.py` & `chempy-0.9.0/chempy/tests/test_chemistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 @requires(parsing_library)
 def test_Substance():
     s = Substance.from_formula("H+")
     assert s.composition == {0: 1, 1: 1}
     assert s.charge == 1
     assert abs(s.mass - 1.008) < 1e-3
+    assert s in {s: 1}
+    assert hash(s) != hash(Substance.from_formula("He"))
 
 
 def test_Substance__2():
     H2O = Substance(
         name="H2O", charge=0, latex_name=r"\mathrm{H_{2}O}", data={"pKa": 14}
     )  # will_be_missing_in='0.8.0', use data=...
     OH_m = Substance(name="OH-", charge=-1, latex_name=r"\mathrm{OH^{-}}")
@@ -202,14 +204,54 @@
 
     Reaction.from_string("H+ + OH- -> H2O; 1e10/M/s", "H2O H+ OH-".split())
     with pytest.raises(ValueError):
         Reaction.from_string("H2O -> H+ + OH-; 1e-4/M/s", "H2O H+ OH-".split())
 
 
 @requires(parsing_library, units_library)
+def test_Reaction__check_integral():
+
+    Reaction(*balance_stoichiometry({"H2", "O2"}, {"H2O"}))
+
+    class MyInt:
+        def __init__(self, __data):
+            self.__data = __data
+
+        def __eq__(self, other):
+            return self.__data == other
+
+        def __lt__(self, other):
+            return self.__data < other
+
+        def __int__(self):
+            return self.__data
+
+        def __rsub__(self, other):
+            return other - self.__data
+
+    class MyOne:
+        def __eq__(self, other):
+            return 1 == other
+
+        def __lt__(self, other):
+            return 1 < other
+
+        def __int__(self):
+            return 1
+
+        def __rsub__(self, other):
+            return other - 1
+
+    Reaction({"H2": MyInt(2), "O2": MyOne()}, {"H2O": 2})
+
+    with pytest.raises(ValueError):
+        Reaction({"H2": 1, "O2": 0.5}, {"H2O": 1})
+
+
+@requires(parsing_library, units_library)
 def test_Substance__molar_mass():
     mw_water = Substance.from_formula("H2O").molar_mass(default_units)
     q = mw_water / ((15.9994 + 2 * 1.008) * default_units.gram / default_units.mol)
     assert abs(q - 1) < 1e-3
 
 
 @requires(units_library)
@@ -221,15 +263,15 @@
     rate = 1.31e11 / M / s
     fw, bw = eq.as_reactions(kb=rate, units=default_units)
     assert abs((bw.param - rate) / rate) < 1e-15
     assert abs((fw.param / M) / bw.param - 1e-14) / 1e-14 < 1e-15
 
 
 @requires(parsing_library)
-def test_ReactioN__latex():
+def test_Reaction__latex():
     keys = "H2O H2 O2".split()
     subst = {k: Substance.from_formula(k) for k in keys}
     r2 = Reaction.from_string("2 H2O -> 2 H2 + O2", subst)
     assert r2.latex(subst) == r"2 H_{2}O \rightarrow 2 H_{2} + O_{2}"
     r3 = Reaction.from_string("2 H2O -> 2 H2 + O2; 42; name='split'", subst)
     assert (
         r3.latex(subst, with_param=True, with_name=True)
```

### Comparing `chempy-0.8.3/chempy/tests/test_einstein_smoluchowski.py` & `chempy-0.9.0/chempy/tests/test_einstein_smoluchowski.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_electrolytes.py` & `chempy-0.9.0/chempy/tests/test_electrolytes.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_equilibria.py` & `chempy-0.9.0/chempy/tests/test_equilibria.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_henry.py` & `chempy-0.9.0/chempy/tests/test_henry.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_reactionsystem.py` & `chempy-0.9.0/chempy/tests/test_reactionsystem.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_solution.py` & `chempy-0.9.0/chempy/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/tests/test_units.py` & `chempy-0.9.0/chempy/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/thermodynamics/expressions.py` & `chempy-0.9.0/chempy/thermodynamics/expressions.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/thermodynamics/tests/test_expressions.py` & `chempy-0.9.0/chempy/thermodynamics/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/units.py` & `chempy-0.9.0/chempy/units.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_aqueous.py` & `chempy-0.9.0/chempy/util/_aqueous.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_dimensionality.py` & `chempy-0.9.0/chempy/util/_dimensionality.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_expr.py` & `chempy-0.9.0/chempy/util/_expr.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_expr_deprecated.py` & `chempy-0.9.0/chempy/util/_expr_deprecated.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_julia.py` & `chempy-0.9.0/chempy/util/_julia.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/_quantities.py` & `chempy-0.9.0/chempy/util/_quantities.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/arithmeticdict.py` & `chempy-0.9.0/chempy/util/arithmeticdict.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/bkh.py` & `chempy-0.9.0/chempy/util/bkh.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/deprecation.py` & `chempy-0.9.0/chempy/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/graph.py` & `chempy-0.9.0/chempy/util/graph.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/numutil.py` & `chempy-0.9.0/chempy/util/numutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/parsing.py` & `chempy-0.9.0/chempy/util/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         charge :: ( '-' | '+' ) ( '1'..'9'? | '1'..'9'' '0'..'9'+ )
         prime :: ( "*" | "'" )*
         term :: (element
                  | '(' formula ')'
                  | '{' formula '}'
                  | '[' formula ']' ) count prime charge?
         formula :: term+
-        hydrate :: '.' count? formula
+        hydrate :: ( '..' | '\u00B7' ) count? formula
         state :: '(' ( 's' | 'l' | 'g' | 'aq' | 'cr' ) ')'
         compound :: count formula hydrate? state?
 
     Parse a chemical formula, including elements, non-integer
     subscripts, nested ions, complexes, charges (ions), hydrates, and
     state symbols.
 
@@ -110,15 +110,15 @@
         charge :: ( '-' | '+' ) ( '1'..'9'? | '1'..'9'' '0'..'9'+ )
         prime :: ( "*" | "'" )*
         term :: (element
                  | '(' formula ')'
                  | '{' formula '}'
                  | '[' formula ']' ) count prime charge?
         formula :: term+
-        hydrate :: '..' count? formula
+        hydrate :: ( '..' | '\u00B7' ) count? formula
         state :: '(' ( 's' | 'l' | 'g' | 'aq' | 'cr' ) ')'
         compound :: count formula hydrate? state?
     """
     _p = __import__(parsing_library)
     Forward, Group, OneOrMore = _p.Forward, _p.Group, _p.OneOrMore
     Optional, ParseResults, Regex = _p.Optional, _p.ParseResults, _p.Regex
     Suppress = _p.Suppress
@@ -330,15 +330,15 @@
 _latex_mapping["epsilon-"] = "\\varepsilon-"
 _latex_mapping["omicron-"] = "o-"
 _latex_mapping["."] = "^\\bullet "
 _latex_infix_mapping = {"..": "\\cdot "}
 
 _unicode_mapping = {k + "-": v + "-" for k, v in zip(_greek_letters, _greek_u)}
 _unicode_mapping["."] = "⋅"
-_unicode_infix_mapping = {"..": "·"}
+_unicode_infix_mapping = {"..": "\u00b7"}  # 0x00b7: '·'
 
 _html_mapping = {k + "-": "&" + k + ";-" for k in _greek_letters}
 _html_mapping["."] = "&sdot;"
 # _html_infix_mapping = _html_mapping
 _html_infix_mapping = {"..": "&sdot;"}
 
 
@@ -375,22 +375,27 @@
     --------
     >>> formula_to_composition('NH4+') == {0: 1, 1: 4, 7: 1}
     True
     >>> formula_to_composition('.NHO-(aq)') == {0: -1, 1: 1, 7: 1, 8: 1}
     True
     >>> formula_to_composition('Na2CO3..7H2O') == {11: 2, 6: 1, 8: 10, 1: 14}
     True
+    >>> formula_to_composition('UO2.3') == {92: 1, 8: 2.3}
+    True
 
     """
     if prefixes is None:
         prefixes = _latex_mapping.keys()
 
     stoich_tok, chg_tok = _formula_to_parts(formula, prefixes, suffixes)[:2]
     tot_comp = {}
-    parts = stoich_tok.split("..")
+    if '\u00b7' in stoich_tok:
+        parts = stoich_tok.split('\u00b7')
+    else:
+        parts = stoich_tok.split("..")
 
     for idx, stoich in enumerate(parts):
         if idx == 0:
             m = 1
         else:
             m, stoich = _get_leading_integer(stoich)
         comp = _parse_stoich(stoich)
@@ -528,15 +533,18 @@
     sup,
     formula,
     prefixes=None,
     infixes=None,
     suffixes=("(s)", "(l)", "(g)", "(aq)"),
 ):
     parts = _formula_to_parts(formula, prefixes.keys(), suffixes)
-    stoichs = parts[0].split("..")
+    if '\u00b7' in parts[0]:
+        stoichs = parts[0].split('\u00b7')
+    else:
+        stoichs = parts[0].split("..")
     string = ""
     for idx, stoich in enumerate(stoichs):
         if idx == 0:
             m = 1
         else:
             m, stoich = _get_leading_integer(stoich)
             string += _subs("..", infixes)
@@ -596,17 +604,19 @@
         re.sub(r"([{}])", r"\\\1", formula) if re.search(r"[{}]", formula) else formula,
         prefixes,
         infixes,
         **kwargs
     )
 
 
-_unicode_sub = {}
+_unicode_sub = {
+    ".": ".",
+}
 
-for k, v in enumerate("₀₁₂₃₄₅₆₇₈₉"):
+for k, v in enumerate("₀₁₂₃₄₅₆₇₈₉."):
     _unicode_sub[str(k)] = v
 
 _unicode_sup = {
     "+": "⁺",
     "-": "⁻",
 }
```

### Comparing `chempy-0.8.3/chempy/util/periodic.py` & `chempy-0.9.0/chempy/util/periodic.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/pyutil.py` & `chempy-0.9.0/chempy/util/pyutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/regression.py` & `chempy-0.9.0/chempy/util/regression.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/rendering.py` & `chempy-0.9.0/chempy/util/rendering.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/stoich.py` & `chempy-0.9.0/chempy/util/stoich.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/table.py` & `chempy-0.9.0/chempy/util/table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/terminal.py` & `chempy-0.9.0/chempy/util/terminal.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/testing.py` & `chempy-0.9.0/chempy/util/testing.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_arithmeticdict.py` & `chempy-0.9.0/chempy/util/tests/test_arithmeticdict.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_expr.py` & `chempy-0.9.0/chempy/util/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_graph.py` & `chempy-0.9.0/chempy/util/tests/test_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tempfile
 
 from chempy import Reaction, ReactionSystem, Substance
 from ..graph import rsys2dot, rsys2graph
 from ..testing import requires, skipif
 
 try:
-    dot_missing = subprocess.call(["dot", "-?"]) != 0
+    dot_missing = subprocess.run(["dot", "-?"]).returncode != 0
 except OSError:
     dot_missing = True
 
 
 def _get_rsys():
     r1 = Reaction({"A": 2}, {"B": 1}, param=3.0)
     A = Substance("A", latex_name="\\boldsymbol{A}")
```

### Comparing `chempy-0.8.3/chempy/util/tests/test_parsing.py` & `chempy-0.9.0/chempy/util/tests/test_parsing.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     formula_to_composition,
     formula_to_html,
     formula_to_latex,
     formula_to_unicode,
     parsing_library,
     to_reaction,
 )
+
 from ..testing import requires
 
 
 @requires(parsing_library)
 @pytest.mark.parametrize(
     "species, composition",
     [
@@ -621,14 +622,30 @@
         ("K4[Fe(CN)6](s)", r"K₄[Fe(CN)₆](s)"),
         ("K4[Fe(CN)6](aq)", r"K₄[Fe(CN)₆](aq)"),
         ("[Fe(H2O)6][Fe(CN)6]..19H2O", r"[Fe(H₂O)₆][Fe(CN)₆]·19H₂O"),
         ("[Fe(H2O)6][Fe(CN)6]..19H2O(s)", r"[Fe(H₂O)₆][Fe(CN)₆]·19H₂O(s)"),
         ("[Fe(H2O)6][Fe(CN)6]..19H2O(aq)", r"[Fe(H₂O)₆][Fe(CN)₆]·19H₂O(aq)"),
         ("[Fe(CN)6]-3", r"[Fe(CN)₆]³⁻"),
         ("[Fe(CN)6]-3(aq)", r"[Fe(CN)₆]³⁻(aq)"),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6",
+            r"Ca₂.₈₃₂Fe₀.₆₂₈₅Mg₅.₃₉₅(CO₃)₆",
+        ),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6(s)",
+            r"Ca₂.₈₃₂Fe₀.₆₂₈₅Mg₅.₃₉₅(CO₃)₆(s)",
+        ),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6..8H2O(s)",
+            r"Ca₂.₈₃₂Fe₀.₆₂₈₅Mg₅.₃₉₅(CO₃)₆·8H₂O(s)",
+        ),
+        (
+            "Zn(NO3)2..6H2O",
+            r"Zn(NO₃)₂·6H₂O",
+        ),
     ],
 )
 @requires(parsing_library)
 def test_formula_to_unicode(species, unicode):
     assert formula_to_unicode(species) == unicode
 
 
@@ -688,14 +705,34 @@
         ),
         (
             "[Fe(H2O)6][Fe(CN)6]..19H2O(aq)",
             r"[Fe(H<sub>2</sub>O)<sub>6</sub>][Fe(CN)<sub>6</sub>]&sdot;19H<sub>2</sub>O(aq)",
         ),
         ("[Fe(CN)6]-3", r"[Fe(CN)<sub>6</sub>]<sup>3-</sup>"),
         ("[Fe(CN)6]-3(aq)", r"[Fe(CN)<sub>6</sub>]<sup>3-</sup>(aq)"),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6",
+            r"Ca<sub>2.832</sub>Fe<sub>0.6285</sub>Mg<sub>5.395</sub>(CO<sub>3</sub>)<sub>6</sub>",
+        ),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6(s)",
+            r"Ca<sub>2.832</sub>Fe<sub>0.6285</sub>Mg<sub>5.395</sub>(CO<sub>3</sub>)<sub>6</sub>(s)",
+        ),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6..8H2O(s)",
+            r"Ca<sub>2.832</sub>Fe<sub>0.6285</sub>Mg<sub>5.395</sub>(CO<sub>3</sub>)<sub>6</sub>&sdot;8H<sub>2</sub>O(s)",
+        ),
+        (
+            "Ca2.832Fe0.6285Mg5.395(CO3)6..8H2O(s)",
+            r"Ca<sub>2.832</sub>Fe<sub>0.6285</sub>Mg<sub>5.395</sub>(CO<sub>3</sub>)<sub>6</sub>&sdot;8H<sub>2</sub>O(s)",
+        ),
+        (
+            "Zn(NO3)2..6H2O",
+            r"Zn(NO<sub>3</sub>)<sub>2</sub>&sdot;6H<sub>2</sub>O",
+        ),
     ],
 )
 @requires(parsing_library)
 def test_formula_to_html(species, html):
     assert formula_to_html(species) == html
 
 
@@ -708,7 +745,13 @@
         ("(Na@C60)+", r"(Na@C<sub>60</sub>)<sup>+</sup>"),
     ],
 )
 @requires(parsing_library)
 def test_formula_to_html_caged(species, html):
     """Should produce HTML for cage species."""
     assert formula_to_html(species) == html
+
+
+def test_composition_dot_as_crystal_water_chempy08x():
+    ref = {30: 1, 7: 2, 8: 12, 1: 12}
+    assert formula_to_composition('Zn(NO3)2{}6H2O'.format('\u00B7')) == ref
+    assert formula_to_composition('Zn(NO3)2..6H2O') == ref
```

### Comparing `chempy-0.8.3/chempy/util/tests/test_periodic.py` & `chempy-0.9.0/chempy/util/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_pyutil.py` & `chempy-0.9.0/chempy/util/tests/test_pyutil.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_regression.py` & `chempy-0.9.0/chempy/util/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_rendering.py` & `chempy-0.9.0/chempy/util/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_stoich.py` & `chempy-0.9.0/chempy/util/tests/test_stoich.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy/util/tests/test_table.py` & `chempy-0.9.0/chempy/util/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy.egg-info/PKG-INFO` & `chempy-0.9.0/chempy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: chempy
-Version: 0.8.3
+Version: 0.9.0
 Summary: ChemPy is a Python package useful for solving problems in chemistry.
 Home-page: https://github.com/bjodah/chempy
 Author: Bjoern I. Dahlgren
 Author-email: bjodah@gmail.com
 License: BSD
 Keywords: chemistry,water properties,physical chemistry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -29,21 +28,21 @@
 License-File: AUTHORS
 
 ChemPy
 ======
 
 .. image:: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml/badge.svg
    :target: https://github.com/bjodah/chempy/actions/workflows/lint_python.yml
-   :alt: Build status
+   :alt: Github Actions CI status
+.. image:: https://hackspett.bjodah.se/api/badges/1/status.svg
+   :target: https://hackspett.bjodah.se/repos/1
+   :alt: Woodpecker CI status
 .. image:: https://img.shields.io/pypi/v/chempy.svg
    :target: https://pypi.python.org/pypi/chempy
    :alt: PyPI version
-.. image:: https://img.shields.io/badge/python-3.8,3.9-blue.svg
-   :target: https://www.python.org/
-   :alt: Python version
 .. image:: https://img.shields.io/pypi/l/chempy.svg
    :target: https://github.com/bjodah/chempy/blob/master/LICENSE
    :alt: License
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
@@ -133,21 +132,21 @@
 `Dockerfile <scripts/environment/Dockerfile>`_.
 
 Using Docker
 ~~~~~~~~~~~~
 If you have `Docker <https://www.docker.com>`_ installed, you may use it to host a jupyter
 notebook server::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 8888
+  $ ./scripts/host-env.sh host-notebook --port 8888
 
 the first time you run the command, some dependencies will be downloaded. When the installation
 is complete there will be a link visible which you can open in your browser. You can also run
 the test suite using the same docker-image::
 
-  $ ./scripts/host-jupyter-using-docker.sh . 0
+  $ ./scripts/host-env.sh run-tests
 
 there will be a few skipped test (due to some dependencies not being installed by default) and
 quite a few warnings.
 
 
 Examples
 --------
@@ -400,36 +399,26 @@
    ...     print('[H2O] = %.2f M (at %d °C)' % (to_unitless(concentration_H2O, u.molar), T_C))
    ...
    [H2O] = 55.46 M (at 15 °C)
    [H2O] = 55.35 M (at 25 °C)
    [H2O] = 55.18 M (at 35 °C)
 
 
-Run notebooks using binder
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-Using only a web-browser (and an internet connection) it is possible to explore the
-notebooks here: (by the courtesy of the people behind mybinder)
-
-.. image:: http://mybinder.org/badge.svg
-   :target: https://mybinder.org/v2/gh/bjodah/chempy/f5f2546e79e165ba8fb258fc87d83a7fbdcbad64?filepath=index.ipynb
-   :alt: Binder
-
-
 Citing
 ------
 If you make use of ChemPy in e.g. academic work you may cite the following peer-reviewed publication:
 
 .. image:: http://joss.theoj.org/papers/10.21105/joss.00565/status.svg
    :target: https://doi.org/10.21105/joss.00565
    :alt: Journal of Open Source Software DOI
 
 Depending on what underlying solver you are using you should also cite the appropriate paper
 (you can look at the list of references in the JOSS article). If you need to reference,
 in addition to the paper, a specific point version of ChemPy (for e.g. reproducibility)
-you can get per-version DOIs from the zendodo archive:
+you can get per-version DOIs from the zenodo archive:
 
 .. image:: https://zenodo.org/badge/8840/bjodah/chempy.svg
    :target: https://zenodo.org/badge/latestdoi/8840/bjodah/chempy
    :alt: Zenodo DOI
 
 Licensing
 ---------
@@ -450,9 +439,7 @@
 (see further details `here <CONTRIBUTING.rst>`_).
 
 
 Author
 ------
 Björn I. Dahlgren, contact:
  - gmail address: bjodah
-
-
```

### Comparing `chempy-0.8.3/chempy.egg-info/SOURCES.txt` & `chempy-0.9.0/chempy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chempy-0.8.3/chempy.egg-info/requires.txt` & `chempy-0.9.0/chempy.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 dot2tex>=2.11.3
 matplotlib>=2.2.3
 numpy>1.11.3
 pulp>=1.6.8
 pyneqsys>=0.5.5
-pyodesys>=0.14.1
+pyodesys>=0.14.4
 pyparsing>=2.0.3
 quantities>=0.12.1
 scipy>=1.0.1
 sym>=0.3.4
 sympy!=1.2,>=1.1.1
 
 [all]
@@ -15,15 +15,15 @@
 appdirs
 black
 bokeh>=0.13.0
 ipywidgets
 numpydoc
 pycodeexport>=0.1.3
 pycompilation>=0.4.12
-pycvodes>=0.14.0
+pycvodes>=0.14.5
 pygslodeiv2>=0.9.4
 pykinsol>=0.1.6
 pyodeint>=0.10.4
 pytest-cov
 pytest-flake8
 pytest>=3.9
 rstcheck
@@ -31,15 +31,15 @@
 
 [docs]
 Sphinx
 numpydoc
 sphinx_rtd_theme
 
 [integrators]
-pycvodes>=0.14.0
+pycvodes>=0.14.5
 pygslodeiv2>=0.9.4
 pyodeint>=0.10.4
 
 [native]
 appdirs
 pycodeexport>=0.1.3
 pycompilation>=0.4.12
```

### Comparing `chempy-0.8.3/setup.cfg` & `chempy-0.9.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 norecursedirs = .* _* build dist conda-recipe scripts benchmarks doc deploy venv *cache*
 flake8-max-line-length = 119
 flake8-ignore = 
 	* E203 W503 W504
 	__init__.py F401 F403
 	arrhenius.py F401
 	chempy/*.* E226
+	chempy/chemistry.py E721
 	chempy/kinetics/tests/test_rates.py E221 E222 E251
 	chempy/properties/** E222
 	debye_huckel.py F401
 	doc/conf.py ALL  # conf.py is a generated file
 	eyring.py F401
 filterwarnings = 
 	ignore::chempy.ChemPyDeprecationWarning
```

### Comparing `chempy-0.8.3/setup.py` & `chempy-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     warnings.warn("Short description from __init__.py probably not read correctly")
 long_descr = io.open(_path_under_setup("README.rst"), encoding="utf-8").read()
 if not len(long_descr) > 100:
     warnings.warn("Long description from README.rst probably not read correctly.")
 _author, _author_email = open(_path_under_setup("AUTHORS"), "rt").readline().split("<")
 
 extras_req = {
-    "integrators": ["pyodeint>=0.10.4", "pycvodes>=0.14.0", "pygslodeiv2>=0.9.4"],
+    "integrators": ["pyodeint>=0.10.4", "pycvodes>=0.14.5", "pygslodeiv2>=0.9.4"],
     "solvers": ["pykinsol>=0.1.6"],
     "native": ["pycompilation>=0.4.12", "pycodeexport>=0.1.3", "appdirs"],
     "docs": ["Sphinx", "sphinx_rtd_theme", "numpydoc"],
     "plotting": ["bokeh>=0.13.0", "ipywidgets"],
     "testing": ["black", "pytest>=3.9", "pytest-cov", "pytest-flake8", "rstcheck"],
 }
 extras_req["all"] = list(chain(extras_req.values()))
@@ -124,15 +124,15 @@
     install_requires=[
         "numpy>1.11.3",
         "scipy>=1.0.1",
         "matplotlib>=2.2.3",
         "sympy>=1.1.1,!=1.2",
         "quantities>=0.12.1",
         "pyneqsys>=0.5.5",
-        "pyodesys>=0.14.1" if sys.version_info[0] >= 3 else "pyodesys<0.12",
+        "pyodesys>=0.14.4" if sys.version_info[0] >= 3 else "pyodesys<0.12",
         "pyparsing>=2.0.3",
         "sym>=0.3.4",
         "pulp>=1.6.8",
         "dot2tex>=2.11.3",
     ],
     extras_require=extras_req,
     python_requires=">=3.8",
```

