# Comparing `tmp/inewave-1.7.5.tar.gz` & `tmp/inewave-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-1.7.5.tar", last modified: Fri Apr 12 22:24:11 2024, max compression
+gzip compressed data, was "inewave-1.8.0.tar", last modified: Wed Apr 24 13:01:50 2024, max compression
```

## Comparing `inewave-1.7.5.tar` & `inewave-1.8.0.tar`

### file list

```diff
@@ -1,880 +1,989 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.929025 inewave-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 22:20:35.000000 inewave-1.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 22:24:11.929025 inewave-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-12 22:20:35.000000 inewave-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.725026 inewave-1.7.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 22:20:35.000000 inewave-1.7.5/examples/plot_dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-12 22:20:35.000000 inewave-1.7.5/examples/plot_modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 22:20:35.000000 inewave-1.7.5/examples/plot_pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 22:20:35.000000 inewave-1.7.5/examples/plot_sistema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.725026 inewave-1.7.5/inewave/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.729026 inewave-1.7.5/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/_utils/formatacao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.729026 inewave-1.7.5/inewave/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/eolica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.729026 inewave-1.7.5/inewave/libs/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/modelos/eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)    19601 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/modelos/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/modelos/usinas_hidreletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/libs/usinas_hidreletricas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.741026 inewave-1.7.5/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    83959 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    38978 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.749026 inewave-1.7.5/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.753026 inewave-1.7.5/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.753026 inewave-1.7.5/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)    31154 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)   143761 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    88425 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (127)    15762 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17065 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    24845 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    21896 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)    23710 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modelos/volref_saz.py
--rw-r--r--   0 runner    (1001) docker     (127)    13967 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (127)    19079 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/newave/volref_saz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.753026 inewave-1.7.5/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.753026 inewave-1.7.5/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/modelos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistcf/nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.773026 inewave-1.7.5/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/mevminsin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.797026 inewave-1.7.5/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.797026 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivorestricao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.801026 inewave-1.7.5/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/estacaobombeamento.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/restricao.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.929025 inewave-1.7.5/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-12 22:24:11.000000 inewave-1.7.5/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27157 2024-04-12 22:24:11.000000 inewave-1.7.5/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:24:11.000000 inewave-1.7.5/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 22:24:11.000000 inewave-1.7.5/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 22:24:11.000000 inewave-1.7.5/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:24:11.929025 inewave-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 22:20:35.000000 inewave-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.801026 inewave-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.801026 inewave-1.7.5/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.801026 inewave-1.7.5/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/libs/test_eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/libs/test_restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/libs/test_usinas_hidreletricas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.801026 inewave-1.7.5/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.897025 inewave-1.7.5/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/arquivos_nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    46951 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
--rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)    30063 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (127)   847210 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)   295249 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (127)   295245 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105146 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)   295190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)   295196 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283211 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   847164 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dneg_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dpos_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)   120243 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)   267099 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267152 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)   267153 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267144 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)   291239 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)   291240 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   232674 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)   267119 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/eolica.py
--rw-r--r--   0 runner    (1001) docker     (127)    56476 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (127)   267138 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104654 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (127)   120990 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104650 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105178 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105179 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105181 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/gh_fphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105153 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105156 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   847144 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105136 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)    19898 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105141 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105140 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105189 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)    49768 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    26457 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105188 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105191 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)   425676 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)  1087195 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    57012 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (127)    45543 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)    76521 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)   378349 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (127)    50087 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)    52098 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)   267136 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   425677 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)   657056 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/restricoes.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/shist.py
--rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (127)    38821 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/usinas_hidreletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)   271157 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)   283139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   283209 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)   847213 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (127)   847200 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267158 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105174 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)  1105176 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)   847195 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)   267115 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25446 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/volref_saz.py
--rw-r--r--   0 runner    (1001) docker     (127)   847135 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.909025 inewave-1.7.5/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_agrint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_cortes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_cortesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (127)    52011 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_eco_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)    36320 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_forwarh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_ghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_manutt.py
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_selcor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_shist.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazinat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_vazpast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/newave/test_volrefsaz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.909025 inewave-1.7.5/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/test_nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistcf/test_nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:24:11.929025 inewave-1.7.5/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_c_v_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_c_v_rhq_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_c_v_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_c_v_rhv_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cbombsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_celetricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_deletricas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_desvuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dnegevap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dposevap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_edesvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_edesvcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_edesvcsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evapo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evapom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evaporsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_form_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_form_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghfphexat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghidr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghidrm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghidrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmax_fpha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmax_fphc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_gtert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_hjus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_hliq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_hmont.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasree.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasrep.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasrhq.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasrhv.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasusie.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasusih.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mediasusit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_mevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_pivarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_pivarmincr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vbomb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vdesviouh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vevapuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_viol_rhq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_viol_rhv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vmort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vmortm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vmortsin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-12 22:20:35.000000 inewave-1.7.5/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.356959 inewave-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 12:57:52.000000 inewave-1.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-24 13:01:50.356959 inewave-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 12:57:52.000000 inewave-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.120960 inewave-1.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-24 12:57:52.000000 inewave-1.8.0/examples/plot_dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-24 12:57:52.000000 inewave-1.8.0/examples/plot_modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-24 12:57:52.000000 inewave-1.8.0/examples/plot_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-24 12:57:52.000000 inewave-1.8.0/examples/plot_sistema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.120960 inewave-1.8.0/inewave/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.124960 inewave-1.8.0/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/_utils/formatacao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.124960 inewave-1.8.0/inewave/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/eolica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.124960 inewave-1.8.0/inewave/libs/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/modelos/eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19601 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/modelos/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/modelos/usinas_hidreletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16373 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/libs/usinas_hidreletricas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.136960 inewave-1.8.0/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83959 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/evap_avl_desv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/evap_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/evap_eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38978 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/fpha_avl_desv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/fpha_avl_desv_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/fpha_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/fpha_eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.152960 inewave-1.8.0/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.152960 inewave-1.8.0/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.152960 inewave-1.8.0/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31154 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   143761 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88425 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15762 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17065 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32616 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17685 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24845 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21896 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57231 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23710 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modelos/volref_saz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13967 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18425 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19602 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/newave/volref_saz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.152960 inewave-1.8.0/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.152960 inewave-1.8.0/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/modelos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistcf/nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.184960 inewave-1.8.0/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cviol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cviol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cviol_rhq_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cviol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/cviol_rhv_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/mevminsin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.212960 inewave-1.8.0/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.212960 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivorestricao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.212960 inewave-1.8.0/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/estacaobombeamento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/restricao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cviol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cviol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cviol_rhq_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cviol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/cviol_rhv_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/qvertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/valor_agua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_evmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_evminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_evminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_ghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_ghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_ghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_dfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_dfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_dfmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_tbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_tbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_lpp_tbmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_neg_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_pos_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_turbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_turbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_vazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/viol_vazmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vretiradauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/qvertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/valor_agua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_evmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_evminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_evminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_ghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_ghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_ghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_dfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_dfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_dfmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_tbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_tbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_lpp_tbmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_neg_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_pos_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_turbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_turbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_vazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/viol_vazmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vretiradauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.356959 inewave-1.8.0/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-24 13:01:50.000000 inewave-1.8.0/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31080 2024-04-24 13:01:50.000000 inewave-1.8.0/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:50.000000 inewave-1.8.0/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 13:01:50.000000 inewave-1.8.0/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 13:01:50.000000 inewave-1.8.0/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:01:50.356959 inewave-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 12:57:52.000000 inewave-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.212960 inewave-1.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.212960 inewave-1.8.0/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.216960 inewave-1.8.0/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/libs/test_eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/libs/test_restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16356 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/libs/test_usinas_hidreletricas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.216960 inewave-1.8.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.312960 inewave-1.8.0/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/arquivos_nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46951 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24307 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24312 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30063 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847210 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295249 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295245 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105146 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295190 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   295196 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283211 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847164 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105161 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105169 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dneg_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dpos_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120243 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267099 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267152 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267153 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267144 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291239 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   291240 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232674 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267119 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/eolica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56476 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267121 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267138 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104654 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120990 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24311 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-24 12:57:52.000000 inewave-1.8.0/tests/mocks/arquivos/form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104650 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1104652 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105178 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105179 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105181 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/gh_fphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105153 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105154 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105156 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847144 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105136 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19898 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105138 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105141 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105140 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105189 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49768 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26457 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105188 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105191 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)   846407 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)   425676 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1087195 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49720 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57012 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45543 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76521 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)   378349 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50087 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52098 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267136 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267137 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   428805 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   657262 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283145 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/restricoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105160 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20855 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18692 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38821 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/usinas_hidreletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271157 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283209 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24306 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847213 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267101 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847200 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267155 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267156 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267158 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267122 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267130 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105174 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1105176 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847195 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/viol_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267115 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267116 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   267118 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25446 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/volref_saz.py
+-rw-r--r--   0 runner    (1001) docker     (127)   847135 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.324960 inewave-1.8.0/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_agrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52011 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_eco_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_evap_avl_desv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_evap_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_evap_eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36320 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_fpha_avl_desv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_fpha_avl_desv_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_fpha_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_fpha_eco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_manutt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_selcor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_shist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazinat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/newave/test_volrefsaz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.324960 inewave-1.8.0/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/test_nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistcf/test_nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:50.356959 inewave-1.8.0/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_c_v_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_c_v_rhq_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_c_v_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_c_v_rhv_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cbombsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_celetricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cviol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cviol_rhq_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_cviol_rhv_sin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_deletricas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_desvuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dnegevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dposevap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_edesvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_edesvcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_edesvcsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evapo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evapom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evaporsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_form_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_form_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghfphexat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghidr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghidrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghidrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmax_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmax_fphc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_gtert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_hjus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_hliq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_hmont.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasrep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasrhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasrhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasusie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasusih.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mediasusit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_mevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_pivarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_pivarmincr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qturuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_qvertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_valor_agua.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vbomb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vdesviouh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vevapuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_eletricasin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_evmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_evminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_evminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_fpha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_ghminm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_ghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_ghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_dfmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_dfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_dfmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_tbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_tbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_lpp_tbmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_neg_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_pos_evap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_rhq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_rhv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_turbmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_turbmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_vazmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_viol_vazmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vmort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vmortm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vmortsin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vretiradauh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 12:57:53.000000 inewave-1.8.0/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-1.7.5/LICENSE.md` & `inewave-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/PKG-INFO` & `inewave-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 1.7.5
+Version: 1.8.0
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-1.7.5/README.md` & `inewave-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/examples/plot_dger.py` & `inewave-1.8.0/examples/plot_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/examples/plot_modif.py` & `inewave-1.8.0/examples/plot_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/examples/plot_pmo.py` & `inewave-1.8.0/examples/plot_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/examples/plot_sistema.py` & `inewave-1.8.0/examples/plot_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/_utils/formatacao.py` & `inewave-1.8.0/inewave/_utils/formatacao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/config.py` & `inewave-1.8.0/inewave/config.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/eolica.py` & `inewave-1.8.0/inewave/libs/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/modelos/eolica.py` & `inewave-1.8.0/inewave/libs/modelos/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/modelos/restricoes.py` & `inewave-1.8.0/inewave/libs/modelos/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/modelos/usinas_hidreletricas.py` & `inewave-1.8.0/inewave/libs/modelos/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/restricoes.py` & `inewave-1.8.0/inewave/libs/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/libs/usinas_hidreletricas.py` & `inewave-1.8.0/inewave/libs/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/__init__.py` & `inewave-1.8.0/inewave/newave/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Inclui os membros
 
+# Deprecated
+from .avl_cortesfpha_nwv import AvlCortesFpha  # noqa
+from .avl_desvfpha_s import AvlDesvFphaS  # noqa
+from .avl_desvfpha_v_q import AvlDesvFphaVQ  # noqa
+from .eco_fpha import EcoFpha  # noqa
+from .nwv_avl_evap import NwvAvlEvap  # noqa
+from .nwv_cortes_evap import NwvCortesEvap  # noqa
+from .nwv_eco_evap import NwvEcoEvap  # noqa
+
 from .abertura import Abertura  # noqa
 from .adterm import Adterm  # noqa
 from .agrint import Agrint  # noqa
 from .arquivos import Arquivos  # noqa
 from .bid import BID  # noqa
 from .cadic import Cadic  # noqa
 from .caso import Caso  # noqa
@@ -42,21 +51,21 @@
 from .selcor import Selcor  # noqa
 from .sistema import Sistema  # noqa
 from .tecno import Tecno  # noqa
 from .term import Term  # noqa
 from .vazoes import Vazoes  # noqa
 from .vazpast import Vazpast  # noqa
 from .volref_saz import VolrefSaz  # noqa
-from .avl_cortesfpha_nwv import AvlCortesFpha  # noqa
-from .avl_desvfpha_s import AvlDesvFphaS  # noqa
-from .avl_desvfpha_v_q import AvlDesvFphaVQ  # noqa
-from .eco_fpha import EcoFpha  # noqa
-from .nwv_avl_evap import NwvAvlEvap  # noqa
-from .nwv_cortes_evap import NwvCortesEvap  # noqa
-from .nwv_eco_evap import NwvEcoEvap  # noqa
+from .fpha_cortes import FphaCortes  # noqa
+from .fpha_avl_desv_s import FphaAvlDesvS  # noqa
+from .fpha_avl_desv_v_q import FphaAvlDesvVQ  # noqa
+from .fpha_eco import FphaEco  # noqa
+from .evap_avl_desv import EvapAvlDesv  # noqa
+from .evap_cortes import EvapCortes  # noqa
+from .evap_eco import EvapEco  # noqa
 from .energiaf import Energiaf  # noqa
 from .energiab import Energiab  # noqa
 from .energias import Energias  # noqa
 from .enavazf import Enavazf  # noqa
 from .enavazb import Enavazb  # noqa
 from .engnat import Engnat  # noqa
 from .vazaof import Vazaof  # noqa
```

### Comparing `inewave-1.7.5/inewave/newave/adterm.py` & `inewave-1.8.0/inewave/newave/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/agrint.py` & `inewave-1.8.0/inewave/newave/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/arquivos.py` & `inewave-1.8.0/inewave/newave/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-1.8.0/inewave/newave/fpha_cortes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from inewave.newave.modelos.blocos.versaomodelo import (
-    VersaoModelo,
     VersaoModeloLibs,
 )
 from inewave.newave.modelos.avl_cortesfpha_nwv import (
-    TabelaAvlCortesFpha28,
     TabelaAvlCortesFpha,
 )
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
 
-class AvlCortesFpha(ArquivoCSV):
+class FphaCortes(ArquivoCSV):
     """
     Arquivo com os cortes da função de produção para as UHEs
     do NEWAVE.
     """
 
     BLOCKS = [VersaoModeloLibs, TabelaAvlCortesFpha]
-    VERSIONS = {
-        "28": [VersaoModelo, TabelaAvlCortesFpha28],
-        "28.16": [VersaoModeloLibs, TabelaAvlCortesFpha],
-    }
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - codigo_usina (`int`)
```

### Comparing `inewave-1.7.5/inewave/newave/avl_desvfpha_s.py` & `inewave-1.8.0/inewave/newave/fpha_avl_desv_s.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.avl_desvfpha_s import TabelaAvlDesvFphaS
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
 
-class AvlDesvFphaS(BlockFile):
+class FphaAvlDesvS(BlockFile):
     """
     Arquivo com os desvios da função de produção no plano de
     vazão vertida (S).
     """
 
     BLOCKS = [VersaoModelo, TabelaAvlDesvFphaS]
     ENCODING = "iso-8859-1"
```

### Comparing `inewave-1.7.5/inewave/newave/avl_desvfpha_v_q.py` & `inewave-1.8.0/inewave/newave/fpha_avl_desv_v_q.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.avl_desvfpha_v_q import TabelaAvlDesvFphaVQ
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
 
-class AvlDesvFphaVQ(BlockFile):
+class FphaAvlDesvVQ(BlockFile):
     """
     Arquivo com os desvios da função de produção nos planos de
     volume armazenado e vazão turbinada (V-Q).
     """
 
     BLOCKS = [VersaoModelo, TabelaAvlDesvFphaVQ]
     ENCODING = "iso-8859-1"
```

### Comparing `inewave-1.7.5/inewave/newave/cadic.py` & `inewave-1.8.0/inewave/newave/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/caso.py` & `inewave-1.8.0/inewave/newave/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/clast.py` & `inewave-1.8.0/inewave/newave/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/confhd.py` & `inewave-1.8.0/inewave/newave/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/conft.py` & `inewave-1.8.0/inewave/newave/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/cortes.py` & `inewave-1.8.0/inewave/newave/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/cortesh.py` & `inewave-1.8.0/inewave/newave/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/curva.py` & `inewave-1.8.0/inewave/newave/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/cvar.py` & `inewave-1.8.0/inewave/newave/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/dger.py` & `inewave-1.8.0/inewave/newave/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/dsvagua.py` & `inewave-1.8.0/inewave/newave/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/eafpast.py` & `inewave-1.8.0/inewave/newave/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/eco_fpha.py` & `inewave-1.8.0/inewave/newave/fpha_eco.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.eco_fpha import TabelaEcoFpha
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
 
-class EcoFpha(ArquivoCSV):
+class FphaEco(ArquivoCSV):
     """
     Arquivo com o eco da função de produção para as UHEs
     do NEWAVE.
     """
 
     BLOCKS = [VersaoModelo, TabelaEcoFpha]
```

### Comparing `inewave-1.7.5/inewave/newave/enavazb.py` & `inewave-1.8.0/inewave/newave/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/enavazf.py` & `inewave-1.8.0/inewave/newave/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/energiab.py` & `inewave-1.8.0/inewave/newave/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/energiaf.py` & `inewave-1.8.0/inewave/newave/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/energias.py` & `inewave-1.8.0/inewave/newave/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/engnat.py` & `inewave-1.8.0/inewave/newave/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/exph.py` & `inewave-1.8.0/inewave/newave/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/expt.py` & `inewave-1.8.0/inewave/newave/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/forward.py` & `inewave-1.8.0/inewave/newave/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/forwarh.py` & `inewave-1.8.0/inewave/newave/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/ghmin.py` & `inewave-1.8.0/inewave/newave/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/hidr.py` & `inewave-1.8.0/inewave/newave/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/manutt.py` & `inewave-1.8.0/inewave/newave/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/adterm.py` & `inewave-1.8.0/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/agrint.py` & `inewave-1.8.0/inewave/newave/modelos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/arquivos.py` & `inewave-1.8.0/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-1.8.0/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-1.8.0/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-1.8.0/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-1.8.0/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-1.8.0/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-1.8.0/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/cadic.py` & `inewave-1.8.0/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/caso.py` & `inewave-1.8.0/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/clast.py` & `inewave-1.8.0/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/confhd.py` & `inewave-1.8.0/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/conft.py` & `inewave-1.8.0/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/cortes.py` & `inewave-1.8.0/inewave/newave/modelos/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/cortesh.py` & `inewave-1.8.0/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/curva.py` & `inewave-1.8.0/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/cvar.py` & `inewave-1.8.0/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/dger.py` & `inewave-1.8.0/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/dsvagua.py` & `inewave-1.8.0/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/eafpast.py` & `inewave-1.8.0/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/eco_fpha.py` & `inewave-1.8.0/inewave/newave/modelos/eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/enavazb.py` & `inewave-1.8.0/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/enavazf.py` & `inewave-1.8.0/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/energiab.py` & `inewave-1.8.0/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/energiaf.py` & `inewave-1.8.0/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/energias.py` & `inewave-1.8.0/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/engnat.py` & `inewave-1.8.0/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/exph.py` & `inewave-1.8.0/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/expt.py` & `inewave-1.8.0/inewave/newave/modelos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/forward.py` & `inewave-1.8.0/inewave/newave/modelos/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/forwarh.py` & `inewave-1.8.0/inewave/newave/modelos/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/ghmin.py` & `inewave-1.8.0/inewave/newave/modelos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/hidr.py` & `inewave-1.8.0/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/manutt.py` & `inewave-1.8.0/inewave/newave/modelos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/modif.py` & `inewave-1.8.0/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/newavetim.py` & `inewave-1.8.0/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-1.8.0/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-1.8.0/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-1.8.0/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/parp.py` & `inewave-1.8.0/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/parpeol.py` & `inewave-1.8.0/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/parpvaz.py` & `inewave-1.8.0/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/patamar.py` & `inewave-1.8.0/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/penalid.py` & `inewave-1.8.0/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/pmo.py` & `inewave-1.8.0/inewave/newave/modelos/pmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,54 @@
 from typing import IO, List, Optional
 from inewave._utils.formatacao import (
     prepara_vetor_anos_tabela,
     repete_vetor,
 )
 
 
+class BlocoVersaoModeloPMO(Block):
+    """
+    Bloco com a versão do modelo localizado no arquivo `pmo.dat`.
+    """
+
+    __slots__ = ["__line"]
+
+    BEGIN_PATTERN = (
+        " CEPEL                         MODELO ESTRATEGICO DE"
+        + " GERACAO HIDROTERMICA A SUBSISTEMAS              VERSAO"
+    )
+    END_PATTERN = ""
+
+    def __init__(self, previous=None, next=None, data=None) -> None:
+        super().__init__(previous, next, data)
+
+        self.__line = Line([LiteralField(18, 109)])
+
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, BlocoVersaoModeloPMO):
+            return False
+        bloco: BlocoVersaoModeloPMO = o
+        if not all(
+            [
+                isinstance(self.data, str),
+                isinstance(o.data, str),
+            ]
+        ):
+            return False
+        else:
+            return self.data == bloco.data
+
+    # Override
+    def read(self, file: IO, *args, **kwargs):
+
+        linha = file.readline()
+        dados: List[str] = self.__line.read(linha)
+        self.data = dados[0].strip()
+
+
 class BlocoEafPastTendenciaHidrolPMO(Block):
     """
     Bloco de informações de afluências passadas para
     tendência hidrológica localizado no arquivo `pmo.dat`.
     """
 
     __slots__ = ["__line"]
```

### Comparing `inewave-1.7.5/inewave/newave/modelos/re.py` & `inewave-1.8.0/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/ree.py` & `inewave-1.8.0/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/selcor.py` & `inewave-1.8.0/inewave/newave/modelos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/shist.py` & `inewave-1.8.0/inewave/newave/modelos/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/sistema.py` & `inewave-1.8.0/inewave/newave/modelos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/term.py` & `inewave-1.8.0/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazaob.py` & `inewave-1.8.0/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazaof.py` & `inewave-1.8.0/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazaos.py` & `inewave-1.8.0/inewave/newave/modelos/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazinat.py` & `inewave-1.8.0/inewave/newave/modelos/vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazoes.py` & `inewave-1.8.0/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/vazpast.py` & `inewave-1.8.0/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modelos/volref_saz.py` & `inewave-1.8.0/inewave/newave/modelos/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/modif.py` & `inewave-1.8.0/inewave/newave/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/newavetim.py` & `inewave-1.8.0/inewave/newave/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/nwv_avl_evap.py` & `inewave-1.8.0/inewave/newave/evap_avl_desv.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.nwv_avl_evap import TabelaAvlEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
 
-class NwvAvlEvap(ArquivoCSV):
+class EvapAvlDesv(ArquivoCSV):
     """
     Arquivo com a avaliação da evaporação linear do NEWAVE.
     """
 
     BLOCKS = [VersaoModelo, TabelaAvlEvap]
 
     @property
```

### Comparing `inewave-1.7.5/inewave/newave/nwv_cortes_evap.py` & `inewave-1.8.0/inewave/newave/evap_cortes.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.nwv_cortes_evap import TabelaCortesEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
 
-class NwvCortesEvap(ArquivoCSV):
+class EvapCortes(ArquivoCSV):
     """
     Arquivo com os cortes da evaporação linear do NEWAVE.
     """
 
     BLOCKS = [VersaoModelo, TabelaCortesEvap]
 
     @property
```

### Comparing `inewave-1.7.5/inewave/newave/nwv_eco_evap.py` & `inewave-1.8.0/inewave/newave/evap_eco.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from inewave.newave.modelos.nwv_eco_evap import TabelaEcoEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
 
-class NwvEcoEvap(ArquivoCSV):
+class EvapEco(ArquivoCSV):
     """
     Arquivo com o eco dos dados da evaporação linear do NEWAVE.
     """
 
     BLOCKS = [VersaoModelo, TabelaEcoEvap]
 
     @property
```

### Comparing `inewave-1.7.5/inewave/newave/parp.py` & `inewave-1.8.0/inewave/newave/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/parpeol.py` & `inewave-1.8.0/inewave/newave/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/parpvaz.py` & `inewave-1.8.0/inewave/newave/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/patamar.py` & `inewave-1.8.0/inewave/newave/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/penalid.py` & `inewave-1.8.0/inewave/newave/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/pmo.py` & `inewave-1.8.0/inewave/newave/pmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from inewave.newave.modelos.pmo import BlocoVersaoModeloPMO
 from inewave.newave.modelos.pmo import BlocoEafPastTendenciaHidrolPMO
 from inewave.newave.modelos.pmo import BlocoEafPastCfugaMedioPMO
 from inewave.newave.modelos.pmo import BlocoConvergenciaPMO
 from inewave.newave.modelos.pmo import BlocoConfiguracoesExpansaoPMO
 from inewave.newave.modelos.pmo import BlocoMARSPMO
 from inewave.newave.modelos.pmo import BlocoRiscoDeficitENSPMO
 from inewave.newave.modelos.pmo import BlocoCustoOperacaoPMO
@@ -44,14 +45,15 @@
     de execução intermediárias do programa.
 
     """
 
     T = TypeVar("T")
 
     BLOCKS = [
+        BlocoVersaoModeloPMO,
         BlocoEafPastTendenciaHidrolPMO,
         BlocoEafPastCfugaMedioPMO,
         BlocoConvergenciaPMO,
         BlocoConfiguracoesExpansaoPMO,
         BlocoMARSPMO,
         BlocoRiscoDeficitENSPMO,
         BlocoCustoOperacaoPMO,
@@ -68,14 +70,29 @@
         BlocoPenalidadeViolacaoTurbinamentoMaximoPMO,
         BlocoPenalidadeViolacaoTurbinamentoMinimoPMO,
         BlocoGeracaoMinimaUsinasTermicasPMO,
         BlocoGeracaoMaximaUsinasTermicasPMO,
     ]
 
     @property
+    def versao_modelo(self) -> Optional[str]:
+        """
+        A versão do modelo que produziu o arquivo.
+
+        :return: A string de versão do modelo.
+        :rtype: str | None
+        """
+        b = self.data.get_blocks_of_type(BlocoVersaoModeloPMO)
+        if isinstance(b, BlocoVersaoModeloPMO):
+            return b.data
+        elif isinstance(b, list):
+            return b[0].data
+        return None
+
+    @property
     def eafpast_tendencia_hidrologica(self) -> Optional[pd.DataFrame]:
         """
         Energias afluentes passadas por REE para análise da tendência
         hidrológica, em relação à primeira configuração do sistema,
         em MWmes.
 
         - nome_ree (`str`)
```

### Comparing `inewave-1.7.5/inewave/newave/re.py` & `inewave-1.8.0/inewave/newave/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/ree.py` & `inewave-1.8.0/inewave/newave/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/selcor.py` & `inewave-1.8.0/inewave/newave/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/shist.py` & `inewave-1.8.0/inewave/newave/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/sistema.py` & `inewave-1.8.0/inewave/newave/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/term.py` & `inewave-1.8.0/inewave/newave/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazaob.py` & `inewave-1.8.0/inewave/newave/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazaof.py` & `inewave-1.8.0/inewave/newave/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazaos.py` & `inewave-1.8.0/inewave/newave/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazinat.py` & `inewave-1.8.0/inewave/newave/vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazoes.py` & `inewave-1.8.0/inewave/newave/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/vazpast.py` & `inewave-1.8.0/inewave/newave/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/newave/volref_saz.py` & `inewave-1.8.0/inewave/newave/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/arquivos.py` & `inewave-1.8.0/inewave/nwlistcf/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/caso.py` & `inewave-1.8.0/inewave/nwlistcf/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/estados.py` & `inewave-1.8.0/inewave/nwlistcf/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/modelos/arquivos.py` & `inewave-1.8.0/inewave/nwlistcf/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/modelos/caso.py` & `inewave-1.8.0/inewave/nwlistcf/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/modelos/estados.py` & `inewave-1.8.0/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/modelos/nwlistcfdat.py` & `inewave-1.8.0/inewave/nwlistcf/modelos/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/modelos/nwlistcfrel.py` & `inewave-1.8.0/inewave/nwlistcf/modelos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/nwlistcfdat.py` & `inewave-1.8.0/inewave/nwlistcf/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistcf/nwlistcfrel.py` & `inewave-1.8.0/inewave/nwlistcf/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/__init__.py` & `inewave-1.8.0/inewave/nwlistop/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 # Inclui os membros
 
-from .nwlistopdat import Nwlistopdat  # noqa
+# Deprecated
 from .c_v_rhq_s import CVRHQs  # noqa
 from .c_v_rhq import CVRHQ  # noqa
 from .c_v_rhv_s import CVRHVs  # noqa
 from .c_v_rhv import CVRHV  # noqa
+from .celetricas import Celetricas  # noqa
+from .vdesviouh import Vdesviouh  # noqa
+from .vturuh import Vturuh  # noqa
+from .vertuh import Vertuh  # noqa
+from .vagua import Vagua  # noqa
+from .deletricas import Deletricas  # noqa
+from .vevmin import Vevmin  # noqa
+from .vevminm import Vevminm  # noqa
+from .vevminsin import Vevminsin  # noqa
+from .dfphauh import Dfphauh  # noqa
+from .vghmin import Vghmin  # noqa
+from .vghminm import Vghminm  # noqa
+from .vghminsin import Vghminsin  # noqa
+from .vghminuh import Vghminuh  # noqa
+from .dlppdfmax import Dlppdfmax  # noqa
+from .dlppdfmaxm import Dlppdfmaxm  # noqa
+from .dlppdfmaxs import Dlppdfmaxs  # noqa
+from .dlpptbmax import Dlpptbmax  # noqa
+from .dlpptbmaxm import Dlpptbmaxm  # noqa
+from .dlpptbmaxs import Dlpptbmaxs  # noqa
+from .dtbmax import Dtbmax  # noqa
+from .dtbmin import Dtbmin  # noqa
+from .dvazmax import Dvazmax  # noqa
+from .depminuh import Depminuh  # noqa
+from .desvuh import Desvuh  # noqa
+from .dposevap import Dposevap  # noqa
+from .dnegevap import Dnegevap  # noqa
+from .vbomb import Vbomb  # noqa
+
+from .nwlistopdat import Nwlistopdat  # noqa
+from .cviol_rhq_sin import CviolRhqsin  # noqa
+from .cviol_rhq import CviolRhq  # noqa
+from .cviol_rhv_sin import CviolRhvsin  # noqa
+from .cviol_rhv import CviolRhv  # noqa
 from .cbomb import Cbomb  # noqa
 from .cbombsin import Cbombsin  # noqa
 from .cdef import Cdef  # noqa
 from .cdefsin import Cdefsin  # noqa
-from .celetricas import Celetricas  # noqa
+from .cviol_eletricasin import CviolEletricasin  # noqa
 from .cmarg import Cmarg  # noqa
 from .cmargmed import Cmargmed  # noqa
 from .coper import Coper  # noqa
 from .corteolm import Corteolm  # noqa
 from .cterm import Cterm  # noqa
 from .ctermsin import Ctermsin  # noqa
 from .deficit import Def  # noqa
 from .defsin import Defsin  # noqa
-from .deletricas import Deletricas  # noqa
-from .depminuh import Depminuh  # noqa
-from .desvuh import Desvuh  # noqa
-from .dfphauh import Dfphauh  # noqa
-from .dlppdfmax import Dlppdfmax  # noqa
-from .dlppdfmaxs import Dlppdfmaxs  # noqa
-from .dlpptbmax import Dlpptbmax  # noqa
-from .dlpptbmaxm import Dlpptbmaxm  # noqa
-from .dlpptbmaxs import Dlpptbmaxs  # noqa
-from .dtbmax import Dtbmax  # noqa
-from .dtbmin import Dtbmin  # noqa
-from .dvazmax import Dvazmax  # noqa
 from .edesvc import Edesvc  # noqa
 from .edesvcm import Edesvcm  # noqa
 from .edesvcsin import Edesvcsin  # noqa
 from .evapo import Evapo  # noqa
 from .evapom import Evapom  # noqa
 from .evaporsin import Evaporsin  # noqa
 from .evert import Evert  # noqa
@@ -102,33 +124,46 @@
 from .perdfsin import Perdfsin  # noqa
 from .pivarm import Pivarm  # noqa
 from .pivarmincr import Pivarmincr  # noqa
 from .qafluh import Qafluh  # noqa
 from .qincruh import Qincruh  # noqa
 from .rhslppdf import Rhslppdf  # noqa
 from .rhslpptb import Rhslpptb  # noqa
-from .vagua import Vagua  # noqa
+from .valor_agua import ValorAgua  # noqa
 from .varmpuh import Varmpuh  # noqa
 from .varmuh import Varmuh  # noqa
-from .vbomb import Vbomb  # noqa
+from .qbomb import Qbomb  # noqa
 from .vento import Vento  # noqa
-from .vertuh import Vertuh  # noqa
+from .qvertuh import Qvertuh  # noqa
 from .verturb import Verturb  # noqa
 from .verturbm import Verturbm  # noqa
 from .verturbsin import Verturbsin  # noqa
-from .vevmin import Vevmin  # noqa
-from .vevminm import Vevminm  # noqa
-from .vevminsin import Vevminsin  # noqa
-from .vghmin import Vghmin  # noqa
-from .vghminm import Vghminm  # noqa
-from .vghminsin import Vghminsin  # noqa
-from .vghminuh import Vghminuh  # noqa
-from .viol_rhq import ViolRHQ  # noqa
-from .viol_rhv import ViolRHV  # noqa
-from .vturuh import Vturuh  # noqa
-from .vdesviouh import Vdesviouh  # noqa
+from .qturuh import Qturuh  # noqa
+from .qdesviouh import Qdesviouh  # noqa
 from .vmort import Vmort  # noqa
 from .vmortm import Vmortm  # noqa
 from .vmortsin import Vmortsin  # noqa
 from .vevapuh import Vevapuh  # noqa
-from .dposevap import Dposevap  # noqa
-from .dnegevap import Dnegevap  # noqa
+from .viol_eletricasin import ViolEletricasin  # noqa
+from .vretiradauh import Vretiradauh  # noqa
+from .viol_fpha import ViolFpha  # noqa
+from .viol_lpp_dfmax import ViolLppDfmax  # noqa
+from .viol_lpp_dfmaxm import ViolLppDfmaxm  # noqa
+from .viol_lpp_dfmaxsin import ViolLppDfmaxsin  # noqa
+from .viol_lpp_tbmax import ViolLppTbmax  # noqa
+from .viol_lpp_tbmaxm import ViolLppTbmaxm  # noqa
+from .viol_lpp_tbmaxsin import ViolLppTbmaxsin  # noqa
+from .viol_turbmax import ViolTurbmax  # noqa
+from .viol_turbmin import ViolTurbmin  # noqa
+from .viol_vazmax import ViolVazmax  # noqa
+from .viol_vazmin import ViolVazmin  # noqa
+from .viol_evmin import ViolEvmin  # noqa
+from .viol_evminm import ViolEvminm  # noqa
+from .viol_evminsin import ViolEvminsin  # noqa
+from .viol_ghmin import ViolGhmin  # noqa
+from .viol_ghminm import ViolGhminm  # noqa
+from .viol_ghminsin import ViolGhminsin  # noqa
+from .viol_ghminuh import ViolGhminuh  # noqa
+from .viol_rhq import ViolRHQ  # noqa
+from .viol_rhv import ViolRHV  # noqa
+from .viol_pos_evap import ViolPosEvap  # noqa
+from .viol_neg_evap import ViolNegEvap  # noqa
```

### Comparing `inewave-1.7.5/inewave/nwlistop/c_v_rhq.py` & `inewave-1.8.0/inewave/nwlistop/geol.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from inewave.nwlistop.modelos.blocos.restricao import Restricao
-from inewave.nwlistop.modelos.arquivos.arquivorestricaopatamar import (
-    ArquivoRestricaoPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.c_v_rhq import CVRHQAnos
+from inewave.nwlistop.modelos.geol import GEAnos
 
 
-class CVRHQ(ArquivoRestricaoPatamar):
+class Geol(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes ao custo de violação
-    de RHQ por restrição.
+    Armazena os dados das saídas referentes à geração eólica total
+    por patamar, por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `c_v_rhqXXX.out`.
+    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
+    PEE em questão.
 
     """
 
     BLOCKS = [
-        Restricao,
-        CVRHQAnos,
+        Usina,
+        GEAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/c_v_rhv.py` & `inewave-1.8.0/inewave/nwlistop/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/cbomb.py` & `inewave-1.8.0/inewave/nwlistop/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/cmarg.py` & `inewave-1.8.0/inewave/nwlistop/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/cmargmed.py` & `inewave-1.8.0/inewave/nwlistop/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/corteolm.py` & `inewave-1.8.0/inewave/nwlistop/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/cterm.py` & `inewave-1.8.0/inewave/nwlistop/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/deficit.py` & `inewave-1.8.0/inewave/nwlistop/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/depminuh.py` & `inewave-1.8.0/inewave/nwlistop/viol_vazmin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.depminuh import DepminAnos
+from inewave.nwlistop.modelos.viol_vazmin import ViolVazminAnos
 
 
-class Depminuh(ArquivoUsinaPatamar):
+class ViolVazmin(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes À violação de defluência
+    Armazena os dados das saídas referentes à violação de defluência
     mínima da usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `depminuh00x.out`, onde x varia conforme
+    NWLISTOP e reproduzidas nos `viol_vazmin00x.out`, onde x varia conforme
     a usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DepminAnos,
+        ViolVazminAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/desvuh.py` & `inewave-1.8.0/inewave/nwlistop/viol_lpp_dfmax.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousina import (
-    ArquivoUsina,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.desvuh import DesvuhAnos
+from inewave.nwlistop.modelos.viol_lpp_dfmax import ViolLppDfmaxAnos
 
 
-class Desvuh(ArquivoUsina):
+class ViolLppDfmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à retirada de água por usina.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de defluência máxima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `desvuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `viol_lpp_dfmax00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        DesvuhAnos,
+        REE,
+        ViolLppDfmaxAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/dfphauh.py` & `inewave-1.8.0/inewave/nwlistop/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dlppdfmax.py` & `inewave-1.8.0/inewave/nwlistop/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dlppdfmaxm.py` & `inewave-1.8.0/inewave/nwlistop/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dlpptbmax.py` & `inewave-1.8.0/inewave/nwlistop/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dlpptbmaxm.py` & `inewave-1.8.0/inewave/nwlistop/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dnegevap.py` & `inewave-1.8.0/inewave/nwlistop/dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dposevap.py` & `inewave-1.8.0/inewave/nwlistop/dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/dtbmax.py` & `inewave-1.8.0/inewave/nwlistop/viol_vazmax.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dtbmax import DtbmaxAnos
+from inewave.nwlistop.modelos.viol_vazmax import ViolVazmaxAnos
 
 
-class Dtbmax(ArquivoUsinaPatamar):
+class ViolVazmax(ArquivoUsinaPatamar):
     """
     Armazena os dados das saídas referentes à violação de restrição de
-    turbinamento máximo por usina.
+    vazão máxima por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dtbmax00x.out`, onde x varia conforme
+    NWLISTOP e reproduzidas nos `viol_vazmax00x.out`, onde x varia conforme
     a usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DtbmaxAnos,
+        ViolVazmaxAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/dtbmin.py` & `inewave-1.8.0/inewave/nwlistop/viol_fpha.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dtbmin import DtbminAnos
+from inewave.nwlistop.modelos.viol_fpha import ViolFphaAnos
 
 
-class Dtbmin(ArquivoUsinaPatamar):
+class ViolFpha(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação de restrição de
-    turbinamento mínimo por usina.
+    Armazena os dados das saídas referentes à variável de folga da
+    FPHA da usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dtbmin00x.out`, onde x varia conforme
+    NWLISTOP e reproduzidas nos `viol_fpha00x.out`, onde x varia conforme
     a usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DtbminAnos,
+        ViolFphaAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/dvazmax.py` & `inewave-1.8.0/inewave/nwlistop/ghtot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.dvazmax import DvazmaxAnos
+from inewave.nwlistop.modelos.ghtot import GHAnos
 
 
-class Dvazmax(ArquivoUsinaPatamar):
+class Ghtot(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à violação de restrição de
-    vazão máxima por usina.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dvazmax00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        DvazmaxAnos,
+        REE,
+        GHAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/eafb.py` & `inewave-1.8.0/inewave/nwlistop/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/eafbm.py` & `inewave-1.8.0/inewave/nwlistop/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/eafm.py` & `inewave-1.8.0/inewave/nwlistop/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/earmf.py` & `inewave-1.8.0/inewave/nwlistop/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/earmfm.py` & `inewave-1.8.0/inewave/nwlistop/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/earmfp.py` & `inewave-1.8.0/inewave/nwlistop/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/earmfpm.py` & `inewave-1.8.0/inewave/nwlistop/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/earmfpsin.py` & `inewave-1.8.0/inewave/nwlistop/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/edesvc.py` & `inewave-1.8.0/inewave/nwlistop/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/edesvcm.py` & `inewave-1.8.0/inewave/nwlistop/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/evapo.py` & `inewave-1.8.0/inewave/nwlistop/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/evapom.py` & `inewave-1.8.0/inewave/nwlistop/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/evert.py` & `inewave-1.8.0/inewave/nwlistop/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/evertm.py` & `inewave-1.8.0/inewave/nwlistop/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/exces.py` & `inewave-1.8.0/inewave/nwlistop/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/form_rhq.py` & `inewave-1.8.0/inewave/nwlistop/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/form_rhv.py` & `inewave-1.8.0/inewave/nwlistop/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/fteolm.py` & `inewave-1.8.0/inewave/nwlistop/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/geol.py` & `inewave-1.8.0/inewave/nwlistop/ghiduh.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.geol import GEAnos
+from inewave.nwlistop.modelos.ghiduh import GhidAnos
 
 
-class Geol(ArquivoUsinaPatamar):
+class Ghiduh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração eólica total
-    por patamar, por usina.
+    Armazena os dados das saídas referentes à geração hidráulica por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
-    PEE em questão.
+    NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        GEAnos,
+        GhidAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/geolm.py` & `inewave-1.8.0/inewave/nwlistop/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/gh_fphexat.py` & `inewave-1.8.0/inewave/nwlistop/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghidr.py` & `inewave-1.8.0/inewave/nwlistop/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghidrm.py` & `inewave-1.8.0/inewave/nwlistop/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghiduh.py` & `inewave-1.8.0/inewave/nwlistop/qturuh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.ghiduh import GhidAnos
+from inewave.nwlistop.modelos.qturuh import QturAnos
 
 
-class Ghiduh(ArquivoUsinaPatamar):
+class Qturuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidráulica por usina.
+    Armazena os dados das saídas referentes às vazões turbinadas por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `qturuh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        GhidAnos,
+        QturAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmax.py` & `inewave-1.8.0/inewave/nwlistop/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmax_fpha.py` & `inewave-1.8.0/inewave/nwlistop/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmax_fphc.py` & `inewave-1.8.0/inewave/nwlistop/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmaxm.py` & `inewave-1.8.0/inewave/nwlistop/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmaxmr.py` & `inewave-1.8.0/inewave/nwlistop/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghmaxr.py` & `inewave-1.8.0/inewave/nwlistop/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/ghtot.py` & `inewave-1.8.0/inewave/nwlistop/viol_lpp_tbmax.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.ghtot import GHAnos
+from inewave.nwlistop.modelos.viol_lpp_tbmax import ViolLppTbmaxAnos
 
 
-class Ghtot(ArquivoREEPatamar):
+class ViolLppTbmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
-    por patamar, por REE.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de turbinamento máximo por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `viol_lpp_tbmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        GHAnos,
+        ViolLppTbmaxAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/ghtotm.py` & `inewave-1.8.0/inewave/nwlistop/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/gtert.py` & `inewave-1.8.0/inewave/nwlistop/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/gttot.py` & `inewave-1.8.0/inewave/nwlistop/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/hjus.py` & `inewave-1.8.0/inewave/nwlistop/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/hliq.py` & `inewave-1.8.0/inewave/nwlistop/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/hmont.py` & `inewave-1.8.0/inewave/nwlistop/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/intercambio.py` & `inewave-1.8.0/inewave/nwlistop/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/invade.py` & `inewave-1.8.0/inewave/nwlistop/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/invadem.py` & `inewave-1.8.0/inewave/nwlistop/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasmerc.py` & `inewave-1.8.0/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasree.py` & `inewave-1.8.0/inewave/nwlistop/mediasree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasrep.py` & `inewave-1.8.0/inewave/nwlistop/mediasrep.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasrhq.py` & `inewave-1.8.0/inewave/nwlistop/mediasrhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasrhv.py` & `inewave-1.8.0/inewave/nwlistop/mediasrhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediassin.py` & `inewave-1.8.0/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasusie.py` & `inewave-1.8.0/inewave/nwlistop/mediasusie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasusih.py` & `inewave-1.8.0/inewave/nwlistop/mediasusih.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mediasusit.py` & `inewave-1.8.0/inewave/nwlistop/mediasusit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mercl.py` & `inewave-1.8.0/inewave/nwlistop/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mevmin.py` & `inewave-1.8.0/inewave/nwlistop/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/mevminm.py` & `inewave-1.8.0/inewave/nwlistop/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivorestricao.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivorestricao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivorestricaopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/estacaobombeamento.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/estacaobombeamento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/restricao.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/restricao.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-1.8.0/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhq.py` & `inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhq_s.py` & `inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhv.py` & `inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/c_v_rhv_s.py` & `inewave-1.8.0/inewave/nwlistop/modelos/c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cbomb.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cbombsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cdef.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cdefsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/celetricas.py` & `inewave-1.8.0/inewave/nwlistop/modelos/celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cmarg.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cmargmed.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/coper.py` & `inewave-1.8.0/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/corteolm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/cterm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ctermsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/def.py` & `inewave-1.8.0/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/defsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/deletricas.py` & `inewave-1.8.0/inewave/nwlistop/modelos/deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/depminuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/desvuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dfphauh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dnegevap.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dposevap.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dtbmax.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dtbmin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/dvazmax.py` & `inewave-1.8.0/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/eaf.py` & `inewave-1.8.0/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/eafb.py` & `inewave-1.8.0/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/eafbm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/eafbsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/eafm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmf.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmfm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmfp.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmfpm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/earmfsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/edesvc.py` & `inewave-1.8.0/inewave/nwlistop/modelos/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/edesvcm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/edesvcsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evapo.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evapom.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evaporsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evert.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evertm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/evertsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/exces.py` & `inewave-1.8.0/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/excessin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/form_rhq.py` & `inewave-1.8.0/inewave/nwlistop/modelos/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/form_rhv.py` & `inewave-1.8.0/inewave/nwlistop/modelos/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/fteolm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/fteolsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/geol.py` & `inewave-1.8.0/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/geolm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/geolsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/gh_fphexat.py` & `inewave-1.8.0/inewave/nwlistop/modelos/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghidr.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghidrm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghidrsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghiduh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmax.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmax_fpha.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmax_fphc.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghtot.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghtotm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/gtert.py` & `inewave-1.8.0/inewave/nwlistop/modelos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/gttot.py` & `inewave-1.8.0/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/gttotsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/hjus.py` & `inewave-1.8.0/inewave/nwlistop/modelos/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/hliq.py` & `inewave-1.8.0/inewave/nwlistop/modelos/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/hmont.py` & `inewave-1.8.0/inewave/nwlistop/modelos/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/intercambio.py` & `inewave-1.8.0/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/invade.py` & `inewave-1.8.0/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/invadem.py` & `inewave-1.8.0/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasree.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasrep.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasrep.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasrhq.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasrhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasrhv.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasrhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediassin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasusie.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasusie.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasusih.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasusih.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mediasusit.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mediasusit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mercl.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/merclsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mevmin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mevminm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/mevminsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/nwlistopdat.py` & `inewave-1.8.0/inewave/nwlistop/modelos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/perdf.py` & `inewave-1.8.0/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/perdfm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/perdfsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/pivarm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/varmpuh.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class PivarmAnos(ValoresSerie):
+class VarmAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de valor de água por
+    Bloco com as informações das tabelas de volume armazenado por
     usina por mês/ano de estudo.
     """
 
     __slots__ = []
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(15, 7 + 15 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/pivarmincr.py` & `inewave-1.8.0/inewave/nwlistop/modelos/varmuh.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class PivarmAnos(ValoresSerie):
+class VarmAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de valor de água por
+    Bloco com as informações das tabelas de volume armazenado por
     usina por mês/ano de estudo.
     """
 
     __slots__ = []
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(15, 7 + 15 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/qafluh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/qincruh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-1.8.0/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-1.8.0/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vagua.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/varmpuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vento.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class VarmAnos(ValoresSerie):
+class VentoAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de volume armazenado por
+    Bloco com as informações das tabelas de vento por
     usina por mês/ano de estudo.
     """
 
     __slots__ = []
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
+        + [FloatField(9, 6 + 9 * i, 4) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/varmuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/qturuh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 
-class VarmAnos(ValoresSerie):
+class QturAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de volume armazenado por
+    Bloco com as informações das tabelas de vazão turbinada por
     usina por mês/ano de estudo.
     """
 
     __slots__ = []
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
+            LiteralField(5, 6),
         ]
         + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vbomb.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vdesviouh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vento.py` & `inewave-1.8.0/inewave/nwlistop/modelos/viol_neg_evap.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class VentoAnos(ValoresSerie):
+class ViolNegEvapAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vento por
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de desvio negativo
+    da evaporação por usina por mês/ano de estudo.
     """
 
     __slots__ = []
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 6 + 9 * i, 4) for i in range(len(MESES_DF))]  # type: ignore
+        + [FloatField(14, 15 + 15 * i, 7, format="E") for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vertuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/verturb.py` & `inewave-1.8.0/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/verturbm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/verturbsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vevapuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vevmin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vevminm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vevminsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vghmin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vghminm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vghminsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vghminuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/viol_rhq.py` & `inewave-1.8.0/inewave/nwlistop/modelos/viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/viol_rhv.py` & `inewave-1.8.0/inewave/nwlistop/modelos/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vmort.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vmortm.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vmortsin.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/modelos/vturuh.py` & `inewave-1.8.0/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/nwlistopdat.py` & `inewave-1.8.0/inewave/nwlistop/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/perdf.py` & `inewave-1.8.0/inewave/nwlistop/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/perdfm.py` & `inewave-1.8.0/inewave/nwlistop/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/pivarm.py` & `inewave-1.8.0/inewave/nwlistop/varmpuh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousina import (
     ArquivoUsina,
 )
-from inewave.nwlistop.modelos.pivarm import PivarmAnos
+from inewave.nwlistop.modelos.varmpuh import VarmAnos
 
 
-class Pivarm(ArquivoUsina):
+class Varmpuh(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes aos valores da água
-    por usina.
+    Armazena os dados das saídas referentes aos armazenamentos em
+    percentual por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `pivarm00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `varmpuh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        PivarmAnos,
+        VarmAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/pivarmincr.py` & `inewave-1.8.0/inewave/nwlistop/vretiradauh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousina import (
     ArquivoUsina,
 )
-from inewave.nwlistop.modelos.pivarmincr import PivarmAnos
+from inewave.nwlistop.modelos.vretiradauh import VretiradauhAnos
 
 
-class Pivarmincr(ArquivoUsina):
+class Vretiradauh(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes aos valores da água
-    incrementais por usina.
+    Armazena os dados das saídas referentes à retirada de água por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `pivarmincr00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `vretiradauh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        PivarmAnos,
+        VretiradauhAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/qafluh.py` & `inewave-1.8.0/inewave/nwlistop/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/qincruh.py` & `inewave-1.8.0/inewave/nwlistop/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/rhslppdf.py` & `inewave-1.8.0/inewave/nwlistop/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/rhslpptb.py` & `inewave-1.8.0/inewave/nwlistop/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/varmpuh.py` & `inewave-1.8.0/inewave/nwlistop/qvertuh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousina import (
-    ArquivoUsina,
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.varmpuh import VarmAnos
+from inewave.nwlistop.modelos.qvertuh import QvertuhAnos
 
 
-class Varmpuh(ArquivoUsina):
+class Qvertuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes aos armazenamentos em
-    percentual por usina.
+    Armazena os dados das saídas referentes aos vertimentos por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `varmpuh00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `qvertuh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        VarmAnos,
+        QvertuhAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/varmuh.py` & `inewave-1.8.0/inewave/nwlistop/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vbomb.py` & `inewave-1.8.0/inewave/nwlistop/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vdesviouh.py` & `inewave-1.8.0/inewave/nwlistop/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vento.py` & `inewave-1.8.0/inewave/nwlistop/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vertuh.py` & `inewave-1.8.0/inewave/nwlistop/cviol_rhv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.restricao import Restricao
+from inewave.nwlistop.modelos.arquivos.arquivorestricao import (
+    ArquivoRestricao,
 )
-from inewave.nwlistop.modelos.vertuh import VertAnos
+from inewave.nwlistop.modelos.cviol_rhv import CviolRhvAnos
 
 
-class Vertuh(ArquivoUsinaPatamar):
+class CviolRhv(ArquivoRestricao):
     """
-    Armazena os dados das saídas referentes aos vertimentos por usina.
+    Armazena os dados das saídas referentes ao custo de violação
+    de RHV por restrição.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `cviol_rhvXXX.out`.
 
     """
 
     BLOCKS = [
-        Usina,
-        VertAnos,
+        Restricao,
+        CviolRhvAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/verturb.py` & `inewave-1.8.0/inewave/nwlistop/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/verturbm.py` & `inewave-1.8.0/inewave/nwlistop/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vevapuh.py` & `inewave-1.8.0/inewave/nwlistop/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vevmin.py` & `inewave-1.8.0/inewave/nwlistop/viol_rhq.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-from inewave.nwlistop.modelos.vevmin import VevminAnos
+from inewave.nwlistop.modelos.blocos.restricao import Restricao
+from inewave.nwlistop.modelos.arquivos.arquivorestricaopatamar import (
+    ArquivoRestricaoPatamar,
+)
+from inewave.nwlistop.modelos.viol_rhq import ViolRHQAnos
 
 
-class Vevmin(ArquivoREE):
+class ViolRHQ(ArquivoRestricaoPatamar):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por REE.
+    Armazena os dados das saídas referentes aos valores das restrições
+    RHQ por restrição.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevmin00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `viol_rhqXXX.out`.
 
     """
 
     BLOCKS = [
-        REE,
-        VevminAnos,
+        Restricao,
+        ViolRHQAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/vevminm.py` & `inewave-1.8.0/inewave/nwlistop/valor_agua.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
-)
-from inewave.nwlistop.modelos.vevminm import VevminAnos
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
 
+from inewave.nwlistop.modelos.valor_agua import ValorAguaAnos
 
-class Vevminm(ArquivoSubmercado):
+
+class ValorAgua(ArquivoREE):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por Submercado.
+    Armazena os dados das saídas referentes aos valores da água
+    por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `valor_agua00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        Submercado,
-        VevminAnos,
+        REE,
+        ValorAguaAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/vghmin.py` & `inewave-1.8.0/inewave/nwlistop/vghminuh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vghmin import VghminAnos
+from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
 
 
-class Vghmin(ArquivoREEPatamar):
+class Vghminuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação da meta de geração
-    hidraulica mínima por patamar, por REE.
+    Armazena os dados das saídas referentes à violação da meta de
+    geração hidráulica mínima por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghmin00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `vghminuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        VghminAnos,
+        Usina,
+        VGhminuhAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/vghminm.py` & `inewave-1.8.0/inewave/nwlistop/viol_ghminm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.vghminm import VghminAnos
+from inewave.nwlistop.modelos.viol_ghminm import ViolGhminmAnos
 
 
-class Vghminm(ArquivoSubmercadoPatamar):
+class ViolGhminm(ArquivoSubmercadoPatamar):
     """
     Armazena os dados das saídas referentes à violação da meta de geração
     hidráulica mínima por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghmin00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `viol_ghminm00x.out`, onde x varia conforme o
     Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        VghminAnos,
+        ViolGhminmAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/vghminuh.py` & `inewave-1.8.0/inewave/nwlistop/qdesviouh.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
+from inewave.nwlistop.modelos.qdesviouh import QdesviouhAnos
 
 
-class Vghminuh(ArquivoUsinaPatamar):
+class Qdesviouh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação da meta de
-    geração hidráulica mínima por usina.
+    Armazena os dados das saídas referentes ao desvio de água por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghminuh00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `qdesviouh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        VGhminuhAnos,
+        QdesviouhAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/viol_rhq.py` & `inewave-1.8.0/inewave/nwlistop/viol_neg_evap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from inewave.nwlistop.modelos.blocos.restricao import Restricao
-from inewave.nwlistop.modelos.arquivos.arquivorestricaopatamar import (
-    ArquivoRestricaoPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
-from inewave.nwlistop.modelos.viol_rhq import ViolRHQAnos
+from inewave.nwlistop.modelos.viol_neg_evap import ViolNegEvapAnos
 
 
-class ViolRHQ(ArquivoRestricaoPatamar):
+class ViolNegEvap(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes aos valores das restrições
-    RHQ por restrição.
+    Armazena os dados das saídas referentes ao desvios negativos da
+    evaporação da usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `viol_rhqXXX.out`.
+    NWLISTOP e reproduzidas nos `viol_neg_evap00x.out`, onde x varia conforme
+    a usina em questão.
 
     """
 
     BLOCKS = [
-        Restricao,
-        ViolRHQAnos,
+        Usina,
+        ViolNegEvapAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave/nwlistop/viol_rhv.py` & `inewave-1.8.0/inewave/nwlistop/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vmort.py` & `inewave-1.8.0/inewave/nwlistop/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vmortm.py` & `inewave-1.8.0/inewave/nwlistop/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/inewave/nwlistop/vturuh.py` & `inewave-1.8.0/inewave/nwlistop/viol_lpp_dfmaxsin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.vturuh import VturAnos
+from inewave.nwlistop.modelos.viol_lpp_dfmaxsin import ViolLppDfmaxsinAnos
 
 
-class Vturuh(ArquivoUsinaPatamar):
+class ViolLppDfmaxsin(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes às vazões turbinadas por usina.
+    Armazena os dados das saídas referentes à violação das restrições
+    LPP de defluência máxima por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
-    usina em questão.
-
+    NWLISTOP e reproduzidas nos `viol_lpp_dfmaxsin.out`.
     """
 
     BLOCKS = [
-        Usina,
-        VturAnos,
+        ViolLppDfmaxsinAnos,
     ]
```

### Comparing `inewave-1.7.5/inewave.egg-info/PKG-INFO` & `inewave-1.8.0/inewave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 1.7.5
+Version: 1.8.0
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-1.7.5/inewave.egg-info/SOURCES.txt` & `inewave-1.8.0/inewave.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -51,18 +51,25 @@
 inewave/newave/enavazb.py
 inewave/newave/enavazf.py
 inewave/newave/energiab.py
 inewave/newave/energiaf.py
 inewave/newave/energias.py
 inewave/newave/engnat.py
 inewave/newave/ensoaux.py
+inewave/newave/evap_avl_desv.py
+inewave/newave/evap_cortes.py
+inewave/newave/evap_eco.py
 inewave/newave/exph.py
 inewave/newave/expt.py
 inewave/newave/forward.py
 inewave/newave/forwarh.py
+inewave/newave/fpha_avl_desv_s.py
+inewave/newave/fpha_avl_desv_v_q.py
+inewave/newave/fpha_cortes.py
+inewave/newave/fpha_eco.py
 inewave/newave/gee.py
 inewave/newave/ghmin.py
 inewave/newave/gtminpat.py
 inewave/newave/hidr.py
 inewave/newave/itaipu.py
 inewave/newave/manutt.py
 inewave/newave/modif.py
@@ -189,14 +196,19 @@
 inewave/nwlistop/celetricas.py
 inewave/nwlistop/cmarg.py
 inewave/nwlistop/cmargmed.py
 inewave/nwlistop/coper.py
 inewave/nwlistop/corteolm.py
 inewave/nwlistop/cterm.py
 inewave/nwlistop/ctermsin.py
+inewave/nwlistop/cviol_eletricasin.py
+inewave/nwlistop/cviol_rhq.py
+inewave/nwlistop/cviol_rhq_sin.py
+inewave/nwlistop/cviol_rhv.py
+inewave/nwlistop/cviol_rhv_sin.py
 inewave/nwlistop/deficit.py
 inewave/nwlistop/defsin.py
 inewave/nwlistop/deletricas.py
 inewave/nwlistop/depminuh.py
 inewave/nwlistop/desvuh.py
 inewave/nwlistop/dfphauh.py
 inewave/nwlistop/dlppdfmax.py
@@ -281,18 +293,23 @@
 inewave/nwlistop/nwlistopdat.py
 inewave/nwlistop/perdf.py
 inewave/nwlistop/perdfm.py
 inewave/nwlistop/perdfsin.py
 inewave/nwlistop/pivarm.py
 inewave/nwlistop/pivarmincr.py
 inewave/nwlistop/qafluh.py
+inewave/nwlistop/qbomb.py
+inewave/nwlistop/qdesviouh.py
 inewave/nwlistop/qincruh.py
+inewave/nwlistop/qturuh.py
+inewave/nwlistop/qvertuh.py
 inewave/nwlistop/rhslppdf.py
 inewave/nwlistop/rhslpptb.py
 inewave/nwlistop/vagua.py
+inewave/nwlistop/valor_agua.py
 inewave/nwlistop/varmpuh.py
 inewave/nwlistop/varmuh.py
 inewave/nwlistop/vbomb.py
 inewave/nwlistop/vdesviouh.py
 inewave/nwlistop/vento.py
 inewave/nwlistop/vertuh.py
 inewave/nwlistop/verturb.py
@@ -302,19 +319,41 @@
 inewave/nwlistop/vevmin.py
 inewave/nwlistop/vevminm.py
 inewave/nwlistop/vevminsin.py
 inewave/nwlistop/vghmin.py
 inewave/nwlistop/vghminm.py
 inewave/nwlistop/vghminsin.py
 inewave/nwlistop/vghminuh.py
+inewave/nwlistop/viol_eletricasin.py
+inewave/nwlistop/viol_evmin.py
+inewave/nwlistop/viol_evminm.py
+inewave/nwlistop/viol_evminsin.py
+inewave/nwlistop/viol_fpha.py
+inewave/nwlistop/viol_ghmin.py
+inewave/nwlistop/viol_ghminm.py
+inewave/nwlistop/viol_ghminsin.py
+inewave/nwlistop/viol_ghminuh.py
+inewave/nwlistop/viol_lpp_dfmax.py
+inewave/nwlistop/viol_lpp_dfmaxm.py
+inewave/nwlistop/viol_lpp_dfmaxsin.py
+inewave/nwlistop/viol_lpp_tbmax.py
+inewave/nwlistop/viol_lpp_tbmaxm.py
+inewave/nwlistop/viol_lpp_tbmaxsin.py
+inewave/nwlistop/viol_neg_evap.py
+inewave/nwlistop/viol_pos_evap.py
 inewave/nwlistop/viol_rhq.py
 inewave/nwlistop/viol_rhv.py
+inewave/nwlistop/viol_turbmax.py
+inewave/nwlistop/viol_turbmin.py
+inewave/nwlistop/viol_vazmax.py
+inewave/nwlistop/viol_vazmin.py
 inewave/nwlistop/vmort.py
 inewave/nwlistop/vmortm.py
 inewave/nwlistop/vmortsin.py
+inewave/nwlistop/vretiradauh.py
 inewave/nwlistop/vturuh.py
 inewave/nwlistop/modelos/__init__.py
 inewave/nwlistop/modelos/c_v_rhq.py
 inewave/nwlistop/modelos/c_v_rhq_s.py
 inewave/nwlistop/modelos/c_v_rhv.py
 inewave/nwlistop/modelos/c_v_rhv_s.py
 inewave/nwlistop/modelos/cbomb.py
@@ -324,14 +363,19 @@
 inewave/nwlistop/modelos/celetricas.py
 inewave/nwlistop/modelos/cmarg.py
 inewave/nwlistop/modelos/cmargmed.py
 inewave/nwlistop/modelos/coper.py
 inewave/nwlistop/modelos/corteolm.py
 inewave/nwlistop/modelos/cterm.py
 inewave/nwlistop/modelos/ctermsin.py
+inewave/nwlistop/modelos/cviol_eletricasin.py
+inewave/nwlistop/modelos/cviol_rhq.py
+inewave/nwlistop/modelos/cviol_rhq_sin.py
+inewave/nwlistop/modelos/cviol_rhv.py
+inewave/nwlistop/modelos/cviol_rhv_sin.py
 inewave/nwlistop/modelos/def.py
 inewave/nwlistop/modelos/defsin.py
 inewave/nwlistop/modelos/deletricas.py
 inewave/nwlistop/modelos/depminuh.py
 inewave/nwlistop/modelos/desvuh.py
 inewave/nwlistop/modelos/dflppdfmaxm.py
 inewave/nwlistop/modelos/dflpptbmaxm.py
@@ -416,18 +460,23 @@
 inewave/nwlistop/modelos/nwlistopdat.py
 inewave/nwlistop/modelos/perdf.py
 inewave/nwlistop/modelos/perdfm.py
 inewave/nwlistop/modelos/perdfsin.py
 inewave/nwlistop/modelos/pivarm.py
 inewave/nwlistop/modelos/pivarmincr.py
 inewave/nwlistop/modelos/qafluh.py
+inewave/nwlistop/modelos/qbomb.py
+inewave/nwlistop/modelos/qdesviouh.py
 inewave/nwlistop/modelos/qincruh.py
+inewave/nwlistop/modelos/qturuh.py
+inewave/nwlistop/modelos/qvertuh.py
 inewave/nwlistop/modelos/rhslppdf.py
 inewave/nwlistop/modelos/rhslpptb.py
 inewave/nwlistop/modelos/vagua.py
+inewave/nwlistop/modelos/valor_agua.py
 inewave/nwlistop/modelos/varmpuh.py
 inewave/nwlistop/modelos/varmuh.py
 inewave/nwlistop/modelos/vbomb.py
 inewave/nwlistop/modelos/vdesviouh.py
 inewave/nwlistop/modelos/vento.py
 inewave/nwlistop/modelos/vertuh.py
 inewave/nwlistop/modelos/verturb.py
@@ -437,19 +486,41 @@
 inewave/nwlistop/modelos/vevmin.py
 inewave/nwlistop/modelos/vevminm.py
 inewave/nwlistop/modelos/vevminsin.py
 inewave/nwlistop/modelos/vghmin.py
 inewave/nwlistop/modelos/vghminm.py
 inewave/nwlistop/modelos/vghminsin.py
 inewave/nwlistop/modelos/vghminuh.py
+inewave/nwlistop/modelos/viol_eletricasin.py
+inewave/nwlistop/modelos/viol_evmin.py
+inewave/nwlistop/modelos/viol_evminm.py
+inewave/nwlistop/modelos/viol_evminsin.py
+inewave/nwlistop/modelos/viol_fpha.py
+inewave/nwlistop/modelos/viol_ghmin.py
+inewave/nwlistop/modelos/viol_ghminm.py
+inewave/nwlistop/modelos/viol_ghminsin.py
+inewave/nwlistop/modelos/viol_ghminuh.py
+inewave/nwlistop/modelos/viol_lpp_dfmax.py
+inewave/nwlistop/modelos/viol_lpp_dfmaxm.py
+inewave/nwlistop/modelos/viol_lpp_dfmaxsin.py
+inewave/nwlistop/modelos/viol_lpp_tbmax.py
+inewave/nwlistop/modelos/viol_lpp_tbmaxm.py
+inewave/nwlistop/modelos/viol_lpp_tbmaxsin.py
+inewave/nwlistop/modelos/viol_neg_evap.py
+inewave/nwlistop/modelos/viol_pos_evap.py
 inewave/nwlistop/modelos/viol_rhq.py
 inewave/nwlistop/modelos/viol_rhv.py
+inewave/nwlistop/modelos/viol_turbmax.py
+inewave/nwlistop/modelos/viol_turbmin.py
+inewave/nwlistop/modelos/viol_vazmax.py
+inewave/nwlistop/modelos/viol_vazmin.py
 inewave/nwlistop/modelos/vmort.py
 inewave/nwlistop/modelos/vmortm.py
 inewave/nwlistop/modelos/vmortsin.py
+inewave/nwlistop/modelos/vretiradauh.py
 inewave/nwlistop/modelos/vturuh.py
 inewave/nwlistop/modelos/arquivos/__init__.py
 inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivoestacaobombeamentopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivoree.py
 inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
@@ -642,14 +713,15 @@
 tests/mocks/arquivos/vevmin.py
 tests/mocks/arquivos/vevminm.py
 tests/mocks/arquivos/vevminsin.py
 tests/mocks/arquivos/vghmin.py
 tests/mocks/arquivos/vghminm.py
 tests/mocks/arquivos/vghminsin.py
 tests/mocks/arquivos/vghminuh.py
+tests/mocks/arquivos/viol_fpha.py
 tests/mocks/arquivos/viol_rhq.py
 tests/mocks/arquivos/viol_rhv.py
 tests/mocks/arquivos/vmort.py
 tests/mocks/arquivos/vmortm.py
 tests/mocks/arquivos/vmortsin.py
 tests/mocks/arquivos/volref_saz.py
 tests/mocks/arquivos/vturuh.py
@@ -675,18 +747,25 @@
 tests/newave/test_eco_fpha.py
 tests/newave/test_enavazb.py
 tests/newave/test_enavazf.py
 tests/newave/test_energiab.py
 tests/newave/test_energiaf.py
 tests/newave/test_energias.py
 tests/newave/test_engnat.py
+tests/newave/test_evap_avl_desv.py
+tests/newave/test_evap_cortes.py
+tests/newave/test_evap_eco.py
 tests/newave/test_exph.py
 tests/newave/test_expt.py
 tests/newave/test_forward.py
 tests/newave/test_forwarh.py
+tests/newave/test_fpha_avl_desv_s.py
+tests/newave/test_fpha_avl_desv_v_q.py
+tests/newave/test_fpha_cortes.py
+tests/newave/test_fpha_eco.py
 tests/newave/test_ghmin.py
 tests/newave/test_hidr.py
 tests/newave/test_manutt.py
 tests/newave/test_modif.py
 tests/newave/test_newavetim.py
 tests/newave/test_nwv_avl_evap.py
 tests/newave/test_nwv_cortes_evap.py
@@ -728,14 +807,17 @@
 tests/nwlistop/test_celetricas.py
 tests/nwlistop/test_cmarg.py
 tests/nwlistop/test_cmargmed.py
 tests/nwlistop/test_coper.py
 tests/nwlistop/test_corteolm.py
 tests/nwlistop/test_cterm.py
 tests/nwlistop/test_ctermsin.py
+tests/nwlistop/test_cviol_eletricasin.py
+tests/nwlistop/test_cviol_rhq_sin.py
+tests/nwlistop/test_cviol_rhv_sin.py
 tests/nwlistop/test_deficit.py
 tests/nwlistop/test_defsin.py
 tests/nwlistop/test_deletricas.py
 tests/nwlistop/test_depminuh.py
 tests/nwlistop/test_desvuh.py
 tests/nwlistop/test_dfphauh.py
 tests/nwlistop/test_dlppdfmax.py
@@ -820,18 +902,23 @@
 tests/nwlistop/test_nwlistopdat.py
 tests/nwlistop/test_perdf.py
 tests/nwlistop/test_perdfm.py
 tests/nwlistop/test_perdfsin.py
 tests/nwlistop/test_pivarm.py
 tests/nwlistop/test_pivarmincr.py
 tests/nwlistop/test_qafluh.py
+tests/nwlistop/test_qbomb.py
+tests/nwlistop/test_qdesviouh.py
 tests/nwlistop/test_qincruh.py
+tests/nwlistop/test_qturuh.py
+tests/nwlistop/test_qvertuh.py
 tests/nwlistop/test_rhslppdf.py
 tests/nwlistop/test_rhslpptb.py
 tests/nwlistop/test_vagua.py
+tests/nwlistop/test_valor_agua.py
 tests/nwlistop/test_varmpuh.py
 tests/nwlistop/test_varmuh.py
 tests/nwlistop/test_vbomb.py
 tests/nwlistop/test_vdesviouh.py
 tests/nwlistop/test_vento.py
 tests/nwlistop/test_vertuh.py
 tests/nwlistop/test_verturb.py
@@ -841,13 +928,35 @@
 tests/nwlistop/test_vevmin.py
 tests/nwlistop/test_vevminm.py
 tests/nwlistop/test_vevminsin.py
 tests/nwlistop/test_vghmin.py
 tests/nwlistop/test_vghminm.py
 tests/nwlistop/test_vghminsin.py
 tests/nwlistop/test_vghminuh.py
+tests/nwlistop/test_viol_eletricasin.py
+tests/nwlistop/test_viol_evmin.py
+tests/nwlistop/test_viol_evminm.py
+tests/nwlistop/test_viol_evminsin.py
+tests/nwlistop/test_viol_fpha.py
+tests/nwlistop/test_viol_ghmin.py
+tests/nwlistop/test_viol_ghminm.py
+tests/nwlistop/test_viol_ghminsin.py
+tests/nwlistop/test_viol_ghminuh.py
+tests/nwlistop/test_viol_lpp_dfmax.py
+tests/nwlistop/test_viol_lpp_dfmaxm.py
+tests/nwlistop/test_viol_lpp_dfmaxsin.py
+tests/nwlistop/test_viol_lpp_tbmax.py
+tests/nwlistop/test_viol_lpp_tbmaxm.py
+tests/nwlistop/test_viol_lpp_tbmaxsin.py
+tests/nwlistop/test_viol_neg_evap.py
+tests/nwlistop/test_viol_pos_evap.py
 tests/nwlistop/test_viol_rhq.py
 tests/nwlistop/test_viol_rhv.py
+tests/nwlistop/test_viol_turbmax.py
+tests/nwlistop/test_viol_turbmin.py
+tests/nwlistop/test_viol_vazmax.py
+tests/nwlistop/test_viol_vazmin.py
 tests/nwlistop/test_vmort.py
 tests/nwlistop/test_vmortm.py
 tests/nwlistop/test_vmortsin.py
+tests/nwlistop/test_vretiradauh.py
 tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-1.7.5/setup.py` & `inewave-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/libs/test_eolica.py` & `inewave-1.8.0/tests/libs/test_eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/libs/test_restricoes.py` & `inewave-1.8.0/tests/libs/test_restricoes.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,14 @@
 
 def test_registro_rhv():
     m: MagicMock = mock_open(read_data="".join(MockRHV))
     r = RegistroRHV()
     with patch("builtins.open", m):
         with open("", "") as fp:
             r.read(fp)
-    print(r.data)
     assert r.data == [1, "1*vtur(18) + 2*vver(17) + 2*varm(18)"]
     assert r.codigo_restricao == 1
     r.codigo_restricao = 5
     assert r.formula == "1*vtur(18) + 2*vver(17) + 2*varm(18)"
     r.formula = "Teste"
 
 
@@ -324,13 +323,11 @@
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
-        for li in linhas_escritas:
-            print(li)
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Restricoes.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-1.7.5/tests/libs/test_usinas_hidreletricas.py` & `inewave-1.8.0/tests/libs/test_usinas_hidreletricas.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,13 +474,11 @@
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
-        for li in linhas_escritas:
-            print(li)
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = UsinasHidreletricas.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-1.7.5/tests/mocks/arquivos/adterm.py` & `inewave-1.8.0/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/agrint.py` & `inewave-1.8.0/tests/mocks/arquivos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/arquivos.py` & `inewave-1.8.0/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/arquivos_nwlistcf.py` & `inewave-1.8.0/tests/mocks/arquivos/arquivos_nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-1.8.0/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-1.8.0/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-1.8.0/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/c_v_rhq.py` & `inewave-1.8.0/tests/mocks/arquivos/c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/c_v_rhq_s.py` & `inewave-1.8.0/tests/mocks/arquivos/c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/c_v_rhv.py` & `inewave-1.8.0/tests/mocks/arquivos/c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/c_v_rhv_s.py` & `inewave-1.8.0/tests/mocks/arquivos/c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cadic.py` & `inewave-1.8.0/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cbomb.py` & `inewave-1.8.0/tests/mocks/arquivos/cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cbombsin.py` & `inewave-1.8.0/tests/mocks/arquivos/cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cdef.py` & `inewave-1.8.0/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cdefsin.py` & `inewave-1.8.0/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/celetricas.py` & `inewave-1.8.0/tests/mocks/arquivos/celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/clast.py` & `inewave-1.8.0/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cmarg.py` & `inewave-1.8.0/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cmargmed.py` & `inewave-1.8.0/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/confhd.py` & `inewave-1.8.0/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/conft.py` & `inewave-1.8.0/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/coper.py` & `inewave-1.8.0/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/corteolm.py` & `inewave-1.8.0/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cterm.py` & `inewave-1.8.0/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ctermsin.py` & `inewave-1.8.0/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/curva.py` & `inewave-1.8.0/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/cvar.py` & `inewave-1.8.0/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/deficit.py` & `inewave-1.8.0/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/defsin.py` & `inewave-1.8.0/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/deletricas.py` & `inewave-1.8.0/tests/mocks/arquivos/deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/depminuh.py` & `inewave-1.8.0/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/desvuh.py` & `inewave-1.8.0/tests/mocks/arquivos/desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dfphauh.py` & `inewave-1.8.0/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dger.py` & `inewave-1.8.0/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlppdfmax.py` & `inewave-1.8.0/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-1.8.0/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-1.8.0/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlpptbmax.py` & `inewave-1.8.0/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-1.8.0/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-1.8.0/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dneg_evap.py` & `inewave-1.8.0/tests/mocks/arquivos/dneg_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dpos_evap.py` & `inewave-1.8.0/tests/mocks/arquivos/dpos_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dsvagua.py` & `inewave-1.8.0/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dtbmax.py` & `inewave-1.8.0/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dtbmin.py` & `inewave-1.8.0/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/dvazmax.py` & `inewave-1.8.0/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eaf.py` & `inewave-1.8.0/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eafb.py` & `inewave-1.8.0/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eafbm.py` & `inewave-1.8.0/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eafbsin.py` & `inewave-1.8.0/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eafm.py` & `inewave-1.8.0/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eafpast.py` & `inewave-1.8.0/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmf.py` & `inewave-1.8.0/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmfm.py` & `inewave-1.8.0/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmfp.py` & `inewave-1.8.0/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmfpm.py` & `inewave-1.8.0/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmfpsin.py` & `inewave-1.8.0/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/earmfsin.py` & `inewave-1.8.0/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eco_fpha.py` & `inewave-1.8.0/tests/mocks/arquivos/eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/edesvc.py` & `inewave-1.8.0/tests/mocks/arquivos/edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/edesvcm.py` & `inewave-1.8.0/tests/mocks/arquivos/edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/edesvcsin.py` & `inewave-1.8.0/tests/mocks/arquivos/edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/eolica.py` & `inewave-1.8.0/tests/mocks/arquivos/eolica.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/estados.py` & `inewave-1.8.0/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evapo.py` & `inewave-1.8.0/tests/mocks/arquivos/evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evapom.py` & `inewave-1.8.0/tests/mocks/arquivos/evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evaporsin.py` & `inewave-1.8.0/tests/mocks/arquivos/evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evert.py` & `inewave-1.8.0/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evertm.py` & `inewave-1.8.0/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/evertsin.py` & `inewave-1.8.0/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/exces.py` & `inewave-1.8.0/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/excessin.py` & `inewave-1.8.0/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/exph.py` & `inewave-1.8.0/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/expt.py` & `inewave-1.8.0/tests/mocks/arquivos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/form_rhq.py` & `inewave-1.8.0/tests/mocks/arquivos/form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/form_rhv.py` & `inewave-1.8.0/tests/mocks/arquivos/form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/fteolm.py` & `inewave-1.8.0/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/fteolsin.py` & `inewave-1.8.0/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/geol.py` & `inewave-1.8.0/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/geolm.py` & `inewave-1.8.0/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/geolsin.py` & `inewave-1.8.0/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/gh_fphexat.py` & `inewave-1.8.0/tests/mocks/arquivos/gh_fphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghidr.py` & `inewave-1.8.0/tests/mocks/arquivos/ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghidrm.py` & `inewave-1.8.0/tests/mocks/arquivos/ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghidrsin.py` & `inewave-1.8.0/tests/mocks/arquivos/ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghiduh.py` & `inewave-1.8.0/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmax.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmax_fpha.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmax_fphc.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmaxm.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmaxmr.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmaxr.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmaxsin.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghmin.py` & `inewave-1.8.0/tests/mocks/arquivos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghtot.py` & `inewave-1.8.0/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghtotm.py` & `inewave-1.8.0/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ghtotsin.py` & `inewave-1.8.0/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/gtert.py` & `inewave-1.8.0/tests/mocks/arquivos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/gttot.py` & `inewave-1.8.0/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/gttotsin.py` & `inewave-1.8.0/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/hjus.py` & `inewave-1.8.0/tests/mocks/arquivos/hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/hliq.py` & `inewave-1.8.0/tests/mocks/arquivos/hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/hmont.py` & `inewave-1.8.0/tests/mocks/arquivos/hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/intercambio.py` & `inewave-1.8.0/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/invade.py` & `inewave-1.8.0/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/invadem.py` & `inewave-1.8.0/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/manutt.py` & `inewave-1.8.0/tests/mocks/arquivos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/mercl.py` & `inewave-1.8.0/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/merclsin.py` & `inewave-1.8.0/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/mevmin.py` & `inewave-1.8.0/tests/mocks/arquivos/mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/mevminm.py` & `inewave-1.8.0/tests/mocks/arquivos/mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/mevminsin.py` & `inewave-1.8.0/tests/mocks/arquivos/mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/modif.py` & `inewave-1.8.0/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/newavetim.py` & `inewave-1.8.0/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/nwlistcfrel.py` & `inewave-1.8.0/tests/mocks/arquivos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/nwlistopdat.py` & `inewave-1.8.0/tests/mocks/arquivos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-1.8.0/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-1.8.0/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-1.8.0/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/parp.py` & `inewave-1.8.0/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/parpeol.py` & `inewave-1.8.0/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/parpvaz.py` & `inewave-1.8.0/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/patamar.py` & `inewave-1.8.0/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/penalid.py` & `inewave-1.8.0/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/perdf.py` & `inewave-1.8.0/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/perdfm.py` & `inewave-1.8.0/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/perdfsin.py` & `inewave-1.8.0/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/pivarm.py` & `inewave-1.8.0/tests/mocks/arquivos/pivarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2008,7 +2008,29 @@
     " DPADRAO          0.00           0.00           0.00           0.52           0.35           0.37           0.19          11.85      317491.09      498370.16      296310.69         210.67\n",
     " MIN              0.00           0.00           0.00          12.16          11.95          11.91          11.09        -515.75    -9090852.00    -7762951.00    -6434709.50       -5049.98\n",
     " P5               0.00           0.00           0.00          12.31          12.14          12.14          12.17          12.09           7.21          11.30          11.18           9.85\n",
     " P95              0.00           0.00           0.00          13.92          13.21          13.44          12.62          12.81          13.01          13.29          14.18          14.29\n",
     " MAX              0.00           0.00           0.00          14.47          14.06          14.19          13.59          13.28          13.25          14.25          14.46          14.52\n",
     "\n",
 ]
+
+MockPivarm_v29_2 = [
+    "  Caso Teste                              \n",
+    "     VALOR DA AGUA CALCULADO NO PROPRIO ESTAGIO ($/hm3)    USINA:CAMARGOS                                \n",
+    "\n",
+    "     ANO: 2021\n",
+    "                     1              2              3              4              5              6              7              8              9             10             11             12          MEDIA\n",
+    "     1  -0.1414677E+07 -0.1349311E+07 -0.1334812E+07 -0.3122534E+06 -0.5733238E+06 -0.8118121E+06 -0.9579259E+06 -0.1287244E+07 -0.1610343E+07 -0.1938827E+07 -0.1400416E+07 -0.1193002E+07 -0.1181996E+07\n",
+    "     2  -0.1633927E+07 -0.1921184E+07 -0.1903470E+07 -0.2510122E+07 -0.1315049E+07 -0.1194394E+07 -0.7854828E+06 -0.8918289E+06 -0.9381198E+06 -0.8028469E+06 -0.4377851E+06  0.7291253E+00 -0.1194517E+07\n",
+    "     3  -0.1470586E+07 -0.1487987E+07 -0.4378156E+06  0.4789146E+00  0.3522076E+00 -0.1315093E+06 -0.1511477E+06 -0.4878529E+05 -0.6861371E+05 -0.3434183E+04 -0.4708708E+04  0.7652909E+00 -0.3170488E+06\n",
+    "     4  -0.1001131E+07 -0.8632798E+06 -0.5095322E+06  0.5867786E+00  0.3681660E+00 -0.1458308E+06 -0.3703057E+06 -0.4865548E+06 -0.4771853E+06 -0.2797431E+06 -0.3693978E+06 -0.4779100E+06 -0.4150725E+06\n",
+    "     5  -0.4394022E+06  0.7009254E+00  0.7982943E+00  0.6948820E+00  0.6731272E+00  0.7516054E+00  0.6621739E+00 -0.2243781E+04 -0.1740437E+04 -0.7347510E+03  0.7666521E+00  0.7963766E+00 -0.3700961E+05\n",
+    "     6  -0.9954916E+06  0.2414514E+00  0.7362821E+00  0.4232431E+00  0.3790797E+00 -0.1609476E+06 -0.2888754E+06 -0.3122430E+06 -0.3584640E+06 -0.3386253E+06 -0.7581071E+04  0.3811179E+00 -0.2051855E+06\n",
+    "     7  -0.1191626E+07 -0.1477003E+07 -0.7068472E+06 -0.7207408E+06 -0.7899582E+06 -0.6012040E+06 -0.1025739E+07 -0.1086481E+07 -0.1088286E+07 -0.1387582E+07 -0.1170988E+07 -0.4186739E+06 -0.9720941E+06\n",
+    "  MEDIA -0.1271068E+07 -0.9755682E+06 -0.7278995E+06 -0.5929452E+06 -0.5217324E+06 -0.5974791E+06 -0.6373254E+06 -0.6762271E+06 -0.7116699E+06 -0.7282038E+06 -0.6689438E+06 -0.3910162E+06 -0.7083398E+06\n",
+    " DPADRAO 0.5510314E+06  0.6807061E+06  0.7767428E+06  0.7558677E+06  0.7142074E+06  0.7226282E+06  0.7491109E+06  0.7806701E+06  0.8726851E+06  0.1074805E+07  0.1119712E+07  0.5807778E+06\n",
+    " MIN    -0.2735416E+07 -0.3664930E+07 -0.4198116E+07 -0.5733930E+07 -0.5186678E+07 -0.7157272E+07 -0.8462130E+07 -0.9812189E+07 -0.6095935E+07 -0.7423367E+07 -0.7979637E+07 -0.4036746E+07\n",
+    " P5     -0.2299674E+07 -0.2205085E+07 -0.2325010E+07 -0.2281097E+07 -0.2170567E+07 -0.2214207E+07 -0.1921539E+07 -0.1952641E+07 -0.2229460E+07 -0.2769849E+07 -0.3480252E+07 -0.1660316E+07\n",
+    " P95    -0.4034075E+06  0.4249327E+00  0.7811375E+00  0.7300804E+00  0.6745794E+00  0.5851984E+00 -0.7322466E+04 -0.2296590E+04 -0.1844317E+04  0.0000000E+00  0.7381992E+00  0.7933396E+00\n",
+    " MAX    -0.3530049E+04  0.4580274E+04  0.7991294E+00  0.7966098E+00  0.7876535E+00  0.7873833E+00  0.7144043E+00  0.3738879E+00  0.7184766E+00  0.7333333E+00  0.7987911E+00  0.7988697E+00\n",
+    "\n",
+]
```

### Comparing `inewave-1.7.5/tests/mocks/arquivos/pmo.py` & `inewave-1.8.0/tests/mocks/arquivos/pmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+MockVersaoModeloPMO = [
+    " CEPEL                         MODELO ESTRATEGICO DE GERACAO HIDROTERMICA A SUBSISTEMAS              VERSAO  29.3.1                             \n"
+]
+
 MockBlocoEafPastTendenciaHidrolPMO = [
     "         ENERGIAS AFLUENTES PASSADAS PARA A TENDENCIA HIDROLOGICA EM REFERENCIA A PRIMEIRA CONFIGURACAO DO SISTEMA (MWmes)\n",
     " X--------------------------------------------------------------------------------------------------------------------------------------------X\n",
     " SISTEMA           1          2          3          4          5          6          7          8          9         10         11         12\n",
     " X--------------------------------------------------------------------------------------------------------------------------------------------X\n",
     " SUDESTE       7196.96    9745.33   11886.20    7767.14    4202.72    3035.47    2315.42    2114.86    1668.24    2063.36    4073.77    4769.50\n",
     " MADEIRA       9650.59   11146.05   11085.25    9915.49    6337.30    3964.90    2982.11    1775.02    1524.38    1085.95    1459.81    3889.26\n",
@@ -7091,15 +7095,16 @@
     "                            VALOR ESPERADO TOTAL:                 22323.17\n",
     "                 DESVIO PADRAO DO VALOR ESPERADO:                   107.00\n",
     "\n",
     "\n",
 ]
 
 MockPMO = (
-    MockBlocoEafPastTendenciaHidrolPMO
+    MockVersaoModeloPMO
+    + MockBlocoEafPastTendenciaHidrolPMO
     + MockBlocoEafPastCfugaMedioPMO
     + MockBlocoEnergiaArmazenadaMaximaPMO
     + MockBlocoEnergiaArmazenadaInicialPMO
     + MockBlocoVolumeArmazenadoInicialPMO
     + MockBlocoGeracaoMaximaUsinasTermicasPMO
     + MockBlocoGeracaoMinimaUsinasTermicasPMO
     + MockBlocoConvergenciaPMO
```

### Comparing `inewave-1.7.5/tests/mocks/arquivos/qafluh.py` & `inewave-1.8.0/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/qincruh.py` & `inewave-1.8.0/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/re.py` & `inewave-1.8.0/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/ree.py` & `inewave-1.8.0/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/restricoes.py` & `inewave-1.8.0/tests/mocks/arquivos/restricoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/rhslppdf.py` & `inewave-1.8.0/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/rhslpptb.py` & `inewave-1.8.0/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/selcor.py` & `inewave-1.8.0/tests/mocks/arquivos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/sistema.py` & `inewave-1.8.0/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/term.py` & `inewave-1.8.0/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/usinas_hidreletricas.py` & `inewave-1.8.0/tests/mocks/arquivos/usinas_hidreletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vagua.py` & `inewave-1.8.0/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/varmpuh.py` & `inewave-1.8.0/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/varmuh.py` & `inewave-1.8.0/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vazpast.py` & `inewave-1.8.0/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vbomb.py` & `inewave-1.8.0/tests/mocks/arquivos/vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vdesviouh.py` & `inewave-1.8.0/tests/mocks/arquivos/vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vento.py` & `inewave-1.8.0/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vertuh.py` & `inewave-1.8.0/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/verturb.py` & `inewave-1.8.0/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/verturbm.py` & `inewave-1.8.0/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/verturbsin.py` & `inewave-1.8.0/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vevapuh.py` & `inewave-1.8.0/tests/mocks/arquivos/vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vevmin.py` & `inewave-1.8.0/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vevminm.py` & `inewave-1.8.0/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vevminsin.py` & `inewave-1.8.0/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vghmin.py` & `inewave-1.8.0/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vghminm.py` & `inewave-1.8.0/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vghminsin.py` & `inewave-1.8.0/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vghminuh.py` & `inewave-1.8.0/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/viol_rhq.py` & `inewave-1.8.0/tests/mocks/arquivos/viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/viol_rhv.py` & `inewave-1.8.0/tests/mocks/arquivos/viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vmort.py` & `inewave-1.8.0/tests/mocks/arquivos/vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vmortm.py` & `inewave-1.8.0/tests/mocks/arquivos/vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vmortsin.py` & `inewave-1.8.0/tests/mocks/arquivos/vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/volref_saz.py` & `inewave-1.8.0/tests/mocks/arquivos/volref_saz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/arquivos/vturuh.py` & `inewave-1.8.0/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/mocks/mock_open.py` & `inewave-1.8.0/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_adterm.py` & `inewave-1.8.0/tests/newave/test_adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_agrint.py` & `inewave-1.8.0/tests/newave/test_agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_arquivos.py` & `inewave-1.8.0/tests/newave/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-1.8.0/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_avl_desvfpha_s.py` & `inewave-1.8.0/tests/newave/test_avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-1.8.0/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_cadic.py` & `inewave-1.8.0/tests/newave/test_cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_caso.py` & `inewave-1.8.0/tests/newave/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_clast.py` & `inewave-1.8.0/tests/newave/test_clast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_confhd.py` & `inewave-1.8.0/tests/newave/test_confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_conft.py` & `inewave-1.8.0/tests/newave/test_conft.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_cortes.py` & `inewave-1.8.0/tests/newave/test_cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_cortesh.py` & `inewave-1.8.0/tests/newave/test_cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_curva.py` & `inewave-1.8.0/tests/newave/test_curva.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_cvar.py` & `inewave-1.8.0/tests/newave/test_cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_dger.py` & `inewave-1.8.0/tests/newave/test_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_dsvagua.py` & `inewave-1.8.0/tests/newave/test_dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_eafpast.py` & `inewave-1.8.0/tests/newave/test_eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_eco_fpha.py` & `inewave-1.8.0/tests/newave/test_eco_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_enavazb.py` & `inewave-1.8.0/tests/newave/test_enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_enavazf.py` & `inewave-1.8.0/tests/newave/test_enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_energiab.py` & `inewave-1.8.0/tests/newave/test_energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_energiaf.py` & `inewave-1.8.0/tests/newave/test_energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_energias.py` & `inewave-1.8.0/tests/newave/test_energias.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_engnat.py` & `inewave-1.8.0/tests/newave/test_engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_exph.py` & `inewave-1.8.0/tests/newave/test_exph.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_expt.py` & `inewave-1.8.0/tests/newave/test_expt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_forward.py` & `inewave-1.8.0/tests/newave/test_forward.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_forwarh.py` & `inewave-1.8.0/tests/newave/test_forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_ghmin.py` & `inewave-1.8.0/tests/newave/test_ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_hidr.py` & `inewave-1.8.0/tests/newave/test_hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_manutt.py` & `inewave-1.8.0/tests/newave/test_manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_modif.py` & `inewave-1.8.0/tests/newave/test_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_newavetim.py` & `inewave-1.8.0/tests/newave/test_newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_nwv_avl_evap.py` & `inewave-1.8.0/tests/newave/test_nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_nwv_cortes_evap.py` & `inewave-1.8.0/tests/newave/test_nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_nwv_eco_evap.py` & `inewave-1.8.0/tests/newave/test_nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_parp.py` & `inewave-1.8.0/tests/newave/test_parp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_parpeol.py` & `inewave-1.8.0/tests/newave/test_parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_parpvaz.py` & `inewave-1.8.0/tests/newave/test_parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_patamar.py` & `inewave-1.8.0/tests/newave/test_patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_penalid.py` & `inewave-1.8.0/tests/newave/test_penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_pmo.py` & `inewave-1.8.0/tests/newave/test_pmo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from inewave.newave.modelos.pmo import (
+    BlocoVersaoModeloPMO,
     BlocoConvergenciaPMO,
     BlocoEafPastTendenciaHidrolPMO,
     BlocoEafPastCfugaMedioPMO,
     BlocoConfiguracoesExpansaoPMO,
     BlocoMARSPMO,
     BlocoRiscoDeficitENSPMO,
     BlocoCustoOperacaoPMO,
@@ -24,14 +25,15 @@
 
 from inewave.newave import Pmo
 from datetime import datetime
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
+from tests.mocks.arquivos.pmo import MockVersaoModeloPMO
 from tests.mocks.arquivos.pmo import MockBlocoEafPastTendenciaHidrolPMO
 from tests.mocks.arquivos.pmo import MockBlocoEafPastCfugaMedioPMO
 from tests.mocks.arquivos.pmo import MockBlocoConvergenciaPMO
 from tests.mocks.arquivos.pmo import (
     MockBlocoConfiguracoesExpansaoEntradaReservatorioPMO,
 )
 from tests.mocks.arquivos.pmo import MockBlocoProdutibilidadesPMO
@@ -59,14 +61,24 @@
     MockBlocoGeracaoMaximaUsinasTermicasPMO,
 )
 from tests.mocks.arquivos.pmo import MockPMO
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
+def test_versao_modelo():
+    m: MagicMock = mock_open(read_data="".join(MockVersaoModeloPMO))
+    b = BlocoVersaoModeloPMO()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            b.read(fp)
+
+    assert b.data == "29.3.1"
+
+
 def test_eafpast_tendencia_hidrologica():
     m: MagicMock = mock_open(
         read_data="".join(MockBlocoEafPastTendenciaHidrolPMO)
     )
     b = BlocoEafPastTendenciaHidrolPMO()
     with patch("builtins.open", m):
         with open("", "") as fp:
@@ -372,14 +384,15 @@
     assert b.data.iloc[-1, -1] == datetime(2027, 12, 1)
 
 
 def test_atributos_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
         pmo = Pmo.read(ARQ_TESTE)
+        assert pmo.versao_modelo is not None
         assert pmo.eafpast_tendencia_hidrologica is not None
         assert pmo.eafpast_cfuga_medio is not None
         assert pmo.convergencia is not None
         assert pmo.configuracoes_alteracao_potencia is not None
         assert pmo.configuracoes_entrada_reservatorio is not None
         assert pmo.configuracoes_qualquer_modificacao is not None
         assert pmo.retas_perdas_engolimento(1) is not None
@@ -405,14 +418,15 @@
         assert pmo.geracao_maxima_usinas_termicas is not None
 
 
 def test_atributos_nao_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConvergenciaPMO))
     with patch("builtins.open", m):
         pmo = Pmo.read(ARQ_TESTE)
+        assert pmo.versao_modelo is None
         assert pmo.convergencia is not None
         assert pmo.custo_operacao_series_simuladas is None
         assert pmo.custo_operacao_total is None
         assert pmo.desvio_custo_operacao_total is None
         assert pmo.produtibilidades_equivalentes is None
         assert pmo.energia_armazenada_maxima is None
         assert pmo.energia_armazenada_inicial is None
```

### Comparing `inewave-1.7.5/tests/newave/test_re.py` & `inewave-1.8.0/tests/newave/test_re.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_ree.py` & `inewave-1.8.0/tests/newave/test_ree.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_selcor.py` & `inewave-1.8.0/tests/newave/test_selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_shist.py` & `inewave-1.8.0/tests/newave/test_shist.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_sistema.py` & `inewave-1.8.0/tests/newave/test_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_term.py` & `inewave-1.8.0/tests/newave/test_term.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazaob.py` & `inewave-1.8.0/tests/newave/test_vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazaof.py` & `inewave-1.8.0/tests/newave/test_vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazaos.py` & `inewave-1.8.0/tests/newave/test_vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazinat.py` & `inewave-1.8.0/tests/newave/test_vazinat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazoes.py` & `inewave-1.8.0/tests/newave/test_vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_vazpast.py` & `inewave-1.8.0/tests/newave/test_vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/newave/test_volrefsaz.py` & `inewave-1.8.0/tests/newave/test_volrefsaz.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistcf/test_arquivos.py` & `inewave-1.8.0/tests/nwlistcf/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistcf/test_caso.py` & `inewave-1.8.0/tests/nwlistcf/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistcf/test_estados.py` & `inewave-1.8.0/tests/nwlistcf/test_estados.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistcf/test_nwlistcfdat.py` & `inewave-1.8.0/tests/nwlistcf/test_nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistcf/test_nwlistcfrel.py` & `inewave-1.8.0/tests/nwlistcf/test_nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_c_v_rhq.py` & `inewave-1.8.0/tests/nwlistop/test_c_v_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_c_v_rhq_s.py` & `inewave-1.8.0/tests/nwlistop/test_c_v_rhq_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_c_v_rhv.py` & `inewave-1.8.0/tests/nwlistop/test_c_v_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_c_v_rhv_s.py` & `inewave-1.8.0/tests/nwlistop/test_c_v_rhv_s.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cbomb.py` & `inewave-1.8.0/tests/nwlistop/test_cbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cbombsin.py` & `inewave-1.8.0/tests/nwlistop/test_cbombsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cdef.py` & `inewave-1.8.0/tests/nwlistop/test_cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cdefsin.py` & `inewave-1.8.0/tests/nwlistop/test_cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_celetricas.py` & `inewave-1.8.0/tests/nwlistop/test_celetricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cmarg.py` & `inewave-1.8.0/tests/nwlistop/test_cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cmargmed.py` & `inewave-1.8.0/tests/nwlistop/test_cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_coper.py` & `inewave-1.8.0/tests/nwlistop/test_coper.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_corteolm.py` & `inewave-1.8.0/tests/nwlistop/test_corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_cterm.py` & `inewave-1.8.0/tests/nwlistop/test_cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ctermsin.py` & `inewave-1.8.0/tests/nwlistop/test_ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_deficit.py` & `inewave-1.8.0/tests/nwlistop/test_deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_defsin.py` & `inewave-1.8.0/tests/nwlistop/test_defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_deletricas.py` & `inewave-1.8.0/tests/nwlistop/test_deletricas.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_depminuh.py` & `inewave-1.8.0/tests/nwlistop/test_depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_desvuh.py` & `inewave-1.8.0/tests/nwlistop/test_desvuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dfphauh.py` & `inewave-1.8.0/tests/nwlistop/test_dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlppdfmax.py` & `inewave-1.8.0/tests/nwlistop/test_dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-1.8.0/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-1.8.0/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlpptbmax.py` & `inewave-1.8.0/tests/nwlistop/test_dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-1.8.0/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-1.8.0/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dnegevap.py` & `inewave-1.8.0/tests/nwlistop/test_dnegevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dposevap.py` & `inewave-1.8.0/tests/nwlistop/test_dposevap.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dtbmax.py` & `inewave-1.8.0/tests/nwlistop/test_dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dtbmin.py` & `inewave-1.8.0/tests/nwlistop/test_dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_dvazmax.py` & `inewave-1.8.0/tests/nwlistop/test_dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_eaf.py` & `inewave-1.8.0/tests/nwlistop/test_eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_eafb.py` & `inewave-1.8.0/tests/nwlistop/test_eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_eafbm.py` & `inewave-1.8.0/tests/nwlistop/test_eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_eafbsin.py` & `inewave-1.8.0/tests/nwlistop/test_eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_eafm.py` & `inewave-1.8.0/tests/nwlistop/test_eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmf.py` & `inewave-1.8.0/tests/nwlistop/test_earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmfm.py` & `inewave-1.8.0/tests/nwlistop/test_earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmfp.py` & `inewave-1.8.0/tests/nwlistop/test_earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmfpm.py` & `inewave-1.8.0/tests/nwlistop/test_earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmfpsin.py` & `inewave-1.8.0/tests/nwlistop/test_earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_earmfsin.py` & `inewave-1.8.0/tests/nwlistop/test_earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_edesvc.py` & `inewave-1.8.0/tests/nwlistop/test_edesvc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_edesvcm.py` & `inewave-1.8.0/tests/nwlistop/test_edesvcm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_edesvcsin.py` & `inewave-1.8.0/tests/nwlistop/test_edesvcsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evapo.py` & `inewave-1.8.0/tests/nwlistop/test_evapo.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evapom.py` & `inewave-1.8.0/tests/nwlistop/test_evapom.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evaporsin.py` & `inewave-1.8.0/tests/nwlistop/test_evaporsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evert.py` & `inewave-1.8.0/tests/nwlistop/test_evert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evertm.py` & `inewave-1.8.0/tests/nwlistop/test_evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_evertsin.py` & `inewave-1.8.0/tests/nwlistop/test_evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_exces.py` & `inewave-1.8.0/tests/nwlistop/test_exces.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_excessin.py` & `inewave-1.8.0/tests/nwlistop/test_excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_form_rhq.py` & `inewave-1.8.0/tests/nwlistop/test_form_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_form_rhv.py` & `inewave-1.8.0/tests/nwlistop/test_form_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_fteolm.py` & `inewave-1.8.0/tests/nwlistop/test_fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_fteolsin.py` & `inewave-1.8.0/tests/nwlistop/test_fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_geol.py` & `inewave-1.8.0/tests/nwlistop/test_geol.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_geolm.py` & `inewave-1.8.0/tests/nwlistop/test_geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_geolsin.py` & `inewave-1.8.0/tests/nwlistop/test_geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghfphexat.py` & `inewave-1.8.0/tests/nwlistop/test_ghfphexat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghidr.py` & `inewave-1.8.0/tests/nwlistop/test_ghidr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghidrm.py` & `inewave-1.8.0/tests/nwlistop/test_ghidrm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghidrsin.py` & `inewave-1.8.0/tests/nwlistop/test_ghidrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghiduh.py` & `inewave-1.8.0/tests/nwlistop/test_ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmax.py` & `inewave-1.8.0/tests/nwlistop/test_ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmax_fpha.py` & `inewave-1.8.0/tests/nwlistop/test_ghmax_fpha.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmax_fphc.py` & `inewave-1.8.0/tests/nwlistop/test_ghmax_fphc.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmaxm.py` & `inewave-1.8.0/tests/nwlistop/test_ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmaxmr.py` & `inewave-1.8.0/tests/nwlistop/test_ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmaxr.py` & `inewave-1.8.0/tests/nwlistop/test_ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmaxrsin.py` & `inewave-1.8.0/tests/nwlistop/test_ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghmaxsin.py` & `inewave-1.8.0/tests/nwlistop/test_ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghtot.py` & `inewave-1.8.0/tests/nwlistop/test_ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghtotm.py` & `inewave-1.8.0/tests/nwlistop/test_ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_ghtotsin.py` & `inewave-1.8.0/tests/nwlistop/test_ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_gtert.py` & `inewave-1.8.0/tests/nwlistop/test_gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_gttot.py` & `inewave-1.8.0/tests/nwlistop/test_gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_gttotsin.py` & `inewave-1.8.0/tests/nwlistop/test_gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_hjus.py` & `inewave-1.8.0/tests/nwlistop/test_hjus.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_hliq.py` & `inewave-1.8.0/tests/nwlistop/test_hliq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_hmont.py` & `inewave-1.8.0/tests/nwlistop/test_hmont.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_intercambio.py` & `inewave-1.8.0/tests/nwlistop/test_intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_invade.py` & `inewave-1.8.0/tests/nwlistop/test_invade.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_invadem.py` & `inewave-1.8.0/tests/nwlistop/test_invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_mercl.py` & `inewave-1.8.0/tests/nwlistop/test_mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_merclsin.py` & `inewave-1.8.0/tests/nwlistop/test_merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_mevmin.py` & `inewave-1.8.0/tests/nwlistop/test_mevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_mevminm.py` & `inewave-1.8.0/tests/nwlistop/test_mevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_mevminsin.py` & `inewave-1.8.0/tests/nwlistop/test_mevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_nwlistopdat.py` & `inewave-1.8.0/tests/nwlistop/test_nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_perdf.py` & `inewave-1.8.0/tests/nwlistop/test_perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_perdfm.py` & `inewave-1.8.0/tests/nwlistop/test_perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_perdfsin.py` & `inewave-1.8.0/tests/nwlistop/test_perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_pivarm.py` & `inewave-1.8.0/tests/nwlistop/test_pivarm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_pivarmincr.py` & `inewave-1.8.0/tests/nwlistop/test_pivarmincr.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_qafluh.py` & `inewave-1.8.0/tests/nwlistop/test_qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_qincruh.py` & `inewave-1.8.0/tests/nwlistop/test_qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_rhslppdf.py` & `inewave-1.8.0/tests/nwlistop/test_rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_rhslpptb.py` & `inewave-1.8.0/tests/nwlistop/test_rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vagua.py` & `inewave-1.8.0/tests/nwlistop/test_vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_varmpuh.py` & `inewave-1.8.0/tests/nwlistop/test_varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_varmuh.py` & `inewave-1.8.0/tests/nwlistop/test_varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vbomb.py` & `inewave-1.8.0/tests/nwlistop/test_vbomb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vdesviouh.py` & `inewave-1.8.0/tests/nwlistop/test_vdesviouh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vento.py` & `inewave-1.8.0/tests/nwlistop/test_vento.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vertuh.py` & `inewave-1.8.0/tests/nwlistop/test_vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_verturb.py` & `inewave-1.8.0/tests/nwlistop/test_verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_verturbm.py` & `inewave-1.8.0/tests/nwlistop/test_verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_verturbsin.py` & `inewave-1.8.0/tests/nwlistop/test_verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vevapuh.py` & `inewave-1.8.0/tests/nwlistop/test_vevapuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vevmin.py` & `inewave-1.8.0/tests/nwlistop/test_vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vevminm.py` & `inewave-1.8.0/tests/nwlistop/test_vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vevminsin.py` & `inewave-1.8.0/tests/nwlistop/test_vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vghmin.py` & `inewave-1.8.0/tests/nwlistop/test_vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vghminm.py` & `inewave-1.8.0/tests/nwlistop/test_vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vghminsin.py` & `inewave-1.8.0/tests/nwlistop/test_vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vghminuh.py` & `inewave-1.8.0/tests/nwlistop/test_vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_viol_rhq.py` & `inewave-1.8.0/tests/nwlistop/test_viol_rhq.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_viol_rhv.py` & `inewave-1.8.0/tests/nwlistop/test_viol_rhv.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vmort.py` & `inewave-1.8.0/tests/nwlistop/test_vmort.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vmortm.py` & `inewave-1.8.0/tests/nwlistop/test_vmortm.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vmortsin.py` & `inewave-1.8.0/tests/nwlistop/test_vmortsin.py`

 * *Files identical despite different names*

### Comparing `inewave-1.7.5/tests/nwlistop/test_vturuh.py` & `inewave-1.8.0/tests/nwlistop/test_vturuh.py`

 * *Files identical despite different names*

