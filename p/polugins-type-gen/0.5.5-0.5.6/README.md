# Comparing `tmp/polugins_type_gen-0.5.5.tar.gz` & `tmp/polugins_type_gen-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polugins_type_gen-0.5.5.tar", max compression
+gzip compressed data, was "polugins_type_gen-0.5.6.tar", max compression
```

## Comparing `polugins_type_gen-0.5.5.tar` & `polugins_type_gen-0.5.6.tar`

### file list

```diff
@@ -1,228 +1,244 @@
--rw-r--r--   0        0        0      137 2024-03-31 08:06:17.570440 polugins_type_gen-0.5.5/README.md
--rw-r--r--   0        0        0     1155 2024-03-31 08:06:17.570440 polugins_type_gen-0.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 08:06:17.570440 polugins_type_gen-0.5.5/src/polugins_type_gen/__init__.py
--rw-r--r--   0        0        0       76 2024-03-31 08:06:17.570440 polugins_type_gen-0.5.5/src/polugins_type_gen/__main__.py
--rw-r--r--   0        0        0   202000 2024-03-31 08:06:17.574440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   187053 2024-03-31 08:06:17.578440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/expr/expr.pyi
--rw-r--r--   0        0        0   118395 2024-03-31 08:06:17.578440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   109948 2024-03-31 08:06:17.578440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/series/series.pyi
--rw-r--r--   0        0        0   203701 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   188478 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/expr/expr.pyi
--rw-r--r--   0        0        0   119581 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   113608 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/series/series.pyi
--rw-r--r--   0        0        0   203701 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   188477 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/expr/expr.pyi
--rw-r--r--   0        0        0   119599 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   113608 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/series/series.pyi
--rw-r--r--   0        0        0   208700 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   197547 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/expr/expr.pyi
--rw-r--r--   0        0        0   120067 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115250 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/series/series.pyi
--rw-r--r--   0        0        0   214621 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   209693 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/expr/expr.pyi
--rw-r--r--   0        0        0   123708 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115386 2024-03-31 08:06:17.582440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/series/series.pyi
--rw-r--r--   0        0        0   214826 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   209693 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/expr/expr.pyi
--rw-r--r--   0        0        0   123708 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115470 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/series/series.pyi
--rw-r--r--   0        0        0   215930 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   211358 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/expr/expr.pyi
--rw-r--r--   0        0        0   123708 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115527 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/series/series.pyi
--rw-r--r--   0        0        0   215921 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   211623 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/expr/expr.pyi
--rw-r--r--   0        0        0   123980 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115661 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/series/series.pyi
--rw-r--r--   0        0        0   215921 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   211623 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/expr/expr.pyi
--rw-r--r--   0        0        0   124768 2024-03-31 08:06:17.586440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115661 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/series/series.pyi
--rw-r--r--   0        0        0   219412 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   212340 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/expr/expr.pyi
--rw-r--r--   0        0        0   124784 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115560 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/series/series.pyi
--rw-r--r--   0        0        0   212365 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   208256 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/expr/expr.pyi
--rw-r--r--   0        0        0   122214 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   114359 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/series/series.pyi
--rw-r--r--   0        0        0   212365 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   208256 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/expr/expr.pyi
--rw-r--r--   0        0        0   122214 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   114359 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/series/series.pyi
--rw-r--r--   0        0        0   213962 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   209686 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/expr/expr.pyi
--rw-r--r--   0        0        0   123271 2024-03-31 08:06:17.590440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   115499 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/series/series.pyi
--rw-r--r--   0        0        0   220492 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   213716 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/expr/expr.pyi
--rw-r--r--   0        0        0   124105 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   116362 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/series/series.pyi
--rw-r--r--   0        0        0   235341 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   279977 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/expr/expr.pyi
--rw-r--r--   0        0        0   129750 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   126656 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/series/series.pyi
--rw-r--r--   0        0        0   236227 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   279996 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/expr/expr.pyi
--rw-r--r--   0        0        0   130618 2024-03-31 08:06:17.594440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   127009 2024-03-31 08:06:17.598440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/series/series.pyi
--rw-r--r--   0        0        0   243492 2024-03-31 08:06:17.598440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   280112 2024-03-31 08:06:17.598440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/expr/expr.pyi
--rw-r--r--   0        0        0   135137 2024-03-31 08:06:17.598440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   127009 2024-03-31 08:06:17.598440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/series/series.pyi
--rw-r--r--   0        0        0   246531 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   280112 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/expr/expr.pyi
--rw-r--r--   0        0        0   135501 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   127139 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/series/series.pyi
--rw-r--r--   0        0        0   221654 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   218322 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/expr/expr.pyi
--rw-r--r--   0        0        0   124918 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   118017 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/series/series.pyi
--rw-r--r--   0        0        0   222371 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   218700 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/expr/expr.pyi
--rw-r--r--   0        0        0   125632 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   118206 2024-03-31 08:06:17.602440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/series/series.pyi
--rw-r--r--   0        0        0   222426 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   264845 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/expr/expr.pyi
--rw-r--r--   0        0        0   125715 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   118188 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/series/series.pyi
--rw-r--r--   0        0        0   230560 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   274018 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/expr/expr.pyi
--rw-r--r--   0        0        0   128405 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   120563 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/series/series.pyi
--rw-r--r--   0        0        0   231685 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   277726 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/expr/expr.pyi
--rw-r--r--   0        0        0   129124 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   122692 2024-03-31 08:06:17.606440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/series/series.pyi
--rw-r--r--   0        0        0   234690 2024-03-31 08:06:17.610440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   278619 2024-03-31 08:06:17.610440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/expr/expr.pyi
--rw-r--r--   0        0        0   129124 2024-03-31 08:06:17.610440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   125575 2024-03-31 08:06:17.610440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/series/series.pyi
--rw-r--r--   0        0        0   258422 2024-03-31 08:06:17.610440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   281929 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/expr/expr.pyi
--rw-r--r--   0        0        0   151704 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   133052 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/series/series.pyi
--rw-r--r--   0        0        0   258469 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   284476 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/expr/expr.pyi
--rw-r--r--   0        0        0   152238 2024-03-31 08:06:17.614440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   133202 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/series/series.pyi
--rw-r--r--   0        0        0   265646 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   296486 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/expr/expr.pyi
--rw-r--r--   0        0        0   159538 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   137670 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/series/series.pyi
--rw-r--r--   0        0        0   265791 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   298079 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/expr/expr.pyi
--rw-r--r--   0        0        0   159794 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   139057 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/series/series.pyi
--rw-r--r--   0        0        0   265314 2024-03-31 08:06:17.618440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   298000 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/expr/expr.pyi
--rw-r--r--   0        0        0   159400 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   139331 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/series/series.pyi
--rw-r--r--   0        0        0   271168 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   302075 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/expr/expr.pyi
--rw-r--r--   0        0        0   159900 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   143267 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/series/series.pyi
--rw-r--r--   0        0        0   271168 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   303067 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/expr/expr.pyi
--rw-r--r--   0        0        0   161034 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   143267 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/series/series.pyi
--rw-r--r--   0        0        0   273151 2024-03-31 08:06:17.622440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   300748 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/expr/expr.pyi
--rw-r--r--   0        0        0   161034 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   144594 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/series/series.pyi
--rw-r--r--   0        0        0   273187 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   300748 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/expr/expr.pyi
--rw-r--r--   0        0        0   161034 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   144594 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/series/series.pyi
--rw-r--r--   0        0        0   273280 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   300748 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/expr/expr.pyi
--rw-r--r--   0        0        0   161034 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   144594 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/series/series.pyi
--rw-r--r--   0        0        0   258762 2024-03-31 08:06:17.626440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   285703 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/expr/expr.pyi
--rw-r--r--   0        0        0   152259 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   133634 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/series/series.pyi
--rw-r--r--   0        0        0   259358 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   288473 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/expr/expr.pyi
--rw-r--r--   0        0        0   153465 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   136036 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/series/series.pyi
--rw-r--r--   0        0        0   259817 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   288726 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/expr/expr.pyi
--rw-r--r--   0        0        0   152522 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   136603 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/series/series.pyi
--rw-r--r--   0        0        0   259817 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   288726 2024-03-31 08:06:17.630440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/expr/expr.pyi
--rw-r--r--   0        0        0   152522 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   136603 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/series/series.pyi
--rw-r--r--   0        0        0   260303 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   296367 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/expr/expr.pyi
--rw-r--r--   0        0        0   152890 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   136668 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/series/series.pyi
--rw-r--r--   0        0        0   275889 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   303962 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/expr/expr.pyi
--rw-r--r--   0        0        0   160309 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   145255 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/series/series.pyi
--rw-r--r--   0        0        0   275891 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   303971 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/expr/expr.pyi
--rw-r--r--   0        0        0   160309 2024-03-31 08:06:17.634440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   145255 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/series/series.pyi
--rw-r--r--   0        0        0   283580 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314343 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173580 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156258 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/series/series.pyi
--rw-r--r--   0        0        0   283633 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314655 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173652 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156042 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/series/series.pyi
--rw-r--r--   0        0        0   283674 2024-03-31 08:06:17.638440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314674 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173634 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156058 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/series/series.pyi
--rw-r--r--   0        0        0   283674 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314674 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173634 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156503 2024-03-31 08:06:17.642440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/series/series.pyi
--rw-r--r--   0        0        0   287086 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   315233 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173634 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156550 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/series/series.pyi
--rw-r--r--   0        0        0   284997 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   317000 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/expr/expr.pyi
--rw-r--r--   0        0        0   174644 2024-03-31 08:06:17.646440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   157363 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/series/series.pyi
--rw-r--r--   0        0        0   275823 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   303971 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/expr/expr.pyi
--rw-r--r--   0        0        0   160309 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   145255 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/series/series.pyi
--rw-r--r--   0        0        0   277208 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   307271 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/expr/expr.pyi
--rw-r--r--   0        0        0   161860 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   151043 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/series/series.pyi
--rw-r--r--   0        0        0   279730 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   309374 2024-03-31 08:06:17.650440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/expr/expr.pyi
--rw-r--r--   0        0        0   164582 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   152052 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/series/series.pyi
--rw-r--r--   0        0        0   279723 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   312553 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/expr/expr.pyi
--rw-r--r--   0        0        0   164578 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   152052 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/series/series.pyi
--rw-r--r--   0        0        0   284560 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314071 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173817 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   155688 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/series/series.pyi
--rw-r--r--   0        0        0   284890 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314347 2024-03-31 08:06:17.654440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173881 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   156299 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/series/series.pyi
--rw-r--r--   0        0        0   284700 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314310 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173574 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   155954 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/series/series.pyi
--rw-r--r--   0        0        0   283559 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/dataframe/frame.pyi
--rw-r--r--   0        0        0   314337 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/expr/expr.pyi
--rw-r--r--   0        0        0   173574 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/lazyframe/frame.pyi
--rw-r--r--   0        0        0   155942 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/series/series.pyi
--rw-r--r--   0        0        0     1337 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_testing/namespaces.py
--rw-r--r--   0        0        0       89 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/_version.py
--rw-r--r--   0        0        0     3655 2024-03-31 08:06:17.658440 polugins_type_gen-0.5.5/src/polugins_type_gen/cli.py
--rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 polugins_type_gen-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      137 2024-04-24 15:09:44.420876 polugins_type_gen-0.5.6/README.md
+-rw-r--r--   0        0        0     1155 2024-04-24 15:09:44.420876 polugins_type_gen-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 15:09:44.420876 polugins_type_gen-0.5.6/src/polugins_type_gen/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-24 15:09:44.420876 polugins_type_gen-0.5.6/src/polugins_type_gen/__main__.py
+-rw-r--r--   0        0        0   202000 2024-04-24 15:09:44.420876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   187053 2024-04-24 15:09:44.424876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   118395 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   109948 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/series/series.pyi
+-rw-r--r--   0        0        0   203701 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   188478 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   119581 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   113608 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/series/series.pyi
+-rw-r--r--   0        0        0   203701 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   188477 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   119599 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   113608 2024-04-24 15:09:44.428876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/series/series.pyi
+-rw-r--r--   0        0        0   208700 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   197547 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   120067 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115250 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/series/series.pyi
+-rw-r--r--   0        0        0   214621 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   209693 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   123708 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115386 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/series/series.pyi
+-rw-r--r--   0        0        0   214826 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   209693 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   123708 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115470 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/series/series.pyi
+-rw-r--r--   0        0        0   215930 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   211358 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   123708 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115527 2024-04-24 15:09:44.432876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/series/series.pyi
+-rw-r--r--   0        0        0   215921 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   211623 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   123980 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115661 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/series/series.pyi
+-rw-r--r--   0        0        0   215921 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   211623 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   124768 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115661 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/series/series.pyi
+-rw-r--r--   0        0        0   219412 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   212340 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   124784 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115560 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/series/series.pyi
+-rw-r--r--   0        0        0   212365 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   208256 2024-04-24 15:09:44.436876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   122214 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   114359 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/series/series.pyi
+-rw-r--r--   0        0        0   212365 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   208256 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   122214 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   114359 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/series/series.pyi
+-rw-r--r--   0        0        0   213962 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   209686 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   123271 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   115499 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/series/series.pyi
+-rw-r--r--   0        0        0   220492 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   213716 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   124105 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   116362 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/series/series.pyi
+-rw-r--r--   0        0        0   235341 2024-04-24 15:09:44.440876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   279977 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   129750 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   126656 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/series/series.pyi
+-rw-r--r--   0        0        0   236227 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   279996 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   130618 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   127009 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/series/series.pyi
+-rw-r--r--   0        0        0   243492 2024-04-24 15:09:44.444876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   280112 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   135137 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   127009 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/series/series.pyi
+-rw-r--r--   0        0        0   246531 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   280112 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   135501 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   127139 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/series/series.pyi
+-rw-r--r--   0        0        0   221654 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   218322 2024-04-24 15:09:44.448876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   124918 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   118017 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/series/series.pyi
+-rw-r--r--   0        0        0   222371 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   218700 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   125632 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   118206 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/series/series.pyi
+-rw-r--r--   0        0        0   222426 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   264845 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   125715 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   118188 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/series/series.pyi
+-rw-r--r--   0        0        0   230560 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   274018 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   128405 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   120563 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/series/series.pyi
+-rw-r--r--   0        0        0   231685 2024-04-24 15:09:44.452876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   277726 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   129124 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   122692 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/series/series.pyi
+-rw-r--r--   0        0        0   234690 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   278619 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   129124 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   125575 2024-04-24 15:09:44.456876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/series/series.pyi
+-rw-r--r--   0        0        0   258422 2024-04-24 15:09:44.460876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   281929 2024-04-24 15:09:44.460876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   151704 2024-04-24 15:09:44.460876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   133052 2024-04-24 15:09:44.460876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/series/series.pyi
+-rw-r--r--   0        0        0   258469 2024-04-24 15:09:44.460876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   284476 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   152238 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   133202 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/series/series.pyi
+-rw-r--r--   0        0        0   265646 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   296486 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   159538 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   137670 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/series/series.pyi
+-rw-r--r--   0        0        0   265791 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   298079 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   159794 2024-04-24 15:09:44.464876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   139057 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/series/series.pyi
+-rw-r--r--   0        0        0   265314 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   298000 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   159400 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   139331 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/series/series.pyi
+-rw-r--r--   0        0        0   271168 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   302075 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   159900 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   143267 2024-04-24 15:09:44.468876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/series/series.pyi
+-rw-r--r--   0        0        0   271168 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   303067 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   161034 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   143267 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/series/series.pyi
+-rw-r--r--   0        0        0   273151 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   300748 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   161034 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   144594 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/series/series.pyi
+-rw-r--r--   0        0        0   273187 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   300748 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   161034 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   144594 2024-04-24 15:09:44.472876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/series/series.pyi
+-rw-r--r--   0        0        0   273280 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   300748 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   161034 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   144594 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/series/series.pyi
+-rw-r--r--   0        0        0   258762 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   285703 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   152259 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   133634 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/series/series.pyi
+-rw-r--r--   0        0        0   259358 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   288473 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   153465 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   136036 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/series/series.pyi
+-rw-r--r--   0        0        0   259817 2024-04-24 15:09:44.476876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   288726 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   152522 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   136603 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/series/series.pyi
+-rw-r--r--   0        0        0   259817 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   288726 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   152522 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   136603 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/series/series.pyi
+-rw-r--r--   0        0        0   260303 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   296367 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   152890 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   136668 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/series/series.pyi
+-rw-r--r--   0        0        0   275889 2024-04-24 15:09:44.480876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   303962 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   160309 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   145255 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/series/series.pyi
+-rw-r--r--   0        0        0   275891 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   303971 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   160309 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   145255 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/series/series.pyi
+-rw-r--r--   0        0        0   283580 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314343 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173580 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156258 2024-04-24 15:09:44.484876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/series/series.pyi
+-rw-r--r--   0        0        0   283633 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314655 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173652 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156042 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/series/series.pyi
+-rw-r--r--   0        0        0   283674 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314674 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173634 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156058 2024-04-24 15:09:44.488876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/series/series.pyi
+-rw-r--r--   0        0        0   283674 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314674 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173634 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156503 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/series/series.pyi
+-rw-r--r--   0        0        0   287086 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   315233 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173634 2024-04-24 15:09:44.492876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156550 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/series/series.pyi
+-rw-r--r--   0        0        0   284997 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   317000 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   174644 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   157363 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/series/series.pyi
+-rw-r--r--   0        0        0   285631 2024-04-24 15:09:44.496876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.18/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   318598 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.18/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   174644 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.18/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   157491 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.18/polars/series/series.pyi
+-rw-r--r--   0        0        0   281533 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.19/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   318582 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.19/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173017 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.19/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   157463 2024-04-24 15:09:44.500876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.19/polars/series/series.pyi
+-rw-r--r--   0        0        0   275823 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   303971 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   160309 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   145255 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/series/series.pyi
+-rw-r--r--   0        0        0   282038 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.21/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   322421 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.21/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173647 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.21/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   160180 2024-04-24 15:09:44.504876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.21/polars/series/series.pyi
+-rw-r--r--   0        0        0   281893 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.22/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   322421 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.22/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173327 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.22/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   160180 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.22/polars/series/series.pyi
+-rw-r--r--   0        0        0   277208 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   307271 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   161860 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   151043 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/series/series.pyi
+-rw-r--r--   0        0        0   279730 2024-04-24 15:09:44.508876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   309374 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   164582 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   152052 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/series/series.pyi
+-rw-r--r--   0        0        0   279723 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   312553 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   164578 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   152052 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/series/series.pyi
+-rw-r--r--   0        0        0   284560 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314071 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173817 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   155688 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/series/series.pyi
+-rw-r--r--   0        0        0   284890 2024-04-24 15:09:44.512876 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314347 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173881 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   156299 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/series/series.pyi
+-rw-r--r--   0        0        0   284700 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314310 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173574 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   155954 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/series/series.pyi
+-rw-r--r--   0        0        0   283559 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/dataframe/frame.pyi
+-rw-r--r--   0        0        0   314337 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/expr/expr.pyi
+-rw-r--r--   0        0        0   173574 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/lazyframe/frame.pyi
+-rw-r--r--   0        0        0   155942 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/series/series.pyi
+-rw-r--r--   0        0        0     1337 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_testing/namespaces.py
+-rw-r--r--   0        0        0       89 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/_version.py
+-rw-r--r--   0        0        0     3655 2024-04-24 15:09:44.516877 polugins_type_gen-0.5.6/src/polugins_type_gen/cli.py
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 polugins_type_gen-0.5.6/PKG-INFO
```

### Comparing `polugins_type_gen-0.5.5/pyproject.toml` & `polugins_type_gen-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polugins_type_gen"
-version = "0.5.5"
+version = "0.5.6"
 description = "Type stub generator Polugins."
 authors = ["StefanBRas <opensource@bruhn.io>"]
 readme = "README.md"
 packages = [{include = "polugins_type_gen", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9" # 3.8 cannot be used because we use ast.unparse
```

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.14/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.14/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.15/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.15/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.16/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.16/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.16.18/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.16.18/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.10/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.10/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.11/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.11/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.12/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.12/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.13/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.13/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.14/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.14/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.15/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.15/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.3/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.3/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.5/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.5/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.17.9/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.17.9/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.0/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.0/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.11/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.11/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.12/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.12/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.13/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.13/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.15/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.15/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.2/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.2/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.3/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.3/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.4/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.4/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.6/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.6/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.7/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.7/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.18.8/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.18.8/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.0/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.0/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.1/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.1/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.11/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.11/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.12/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.12/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.13/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.13/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.14/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.14/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.15/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.15/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.17/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.17/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.18/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.18/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.19/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.19/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.2/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.2/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.3/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.3/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.5/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.5/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.6/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.6/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.19.7/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.19.7/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.0/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.0/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.1/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.1/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.10/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.10/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.13/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.13/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.14/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.14/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.15/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.15/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.16/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.16/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.17/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.17/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.2/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.2/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.3/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.3/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.4/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.4/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.5/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.5/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.6/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.6/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.7/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.7/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.8/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.8/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/dataframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/dataframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/expr/expr.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/expr/expr.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/lazyframe/frame.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/lazyframe/frame.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_stubs/0.20.9/polars/series/series.pyi` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_stubs/0.20.9/polars/series/series.pyi`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/_testing/namespaces.py` & `polugins_type_gen-0.5.6/src/polugins_type_gen/_testing/namespaces.py`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/src/polugins_type_gen/cli.py` & `polugins_type_gen-0.5.6/src/polugins_type_gen/cli.py`

 * *Files identical despite different names*

### Comparing `polugins_type_gen-0.5.5/PKG-INFO` & `polugins_type_gen-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polugins_type_gen
-Version: 0.5.5
+Version: 0.5.6
 Summary: Type stub generator Polugins.
 Author: StefanBRas
 Author-email: opensource@bruhn.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

