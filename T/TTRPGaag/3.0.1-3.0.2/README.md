# Comparing `tmp/TTRPGaag-3.0.1.tar.gz` & `tmp/ttrpgaag-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TTRPGaag-3.0.1.tar", last modified: Tue Mar  5 12:03:51 2024, max compression
+gzip compressed data, was "ttrpgaag-3.0.2.tar", last modified: Wed Apr 24 12:37:39 2024, max compression
```

## Comparing `TTRPGaag-3.0.1.tar` & `ttrpgaag-3.0.2.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.462503 TTRPGaag-3.0.1/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 TTRPGaag-3.0.1/LICENSE
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 TTRPGaag-3.0.1/MANIFEST.in
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1101 2024-03-05 12:03:51.461823 TTRPGaag-3.0.1/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      874 2024-03-05 12:03:28.000000 TTRPGaag-3.0.1/README.md
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.368057 TTRPGaag-3.0.1/RPG/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6148 2023-10-11 15:24:19.000000 TTRPGaag-3.0.1/RPG/.DS_Store
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-03-05 11:41:21.000000 TTRPGaag-3.0.1/RPG/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-03-05 11:59:38.000000 TTRPGaag-3.0.1/RPG/baralho.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.374041 TTRPGaag-3.0.1/RPG/dado/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 TTRPGaag-3.0.1/RPG/dado/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 TTRPGaag-3.0.1/RPG/dado/dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-03-05 11:41:21.000000 TTRPGaag-3.0.1/RPG/dado/dados.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.376950 TTRPGaag-3.0.1/RPG/dado/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/dado/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1513 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/dado/helpers/converter_notacao_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/dado/helpers/monta_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/dado/rolar_dado_notacao.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-03-05 11:41:21.000000 TTRPGaag-3.0.1/RPG/iniciativa.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.377832 TTRPGaag-3.0.1/RPG/sistemas/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.380129 TTRPGaag-3.0.1/RPG/sistemas/dnd/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.384280 TTRPGaag-3.0.1/RPG/sistemas/dnd/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/data/mecanicas.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/data/tesouro.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.391569 TTRPGaag-3.0.1/RPG/sistemas/dnd/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      406 2023-10-11 18:00:52.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/helpers/checa_testes.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-01-22 19:11:09.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/rola_tesouro.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5270 2024-02-28 11:57:10.000000 TTRPGaag-3.0.1/RPG/sistemas/dnd/teste.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.401678 TTRPGaag-3.0.1/RPG/sistemas/pf2/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-03-05 11:41:21.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/PC.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     6182 2023-11-27 11:50:56.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/calcula_dano.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.418600 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/defesas_monstros.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/proficiency.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/saves.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/skills.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/tipos_ataques.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/data/tipos_defesas.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.425676 TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/atributo.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2023-11-27 11:50:56.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      856 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/proficiencias.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 TTRPGaag-3.0.1/RPG/sistemas/pf2/proficiencia.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.430820 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1316 2023-10-09 18:35:46.000000 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/consulta_critico.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.432989 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/data/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/data/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 TTRPGaag-3.0.1/RPG/sistemas/rolemaster/data/criticos.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.436444 TTRPGaag-3.0.1/RPG/tabela_rolavel/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2023-09-12 14:37:16.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/__init__.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.449419 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-11 16:29:38.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/__init__.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      716 2023-09-11 16:58:08.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2023-10-09 18:33:14.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/ajusta_resultados.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/rolamento_dado.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     2853 2023-09-11 17:07:22.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/rolar_tabela.py
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     4450 2023-10-09 18:32:48.000000 TTRPGaag-3.0.1/RPG/tabela_rolavel/tabela_rolavel.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.460479 TTRPGaag-3.0.1/TTRPGaag.egg-info/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1101 2024-03-05 12:03:51.000000 TTRPGaag-3.0.1/TTRPGaag.egg-info/PKG-INFO
--rw-r--r--   0 alessandroguarita   (502) staff       (20)     1809 2024-03-05 12:03:51.000000 TTRPGaag-3.0.1/TTRPGaag.egg-info/SOURCES.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-03-05 12:03:51.000000 TTRPGaag-3.0.1/TTRPGaag.egg-info/dependency_links.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-03-05 12:03:51.000000 TTRPGaag-3.0.1/TTRPGaag.egg-info/top_level.txt
--rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-03-05 12:03:51.462663 TTRPGaag-3.0.1/setup.cfg
--rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-03-05 12:00:34.000000 TTRPGaag-3.0.1/setup.py
-drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-03-05 12:03:51.461088 TTRPGaag-3.0.1/tests/
--rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 TTRPGaag-3.0.1/tests/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.610753 ttrpgaag-3.0.2/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1075 2023-10-09 18:00:41.000000 ttrpgaag-3.0.2/LICENSE
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       47 2023-10-09 18:12:41.000000 ttrpgaag-3.0.2/MANIFEST.in
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1169 2024-04-24 12:37:39.610284 ttrpgaag-3.0.2/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      942 2024-04-23 18:50:06.000000 ttrpgaag-3.0.2/README.md
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.561943 ttrpgaag-3.0.2/RPG/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      254 2024-04-23 18:35:00.000000 ttrpgaag-3.0.2/RPG/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6480 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/baralho.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.566280 ttrpgaag-3.0.2/RPG/dado/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       94 2023-10-11 14:22:30.000000 ttrpgaag-3.0.2/RPG/dado/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3357 2023-11-13 11:34:50.000000 ttrpgaag-3.0.2/RPG/dado/dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     2117 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/dado/dados.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.569497 ttrpgaag-3.0.2/RPG/dado/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1513 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/converter_notacao_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      295 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/helpers/monta_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1281 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/dado/rolar_dado_notacao.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      803 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/iniciativa.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.571281 ttrpgaag-3.0.2/RPG/sistemas/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.574453 ttrpgaag-3.0.2/RPG/sistemas/dnd/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       91 2023-09-14 17:58:19.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.576318 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      245 2024-01-22 19:11:21.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/mecanicas.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     7566 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/data/tesouro.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.578251 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      247 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/calcular_mod_atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      406 2023-10-11 18:00:52.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/helpers/checa_testes.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1044 2024-01-22 19:11:09.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/rola_tesouro.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5270 2024-02-28 11:57:10.000000 ttrpgaag-3.0.2/RPG/sistemas/dnd/teste.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.582308 ttrpgaag-3.0.2/RPG/sistemas/pf2/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     8697 2024-04-22 12:53:12.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/PC.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      191 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     6182 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/calcula_dano.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.589910 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      494 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3279 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/defesas_monstros.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      109 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/proficiency.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       74 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/saves.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      405 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/skills.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      119 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/tipos_ataques.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      101 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/data/tipos_defesas.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.592666 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-12-01 15:28:03.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      280 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/atributo.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     5426 2023-11-27 11:50:56.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/base_calcula_dano.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      856 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/proficiencias.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      855 2023-12-06 18:02:34.000000 ttrpgaag-3.0.2/RPG/sistemas/pf2/proficiencia.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.595230 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       64 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1316 2024-04-23 18:43:15.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/consulta_critico.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.597636 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)    28276 2023-09-14 16:09:39.000000 ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/criticos.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.601222 ttrpgaag-3.0.2/RPG/tabela_rolavel/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       80 2024-04-23 17:09:37.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/__init__.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.605709 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-09-11 16:29:38.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/__init__.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1014 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajeita_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      724 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajusta_resultados.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      183 2023-09-11 16:58:08.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/busca_index_item_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      322 2023-09-11 16:58:26.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/rolamento_dado.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     3215 2024-04-23 18:48:05.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/rolar_tabela.py
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     4480 2024-04-24 11:59:30.000000 ttrpgaag-3.0.2/RPG/tabela_rolavel/tabela_rolavel.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.609765 ttrpgaag-3.0.2/TTRPGaag.egg-info/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1169 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/PKG-INFO
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)     1795 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/SOURCES.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        1 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/dependency_links.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       10 2024-04-24 12:37:39.000000 ttrpgaag-3.0.2/TTRPGaag.egg-info/top_level.txt
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)       38 2024-04-24 12:37:39.610866 ttrpgaag-3.0.2/setup.cfg
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)      480 2024-04-24 12:23:02.000000 ttrpgaag-3.0.2/setup.py
+drwxr-xr-x   0 alessandroguarita   (502) staff       (20)        0 2024-04-24 12:37:39.609125 ttrpgaag-3.0.2/tests/
+-rw-r--r--   0 alessandroguarita   (502) staff       (20)        0 2023-10-09 18:10:54.000000 ttrpgaag-3.0.2/tests/__init__.py
```

### Comparing `TTRPGaag-3.0.1/LICENSE` & `ttrpgaag-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/PKG-INFO` & `ttrpgaag-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 3.0.1
+Version: 3.0.2
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
```

### Comparing `TTRPGaag-3.0.1/README.md` & `ttrpgaag-3.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
```

### Comparing `TTRPGaag-3.0.1/RPG/baralho.py` & `ttrpgaag-3.0.2/RPG/baralho.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/dado/dado.py` & `ttrpgaag-3.0.2/RPG/dado/dado.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/dado/dados.py` & `ttrpgaag-3.0.2/RPG/dado/dados.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/dado/helpers/converter_notacao_dado.py` & `ttrpgaag-3.0.2/RPG/dado/helpers/converter_notacao_dado.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/dado/rolar_dado_notacao.py` & `ttrpgaag-3.0.2/RPG/dado/rolar_dado_notacao.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/iniciativa.py` & `ttrpgaag-3.0.2/RPG/iniciativa.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/dnd/data/tesouro.py` & `ttrpgaag-3.0.2/RPG/sistemas/dnd/data/tesouro.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/dnd/rola_tesouro.py` & `ttrpgaag-3.0.2/RPG/sistemas/dnd/rola_tesouro.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/dnd/teste.py` & `ttrpgaag-3.0.2/RPG/sistemas/dnd/teste.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/PC.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/PC.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/calcula_dano.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/calcula_dano.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/data/defesas_monstros.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/data/defesas_monstros.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/base_calcula_dano.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/base_calcula_dano.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/helpers/proficiencias.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/helpers/proficiencias.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/pf2/proficiencia.py` & `ttrpgaag-3.0.2/RPG/sistemas/pf2/proficiencia.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/rolemaster/consulta_critico.py` & `ttrpgaag-3.0.2/RPG/sistemas/rolemaster/consulta_critico.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/sistemas/rolemaster/data/criticos.py` & `ttrpgaag-3.0.2/RPG/sistemas/rolemaster/data/criticos.py`

 * *Files identical despite different names*

### Comparing `TTRPGaag-3.0.1/RPG/tabela_rolavel/helpers/ajeita_tabela.py` & `ttrpgaag-3.0.2/RPG/tabela_rolavel/helpers/ajeita_tabela.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+def ordena_dicionario(tabela: dict):
+    numeros = sorted(tabela)
+    return {chave: tabela[chave] for chave in numeros}
+
+
 def ajeita_tabela(tabela: list[tuple, str]) -> list[tuple, str]:
     """
     Pega uma _tabela que tenha itens com apenas um rolamento e coloca na tupla como valor mínimo e máximo
     :param tabela: a _tabela a ser arrumada
     :return: lista
     """
     nova_tabela = []
@@ -16,7 +21,16 @@
             alcance_rolamento = (int(alcance_rolamento[0]), alcance_rolamento[1])
 
         linha = (alcance_rolamento, resultado_rolamento)
         nova_tabela.append(linha)
 
 
     return nova_tabela
+
+
+def converte_lista(tabela):
+    tabela = ajeita_tabela(tabela)
+    dicionario = {}
+    for linha in tabela:
+        dicionario[linha[0][1]] = linha[1]
+
+    return dicionario
```

### Comparing `TTRPGaag-3.0.1/RPG/tabela_rolavel/rolar_tabela.py` & `ttrpgaag-3.0.2/RPG/tabela_rolavel/rolar_tabela.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-from .helpers.ajeita_tabela import ajeita_tabela
-from .helpers.ajusta_resultados import verifica_resultado_fora_alcance, rola_dados_resultado
+from .helpers.ajeita_tabela import ordena_dicionario, converte_lista
+from .helpers.ajusta_resultados import rola_dados_resultado
 
-
-def rolar_tabela(valor: int, tabela: list, coluna=None, rolar_dados=True) -> str:
-    """
-    Busca o resultado em uma tabela de RPG retornando a linha e a eventual
+def rolar_tabela(tabela: list | dict, valor: int, coluna: str | int | None=None, rolar_dados: bool=True) -> str:
+    """Busca o resultado em uma tabela de RPG retornando a linha e a eventual 
     coluna, caso tenha. Se o texto possuir notação de dados (exemplo: 1d6)
     também já rola o resultado.
 
-    O padrão de cada linha é ((inicio, fim), resultado da busca).
-    É possível colocar apenas um valor na primeira tupla caso esse item só tenha
-    um valor. Resultado da busca pode ser uma string como "1d6 gp" ou um
-    dicionário com o formato { "col 1": "resultado col 1", "col2": "valor col2" }
+    A tabela pode ser um dicionário ou uma lista.
+    Como dicionário, cada chave é o número mais alto (exemplo: de 3 até 6, seria 6).
+    Por exemplo: {2: 'resultado 1', 4: 'resultado 2'}
 
-    :param valor: o valor a ser buscado
-    :param tabela: a lista a ser usada conforme indicado acima.
-    :param coluna: qual a coluna a ser buscada pelo resultado, se não tiver colunas, ignore
-    :param rolar_dados: booleano para indicar se o resultado que contenha dados a ser rolado (ex.: "1d10 gp"). Se não quiser que já retorne o dado rolado,     marque False
+    Como lista o padrão de cada linha é ((inicio, fim), resultado da busca).
+    É possível colocar apenas um valor na primeira tupla caso esse item só tenha
+    um valor.
+    
+    O resultado da tabela pode ser uma string como "1d6 gp" ou um dicionário com
+    o formato { "col 1": "resultado col 1", "col2": "valor col2" } para tabelas
+    com colunas
+
+    Args:
+        tabela (list | dict): a tabela a ser buscado, pode aparecer em dois formatos: dicionário ou lista.
+        valor (int): o valor a ser buscado
+        coluna (str, int, optional): qual a coluna a ser buscada pelo resultado, se não tiver colunas, ignore. Defaults to None.
+        rolar_dados (bool, optional): booleano para indicar se o resultado que contenha dados a ser rolado (ex.: "1d10 gp"). Se não quiser que já retorne o dado rolado, marque False. Defaults to True.
 
-    :return:
+    Returns:
+        str: O resultado da tabela
     """
-    # Ajeita a _tabela para o caso da tupla não ter dois itens
-    nova_tabela = ajeita_tabela(tabela)
+    # Converte a lista para dicionário
+    tabela = tabela if type(tabela) is dict else converte_lista(tabela)
+    # Ordena o dicionário em ordem numérica, caso esteja fora de ordem
+    tabela = ordena_dicionario(tabela)
+
+    # Converte o dicionário em duas listas para realizar a busca
+    # e gera o índice do item rolado
+    chaves, valores = list(tabela.keys()), list(tabela.values())
+    indice = next((chave[0] for chave in enumerate(chaves) if chave[1] >= valor), -1)
 
-    # pega os índices a serem buscados
-    indice_menor = nova_tabela[0][0][0]
-    indice_maior = nova_tabela[-1][0][1]
-
-    # Busca a linha da _tabela
-    resultado = next(
-        (item for (x, y), item in nova_tabela if x <= valor <= y),
-        None
-    )
-
-    resultado = verifica_resultado_fora_alcance(valor, indice_menor, indice_maior, nova_tabela, resultado)
-
-    # se tiver mais de uma coluna, seleciona a coluna
+    # Gera o resultado da busca
+    resultado = valores[indice]
     resultado = resultado[coluna] if coluna else resultado
 
-    # transforma o texto que contenha notação de _dados em texto com resultado
     resultado = rola_dados_resultado(rolar_dados, resultado)
-
+    
     return resultado
+    
 
 
 if __name__ == "__main__":
     # Exemplo de uso
     exemplo_tabela = [
         ((1, 6), {"coluna 1": "2d6 moedas de ouro", "coluna 2": "2d10+1d6 moedas de ouro e 1d6 de prata",
                   "coluna 3": "d8*2 moedas de ouro"}),
```

### Comparing `TTRPGaag-3.0.1/RPG/tabela_rolavel/tabela_rolavel.py` & `ttrpgaag-3.0.2/RPG/tabela_rolavel/tabela_rolavel.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from .helpers.rolamento_dado import DadoRolado
 from RPG.dado import rolar_dado_notacao
 
 
 class TabelaRolavel:
     def __init__(self, tabela: list = None, dados: str | int = None):
         """
-        Cria um objeto com uma tabela vazia ou já existente para ser rolada e métodos para que busquem o
+        Cria um objeto com uma tabela vazia ou já existente (no formato de lista) para ser rolada e métodos para que busquem o
         resultado diretamente nela.
 
-        :param tabela: a tabela a ser buscada, se não passar o parâmetro, cria uma tabela vazia (que deve ser preenchida com .insere_linha_tabela()
-        :param dados: a notação de dados a ser usado para rolar na tabela. Também pode ser passado um valor fixo (que pode ser alterado com o método .rolar())
+        Args:
+            tabela: a tabela a ser buscada, se não passar o parâmetro, cria uma tabela vazia (que deve ser preenchida com .insere_linha_tabela()
+            dados: a notação de dados a ser usado para rolar na tabela. Também pode ser passado um valor fixo (que pode ser alterado com o método .rolar())
         """
         self._tabela = ajeita_tabela(tabela) if tabela else []
         self._dados = dados
         self._dado_rolado = DadoRolado(rolamento=0, modificador=0)
         self._resultado = ''
 
         if dados:
@@ -68,15 +69,15 @@
         :param modificador_dado: Para o caso de haver algum modificador não básico aplicado na tabela (ex.: role na tabela X com +10)
         :param coluna: Caso o resultado tenha mais de uma coluna. Seleciona a coluna e rola dos dados dentro dela
         """
         valor_fixo = self._dados if not valor_fixo else valor_fixo
         dado = valor_fixo if type(valor_fixo) == int else rolar_dado_notacao(valor_fixo)
 
         self._dado_rolado = DadoRolado(dado, modificador_dado)
-        self._resultado = rolar_tabela(self._dado_rolado.total, self._tabela, coluna)
+        self._resultado = rolar_tabela(self._tabela, self._dado_rolado.total, coluna)
 
     # Getters ========================================================================================================
     @property
     def tabela(self):
         return self._tabela
 
     @property
```

### Comparing `TTRPGaag-3.0.1/TTRPGaag.egg-info/PKG-INFO` & `ttrpgaag-3.0.2/TTRPGaag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: TTRPGaag
-Version: 3.0.1
+Version: 3.0.2
 Summary: Pacote básico de Ferramentas de RPG em português
 Author: Alessandro Guarita
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RPG
 Pacote Python com as minhas ferramentas de RPG
 
+- **3.0.2** - `rolar_tabela` agora usa prioritariamente dicionário
 - **3.0.1** - Otimização no embaralhamento de cartas, usando função nativa do módulo random.
 - **3.0.0** - PF2
   - Alteração do parâmetro `.defesa_base` para `.defesa_monstro_base` para deixar mais claro seu uso
   - Alteração do import do módulo `calcula_proficiencia` para `proficiencia` pois ganhou outra função: `aumentar_proficiencia` 
   - Lista de skills em Data
   - Classe de PC para representar um personagem
 - **2.2.3** - Inclusão dos danos só de rolamento no PF2
```

### Comparing `TTRPGaag-3.0.1/TTRPGaag.egg-info/SOURCES.txt` & `ttrpgaag-3.0.2/TTRPGaag.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-RPG/.DS_Store
 RPG/__init__.py
 RPG/baralho.py
 RPG/iniciativa.py
 RPG/dado/__init__.py
 RPG/dado/dado.py
 RPG/dado/dados.py
 RPG/dado/rolar_dado_notacao.py
```

