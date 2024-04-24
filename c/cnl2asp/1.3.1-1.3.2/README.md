# Comparing `tmp/cnl2asp-1.3.1.tar.gz` & `tmp/cnl2asp-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2asp-1.3.1.tar", last modified: Thu Apr 11 12:26:09 2024, max compression
+gzip compressed data, was "cnl2asp-1.3.2.tar", last modified: Wed Apr 24 14:48:04 2024, max compression
```

## Comparing `cnl2asp-1.3.1.tar` & `cnl2asp-1.3.2.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.678627 cnl2asp-1.3.1/
--rw-rw-r--   0 simone    (1000) simone    (1000)    11357 2024-04-10 06:53:15.000000 cnl2asp-1.3.1/LICENSE
--rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)    10643 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/README.md
--rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-04-11 12:26:09.678627 cnl2asp-1.3.1/setup.cfg
--rw-rw-r--   0 simone    (1000) simone    (1000)     1039 2024-04-10 13:27:01.000000 cnl2asp-1.3.1/setup.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.666628 cnl2asp-1.3.1/src/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.666628 cnl2asp-1.3.1/src/cnl2asp/
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.670628 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1517 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_aggregate.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4505 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_atom.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1837 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_attribute.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     1594 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_conjunction.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      471 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_element.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1053 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_encoding.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     6394 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_operation.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)      510 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_program.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4703 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_rule.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      414 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_temporal_formula.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.670628 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     8020 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      561 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1638 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      609 2024-04-10 11:30:37.000000 cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     6992 2024-04-10 14:25:04.000000 cnl2asp-1.3.1/src/cnl2asp/cnl2asp.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/converter/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/converter/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    25041 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/asp_converter.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     7333 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/cnl2json_converter.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     4916 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/converter/converter_interface.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/exception/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/exception/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     2369 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/exception/cnl2asp_exceptions.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    16830 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/grammar.lark
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/parser/
--rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/parser/__init__.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     3199 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/command.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)    45312 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/parser.py
--rwxrwxr-x   0 simone    (1000) simone    (1000)     7027 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/parser/proposition_builder.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/specification/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1103 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/aggregate_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     4080 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/attribute_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      741 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      540 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/constant_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    13928 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/entity_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1667 2024-04-10 11:16:53.000000 cnl2asp-1.3.1/src/cnl2asp/specification/name_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3215 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/operation_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1122 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/problem.py
--rw-rw-r--   0 simone    (1000) simone    (1000)    11502 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/proposition.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1081 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/relation_component.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     3963 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/signaturemanager.py
--rw-rw-r--   0 simone    (1000) simone    (1000)     1288 2024-04-10 11:15:14.000000 cnl2asp-1.3.1/src/cnl2asp/specification/specification.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp/utility/
--rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/utility/__init__.py
--rw-rw-r--   0 simone    (1000) simone    (1000)      933 2024-04-10 06:54:38.000000 cnl2asp-1.3.1/src/cnl2asp/utility/utility.py
-drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-11 12:26:09.674627 cnl2asp-1.3.1/src/cnl2asp.egg-info/
--rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/PKG-INFO
--rw-rw-r--   0 simone    (1000) simone    (1000)     1993 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/SOURCES.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/dependency_links.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)       30 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/requires.txt
--rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-04-11 12:26:09.000000 cnl2asp-1.3.1/src/cnl2asp.egg-info/top_level.txt
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11357 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/LICENSE
+-rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)      922 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/README.md
+-rw-rw-r--   0 simone    (1000) simone    (1000)       38 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/setup.cfg
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1128 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/setup.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.073338 cnl2asp-1.3.2/src/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.073338 cnl2asp-1.3.2/src/cnl2asp/
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1517 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_aggregate.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4505 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_atom.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1837 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_attribute.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     1594 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_conjunction.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      471 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_element.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1060 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_encoding.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     6394 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_operation.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)      510 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_program.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4703 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_rule.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      414 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_temporal_formula.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     8020 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      561 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1638 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      609 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    10236 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/cnl2asp.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/converter/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    25041 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/asp_converter.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     7333 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/cnl2json_converter.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     4916 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/converter/converter_interface.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/exception/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/exception/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2369 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/exception/cnl2asp_exceptions.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    16830 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/grammar.lark
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/parser/
+-rwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/__init__.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     3199 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/command.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)    45312 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/parser.py
+-rwxrwxr-x   0 simone    (1000) simone    (1000)     7027 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/parser/proposition_builder.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/specification/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1103 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/aggregate_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     4080 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/attribute_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      741 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      540 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/constant_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    13928 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/entity_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1667 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/name_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3215 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/operation_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1122 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/problem.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)    11502 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/proposition.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1081 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/relation_component.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     3963 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/signaturemanager.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)     1288 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/specification/specification.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp/utility/
+-rw-rw-r--   0 simone    (1000) simone    (1000)        0 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/utility/__init__.py
+-rw-rw-r--   0 simone    (1000) simone    (1000)      933 2024-04-24 14:34:47.000000 cnl2asp-1.3.2/src/cnl2asp/utility/utility.py
+drwxrwxr-x   0 simone    (1000) simone    (1000)        0 2024-04-24 14:48:04.077338 cnl2asp-1.3.2/src/cnl2asp.egg-info/
+-rw-r--r--   0 simone    (1000) simone    (1000)      654 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/PKG-INFO
+-rw-rw-r--   0 simone    (1000) simone    (1000)     2031 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/SOURCES.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        1 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/dependency_links.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       49 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/entry_points.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)       30 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/requires.txt
+-rw-rw-r--   0 simone    (1000) simone    (1000)        8 2024-04-24 14:48:04.000000 cnl2asp-1.3.2/src/cnl2asp.egg-info/top_level.txt
```

### Comparing `cnl2asp-1.3.1/LICENSE` & `cnl2asp-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/PKG-INFO` & `cnl2asp-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.1
+Version: 1.3.2
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.1/setup.py` & `cnl2asp-1.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from textwrap import dedent
 
 from setuptools import setup, find_packages
 
 setup(
     name='cnl2asp',
-    version='1.3.1',
+    version='1.3.2',
     description='A tool for converting a Controlled Natural Language based on English into Answer Set Programming',
     long_description=dedent('''\
                             A tool for converting a Controlled Natural Language based on English into Answer Set Programming
                             
                             Documentation is available at:
                             https://dodaro.github.io/cnl2asp/
                             '''),
@@ -18,9 +18,12 @@
     author_email='carmine.dodaro@unical.it',
     maintainer='Simone Caruso',
     maintainer_email='simone.caruso@edu.unige.it',
     package_dir={'': 'src'},
     packages=find_packages('src', exclude=['tests*']),
     package_data={'': ['grammar.lark']},
     install_requires=['lark', 'inflect', 'multipledispatch'],
+    entry_points={
+        'console_scripts': ['cnl2asp = cnl2asp.cnl2asp:main'],
+    },
     python_requires=">=3.10"
 )
```

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_aggregate.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_aggregate.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_atom.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_atom.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_attribute.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_attribute.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_conjunction.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_conjunction.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_encoding.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_encoding.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     def __str__(self):
         string = ''
         for constant in self._constants:
             if constant[1]:
                 string += f'#const {constant[0]} = {constant[1]}.\n'
         for program in self._programs:
             string += str(program)
-        return string.strip()
+        return string.strip() + '\n'
```

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_operation.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_operation.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/asp_rule.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/asp_rule.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/clingo_wrapper.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_result_parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py` & `cnl2asp-1.3.2/src/cnl2asp/ASP_elements/solver/telingo_wrapper.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/cnl2asp.py` & `cnl2asp-1.3.2/src/cnl2asp/cnl2asp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
+import argparse
+import json
 import os
+import sys
 import tempfile
 import traceback
 from enum import Enum
 from textwrap import indent
 from typing import TextIO
 
 from cnl2asp.utility.utility import Utility
@@ -115,21 +118,21 @@
             print("Error in asp conversion:", str(e))
             if self._debug:
                 traceback.print_exception(e)
             return ''
 
     def optimize(self, asp_encoding: str):
         from clingo.ast import parse_files
-        from ngo import optimize, Predicate
+        from ngo import optimize, auto_detect_input, auto_detect_output
         prg = []
         with tempfile.NamedTemporaryFile(mode="w") as file:
             file.write(asp_encoding)
             file.seek(0)
             parse_files([file.name], prg.append)
-            prg = optimize(prg, [Predicate("node",1)], [Predicate("assigned_to",2)])
+            prg = optimize(prg, auto_detect_input(prg), auto_detect_output(prg))
             optimized_encoding = ''
             for stm in prg:
                 optimized_encoding += str(stm) + '\n'
         return optimized_encoding
 
     def __get_type(self, name: str):
         if SignatureManager.is_temporal_entity(name):
@@ -165,7 +168,73 @@
     def get_symbols(self) -> list[Symbol]:
         self.compile()
         signatures: list[Symbol] = []
         for signature in SignatureManager().signatures:
             signatures.append(self.__convert_signature(signature))
         SignatureManager().signatures = []
         return signatures
+
+
+def main():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-c', '--check-syntax', action='store_true', help='Checks that the input fits the grammar')
+    parser.add_argument('--cnl2json', action='store_true', help=argparse.SUPPRESS)
+    parser.add_argument('--symbols', action='store_true', help='Return the list of symbols generated for the compilation')
+    parser.add_argument('-p', '--print-with-functions', action='store_true',
+                        help='Print atoms with functions. ')
+    parser.add_argument('--debug', action='store_true', help=argparse.SUPPRESS)
+    parser.add_argument('--solve', type=str, choices=["clingo", "telingo"], help='Call the corresponding solver and print a cnl-translated output')
+    parser.add_argument('-o', '--optimize', action='store_true', help='Optimize the output using ngo')
+    parser.add_argument('input_file')
+    parser.add_argument('output_file', type=str, nargs='?', default='')
+    args = parser.parse_args()
+
+    Utility.PRINT_WITH_FUNCTIONS = args.print_with_functions
+
+    input_file = args.input_file
+
+    in_file = open(input_file, 'r')
+    cnl2asp = Cnl2asp(in_file, args.debug)
+
+    if args.check_syntax:
+        if cnl2asp.check_syntax():
+            print("Input file fits the grammar.")
+    elif args.cnl2json:
+        print(json.dumps(cnl2asp.cnl_to_json()))
+    elif args.symbols:
+        print(cnl2asp.get_symbols())
+    else:
+        asp_encoding = cnl2asp.compile()
+        if args.optimize:
+            asp_encoding = cnl2asp.optimize(asp_encoding)
+        try:
+            out = sys.stdout
+            if args.output_file:
+                if str(asp_encoding):
+                    print("Compilation completed.")
+                out = open(args.output_file, "w")
+            out.write(asp_encoding)
+            if args.solve:
+                if args.solve == "clingo":
+                    from cnl2asp.ASP_elements.solver.clingo_wrapper import Clingo
+                    from cnl2asp.ASP_elements.solver.clingo_result_parser import ClingoResultParser
+                    solver = Clingo()
+                    print("\n*********")
+                    print(f"Running {args.solve}...\n")
+                    solver.load(str(asp_encoding))
+                    res = solver.solve()
+                    clingo_res = ClingoResultParser(cnl2asp.parse_input(), res)
+                    model = clingo_res.parse_model()
+                    print("SOLUTION:\n" + model)
+                elif args.solve == "telingo":
+                    from cnl2asp.ASP_elements.solver.telingo_result_parser import TelingoResultParser
+                    from cnl2asp.ASP_elements.solver.telingo_wrapper import Telingo
+                    solver = Telingo()
+                    print("\n*********")
+                    print(f"Running {args.solve}...\n")
+                    solver.load(str(asp_encoding))
+                    res = solver.solve()
+                    telingo_res = TelingoResultParser(cnl2asp.parse_input(), res)
+                    model = telingo_res.parse_model()
+                    print("SOLUTION:\n" + model)
+        except Exception as e:
+            print("Error in writing output", str(e))
```

### Comparing `cnl2asp-1.3.1/src/cnl2asp/converter/asp_converter.py` & `cnl2asp-1.3.2/src/cnl2asp/converter/asp_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/converter/cnl2json_converter.py` & `cnl2asp-1.3.2/src/cnl2asp/converter/cnl2json_converter.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/converter/converter_interface.py` & `cnl2asp-1.3.2/src/cnl2asp/converter/converter_interface.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/exception/cnl2asp_exceptions.py` & `cnl2asp-1.3.2/src/cnl2asp/exception/cnl2asp_exceptions.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/grammar.lark` & `cnl2asp-1.3.2/src/cnl2asp/grammar.lark`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/parser/command.py` & `cnl2asp-1.3.2/src/cnl2asp/parser/command.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/parser/parser.py` & `cnl2asp-1.3.2/src/cnl2asp/parser/parser.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/parser/proposition_builder.py` & `cnl2asp-1.3.2/src/cnl2asp/parser/proposition_builder.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/aggregate_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/aggregate_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/attribute_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/attribute_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/constant_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/constant_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/entity_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/entity_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/name_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/name_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/operation_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/operation_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/problem.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/problem.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/proposition.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/proposition.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/relation_component.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/relation_component.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/signaturemanager.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/signaturemanager.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/specification/specification.py` & `cnl2asp-1.3.2/src/cnl2asp/specification/specification.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp/utility/utility.py` & `cnl2asp-1.3.2/src/cnl2asp/utility/utility.py`

 * *Files identical despite different names*

### Comparing `cnl2asp-1.3.1/src/cnl2asp.egg-info/PKG-INFO` & `cnl2asp-1.3.2/src/cnl2asp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnl2asp
-Version: 1.3.1
+Version: 1.3.2
 Summary: A tool for converting a Controlled Natural Language based on English into Answer Set Programming
 Home-page: https://github.com/dodaro/cnl2asp/tree/main
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 Maintainer: Simone Caruso
 Maintainer-email: simone.caruso@edu.unige.it
 License: Apache License
```

### Comparing `cnl2asp-1.3.1/src/cnl2asp.egg-info/SOURCES.txt` & `cnl2asp-1.3.2/src/cnl2asp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 src/cnl2asp/__init__.py
 src/cnl2asp/cnl2asp.py
 src/cnl2asp/grammar.lark
 src/cnl2asp.egg-info/PKG-INFO
 src/cnl2asp.egg-info/SOURCES.txt
 src/cnl2asp.egg-info/dependency_links.txt
+src/cnl2asp.egg-info/entry_points.txt
 src/cnl2asp.egg-info/requires.txt
 src/cnl2asp.egg-info/top_level.txt
 src/cnl2asp/ASP_elements/__init__.py
 src/cnl2asp/ASP_elements/asp_aggregate.py
 src/cnl2asp/ASP_elements/asp_atom.py
 src/cnl2asp/ASP_elements/asp_attribute.py
 src/cnl2asp/ASP_elements/asp_conjunction.py
```

