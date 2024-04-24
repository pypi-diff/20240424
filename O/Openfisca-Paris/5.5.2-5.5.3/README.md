# Comparing `tmp/Openfisca-Paris-5.5.2.tar.gz` & `tmp/openfisca_paris-5.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Openfisca-Paris-5.5.2.tar", last modified: Tue Mar 12 16:16:00 2024, max compression
+gzip compressed data, was "openfisca_paris-5.5.3.tar", last modified: Wed Apr 24 08:24:22 2024, max compression
```

## Comparing `Openfisca-Paris-5.5.2.tar` & `openfisca_paris-5.5.3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.408900 Openfisca-Paris-5.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.408900 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-12 16:16:00.000000 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-12 16:16:00.000000 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 16:16:00.000000 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-12 16:16:00.000000 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-12 16:16:00.000000 Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-12 16:16:00.408900 Openfisca-Paris-5.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.400900 Openfisca-Paris-5.5.2/openfisca_paris/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.400900 Openfisca-Paris-5.5.2/openfisca_paris/familles/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/familles/aspeh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/familles/paris_energie_familles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/familles/paris_forfait_familles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.396900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.400900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.400900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.400900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/aspeh/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/paris_pass.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/plfm/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10499 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_logement_fam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_logement_fam_mono.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/paris_solidarite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.404900 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_pass_seniors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/personnes_agees.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/psol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:16:00.408900 Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/paris_pass_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/personne_handicapee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/psol.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 16:16:00.408900 Openfisca-Paris-5.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-12 16:15:44.000000 Openfisca-Paris-5.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 08:24:22.000000 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-24 08:24:22.000000 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:24:22.000000 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:24:22.000000 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 08:24:22.000000 openfisca_paris-5.5.3/Openfisca_Paris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.860602 openfisca_paris-5.5.3/openfisca_paris/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.860602 openfisca_paris-5.5.3/openfisca_paris/familles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/familles/aspeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/familles/paris_energie_familles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/familles/paris_forfait_familles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.856602 openfisca_paris-5.5.3/openfisca_paris/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.860602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.860602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.860602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/aspeh/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.864602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.864602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/paris_pass.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.864602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.864602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.864602 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/plfm/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10499 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_logement_fam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_logement_fam_mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/paris_solidarite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_pass_seniors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/personnes_agees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_agees/psol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/paris_pass_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/personne_handicapee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/psol.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:24:22.868602 openfisca_paris-5.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 08:23:55.000000 openfisca_paris-5.5.3/setup.py
```

### Comparing `Openfisca-Paris-5.5.2/LICENSE.AGPL.txt` & `openfisca_paris-5.5.3/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/PKG-INFO` & `openfisca_paris-5.5.3/Openfisca_Paris.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 5.5.2
+Version: 5.5.3
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -13,11 +13,11 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE.AGPL.txt
 Requires-Dist: OpenFisca-Core<42,>=40.0.1
-Requires-Dist: OpenFisca-France<160,>=149.1.1
+Requires-Dist: OpenFisca-France<165,>=149.1.1
 Provides-Extra: test
 Requires-Dist: nose; extra == "test"
 Requires-Dist: pytest>=5.4.2; extra == "test"
```

### Comparing `Openfisca-Paris-5.5.2/Openfisca_Paris.egg-info/SOURCES.txt` & `openfisca_paris-5.5.3/Openfisca_Paris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/PKG-INFO` & `openfisca_paris-5.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 5.5.2
+Version: 5.5.3
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -13,11 +13,11 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Description-Content-Type: text/markdown
 License-File: LICENSE.AGPL.txt
 Requires-Dist: OpenFisca-Core<42,>=40.0.1
-Requires-Dist: OpenFisca-France<160,>=149.1.1
+Requires-Dist: OpenFisca-France<165,>=149.1.1
 Provides-Extra: test
 Requires-Dist: nose; extra == "test"
 Requires-Dist: pytest>=5.4.2; extra == "test"
```

### Comparing `Openfisca-Paris-5.5.2/README.md` & `openfisca_paris-5.5.3/README.md`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/familles/aspeh.py` & `openfisca_paris-5.5.3/openfisca_paris/familles/aspeh.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/familles/paris_energie_familles.py` & `openfisca_paris-5.5.3/openfisca_paris/familles/paris_energie_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/familles/paris_forfait_familles.py` & `openfisca_paris-5.5.3/openfisca_paris/familles/paris_forfait_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml` & `openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml` & `openfisca_paris-5.5.3/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml` & `openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml` & `openfisca_paris-5.5.3/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris.py` & `openfisca_paris-5.5.3/openfisca_paris/paris.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_complement_sante.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_logement.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_logement_fam.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_logement_fam.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_logement_fam_mono.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_logement_fam_mono.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_pass.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_pass.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/paris_solidarite.py` & `openfisca_paris-5.5.3/openfisca_paris/paris_solidarite.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_complement_sante.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_logement.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/paris_pass_seniors.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_agees/paris_pass_seniors.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/personnes_agees.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_agees/personnes_agees.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_agees/psol.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_agees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/paris_complement_sante.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/paris_pass_access.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/paris_pass_access.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/personne_handicapee.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/personne_handicapee.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/openfisca_paris/personnes_handicapees/psol.py` & `openfisca_paris-5.5.3/openfisca_paris/personnes_handicapees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-5.5.2/setup.py` & `openfisca_paris-5.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="Openfisca-Paris",
-    version="5.5.2",
+    version="5.5.3",
     author="OpenFisca Team",
     author_email="contact@openfisca.fr",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
@@ -21,15 +21,15 @@
     keywords="benefit france paris microsimulation social tax",
     license="http://www.fsf.org/licensing/licenses/agpl-3.0.html",
 
     packages=find_namespace_packages(),
     include_package_data=True,
     install_requires=[
         'OpenFisca-Core >= 40.0.1, < 42',
-        'OpenFisca-France >= 149.1.1, < 160',
+        'OpenFisca-France >= 149.1.1, < 165',
     ],
     extras_require={
         'test': [
             'nose',
             'pytest >= 5.4.2'
         ]
     },
```

