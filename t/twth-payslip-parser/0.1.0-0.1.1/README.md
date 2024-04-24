# Comparing `tmp/twth_payslip_parser-0.1.0.tar.gz` & `tmp/twth_payslip_parser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twth_payslip_parser-0.1.0.tar", max compression
+gzip compressed data, was "twth_payslip_parser-0.1.1.tar", max compression
```

## Comparing `twth_payslip_parser-0.1.0.tar` & `twth_payslip_parser-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       78 2024-04-24 16:13:27.628067 twth_payslip_parser-0.1.0/README.md
--rw-r--r--   0        0        0      429 2024-04-24 16:13:57.737099 twth_payslip_parser-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      359 2024-04-24 16:31:57.158148 twth_payslip_parser-0.1.0/twth_payslip_parser/__init__.py
--rw-r--r--   0        0        0      496 2024-04-24 16:09:53.208716 twth_payslip_parser-0.1.0/twth_payslip_parser/decrypter.py
--rw-r--r--   0        0        0     1624 2024-04-24 16:29:15.436589 twth_payslip_parser-0.1.0/twth_payslip_parser/parser.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 twth_payslip_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-04-24 16:13:27.628067 twth_payslip_parser-0.1.1/README.md
+-rw-r--r--   0        0        0      429 2024-04-24 17:55:39.067414 twth_payslip_parser-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      343 2024-04-24 17:52:13.068283 twth_payslip_parser-0.1.1/twth_payslip_parser/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-24 16:09:53.208716 twth_payslip_parser-0.1.1/twth_payslip_parser/decrypter.py
+-rw-r--r--   0        0        0     1624 2024-04-24 16:29:15.436589 twth_payslip_parser-0.1.1/twth_payslip_parser/parser.py
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 twth_payslip_parser-0.1.1/PKG-INFO
```

### Comparing `twth_payslip_parser-0.1.0/twth_payslip_parser/parser.py` & `twth_payslip_parser-0.1.1/twth_payslip_parser/parser.py`

 * *Files identical despite different names*

