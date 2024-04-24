# Comparing `tmp/odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1.tar.gz` & `tmp/odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1.tar", last modified: Mon Feb 19 15:51:18 2024, max compression
+gzip compressed data, was "dist/odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0.tar", last modified: Wed Apr 24 07:21:25 2024, max compression
```

## Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1.tar` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/
--rw-r--r--   0 root         (0) root         (0)     3095 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3095 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1297 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 15:51:17.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2039 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     2292 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.xml
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/__manifest__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2473 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/tests/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/tests/test_res_partner_ticket_massive_creation_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     5075 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/i18n/ca_ES.po
--rw-rw-rw-   0 root         (0) root         (0)     5074 2024-02-19 15:50:47.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/i18n/es.po
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-19 15:51:18.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1337 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.xml
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/__manifest__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/CHANGELOG.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/tests/test_helpdesk_ticket_massive_creation_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     5184 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/i18n/ca_ES.po
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2024-04-24 07:20:42.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/i18n/es.po
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 07:21:25.000000 odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/setup.cfg
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/PKG-INFO` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-helpdesk_ticket_massive_creation
-Version: 12.0.0.2.0.99.dev1
+Version: 12.0.0.3.0
 Summary: Create helpdesk tickets massively, from multiple preselected partners.
 Home-page: https://gitlab.com/somitcoop/erp-research/odoo-helpdesk
 Author: Som It Cooperatiu SCCL, Som Connexió SCCL, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -30,32 +30,32 @@
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 
 |badge1| |badge2|
 
-Create helpdesk tickets massively, from multiple preselected partners
+Create helpdesk tickets massively, from multiple preselected partners or contracts
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Configuration
 =============
 
 No configuration needed for this module.
 
 Usage
 =====
 
-To create tickets (with same content) for multiple partners:
+To create tickets (with same content) for multiple partners / contracts:
 
-- Contacts (tree view) + select partners > Actions > Create tickets massively
+- Contacts (tree view) / Contracts (tree view) + selection > Actions > Create tickets massively
 - Fill ticket information > Create.
 
 
 Known issues / Roadmap
 ======================
 
 There are no issues for the moment.
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/PKG-INFO` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-helpdesk-ticket-massive-creation
-Version: 12.0.0.2.0.99.dev1
+Version: 12.0.0.3.0
 Summary: Create helpdesk tickets massively, from multiple preselected partners.
 Home-page: https://gitlab.com/somitcoop/erp-research/odoo-helpdesk
 Author: Som It Cooperatiu SCCL, Som Connexió SCCL, Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -30,32 +30,32 @@
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 
 |badge1| |badge2|
 
-Create helpdesk tickets massively, from multiple preselected partners
+Create helpdesk tickets massively, from multiple preselected partners or contracts
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Configuration
 =============
 
 No configuration needed for this module.
 
 Usage
 =====
 
-To create tickets (with same content) for multiple partners:
+To create tickets (with same content) for multiple partners / contracts:
 
-- Contacts (tree view) + select partners > Actions > Create tickets massively
+- Contacts (tree view) / Contracts (tree view) + selection > Actions > Create tickets massively
 - Fill ticket information > Create.
 
 
 Known issues / Roadmap
 ======================
 
 There are no issues for the moment.
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/SOURCES.txt` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo12_addon_helpdesk_ticket_massive_creation.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 setup.py
+odoo/addons/helpdesk_ticket_massive_creation/CHANGELOG.md
 odoo/addons/helpdesk_ticket_massive_creation/README.rst
 odoo/addons/helpdesk_ticket_massive_creation/__init__.py
 odoo/addons/helpdesk_ticket_massive_creation/__manifest__.py
 odoo/addons/helpdesk_ticket_massive_creation/i18n/ca_ES.po
 odoo/addons/helpdesk_ticket_massive_creation/i18n/es.po
 odoo/addons/helpdesk_ticket_massive_creation/tests/__init__.py
-odoo/addons/helpdesk_ticket_massive_creation/tests/test_res_partner_ticket_massive_creation_wizard.py
+odoo/addons/helpdesk_ticket_massive_creation/tests/test_helpdesk_ticket_massive_creation_wizard.py
 odoo/addons/helpdesk_ticket_massive_creation/wizards/__init__.py
-odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/__init__.py
-odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.py
-odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.xml
+odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/__init__.py
+odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.py
+odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.xml
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/PKG-INFO
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/SOURCES.txt
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/dependency_links.txt
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/not-zip-safe
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/requires.txt
 odoo12_addon_helpdesk_ticket_massive_creation.egg-info/top_level.txt
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.xml` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.xml`

 * *Files 18% similar despite different names*

#### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.xml` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.xml`

```diff
@@ -1,12 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
-    <record id="view_form_res_partner_ticket_massive_creation_wizard" model="ir.ui.view">
-      <field name="name">Massive ticket creation from res_partner wizard</field>
+    <record id="view_form_helpdesk_ticket_massive_creation_wizard" model="ir.ui.view">
+      <field name="name">Massive ticket creation from wizard</field>
       <field name="model">helpdesk.ticket.massive.creation.wizard</field>
       <field name="arch" type="xml">
         <form string="Helpdesk Ticket">
           <sheet>
             <div class="oe_structure">
               <div class="oe_title">
                 <h3 class="o_row">
@@ -38,9 +38,10 @@
             <button type="object" name="button_create" string="Create" confirm="Are you sure you want to create these tickets?"/>
             <button special="cancel" string="Cancel" class="btn-secondary"/>
           </footer>
         </form>
       </field>
     </record>
     <act_window id="action_res_partner_create_helpdesk_ticket_massively" name="Create tickets massively" src_model="res.partner" res_model="helpdesk.ticket.massive.creation.wizard" view_type="form" view_mode="form" target="new" multi="True"/>
+    <act_window id="action_contract_contract_create_helpdesk_ticket_massively" name="Create tickets massively" src_model="contract.contract" res_model="helpdesk.ticket.massive.creation.wizard" view_type="form" view_mode="form" target="new" multi="True"/>
   </data>
 </odoo>
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/__manifest__.py` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/__manifest__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Copyright 2023-SomItCoop SCCL(<https://gitlab.com/somitcoop>)
 # License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl.html).
 {
-    "version": "12.0.0.2.0",
+    "version": "12.0.0.3.0",
     "name": "Massive ticket creation from selected partners",
     "depends": [
         "helpdesk_mgmt",
         "contacts",
+        "helpdesk_ticket_contract_contract",
     ],
     "author": """
         Som It Cooperatiu SCCL,
         Som Connexió SCCL,
         Odoo Community Association (OCA)
     """,
     "category": "Auth",
     "website": "https://gitlab.com/somitcoop/erp-research/odoo-helpdesk",
     "license": "AGPL-3",
     "summary": """
         Create helpdesk tickets massively, from multiple preselected partners.
     """,
     "data": [
-        "wizards/res_partner_ticket_massive_creation/res_partner_ticket_massive_creation.xml"  # noqa
+        "wizards/helpdesk_ticket_massive_creation/helpdesk_ticket_massive_creation.xml"  # noqa
     ],
     "demo": [],
     "application": True,
     "installable": True,
 }
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/README.rst` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,32 +15,32 @@
     :alt: Beta
 .. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 
 |badge1| |badge2|
 
-Create helpdesk tickets massively, from multiple preselected partners
+Create helpdesk tickets massively, from multiple preselected partners or contracts
 
 **Table of contents**
 
 .. contents::
    :local:
 
 Configuration
 =============
 
 No configuration needed for this module.
 
 Usage
 =====
 
-To create tickets (with same content) for multiple partners:
+To create tickets (with same content) for multiple partners / contracts:
 
-- Contacts (tree view) + select partners > Actions > Create tickets massively
+- Contacts (tree view) / Contracts (tree view) + selection > Actions > Create tickets massively
 - Fill ticket information > Create.
 
 
 Known issues / Roadmap
 ======================
 
 There are no issues for the moment.
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/i18n/ca_ES.po` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/i18n/ca_ES.po`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Are you sure you want to create these tickets?"
 msgstr "Estàs segura de crear aquests tiquets?"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__user_id
 msgid "Assigned user"
 msgstr "Agent assignada"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Cancel"
 msgstr "Cancel·lar"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__category_id
 msgid "Category"
 msgstr "Categoria"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Create"
 msgstr "Crear"
 
 #. module: helpdesk_ticket_massive_creation
+#: model:ir.actions.act_window,name:helpdesk_ticket_massive_creation.action_contract_contract_create_helpdesk_ticket_massively
 #: model:ir.actions.act_window,name:helpdesk_ticket_massive_creation.action_res_partner_create_helpdesk_ticket_massively
 msgid "Create tickets massively"
 msgstr "Crear tiquets massivament"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__create_uid
 msgid "Created by"
@@ -53,20 +54,20 @@
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__create_date
 msgid "Created on"
 msgstr "Creat el"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__description
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Description"
 msgstr "Descripció"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Helpdesk Ticket"
 msgstr "Tiquet"
 
 #. module: helpdesk_ticket_massive_creation
 #: selection:helpdesk.ticket.massive.creation.wizard,priority:0
 msgid "High"
 msgstr "Alta"
@@ -88,15 +89,15 @@
 
 #. module: helpdesk_ticket_massive_creation
 #: selection:helpdesk.ticket.massive.creation.wizard,priority:0
 msgid "Medium"
 msgstr "Mitjana"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "New subject..."
 msgstr "Nou assumpte..."
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__priority
 msgid "Priority"
 msgstr "Prioritat"
```

### Comparing `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.2.0.99.dev1/odoo/addons/helpdesk_ticket_massive_creation/i18n/es.po` & `odoo12-addon-helpdesk_ticket_massive_creation-12.0.0.3.0/odoo/addons/helpdesk_ticket_massive_creation/i18n/es.po`

 * *Files 6% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Are you sure you want to create these tickets?"
 msgstr "Estás segura de crear estos tíquets?"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__user_id
 msgid "Assigned user"
 msgstr "Agente asignada"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Cancel"
 msgstr "Cancelar"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__category_id
 msgid "Category"
 msgstr "Categoría"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Create"
 msgstr "Crear"
 
 #. module: helpdesk_ticket_massive_creation
+#: model:ir.actions.act_window,name:helpdesk_ticket_massive_creation.action_contract_contract_create_helpdesk_ticket_massively
 #: model:ir.actions.act_window,name:helpdesk_ticket_massive_creation.action_res_partner_create_helpdesk_ticket_massively
 msgid "Create tickets massively"
 msgstr "Crear tíquets masivamente"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__create_uid
 msgid "Created by"
@@ -53,20 +54,20 @@
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__create_date
 msgid "Created on"
 msgstr "Creado el"
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__description
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Description"
 msgstr "Descripción"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "Helpdesk Ticket"
 msgstr "Tíquet"
 
 #. module: helpdesk_ticket_massive_creation
 #: selection:helpdesk.ticket.massive.creation.wizard,priority:0
 msgid "High"
 msgstr "Alta"
@@ -88,15 +89,15 @@
 
 #. module: helpdesk_ticket_massive_creation
 #: selection:helpdesk.ticket.massive.creation.wizard,priority:0
 msgid "Medium"
 msgstr "Media"
 
 #. module: helpdesk_ticket_massive_creation
-#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_res_partner_ticket_massive_creation_wizard
+#: model_terms:ir.ui.view,arch_db:helpdesk_ticket_massive_creation.view_form_helpdesk_ticket_massive_creation_wizard
 msgid "New subject..."
 msgstr "Nuevo asunto..."
 
 #. module: helpdesk_ticket_massive_creation
 #: model:ir.model.fields,field_description:helpdesk_ticket_massive_creation.field_helpdesk_ticket_massive_creation_wizard__priority
 msgid "Priority"
 msgstr "Prioridad"
```

