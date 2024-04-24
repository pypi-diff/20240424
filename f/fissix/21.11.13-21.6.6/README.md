# Comparing `tmp/fissix-21.11.13.tar.gz` & `tmp/fissix-21.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissix-21.11.13.tar", last modified: Sat Nov 13 23:27:15 2021, max compression
+gzip compressed data, was "fissix-21.6.6.tar", last modified: Mon Jun  7 02:57:07 2021, max compression
```

## Comparing `fissix-21.11.13.tar` & `fissix-21.6.6.tar`

### file list

```diff
@@ -1,126 +1,127 @@
--rw-r--r--   0        0        0      789 2021-06-07 00:05:30.710065 fissix-21.11.13/.gitignore
--rw-r--r--   0        0        0       79 2021-06-07 00:05:30.710178 fissix-21.11.13/.gitmodules
--rw-r--r--   0        0        0      156 2021-06-07 00:05:30.710302 fissix-21.11.13/.readthedocs.yml
--rw-r--r--   0        0        0     2899 2021-11-13 23:21:42.044196 fissix-21.11.13/CHANGELOG.md
--rw-r--r--   0        0        0    12930 2021-06-07 00:05:30.710651 fissix-21.11.13/LICENSE
--rw-r--r--   0        0        0       43 2021-06-07 00:05:30.710762 fissix-21.11.13/MANIFEST.in
--rw-r--r--   0        0        0     1220 2021-06-07 00:05:30.710900 fissix-21.11.13/README.md
-drwxr-xr-x   0        0        0        0 2021-06-07 00:05:30.710953 fissix-21.11.13/cpython/
--rw-r--r--   0        0        0      284 2021-06-07 00:05:30.711219 fissix-21.11.13/docs/_static/custom.css
--rw-r--r--   0        0        0      342 2021-06-07 00:05:30.711392 fissix-21.11.13/docs/_templates/badges.html
--rw-r--r--   0        0        0      291 2021-06-07 00:05:30.711511 fissix-21.11.13/docs/api.rst
--rw-r--r--   0        0        0       70 2021-06-07 02:43:35.125261 fissix-21.11.13/docs/changelog.rst
--rw-r--r--   0        0        0     2703 2021-06-07 00:05:30.711652 fissix-21.11.13/docs/conf.py
--rw-r--r--   0        0        0    10515 2021-06-07 00:05:30.711857 fissix-21.11.13/docs/fixers.rst
--rw-r--r--   0        0        0      151 2021-06-07 02:44:14.141972 fissix-21.11.13/docs/index.rst
--rw-r--r--   0        0        0     6724 2021-06-07 00:05:30.712199 fissix-21.11.13/fissix/Grammar.txt
--rw-r--r--   0        0        0      793 2021-06-07 00:05:30.712314 fissix-21.11.13/fissix/PatternGrammar.txt
--rw-r--r--   0        0        0     1676 2021-06-07 02:47:46.468632 fissix-21.11.13/fissix/__init__.py
--rw-r--r--   0        0        0       66 2021-06-07 02:23:30.941246 fissix-21.11.13/fissix/__main__.py
--rw-r--r--   0        0        0       25 2021-11-13 23:21:42.052686 fissix-21.11.13/fissix/__version__.py
--rw-r--r--   0        0        0     6747 2021-06-07 02:23:30.941602 fissix-21.11.13/fissix/btm_matcher.py
--rw-r--r--   0        0        0     9975 2021-06-07 00:05:30.712782 fissix-21.11.13/fissix/btm_utils.py
--rw-r--r--   0        0        0     6558 2021-06-07 02:27:43.677241 fissix-21.11.13/fissix/fixer_base.py
--rw-r--r--   0        0        0    15418 2021-06-07 02:23:30.942293 fissix-21.11.13/fissix/fixer_util.py
--rw-r--r--   0        0        0       47 2021-06-07 00:05:30.713241 fissix-21.11.13/fissix/fixes/__init__.py
--rw-r--r--   0        0        0     2314 2021-06-07 02:23:30.942604 fissix-21.11.13/fissix/fixes/fix_apply.py
--rw-r--r--   0        0        0      998 2021-06-07 00:05:30.713464 fissix-21.11.13/fissix/fixes/fix_asserts.py
--rw-r--r--   0        0        0      321 2021-06-07 00:05:30.713559 fissix-21.11.13/fissix/fixes/fix_basestring.py
--rw-r--r--   0        0        0      591 2021-06-07 00:05:30.713662 fissix-21.11.13/fissix/fixes/fix_buffer.py
--rw-r--r--   0        0        0     3748 2021-06-07 02:23:30.942897 fissix-21.11.13/fissix/fixes/fix_dict.py
--rw-r--r--   0        0        0     3547 2021-11-13 23:01:28.426040 fissix-21.11.13/fissix/fixes/fix_except.py
--rw-r--r--   0        0        0      979 2021-06-07 00:05:30.714050 fissix-21.11.13/fissix/fixes/fix_exec.py
--rw-r--r--   0        0        0     2078 2021-06-07 00:05:30.714196 fissix-21.11.13/fissix/fixes/fix_execfile.py
--rw-r--r--   0        0        0     2433 2021-06-07 00:05:30.714319 fissix-21.11.13/fissix/fixes/fix_exitfunc.py
--rw-r--r--   0        0        0     2709 2021-06-07 02:23:30.943432 fissix-21.11.13/fissix/fixes/fix_filter.py
--rw-r--r--   0        0        0      618 2021-06-07 00:05:30.714551 fissix-21.11.13/fissix/fixes/fix_funcattrs.py
--rw-r--r--   0        0        0      548 2021-06-07 00:05:30.714658 fissix-21.11.13/fissix/fixes/fix_future.py
--rw-r--r--   0        0        0      452 2021-06-07 00:05:30.714761 fissix-21.11.13/fissix/fixes/fix_getcwdu.py
--rw-r--r--   0        0        0     3276 2021-06-07 02:23:30.943702 fissix-21.11.13/fissix/fixes/fix_has_key.py
--rw-r--r--   0        0        0     4882 2021-06-07 00:05:30.715016 fissix-21.11.13/fissix/fixes/fix_idioms.py
--rw-r--r--   0        0        0     3256 2021-06-07 02:23:30.943956 fissix-21.11.13/fissix/fixes/fix_import.py
--rw-r--r--   0        0        0     5392 2021-06-07 00:05:30.715290 fissix-21.11.13/fissix/fixes/fix_imports.py
--rw-r--r--   0        0        0      252 2021-06-07 00:05:30.715394 fissix-21.11.13/fissix/fixes/fix_imports2.py
--rw-r--r--   0        0        0      708 2021-06-07 02:23:30.944143 fissix-21.11.13/fissix/fixes/fix_input.py
--rw-r--r--   0        0        0     1181 2021-06-07 00:05:30.715626 fissix-21.11.13/fissix/fixes/fix_intern.py
--rw-r--r--   0        0        0     1757 2021-06-07 00:05:30.715766 fissix-21.11.13/fissix/fixes/fix_isinstance.py
--rw-r--r--   0        0        0     1550 2021-06-07 00:05:30.715869 fissix-21.11.13/fissix/fixes/fix_itertools.py
--rw-r--r--   0        0        0     2124 2021-06-07 00:05:30.715989 fissix-21.11.13/fissix/fixes/fix_itertools_imports.py
--rw-r--r--   0        0        0      474 2021-06-07 00:05:30.716089 fissix-21.11.13/fissix/fixes/fix_long.py
--rw-r--r--   0        0        0     3726 2021-06-07 02:23:30.944356 fissix-21.11.13/fissix/fixes/fix_map.py
--rw-r--r--   0        0        0     8117 2021-06-07 02:23:30.944607 fissix-21.11.13/fissix/fixes/fix_metaclass.py
--rw-r--r--   0        0        0      586 2021-06-07 00:05:30.716476 fissix-21.11.13/fissix/fixes/fix_methodattrs.py
--rw-r--r--   0        0        0      571 2021-06-07 02:23:30.944821 fissix-21.11.13/fissix/fixes/fix_ne.py
--rw-r--r--   0        0        0     3178 2021-06-07 02:23:30.945032 fissix-21.11.13/fissix/fixes/fix_next.py
--rw-r--r--   0        0        0      592 2021-06-07 00:05:30.716785 fissix-21.11.13/fissix/fixes/fix_nonzero.py
--rw-r--r--   0        0        0     1006 2021-06-07 02:23:30.945221 fissix-21.11.13/fissix/fixes/fix_numliterals.py
--rw-r--r--   0        0        0     3439 2021-06-07 00:05:30.717037 fissix-21.11.13/fissix/fixes/fix_operator.py
--rw-r--r--   0        0        0     1228 2021-06-07 00:05:30.717137 fissix-21.11.13/fissix/fixes/fix_paren.py
--rw-r--r--   0        0        0     2705 2021-06-07 02:23:30.945432 fissix-21.11.13/fissix/fixes/fix_print.py
--rw-r--r--   0        0        0     3002 2021-06-07 02:23:30.945643 fissix-21.11.13/fissix/fixes/fix_raise.py
--rw-r--r--   0        0        0      455 2021-06-07 00:05:30.717485 fissix-21.11.13/fissix/fixes/fix_raw_input.py
--rw-r--r--   0        0        0      834 2021-06-07 00:05:30.717587 fissix-21.11.13/fissix/fixes/fix_reduce.py
--rw-r--r--   0        0        0     1118 2021-06-07 00:05:30.717684 fissix-21.11.13/fissix/fixes/fix_reload.py
--rw-r--r--   0        0        0     2327 2021-06-07 00:05:30.717799 fissix-21.11.13/fissix/fixes/fix_renames.py
--rw-r--r--   0        0        0      613 2021-06-07 00:05:30.717899 fissix-21.11.13/fissix/fixes/fix_repr.py
--rw-r--r--   0        0        0     1694 2021-06-07 00:05:30.718015 fissix-21.11.13/fissix/fixes/fix_set_literal.py
--rw-r--r--   0        0        0     3618 2021-06-07 00:05:30.718145 fissix-21.11.13/fissix/fixes/fix_sorted.py
--rw-r--r--   0        0        0      449 2021-06-07 00:05:30.718266 fissix-21.11.13/fissix/fixes/fix_standarderror.py
--rw-r--r--   0        0        0     1049 2021-06-07 00:05:30.718362 fissix-21.11.13/fissix/fixes/fix_sys_exc.py
--rw-r--r--   0        0        0     1583 2021-06-07 02:23:30.945849 fissix-21.11.13/fissix/fixes/fix_throw.py
--rw-r--r--   0        0        0     5478 2021-06-07 02:23:30.946088 fissix-21.11.13/fissix/fixes/fix_tuple_params.py
--rw-r--r--   0        0        0     1673 2021-06-07 00:05:30.718729 fissix-21.11.13/fissix/fixes/fix_types.py
--rw-r--r--   0        0        0     1305 2021-06-07 02:23:30.946285 fissix-21.11.13/fissix/fixes/fix_unicode.py
--rw-r--r--   0        0        0     8959 2021-11-13 23:01:28.426383 fissix-21.11.13/fissix/fixes/fix_urllib.py
--rw-r--r--   0        0        0     1207 2021-06-07 02:23:30.946771 fissix-21.11.13/fissix/fixes/fix_ws_comma.py
--rw-r--r--   0        0        0     2689 2021-06-07 02:23:30.946988 fissix-21.11.13/fissix/fixes/fix_xrange.py
--rw-r--r--   0        0        0      689 2021-06-07 00:05:30.719327 fissix-21.11.13/fissix/fixes/fix_xreadlines.py
--rw-r--r--   0        0        0     1289 2021-06-07 02:23:30.947191 fissix-21.11.13/fissix/fixes/fix_zip.py
--rw-r--r--   0        0        0    11962 2021-06-07 02:23:30.947487 fissix-21.11.13/fissix/main.py
--rw-r--r--   0        0        0     7034 2021-06-07 02:23:30.947771 fissix-21.11.13/fissix/patcomp.py
--rw-r--r--   0        0        0      143 2021-06-07 00:05:30.719922 fissix-21.11.13/fissix/pgen2/__init__.py
--rw-r--r--   0        0        0     9584 2021-06-07 00:05:30.720075 fissix-21.11.13/fissix/pgen2/conv.py
--rw-r--r--   0        0        0     5897 2021-06-07 02:23:30.948120 fissix-21.11.13/fissix/pgen2/driver.py
--rw-r--r--   0        0        0     5591 2021-06-07 00:05:30.720368 fissix-21.11.13/fissix/pgen2/grammar.py
--rw-r--r--   0        0        0     1528 2021-06-07 00:05:30.720486 fissix-21.11.13/fissix/pgen2/literals.py
--rw-r--r--   0        0        0     8113 2021-06-07 00:05:30.720639 fissix-21.11.13/fissix/pgen2/parse.py
--rw-r--r--   0        0        0    13807 2021-06-07 00:05:30.720816 fissix-21.11.13/fissix/pgen2/pgen.py
--rwxr-xr-x   0        0        0     1306 2021-06-07 00:05:30.720938 fissix-21.11.13/fissix/pgen2/token.py
--rw-r--r--   0        0        0    21615 2021-06-07 02:49:46.157734 fissix-21.11.13/fissix/pgen2/tokenize.py
--rw-r--r--   0        0        0     1265 2021-06-07 02:23:30.948357 fissix-21.11.13/fissix/pygram.py
--rw-r--r--   0        0        0    27897 2021-06-07 00:05:30.721599 fissix-21.11.13/fissix/pytree.py
--rw-r--r--   0        0        0    27385 2021-06-07 02:23:30.948768 fissix-21.11.13/fissix/refactor.py
--rw-r--r--   0        0        0        0 2021-06-07 00:05:30.722024 fissix-21.11.13/fissix/tests/__init__.py
--rw-r--r--   0        0        0       58 2021-06-07 02:23:30.949117 fissix-21.11.13/fissix/tests/__main__.py
--rw-r--r--   0        0        0      402 2021-06-07 00:05:30.722279 fissix-21.11.13/fissix/tests/data/README
--rw-r--r--   0        0        0       37 2021-06-07 00:05:30.722367 fissix-21.11.13/fissix/tests/data/bom.py
--rw-r--r--   0        0        0       50 2021-06-07 00:05:30.722457 fissix-21.11.13/fissix/tests/data/crlf.py
--rwxr-xr-x   0        0        0      231 2021-06-07 00:05:30.722564 fissix-21.11.13/fissix/tests/data/different_encoding.py
--rwxr-xr-x   0        0        0       40 2021-06-07 00:05:30.722663 fissix-21.11.13/fissix/tests/data/false_encoding.py
--rw-r--r--   0        0        0       89 2021-06-07 00:05:30.722823 fissix-21.11.13/fissix/tests/data/fixers/bad_order.py
--rw-r--r--   0        0        0        0 2021-06-07 00:05:30.722928 fissix-21.11.13/fissix/tests/data/fixers/myfixes/__init__.py
--rw-r--r--   0        0        0      131 2021-06-07 00:05:30.723046 fissix-21.11.13/fissix/tests/data/fixers/myfixes/fix_explicit.py
--rw-r--r--   0        0        0      132 2021-06-07 00:05:30.723141 fissix-21.11.13/fissix/tests/data/fixers/myfixes/fix_first.py
--rw-r--r--   0        0        0      133 2021-06-07 00:05:30.723230 fissix-21.11.13/fissix/tests/data/fixers/myfixes/fix_last.py
--rw-r--r--   0        0        0      346 2021-06-07 00:05:30.723328 fissix-21.11.13/fissix/tests/data/fixers/myfixes/fix_parrot.py
--rw-r--r--   0        0        0      135 2021-06-07 00:05:30.723425 fissix-21.11.13/fissix/tests/data/fixers/myfixes/fix_preorder.py
--rw-r--r--   0        0        0       75 2021-06-07 00:05:30.723526 fissix-21.11.13/fissix/tests/data/fixers/no_fixer_cls.py
--rw-r--r--   0        0        0       23 2021-06-07 00:05:30.723631 fissix-21.11.13/fissix/tests/data/fixers/parrot_example.py
--rw-r--r--   0        0        0    95775 2021-06-07 00:05:30.724163 fissix-21.11.13/fissix/tests/data/infinite_recursion.py
--rw-r--r--   0        0        0    33729 2021-06-07 00:05:30.724501 fissix-21.11.13/fissix/tests/data/py2_test_grammar.py
--rw-r--r--   0        0        0    31245 2021-06-07 02:23:30.949770 fissix-21.11.13/fissix/tests/data/py3_test_grammar.py
--rwxr-xr-x   0        0        0     2470 2021-06-07 02:23:30.950100 fissix-21.11.13/fissix/tests/pytree_idempotency.py
--rw-r--r--   0        0        0     1946 2021-06-07 02:23:30.950334 fissix-21.11.13/fissix/tests/support.py
--rw-r--r--   0        0        0      595 2021-06-07 02:23:30.950571 fissix-21.11.13/fissix/tests/test_all_fixers.py
--rw-r--r--   0        0        0   125644 2021-11-13 23:01:28.427508 fissix-21.11.13/fissix/tests/test_fixers.py
--rw-r--r--   0        0        0     6307 2021-06-07 00:05:30.725788 fissix-21.11.13/fissix/tests/test_main.py
--rw-r--r--   0        0        0    22605 2021-06-07 02:23:30.950970 fissix-21.11.13/fissix/tests/test_parser.py
--rw-r--r--   0        0        0    16304 2021-06-07 02:23:30.951292 fissix-21.11.13/fissix/tests/test_pytree.py
--rw-r--r--   0        0        0    12353 2021-06-07 02:23:30.951605 fissix-21.11.13/fissix/tests/test_refactor.py
--rw-r--r--   0        0        0    21189 2021-06-07 02:23:30.951914 fissix-21.11.13/fissix/tests/test_util.py
--rw-r--r--   0        0        0      785 2021-06-07 02:27:55.807138 fissix-21.11.13/makefile
--rw-r--r--   0        0        0      986 2021-06-07 02:29:32.138959 fissix-21.11.13/pyproject.toml
--rw-r--r--   0        0        0      122 2021-06-07 02:29:01.869306 fissix-21.11.13/requirements-dev.txt
--rw-r--r--   0        0        0       15 2021-06-07 02:28:43.791071 fissix-21.11.13/requirements.txt
--rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 fissix-21.11.13/setup.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 fissix-21.11.13/PKG-INFO
+-rw-r--r--   0        0        0      789 2021-06-07 00:05:30.710065 fissix-21.6.6/.gitignore
+-rw-r--r--   0        0        0       79 2021-06-07 00:05:30.710178 fissix-21.6.6/.gitmodules
+-rw-r--r--   0        0        0      156 2021-06-07 00:05:30.710302 fissix-21.6.6/.readthedocs.yml
+-rw-r--r--   0        0        0      346 2021-06-07 00:05:30.710425 fissix-21.6.6/.travis.yml
+-rw-r--r--   0        0        0     2572 2021-06-07 02:42:02.342263 fissix-21.6.6/CHANGELOG.md
+-rw-r--r--   0        0        0    12930 2021-06-07 00:05:30.710651 fissix-21.6.6/LICENSE
+-rw-r--r--   0        0        0       43 2021-06-07 00:05:30.710762 fissix-21.6.6/MANIFEST.in
+-rw-r--r--   0        0        0     1220 2021-06-07 00:05:30.710900 fissix-21.6.6/README.md
+drwxr-xr-x   0        0        0        0 2021-06-07 00:05:30.710953 fissix-21.6.6/cpython/
+-rw-r--r--   0        0        0      284 2021-06-07 00:05:30.711219 fissix-21.6.6/docs/_static/custom.css
+-rw-r--r--   0        0        0      342 2021-06-07 00:05:30.711392 fissix-21.6.6/docs/_templates/badges.html
+-rw-r--r--   0        0        0      291 2021-06-07 00:05:30.711511 fissix-21.6.6/docs/api.rst
+-rw-r--r--   0        0        0       70 2021-06-07 02:43:35.125261 fissix-21.6.6/docs/changelog.rst
+-rw-r--r--   0        0        0     2703 2021-06-07 00:05:30.711652 fissix-21.6.6/docs/conf.py
+-rw-r--r--   0        0        0    10515 2021-06-07 00:05:30.711857 fissix-21.6.6/docs/fixers.rst
+-rw-r--r--   0        0        0      151 2021-06-07 02:44:14.141972 fissix-21.6.6/docs/index.rst
+-rw-r--r--   0        0        0     6724 2021-06-07 00:05:30.712199 fissix-21.6.6/fissix/Grammar.txt
+-rw-r--r--   0        0        0      793 2021-06-07 00:05:30.712314 fissix-21.6.6/fissix/PatternGrammar.txt
+-rw-r--r--   0        0        0     1676 2021-06-07 02:47:46.468632 fissix-21.6.6/fissix/__init__.py
+-rw-r--r--   0        0        0       66 2021-06-07 02:23:30.941246 fissix-21.6.6/fissix/__main__.py
+-rw-r--r--   0        0        0       23 2021-06-07 02:42:02.351456 fissix-21.6.6/fissix/__version__.py
+-rw-r--r--   0        0        0     6747 2021-06-07 02:23:30.941602 fissix-21.6.6/fissix/btm_matcher.py
+-rw-r--r--   0        0        0     9975 2021-06-07 00:05:30.712782 fissix-21.6.6/fissix/btm_utils.py
+-rw-r--r--   0        0        0     6558 2021-06-07 02:27:43.677241 fissix-21.6.6/fissix/fixer_base.py
+-rw-r--r--   0        0        0    15418 2021-06-07 02:23:30.942293 fissix-21.6.6/fissix/fixer_util.py
+-rw-r--r--   0        0        0       47 2021-06-07 00:05:30.713241 fissix-21.6.6/fissix/fixes/__init__.py
+-rw-r--r--   0        0        0     2314 2021-06-07 02:23:30.942604 fissix-21.6.6/fissix/fixes/fix_apply.py
+-rw-r--r--   0        0        0      998 2021-06-07 00:05:30.713464 fissix-21.6.6/fissix/fixes/fix_asserts.py
+-rw-r--r--   0        0        0      321 2021-06-07 00:05:30.713559 fissix-21.6.6/fissix/fixes/fix_basestring.py
+-rw-r--r--   0        0        0      591 2021-06-07 00:05:30.713662 fissix-21.6.6/fissix/fixes/fix_buffer.py
+-rw-r--r--   0        0        0     3748 2021-06-07 02:23:30.942897 fissix-21.6.6/fissix/fixes/fix_dict.py
+-rw-r--r--   0        0        0     3493 2021-06-07 02:23:30.943154 fissix-21.6.6/fissix/fixes/fix_except.py
+-rw-r--r--   0        0        0      979 2021-06-07 00:05:30.714050 fissix-21.6.6/fissix/fixes/fix_exec.py
+-rw-r--r--   0        0        0     2078 2021-06-07 00:05:30.714196 fissix-21.6.6/fissix/fixes/fix_execfile.py
+-rw-r--r--   0        0        0     2433 2021-06-07 00:05:30.714319 fissix-21.6.6/fissix/fixes/fix_exitfunc.py
+-rw-r--r--   0        0        0     2709 2021-06-07 02:23:30.943432 fissix-21.6.6/fissix/fixes/fix_filter.py
+-rw-r--r--   0        0        0      618 2021-06-07 00:05:30.714551 fissix-21.6.6/fissix/fixes/fix_funcattrs.py
+-rw-r--r--   0        0        0      548 2021-06-07 00:05:30.714658 fissix-21.6.6/fissix/fixes/fix_future.py
+-rw-r--r--   0        0        0      452 2021-06-07 00:05:30.714761 fissix-21.6.6/fissix/fixes/fix_getcwdu.py
+-rw-r--r--   0        0        0     3276 2021-06-07 02:23:30.943702 fissix-21.6.6/fissix/fixes/fix_has_key.py
+-rw-r--r--   0        0        0     4882 2021-06-07 00:05:30.715016 fissix-21.6.6/fissix/fixes/fix_idioms.py
+-rw-r--r--   0        0        0     3256 2021-06-07 02:23:30.943956 fissix-21.6.6/fissix/fixes/fix_import.py
+-rw-r--r--   0        0        0     5392 2021-06-07 00:05:30.715290 fissix-21.6.6/fissix/fixes/fix_imports.py
+-rw-r--r--   0        0        0      252 2021-06-07 00:05:30.715394 fissix-21.6.6/fissix/fixes/fix_imports2.py
+-rw-r--r--   0        0        0      708 2021-06-07 02:23:30.944143 fissix-21.6.6/fissix/fixes/fix_input.py
+-rw-r--r--   0        0        0     1181 2021-06-07 00:05:30.715626 fissix-21.6.6/fissix/fixes/fix_intern.py
+-rw-r--r--   0        0        0     1757 2021-06-07 00:05:30.715766 fissix-21.6.6/fissix/fixes/fix_isinstance.py
+-rw-r--r--   0        0        0     1550 2021-06-07 00:05:30.715869 fissix-21.6.6/fissix/fixes/fix_itertools.py
+-rw-r--r--   0        0        0     2124 2021-06-07 00:05:30.715989 fissix-21.6.6/fissix/fixes/fix_itertools_imports.py
+-rw-r--r--   0        0        0      474 2021-06-07 00:05:30.716089 fissix-21.6.6/fissix/fixes/fix_long.py
+-rw-r--r--   0        0        0     3726 2021-06-07 02:23:30.944356 fissix-21.6.6/fissix/fixes/fix_map.py
+-rw-r--r--   0        0        0     8117 2021-06-07 02:23:30.944607 fissix-21.6.6/fissix/fixes/fix_metaclass.py
+-rw-r--r--   0        0        0      586 2021-06-07 00:05:30.716476 fissix-21.6.6/fissix/fixes/fix_methodattrs.py
+-rw-r--r--   0        0        0      571 2021-06-07 02:23:30.944821 fissix-21.6.6/fissix/fixes/fix_ne.py
+-rw-r--r--   0        0        0     3178 2021-06-07 02:23:30.945032 fissix-21.6.6/fissix/fixes/fix_next.py
+-rw-r--r--   0        0        0      592 2021-06-07 00:05:30.716785 fissix-21.6.6/fissix/fixes/fix_nonzero.py
+-rw-r--r--   0        0        0     1006 2021-06-07 02:23:30.945221 fissix-21.6.6/fissix/fixes/fix_numliterals.py
+-rw-r--r--   0        0        0     3439 2021-06-07 00:05:30.717037 fissix-21.6.6/fissix/fixes/fix_operator.py
+-rw-r--r--   0        0        0     1228 2021-06-07 00:05:30.717137 fissix-21.6.6/fissix/fixes/fix_paren.py
+-rw-r--r--   0        0        0     2705 2021-06-07 02:23:30.945432 fissix-21.6.6/fissix/fixes/fix_print.py
+-rw-r--r--   0        0        0     3002 2021-06-07 02:23:30.945643 fissix-21.6.6/fissix/fixes/fix_raise.py
+-rw-r--r--   0        0        0      455 2021-06-07 00:05:30.717485 fissix-21.6.6/fissix/fixes/fix_raw_input.py
+-rw-r--r--   0        0        0      834 2021-06-07 00:05:30.717587 fissix-21.6.6/fissix/fixes/fix_reduce.py
+-rw-r--r--   0        0        0     1118 2021-06-07 00:05:30.717684 fissix-21.6.6/fissix/fixes/fix_reload.py
+-rw-r--r--   0        0        0     2327 2021-06-07 00:05:30.717799 fissix-21.6.6/fissix/fixes/fix_renames.py
+-rw-r--r--   0        0        0      613 2021-06-07 00:05:30.717899 fissix-21.6.6/fissix/fixes/fix_repr.py
+-rw-r--r--   0        0        0     1694 2021-06-07 00:05:30.718015 fissix-21.6.6/fissix/fixes/fix_set_literal.py
+-rw-r--r--   0        0        0     3618 2021-06-07 00:05:30.718145 fissix-21.6.6/fissix/fixes/fix_sorted.py
+-rw-r--r--   0        0        0      449 2021-06-07 00:05:30.718266 fissix-21.6.6/fissix/fixes/fix_standarderror.py
+-rw-r--r--   0        0        0     1049 2021-06-07 00:05:30.718362 fissix-21.6.6/fissix/fixes/fix_sys_exc.py
+-rw-r--r--   0        0        0     1583 2021-06-07 02:23:30.945849 fissix-21.6.6/fissix/fixes/fix_throw.py
+-rw-r--r--   0        0        0     5478 2021-06-07 02:23:30.946088 fissix-21.6.6/fissix/fixes/fix_tuple_params.py
+-rw-r--r--   0        0        0     1673 2021-06-07 00:05:30.718729 fissix-21.6.6/fissix/fixes/fix_types.py
+-rw-r--r--   0        0        0     1305 2021-06-07 02:23:30.946285 fissix-21.6.6/fissix/fixes/fix_unicode.py
+-rw-r--r--   0        0        0     8928 2021-06-07 02:23:30.946564 fissix-21.6.6/fissix/fixes/fix_urllib.py
+-rw-r--r--   0        0        0     1207 2021-06-07 02:23:30.946771 fissix-21.6.6/fissix/fixes/fix_ws_comma.py
+-rw-r--r--   0        0        0     2689 2021-06-07 02:23:30.946988 fissix-21.6.6/fissix/fixes/fix_xrange.py
+-rw-r--r--   0        0        0      689 2021-06-07 00:05:30.719327 fissix-21.6.6/fissix/fixes/fix_xreadlines.py
+-rw-r--r--   0        0        0     1289 2021-06-07 02:23:30.947191 fissix-21.6.6/fissix/fixes/fix_zip.py
+-rw-r--r--   0        0        0    11962 2021-06-07 02:23:30.947487 fissix-21.6.6/fissix/main.py
+-rw-r--r--   0        0        0     7034 2021-06-07 02:23:30.947771 fissix-21.6.6/fissix/patcomp.py
+-rw-r--r--   0        0        0      143 2021-06-07 00:05:30.719922 fissix-21.6.6/fissix/pgen2/__init__.py
+-rw-r--r--   0        0        0     9584 2021-06-07 00:05:30.720075 fissix-21.6.6/fissix/pgen2/conv.py
+-rw-r--r--   0        0        0     5897 2021-06-07 02:23:30.948120 fissix-21.6.6/fissix/pgen2/driver.py
+-rw-r--r--   0        0        0     5591 2021-06-07 00:05:30.720368 fissix-21.6.6/fissix/pgen2/grammar.py
+-rw-r--r--   0        0        0     1528 2021-06-07 00:05:30.720486 fissix-21.6.6/fissix/pgen2/literals.py
+-rw-r--r--   0        0        0     8113 2021-06-07 00:05:30.720639 fissix-21.6.6/fissix/pgen2/parse.py
+-rw-r--r--   0        0        0    13807 2021-06-07 00:05:30.720816 fissix-21.6.6/fissix/pgen2/pgen.py
+-rwxr-xr-x   0        0        0     1306 2021-06-07 00:05:30.720938 fissix-21.6.6/fissix/pgen2/token.py
+-rw-r--r--   0        0        0    21615 2021-06-07 02:49:46.157734 fissix-21.6.6/fissix/pgen2/tokenize.py
+-rw-r--r--   0        0        0     1265 2021-06-07 02:23:30.948357 fissix-21.6.6/fissix/pygram.py
+-rw-r--r--   0        0        0    27897 2021-06-07 00:05:30.721599 fissix-21.6.6/fissix/pytree.py
+-rw-r--r--   0        0        0    27385 2021-06-07 02:23:30.948768 fissix-21.6.6/fissix/refactor.py
+-rw-r--r--   0        0        0        0 2021-06-07 00:05:30.722024 fissix-21.6.6/fissix/tests/__init__.py
+-rw-r--r--   0        0        0       58 2021-06-07 02:23:30.949117 fissix-21.6.6/fissix/tests/__main__.py
+-rw-r--r--   0        0        0      402 2021-06-07 00:05:30.722279 fissix-21.6.6/fissix/tests/data/README
+-rw-r--r--   0        0        0       37 2021-06-07 00:05:30.722367 fissix-21.6.6/fissix/tests/data/bom.py
+-rw-r--r--   0        0        0       50 2021-06-07 00:05:30.722457 fissix-21.6.6/fissix/tests/data/crlf.py
+-rwxr-xr-x   0        0        0      231 2021-06-07 00:05:30.722564 fissix-21.6.6/fissix/tests/data/different_encoding.py
+-rwxr-xr-x   0        0        0       40 2021-06-07 00:05:30.722663 fissix-21.6.6/fissix/tests/data/false_encoding.py
+-rw-r--r--   0        0        0       89 2021-06-07 00:05:30.722823 fissix-21.6.6/fissix/tests/data/fixers/bad_order.py
+-rw-r--r--   0        0        0        0 2021-06-07 00:05:30.722928 fissix-21.6.6/fissix/tests/data/fixers/myfixes/__init__.py
+-rw-r--r--   0        0        0      131 2021-06-07 00:05:30.723046 fissix-21.6.6/fissix/tests/data/fixers/myfixes/fix_explicit.py
+-rw-r--r--   0        0        0      132 2021-06-07 00:05:30.723141 fissix-21.6.6/fissix/tests/data/fixers/myfixes/fix_first.py
+-rw-r--r--   0        0        0      133 2021-06-07 00:05:30.723230 fissix-21.6.6/fissix/tests/data/fixers/myfixes/fix_last.py
+-rw-r--r--   0        0        0      346 2021-06-07 00:05:30.723328 fissix-21.6.6/fissix/tests/data/fixers/myfixes/fix_parrot.py
+-rw-r--r--   0        0        0      135 2021-06-07 00:05:30.723425 fissix-21.6.6/fissix/tests/data/fixers/myfixes/fix_preorder.py
+-rw-r--r--   0        0        0       75 2021-06-07 00:05:30.723526 fissix-21.6.6/fissix/tests/data/fixers/no_fixer_cls.py
+-rw-r--r--   0        0        0       23 2021-06-07 00:05:30.723631 fissix-21.6.6/fissix/tests/data/fixers/parrot_example.py
+-rw-r--r--   0        0        0    95775 2021-06-07 00:05:30.724163 fissix-21.6.6/fissix/tests/data/infinite_recursion.py
+-rw-r--r--   0        0        0    33729 2021-06-07 00:05:30.724501 fissix-21.6.6/fissix/tests/data/py2_test_grammar.py
+-rw-r--r--   0        0        0    31245 2021-06-07 02:23:30.949770 fissix-21.6.6/fissix/tests/data/py3_test_grammar.py
+-rwxr-xr-x   0        0        0     2470 2021-06-07 02:23:30.950100 fissix-21.6.6/fissix/tests/pytree_idempotency.py
+-rw-r--r--   0        0        0     1946 2021-06-07 02:23:30.950334 fissix-21.6.6/fissix/tests/support.py
+-rw-r--r--   0        0        0      595 2021-06-07 02:23:30.950571 fissix-21.6.6/fissix/tests/test_all_fixers.py
+-rw-r--r--   0        0        0   125472 2021-06-07 00:05:30.725641 fissix-21.6.6/fissix/tests/test_fixers.py
+-rw-r--r--   0        0        0     6307 2021-06-07 00:05:30.725788 fissix-21.6.6/fissix/tests/test_main.py
+-rw-r--r--   0        0        0    22605 2021-06-07 02:23:30.950970 fissix-21.6.6/fissix/tests/test_parser.py
+-rw-r--r--   0        0        0    16304 2021-06-07 02:23:30.951292 fissix-21.6.6/fissix/tests/test_pytree.py
+-rw-r--r--   0        0        0    12353 2021-06-07 02:23:30.951605 fissix-21.6.6/fissix/tests/test_refactor.py
+-rw-r--r--   0        0        0    21189 2021-06-07 02:23:30.951914 fissix-21.6.6/fissix/tests/test_util.py
+-rw-r--r--   0        0        0      785 2021-06-07 02:27:55.807138 fissix-21.6.6/makefile
+-rw-r--r--   0        0        0      986 2021-06-07 02:29:32.138959 fissix-21.6.6/pyproject.toml
+-rw-r--r--   0        0        0      122 2021-06-07 02:29:01.869306 fissix-21.6.6/requirements-dev.txt
+-rw-r--r--   0        0        0       15 2021-06-07 02:28:43.791071 fissix-21.6.6/requirements.txt
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 fissix-21.6.6/setup.py
+-rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 fissix-21.6.6/PKG-INFO
```

### Comparing `fissix-21.11.13/.gitignore` & `fissix-21.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/CHANGELOG.md` & `fissix-21.6.6/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,10 @@
 fissix
 ======
 
-v21.11.13
----------
-
-Bug fix release:
-
-* Fix: except fixer checks against the value of a node (#42, #43)
-* Improved urllib fixer to include `__version__` (#44)
-* Tested against Python 3.9 (#32, #45)
-
-```
-$ git shortlog -s v21.6.6...v21.11.13
-     1	Chris Elion
-     3	David Grant
-     5	John Reese
-     2	Thomas Grainger
-```
-
-
 v21.6.6
 -------
 
 Feature release:
 
 - New fixer for `sorted()` and `list.sort()` (#25)
 - Token helpers for LBrace, RBrace, and Colon (#34)
@@ -31,15 +13,15 @@
 - Support for running tests outside of source tree (#31)
 - Documentation for fixers, general API, and usage (#23, #24, #29)
 
 ```
 $ git shortlog -s v20.8.0...v21.6.6
      1	Ashley Whetter
      1	David Grant
-    16	John Reese
+    14	John Reese
      1	Langston Barrett
      5	Larry Huang
      1	Nicholas D Steeves
      1	Stefano Rivera
      2	Thomas Grainger
 ```
```

### Comparing `fissix-21.11.13/LICENSE` & `fissix-21.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/README.md` & `fissix-21.6.6/README.md`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/docs/conf.py` & `fissix-21.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/docs/fixers.rst` & `fissix-21.6.6/docs/fixers.rst`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/Grammar.txt` & `fissix-21.6.6/fissix/Grammar.txt`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/PatternGrammar.txt` & `fissix-21.6.6/fissix/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/__init__.py` & `fissix-21.6.6/fissix/__init__.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/btm_matcher.py` & `fissix-21.6.6/fissix/btm_matcher.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/btm_utils.py` & `fissix-21.6.6/fissix/btm_utils.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixer_base.py` & `fissix-21.6.6/fissix/fixer_base.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixer_util.py` & `fissix-21.6.6/fissix/fixer_util.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_apply.py` & `fissix-21.6.6/fissix/fixes/fix_apply.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_asserts.py` & `fissix-21.6.6/fissix/fixes/fix_asserts.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_buffer.py` & `fissix-21.6.6/fissix/fixes/fix_buffer.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_dict.py` & `fissix-21.6.6/fissix/fixes/fix_dict.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_except.py` & `fissix-21.6.6/fissix/fixes/fix_except.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,18 +50,15 @@
         syms = self.syms
 
         tail = [n.clone() for n in results["tail"]]
 
         try_cleanup = [ch.clone() for ch in results["cleanup"]]
         changed = False
         for except_clause, e_suite in find_excepts(try_cleanup):
-            if (
-                len(except_clause.children) == 4
-                and except_clause.children[2].value != "as"
-            ):
+            if len(except_clause.children) == 4 and except_clause.children[2] != "as":
                 (E, comma, N) = except_clause.children[1:4]
                 comma.replace(Name("as", prefix=" "))
                 changed = True
 
                 if N.type != token.NAME:
                     # Generate a new N for the except clause
                     new_N = Name(self.new_name(), prefix=" ")
```

### Comparing `fissix-21.11.13/fissix/fixes/fix_exec.py` & `fissix-21.6.6/fissix/fixes/fix_exec.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_execfile.py` & `fissix-21.6.6/fissix/fixes/fix_execfile.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_exitfunc.py` & `fissix-21.6.6/fissix/fixes/fix_exitfunc.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_filter.py` & `fissix-21.6.6/fissix/fixes/fix_filter.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_funcattrs.py` & `fissix-21.6.6/fissix/fixes/fix_funcattrs.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_future.py` & `fissix-21.6.6/fissix/fixes/fix_future.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_has_key.py` & `fissix-21.6.6/fissix/fixes/fix_has_key.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_idioms.py` & `fissix-21.6.6/fissix/fixes/fix_idioms.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_import.py` & `fissix-21.6.6/fissix/fixes/fix_import.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_imports.py` & `fissix-21.6.6/fissix/fixes/fix_imports.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_input.py` & `fissix-21.6.6/fissix/fixes/fix_input.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_intern.py` & `fissix-21.6.6/fissix/fixes/fix_intern.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_isinstance.py` & `fissix-21.6.6/fissix/fixes/fix_isinstance.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_itertools.py` & `fissix-21.6.6/fissix/fixes/fix_itertools.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_itertools_imports.py` & `fissix-21.6.6/fissix/fixes/fix_itertools_imports.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_map.py` & `fissix-21.6.6/fissix/fixes/fix_map.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_metaclass.py` & `fissix-21.6.6/fissix/fixes/fix_metaclass.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_methodattrs.py` & `fissix-21.6.6/fissix/fixes/fix_methodattrs.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_ne.py` & `fissix-21.6.6/fissix/fixes/fix_ne.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_next.py` & `fissix-21.6.6/fissix/fixes/fix_next.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_nonzero.py` & `fissix-21.6.6/fissix/fixes/fix_nonzero.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_numliterals.py` & `fissix-21.6.6/fissix/fixes/fix_numliterals.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_operator.py` & `fissix-21.6.6/fissix/fixes/fix_operator.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_paren.py` & `fissix-21.6.6/fissix/fixes/fix_paren.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_print.py` & `fissix-21.6.6/fissix/fixes/fix_print.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_raise.py` & `fissix-21.6.6/fissix/fixes/fix_raise.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_reduce.py` & `fissix-21.6.6/fissix/fixes/fix_reduce.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_reload.py` & `fissix-21.6.6/fissix/fixes/fix_reload.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_renames.py` & `fissix-21.6.6/fissix/fixes/fix_renames.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_repr.py` & `fissix-21.6.6/fissix/fixes/fix_repr.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_set_literal.py` & `fissix-21.6.6/fissix/fixes/fix_set_literal.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_sorted.py` & `fissix-21.6.6/fissix/fixes/fix_sorted.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_sys_exc.py` & `fissix-21.6.6/fissix/fixes/fix_sys_exc.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_throw.py` & `fissix-21.6.6/fissix/fixes/fix_throw.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_tuple_params.py` & `fissix-21.6.6/fissix/fixes/fix_tuple_params.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_types.py` & `fissix-21.6.6/fissix/fixes/fix_types.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_unicode.py` & `fissix-21.6.6/fissix/fixes/fix_unicode.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_urllib.py` & `fissix-21.6.6/fissix/fixes/fix_urllib.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
                 "ProxyDigestAuthHandler",
                 "HTTPHandler",
                 "HTTPSHandler",
                 "FileHandler",
                 "FTPHandler",
                 "CacheFTPHandler",
                 "UnknownHandler",
-                "__version__",
             ],
         ),
         ("urllib.error", ["URLError", "HTTPError"]),
     ],
 }
 
 # Duplicate the url parsing functions for urllib2.
```

### Comparing `fissix-21.11.13/fissix/fixes/fix_ws_comma.py` & `fissix-21.6.6/fissix/fixes/fix_ws_comma.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_xrange.py` & `fissix-21.6.6/fissix/fixes/fix_xrange.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_xreadlines.py` & `fissix-21.6.6/fissix/fixes/fix_xreadlines.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/fixes/fix_zip.py` & `fissix-21.6.6/fissix/fixes/fix_zip.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/main.py` & `fissix-21.6.6/fissix/main.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/patcomp.py` & `fissix-21.6.6/fissix/patcomp.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/conv.py` & `fissix-21.6.6/fissix/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/driver.py` & `fissix-21.6.6/fissix/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/grammar.py` & `fissix-21.6.6/fissix/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/literals.py` & `fissix-21.6.6/fissix/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/parse.py` & `fissix-21.6.6/fissix/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/pgen.py` & `fissix-21.6.6/fissix/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/token.py` & `fissix-21.6.6/fissix/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pgen2/tokenize.py` & `fissix-21.6.6/fissix/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pygram.py` & `fissix-21.6.6/fissix/pygram.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/pytree.py` & `fissix-21.6.6/fissix/pytree.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/refactor.py` & `fissix-21.6.6/fissix/refactor.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/data/infinite_recursion.py` & `fissix-21.6.6/fissix/tests/data/infinite_recursion.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/data/py2_test_grammar.py` & `fissix-21.6.6/fissix/tests/data/py2_test_grammar.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/data/py3_test_grammar.py` & `fissix-21.6.6/fissix/tests/data/py3_test_grammar.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/pytree_idempotency.py` & `fissix-21.6.6/fissix/tests/pytree_idempotency.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/support.py` & `fissix-21.6.6/fissix/tests/support.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_all_fixers.py` & `fissix-21.6.6/fissix/tests/test_all_fixers.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_fixers.py` & `fissix-21.6.6/fissix/tests/test_fixers.py`

 * *Files 0% similar despite different names*

```diff
@@ -904,22 +904,14 @@
         s = """
             try:
                 pass
             except (Exception, SystemExit):
                 pass"""
         self.unchanged(s)
 
-    def test_unchanged_4(self):
-        s = """
-            try:
-                pass
-            except Exception as e:
-                pass"""
-        self.unchanged(s)
-
 
 class Test_raise(FixerTestCase):
     fixer = "raise"
 
     def test_basic(self):
         b = """raise Exception, 5"""
         a = """raise Exception(5)"""
```

### Comparing `fissix-21.11.13/fissix/tests/test_main.py` & `fissix-21.6.6/fissix/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_parser.py` & `fissix-21.6.6/fissix/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_pytree.py` & `fissix-21.6.6/fissix/tests/test_pytree.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_refactor.py` & `fissix-21.6.6/fissix/tests/test_refactor.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/fissix/tests/test_util.py` & `fissix-21.6.6/fissix/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/makefile` & `fissix-21.6.6/makefile`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/pyproject.toml` & `fissix-21.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fissix-21.11.13/setup.py` & `fissix-21.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 package_data = \
 {'': ['*'], 'fissix.tests': ['data/*', 'data/fixers/*']}
 
 install_requires = \
 ['appdirs']
 
 setup(name='fissix',
-      version='21.11.13',
+      version='21.6.6',
       description='Monkeypatches to override default behavior of lib2to3.',
       author='John Reese',
       author_email='john@noswap.com',
       url='https://github.com/jreese/fissix',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

