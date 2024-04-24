# Comparing `tmp/localcosmos_app_kit-0.2.2.tar.gz` & `tmp/localcosmos_app_kit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_app_kit-0.2.2.tar", last modified: Fri Apr 19 07:18:40 2024, max compression
+gzip compressed data, was "localcosmos_app_kit-0.2.3.tar", last modified: Tue Apr 23 06:44:28 2024, max compression
```

## Comparing `localcosmos_app_kit-0.2.2.tar` & `localcosmos_app_kit-0.2.3.tar`

### file list

```diff
@@ -1,1783 +1,1783 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/
--rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit-0.2.2/LICENCE
--rw-r--r--   0 tom       (1000) tom       (1000)     1156 2024-04-10 13:05:33.000000 localcosmos_app_kit-0.2.2/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     1170 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.759316 localcosmos_app_kit-0.2.2/app_kit/
--rw-r--r--   0 tom       (1000) tom       (1000)       19 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      209 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/admin_urls.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.762649 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/
--rw-r--r--   0 tom       (1000) tom       (1000)       64 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/apps.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.762649 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     2370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)      255 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/permissions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3331 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.762649 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     1070 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6796 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3814 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/app_kit_api/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.765983 localcosmos_app_kit-0.2.2/app_kit/appbuilder/
--rw-r--r--   0 tom       (1000) tom       (1000)    28628 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppBuilderBase.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppPreviewBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)   110094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppReleaseBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/ContentImageBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/GBIFlib.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.769316 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/
--rw-r--r--   0 tom       (1000) tom       (1000)     9175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/BackboneTaxonomyJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3327 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/ButtonMatrixJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2735 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/FrontendJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6759 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/GenericFormJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/GlossaryJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6447 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/JSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2755 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/MapJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    25338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/NatureGuideJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    29123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/TaxonProfilesJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/TemplateContentJSONBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      152 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/precompile_fulltree.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.769316 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_ContentImageBuilder.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2378 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_builder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14881 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_builder_base.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_preview_builder.py
--rw-r--r--   0 tom       (1000) tom       (1000)    28055 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_release_builder.py
--rw-r--r--   0 tom       (1000) tom       (1000)       88 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      471 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/context_processors.py
--rw-r--r--   0 tom       (1000) tom       (1000)       82 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/definitions.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.769316 localcosmos_app_kit-0.2.2/app_kit/features/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.769316 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      124 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1812 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.769316 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     2327 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)     1177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/add_taxon_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1529 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbone_taxa_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbonetaxonomy.html
--rw-r--r--   0 tom       (1000) tom       (1000)      622 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_fulltree_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1206 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/remove_backbone_taxon.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2296 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/taxonlist.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)     1401 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)      778 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget_search_only.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     1743 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6504 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1028 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    11368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      153 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/ajax/generic_form_exposed_field_options.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1315 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/buttonmatrix_button.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1084 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/delete_buttonmatrix_element.html
--rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_button.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_buttonmatrix.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.772649 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1351 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templatetags/buttonmatrix_tags.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8015 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.775982 localcosmos_app_kit-0.2.2/app_kit/features/frontend/
--rw-r--r--   0 tom       (1000) tom       (1000)     7586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/PrivateFrontendImporter.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6636 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.775982 localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     2235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/0002_frontend_configuration.py
--rw-r--r--   0 tom       (1000) tom       (1000)      389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/0003_alter_frontendtext_unique_together.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.775982 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.775982 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      829 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/change_frontend.html
--rw-r--r--   0 tom       (1000) tom       (1000)      646 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/install_private_frontend.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/manage_frontend_settings.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1270 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/upload_private_frontend.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1587 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/manage_frontend.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.775982 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     1272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_PrivateFrontendImporter.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1702 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/frontend/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13794 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     5264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    13963 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/generic_forms/
--rw-r--r--   0 tom       (1000) tom       (1000)     9793 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/generic_forms/datePicker.js
--rw-r--r--   0 tom       (1000) tom       (1000)      314 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/generic_forms/genericforms.css
--rw-r--r--   0 tom       (1000) tom       (1000)      160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/generic_forms/genericforms.css~
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      923 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1562 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_value.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3847 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3462 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field_choices.html
--rw-r--r--   0 tom       (1000) tom       (1000)      546 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/generic_field.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1658 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/generic_field_modify.html
--rw-r--r--   0 tom       (1000) tom       (1000)     9240 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/manage_generic_form.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.779316 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templatetags/genericforms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.782649 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    15840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16038 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8369 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_templatetags_old.py
--rw-r--r--   0 tom       (1000) tom       (1000)    40955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1754 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/widgets.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.782649 localcosmos_app_kit-0.2.2/app_kit/features/glossary/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1410 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.782649 localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     2295 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/0002_auto_20201207_1328.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2746 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.782649 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.782649 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     1135 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry.html
--rw-r--r--   0 tom       (1000) tom       (1000)      848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/delete_glossary_entry.html
--rw-r--r--   0 tom       (1000) tom       (1000)      754 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/glossary_entries.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/glossary_entry.html
--rw-r--r--   0 tom       (1000) tom       (1000)      892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/manage_glossary_entry.html
--rw-r--r--   0 tom       (1000) tom       (1000)      566 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/manage_glossary.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)      692 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10825 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      951 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6668 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8509 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/glossary/zip_import.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/maps/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2692 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     1968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/0002_maptaxonomicfilter_filtertaxon.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2142 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      333 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/delete_filter_taxon.html
--rw-r--r--   0 tom       (1000) tom       (1000)     7840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/manage_project_area.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/manage_taxonomic_filter.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2665 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/taxonomic_filters.html
--rw-r--r--   0 tom       (1000) tom       (1000)     7838 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/manage_maps.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.785982 localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     1227 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4821 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9019 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/maps/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.792649 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/fields.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14879 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7259 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filter_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filter_space_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    51676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filters.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.792649 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)    11025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      913 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0002_auto_20201013_0901.py
--rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0003_matrixfilterrestriction.py
--rw-r--r--   0 tom       (1000) tom       (1000)      349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0004_auto_20210616_1315.py
--rw-r--r--   0 tom       (1000) tom       (1000)      391 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0005_metanode_settings.py
--rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0006_auto_20220503_0747.py
--rw-r--r--   0 tom       (1000) tom       (1000)      573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0007_auto_20221110_0613.py
--rw-r--r--   0 tom       (1000) tom       (1000)      393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0008_meta_node_description.py
--rw-r--r--   0 tom       (1000) tom       (1000)      411 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0009_meta_node_morphotype.py
--rw-r--r--   0 tom       (1000) tom       (1000)      403 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0010_matrix_filter_additional_data.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    52381 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.792649 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.795982 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     4066 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes.html
--rw-r--r--   0 tom       (1000) tom       (1000)      532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes_page.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_keynodes_menu.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/copy_tree_branch.html
--rw-r--r--   0 tom       (1000) tom       (1000)      185 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_additional_matrix_filter_space_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      230 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_matrix_filter_value.html
--rw-r--r--   0 tom       (1000) tom       (1000)      217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_nodelink.html
--rw-r--r--   0 tom       (1000) tom       (1000)      370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_overview_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_additional_matrix_filter_space_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_color_filter_space.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1421 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_restrictions.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4455 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_space.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_nodelink_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      610 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_overview_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     9986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/matrix_filters.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1644 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/move_natureguide_node.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node_small.html
--rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/node_loader.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2007 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/node_management_menu.html
--rw-r--r--   0 tom       (1000) tom       (1000)      608 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/nodelist.html
--rw-r--r--   0 tom       (1000) tom       (1000)      195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/reload_matrix_filters.html
--rw-r--r--   0 tom       (1000) tom       (1000)     7146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/manage_nature_guide.html
--rw-r--r--   0 tom       (1000) tom       (1000)      360 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/manage_node.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1932 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/node_analysis.html
--rw-r--r--   0 tom       (1000) tom       (1000)      724 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/nodemenu_loader.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.799315 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)     1352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_colors_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1009 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_description_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_numbers_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)      629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_range_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)      854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_text_description_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4250 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/grid_choices.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/horizontal_choices.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2633 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/range.html
--rw-r--r--   0 tom       (1000) tom       (1000)      834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_colors.html
--rw-r--r--   0 tom       (1000) tom       (1000)      876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_numbers.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_patterns.html
--rw-r--r--   0 tom       (1000) tom       (1000)      911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_taxonfilters.html
--rw-r--r--   0 tom       (1000) tom       (1000)      465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_texts.html
--rw-r--r--   0 tom       (1000) tom       (1000)      798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_colors.html
--rw-r--r--   0 tom       (1000) tom       (1000)      623 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_numbers.html
--rw-r--r--   0 tom       (1000) tom       (1000)       62 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_patterns.html
--rw-r--r--   0 tom       (1000) tom       (1000)      480 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_taxonfilters.html
--rw-r--r--   0 tom       (1000) tom       (1000)      351 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_texts.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.799315 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     6808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)    23054 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    87320 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_matrix_filters.py
--rw-r--r--   0 tom       (1000) tom       (1000)    76980 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)   130947 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    57567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/widgets.py
--rw-r--r--   0 tom       (1000) tom       (1000)    44905 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/zip_import.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.802649 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.802649 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     3659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0002_taxontext_long_text.py
--rw-r--r--   0 tom       (1000) tom       (1000)      392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0003_auto_20221021_0746.py
--rw-r--r--   0 tom       (1000) tom       (1000)      363 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0004_alter_taxontexttype_options.py
--rw-r--r--   0 tom       (1000) tom       (1000)      578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0005_taxonprofile_tags.py
--rw-r--r--   0 tom       (1000) tom       (1000)      474 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0006_taxonprofile_publication_status.py
--rw-r--r--   0 tom       (1000) tom       (1000)      408 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0007_alter_taxonprofile_unique_together.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6874 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.805982 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.805982 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)      655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/batch_change_taxon_profiles_publication_status.html
--rw-r--r--   0 tom       (1000) tom       (1000)      596 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/change_taxon_profile_publication_status.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2591 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_images.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2470 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_traits.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/create_taxon_profile.html
--rw-r--r--   0 tom       (1000) tom       (1000)      689 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile.html
--rw-r--r--   0 tom       (1000) tom       (1000)      342 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_text_type.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3373 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1141 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_type.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_types_order.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1997 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/nature_guide_taxonlist.html
--rw-r--r--   0 tom       (1000) tom       (1000)      628 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/non_nature_guide_taxonlist.html
--rw-r--r--   0 tom       (1000) tom       (1000)      568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/taxonlist.html
--rw-r--r--   0 tom       (1000) tom       (1000)     5999 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profile.html
--rw-r--r--   0 tom       (1000) tom       (1000)     5593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profiles.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1353 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_texts.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.805982 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1064 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templatetags/taxon_profile_tags.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.805982 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     5422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    38014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3688 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    28247 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8299 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/zip_import.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/generic.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/generic_content_validation.py
--rw-r--r--   0 tom       (1000) tom       (1000)    14647 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/generic_content_zip_import.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/global_urls.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/locale/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/locale/de/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.809315 localcosmos_app_kit-0.2.2/app_kit/locale/de/LC_MESSAGES/
--rw-r--r--   0 tom       (1000) tom       (1000)    72219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 tom       (1000) tom       (1000)   121898 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/locale/en/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.809315 localcosmos_app_kit-0.2.2/app_kit/locale/en/LC_MESSAGES/
--rw-r--r--   0 tom       (1000) tom       (1000)      380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 tom       (1000) tom       (1000)    82354 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.809315 localcosmos_app_kit-0.2.2/app_kit/management/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/management/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1278 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/middleware.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.809315 localcosmos_app_kit-0.2.2/app_kit/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     6766 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      378 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/0002_contentimage_features.py
--rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/0003_auto_20220520_0640.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1228 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/0004_auto_20220608_0717.py
--rw-r--r--   0 tom       (1000) tom       (1000)      400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/0005_metaappgenericcontent_position.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)    36009 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      182 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/commands/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/commands/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/commands/fix_staging_domains.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2821 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/middleware.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     2495 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1741 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/public_schema_urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)      544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/setup_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)      388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/setup_urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/setup_views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/
--rw-r--r--   0 tom       (1000) tom       (1000)      887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/contact_us.html
--rw-r--r--   0 tom       (1000) tom       (1000)      968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/delete_account.html
--rw-r--r--   0 tom       (1000) tom       (1000)      778 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/edit_account.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1328 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/my_account.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/setup/
--rw-r--r--   0 tom       (1000) tom       (1000)     1678 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/setup/setup_initial_appkit.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/multi_tenancy/
--rw-r--r--   0 tom       (1000) tom       (1000)     6694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/multi_tenancy/list_app_kits.html
--rw-r--r--   0 tom       (1000) tom       (1000)      750 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/tenant_schema_urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1016 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/permission_rules.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2490 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/server_side_cursors.py
--rw-r--r--   0 tom       (1000) tom       (1000)      267 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/settings.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.812648 localcosmos_app_kit-0.2.2/app_kit/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.815982 localcosmos_app_kit-0.2.2/app_kit/static/anycluster/openlayers/
--rw-r--r--   0 tom       (1000) tom       (1000)   868865 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/anycluster/openlayers/anycluster-openlayers.js
--rw-r--r--   0 tom       (1000) tom       (1000)  1366163 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/anycluster/openlayers/anycluster-openlayers.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.819315 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/
--rw-r--r--   0 tom       (1000) tom       (1000)     3263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ButtonMatrix.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.829315 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/
--rw-r--r--   0 tom       (1000) tom       (1000)    64548 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css
--rw-r--r--   0 tom       (1000) tom       (1000)   151749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)    48488 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   108539 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4897 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
--rw-r--r--   0 tom       (1000) tom       (1000)    76483 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4021 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)    32461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   192348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css
--rw-r--r--   0 tom       (1000) tom       (1000)   492048 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css.map
--rw-r--r--   0 tom       (1000) tom       (1000)   155758 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css
--rw-r--r--   0 tom       (1000) tom       (1000)   625953 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.842648 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/
--rw-r--r--   0 tom       (1000) tom       (1000)   222911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
--rw-r--r--   0 tom       (1000) tom       (1000)   402249 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    78635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   311949 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)   131637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js
--rw-r--r--   0 tom       (1000) tom       (1000)   250568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)    58072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)   190253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.845981 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/
--rw-r--r--   0 tom       (1000) tom       (1000)     2079 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/Alphabetfilter.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3770 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/album.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3428 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/camera.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/observation.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     5892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/occurrence.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    10521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxon_detail.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.849314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/
--rw-r--r--   0 tom       (1000) tom       (1000)     9500 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Amphibia.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    11925 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Animalia.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     5523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Anura.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    20432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Arachnida.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    37205 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Arthropoda.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3750 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Aves.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    10402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Chordata.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    16424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Coleoptera.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     2051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Customfilter.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Fungi.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     5158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    26448 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Insecta.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Lepidoptera.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     6444 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Mammalia.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Mollusca.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3896 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Odonata.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3489 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Plantae.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     7516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/no_filter.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3204 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/wikipedia_button.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.852648 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/
--rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/LICENSE.md
--rw-r--r--   0 tom       (1000) tom       (1000)     3496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.852648 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/
--rw-r--r--   0 tom       (1000) tom       (1000)   524645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/ckeditor.js
--rw-r--r--   0 tom       (1000) tom       (1000)   536734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/ckeditor.js.map
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.859314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/
--rw-r--r--   0 tom       (1000) tom       (1000)      290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/af.js
--rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ar.js
--rw-r--r--   0 tom       (1000) tom       (1000)      516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ast.js
--rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/az.js
--rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/bg.js
--rw-r--r--   0 tom       (1000) tom       (1000)      279 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ca.js
--rw-r--r--   0 tom       (1000) tom       (1000)      654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/cs.js
--rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/da.js
--rw-r--r--   0 tom       (1000) tom       (1000)      419 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/de-ch.js
--rw-r--r--   0 tom       (1000) tom       (1000)      635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/de.js
--rw-r--r--   0 tom       (1000) tom       (1000)      680 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/el.js
--rw-r--r--   0 tom       (1000) tom       (1000)      586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/en-au.js
--rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/en-gb.js
--rw-r--r--   0 tom       (1000) tom       (1000)      495 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/eo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      636 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/es.js
--rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/et.js
--rw-r--r--   0 tom       (1000) tom       (1000)      543 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/eu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fa.js
--rw-r--r--   0 tom       (1000) tom       (1000)      527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fi.js
--rw-r--r--   0 tom       (1000) tom       (1000)      663 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      662 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/gl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/gu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      722 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/he.js
--rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hi.js
--rw-r--r--   0 tom       (1000) tom       (1000)      679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hu.js
--rw-r--r--   0 tom       (1000) tom       (1000)      546 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/id.js
--rw-r--r--   0 tom       (1000) tom       (1000)      679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/it.js
--rw-r--r--   0 tom       (1000) tom       (1000)      659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ja.js
--rw-r--r--   0 tom       (1000) tom       (1000)      881 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/km.js
--rw-r--r--   0 tom       (1000) tom       (1000)      771 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/kn.js
--rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ko.js
--rw-r--r--   0 tom       (1000) tom       (1000)      763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ku.js
--rw-r--r--   0 tom       (1000) tom       (1000)      626 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/lt.js
--rw-r--r--   0 tom       (1000) tom       (1000)      661 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/lv.js
--rw-r--r--   0 tom       (1000) tom       (1000)      518 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/nb.js
--rw-r--r--   0 tom       (1000) tom       (1000)      710 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ne.js
--rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/nl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/no.js
--rw-r--r--   0 tom       (1000) tom       (1000)      237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/oc.js
--rw-r--r--   0 tom       (1000) tom       (1000)      765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/pl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      661 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/pt-br.js
--rw-r--r--   0 tom       (1000) tom       (1000)      509 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/pt.js
--rw-r--r--   0 tom       (1000) tom       (1000)      589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ro.js
--rw-r--r--   0 tom       (1000) tom       (1000)      910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ru.js
--rw-r--r--   0 tom       (1000) tom       (1000)      465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/si.js
--rw-r--r--   0 tom       (1000) tom       (1000)      700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sk.js
--rw-r--r--   0 tom       (1000) tom       (1000)      432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sl.js
--rw-r--r--   0 tom       (1000) tom       (1000)      545 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sq.js
--rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sr-latn.js
--rw-r--r--   0 tom       (1000) tom       (1000)      884 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sv.js
--rw-r--r--   0 tom       (1000) tom       (1000)      406 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/th.js
--rw-r--r--   0 tom       (1000) tom       (1000)      651 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/tk.js
--rw-r--r--   0 tom       (1000) tom       (1000)      643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/tr.js
--rw-r--r--   0 tom       (1000) tom       (1000)      264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/tt.js
--rw-r--r--   0 tom       (1000) tom       (1000)      627 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ug.js
--rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/uk.js
--rw-r--r--   0 tom       (1000) tom       (1000)      648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/vi.js
--rw-r--r--   0 tom       (1000) tom       (1000)      599 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/zh-cn.js
--rw-r--r--   0 tom       (1000) tom       (1000)      586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/zh.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1003 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/package.json
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.859314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/sample/
--rw-r--r--   0 tom       (1000) tom       (1000)     4521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/sample/index.html
--rw-r--r--   0 tom       (1000) tom       (1000)     9567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/sample/styles.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.859314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/src/
--rw-r--r--   0 tom       (1000) tom       (1000)      955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/src/ckeditor.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2118 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/webpack.config.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.859314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/css/
--rw-r--r--   0 tom       (1000) tom       (1000)      637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/css/app.css
--rw-r--r--   0 tom       (1000) tom       (1000)    16095 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/css/app_kit.css
--rw-r--r--   0 tom       (1000) tom       (1000)   166813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/handlebars-v4.0.10.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.862647 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/horizontal-slide/
--rw-r--r--   0 tom       (1000) tom       (1000)     3274 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/horizontal-slide/horizontal-slide.css
--rw-r--r--   0 tom       (1000) tom       (1000)     1216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/horizontal-slide/horizontal-slide.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.865980 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     3776 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/add_element.png
--rw-r--r--   0 tom       (1000) tom       (1000)     5082 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/auditory.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      429 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/burger.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4396 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/checkbox-off.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/checkbox-on.svg
--rw-r--r--   0 tom       (1000) tom       (1000)      815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/close.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.869314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/
--rw-r--r--   0 tom       (1000) tom       (1000)    10402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/BackboneTaxonomy.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     9239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/FactSheets.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    12414 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Frontend.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/GenericForm.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     5933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Glossary.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     5892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Map.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     7516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/NatureGuide.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    10521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/TaxonProfiles.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    14005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/template_content.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3524 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/forward-arrow.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     8347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/gear.gif
--rw-r--r--   0 tom       (1000) tom       (1000)     4042 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/gustatory.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1000 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/lclogo32.png
--rw-r--r--   0 tom       (1000) tom       (1000)     3745 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/microscope.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     3434 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/olfactory.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    12200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/scalpel.svg
--rw-r--r--   0 tom       (1000) tom       (1000)    32016 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner.gif
--rw-r--r--   0 tom       (1000) tom       (1000)    60165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner_huge.gif
--rw-r--r--   0 tom       (1000) tom       (1000)    13011 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner_old.gif
--rw-r--r--   0 tom       (1000) tom       (1000)     3763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/tactile.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     4865 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/visual.svg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.869314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/
--rw-r--r--   0 tom       (1000) tom       (1000)    73792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/hammer.js
--rw-r--r--   0 tom       (1000) tom       (1000)    86927 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/jquery-3.3.1.min.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6710 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/observatory_admin.js
--rw-r--r--   0 tom       (1000) tom       (1000)      457 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/polyfills.js
--rw-r--r--   0 tom       (1000) tom       (1000)    20337 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/popper.min.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.752650 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.872647 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/
--rw-r--r--   0 tom       (1000) tom       (1000)     2973 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Control.Draw.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.Draw.Event.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4728 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.draw.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9137 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Toolbar.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Tooltip.js
--rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/copyright.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.872647 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/
--rw-r--r--   0 tom       (1000) tom       (1000)     2760 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/DrawToolbar.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.872647 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/
--rw-r--r--   0 tom       (1000) tom       (1000)     2254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Circle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1063 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.CircleMarker.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2436 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Feature.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3193 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Marker.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3279 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polygon.js
--rw-r--r--   0 tom       (1000) tom       (1000)    17648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polyline.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Rectangle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3273 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.SimpleShape.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.872647 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/
--rw-r--r--   0 tom       (1000) tom       (1000)     4605 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/EditToolbar.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.875980 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Circle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.CircleMarker.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Marker.js
--rw-r--r--   0 tom       (1000) tom       (1000)    13008 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Poly.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3306 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Rectangle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5387 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.SimpleShape.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4184 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Delete.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8232 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Edit.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.875980 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/
--rw-r--r--   0 tom       (1000) tom       (1000)     5123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/GeometryUtil.js
--rw-r--r--   0 tom       (1000) tom       (1000)      757 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LatLngUtil.js
--rw-r--r--   0 tom       (1000) tom       (1000)      777 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LineUtil.Intersect.js
--rw-r--r--   0 tom       (1000) tom       (1000)      868 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polygon.Intersect.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3044 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polyline.Intersect.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7446 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/TouchEvents.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.879314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     3581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet-2x.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.png
--rw-r--r--   0 tom       (1000) tom       (1000)     4975 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     7165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/leaflet.draw.css
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.879314 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/sortable/
--rw-r--r--   0 tom       (1000) tom       (1000)    43303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/app_kit/sortable/Sortable.min.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.879314 localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/
--rw-r--r--   0 tom       (1000) tom       (1000)    57236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/IdentificationMatrix.js
--rw-r--r--   0 tom       (1000) tom       (1000)    47183 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/IdentificationMatrix_beta.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/crosslink.svg
--rw-r--r--   0 tom       (1000) tom       (1000)     1248 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/jquery-searchfornode-autocomplete.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/noimage.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.755983 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.915979 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/
--rw-r--r--   0 tom       (1000) tom       (1000)      822 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/AssertionError.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7901 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.js
--rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/CollectionEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      125 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/CollectionEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/CollectionEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3248 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      752 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)      511 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Disposable.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Disposable.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      540 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Disposable.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9073 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1652 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1816 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11371 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3779 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5665 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1675 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      430 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2133 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageCanvas.js
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageState.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageState.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      142 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageState.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      525 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4784 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1519 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      500 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2899 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Kinetic.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1337 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/LICENSE.md
--rw-r--r--   0 tom       (1000) tom       (1000)    30833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     5845 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    58212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2473 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3156 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.js
--rw-r--r--   0 tom       (1000) tom       (1000)      572 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1506 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)      929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      838 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEvent.js
--rw-r--r--   0 tom       (1000) tom       (1000)      339 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)      201 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapProperty.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapProperty.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapProperty.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1232 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7563 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.js
--rw-r--r--   0 tom       (1000) tom       (1000)      173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ObjectEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ObjectEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ObjectEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11257 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    16432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/README.md
--rw-r--r--   0 tom       (1000) tom       (1000)     8274 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.js
--rw-r--r--   0 tom       (1000) tom       (1000)      499 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileCache.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileCache.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1015 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileCache.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2300 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2317 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.js
--rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileState.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileState.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileState.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3909 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      828 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3317 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)    42492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     5572 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    72272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.js
--rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewHint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewHint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewHint.js
--rw-r--r--   0 tom       (1000) tom       (1000)      182 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewProperty.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewProperty.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ViewProperty.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5897 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.js
--rw-r--r--   0 tom       (1000) tom       (1000)      211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/asserts.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/asserts.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      304 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/asserts.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      437 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/centerconstraint.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/color.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/color.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5110 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/color.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/colorlike.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      233 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/colorlike.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      800 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/colorlike.js
--rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/console.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/console.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/console.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.922646 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/
--rw-r--r--   0 tom       (1000) tom       (1000)     6027 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      781 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9375 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      626 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6285 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1313 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8198 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1091 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18591 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      439 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5163 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Rotate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1483 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13760 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      286 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4863 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Zoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      743 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2114 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      309 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2714 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      193 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2124 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/defaults.js
--rw-r--r--   0 tom       (1000) tom       (1000)      723 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9638 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1017 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12576 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1711 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/css.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/css.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2779 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/css.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.929313 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dist/
--rw-r--r--   0 tom       (1000) tom       (1000)   748708 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dist/ol.js
--rw-r--r--   0 tom       (1000) tom       (1000)  4228748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dist/ol.js.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2452 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/easing.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/easing.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/easing.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.939312 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/
--rw-r--r--   0 tom       (1000) tom       (1000)     1522 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Event.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Event.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Event.js
--rw-r--r--   0 tom       (1000) tom       (1000)      544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/EventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/KeyCode.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/KeyCode.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      141 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/KeyCode.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3003 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      612 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10962 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3855 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3526 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.939312 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent/
--rw-r--r--   0 tom       (1000) tom       (1000)      256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent/Relationship.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent/Relationship.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent/Relationship.js
--rw-r--r--   0 tom       (1000) tom       (1000)    14578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2724 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    24323 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      824 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.955979 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/
--rw-r--r--   0 tom       (1000) tom       (1000)     3632 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      823 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    17540 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11033 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9633 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.js
--rw-r--r--   0 tom       (1000) tom       (1000)      380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      954 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8828 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2130 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    23660 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.js
--rw-r--r--   0 tom       (1000) tom       (1000)    14290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     3668 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    37006 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.js
--rw-r--r--   0 tom       (1000) tom       (1000)      245 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML32.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      121 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML32.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML32.js
--rw-r--r--   0 tom       (1000) tom       (1000)    12751 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    20323 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    26563 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GPX.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1007 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    15746 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IGC.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3832 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      670 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5305 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1615 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    93722 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      608 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11879 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.js
--rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OSMXML.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OSMXML.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5027 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OSMXML.js
--rw-r--r--   0 tom       (1000) tom       (1000)      115 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OWS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OWS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8683 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OWS.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6011 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1042 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9920 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4959 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1000 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      623 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13534 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9753 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1575 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    43118 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4997 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    25384 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1084 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    21719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKT.js
--rw-r--r--   0 tom       (1000) tom       (1000)      309 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      185 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18326 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      308 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.js
--rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XML.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      242 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XML.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XML.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6403 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1346 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7814 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.962645 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/
--rw-r--r--   0 tom       (1000) tom       (1000)      404 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/And.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      139 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/And.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      429 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/And.js
--rw-r--r--   0 tom       (1000) tom       (1000)      903 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.js
--rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      209 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      631 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.js
--rw-r--r--   0 tom       (1000) tom       (1000)      940 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.js
--rw-r--r--   0 tom       (1000) tom       (1000)      683 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      191 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      660 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Contains.js
--rw-r--r--   0 tom       (1000) tom       (1000)      966 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.js
--rw-r--r--   0 tom       (1000) tom       (1000)      689 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      191 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      666 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.js
--rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      639 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/During.js
--rw-r--r--   0 tom       (1000) tom       (1000)      570 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      603 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      226 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      571 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Filter.js
--rw-r--r--   0 tom       (1000) tom       (1000)      481 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.js
--rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      693 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      672 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.js
--rw-r--r--   0 tom       (1000) tom       (1000)      690 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1451 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.js
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      155 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.js
--rw-r--r--   0 tom       (1000) tom       (1000)      469 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.js
--rw-r--r--   0 tom       (1000) tom       (1000)      505 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      261 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      774 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.js
--rw-r--r--   0 tom       (1000) tom       (1000)      477 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Not.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Not.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      449 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Not.js
--rw-r--r--   0 tom       (1000) tom       (1000)      582 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      599 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.js
--rw-r--r--   0 tom       (1000) tom       (1000)      393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Or.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      136 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Or.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Or.js
--rw-r--r--   0 tom       (1000) tom       (1000)      239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      345 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1060 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.js
--rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      651 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Within.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9716 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10032 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8846 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/readme.md
--rw-r--r--   0 tom       (1000) tom       (1000)      171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xlink.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      150 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xlink.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xlink.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2396 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3802 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1012 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)       99 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      972 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1132 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/functions.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      284 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/functions.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/functions.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.969312 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/
--rw-r--r--   0 tom       (1000) tom       (1000)     2294 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8576 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Circle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1449 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2020 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9203 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4585 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8304 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      510 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LinearRing.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      856 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1898 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5315 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1024 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12366 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.js
--rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      261 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3052 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Point.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1305 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3606 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      971 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.975978 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/area.js
--rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/center.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/center.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/center.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3731 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      964 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1712 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3487 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2002 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2609 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.js
--rw-r--r--   0 tom       (1000) tom       (1000)      556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      206 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      873 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/flip.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1677 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      469 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5891 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1902 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      524 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2526 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1697 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5052 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.js
--rw-r--r--   0 tom       (1000) tom       (1000)      700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      283 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/length.js
--rw-r--r--   0 tom       (1000) tom       (1000)      589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1889 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3946 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      729 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.js
--rw-r--r--   0 tom       (1000) tom       (1000)      353 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.js
--rw-r--r--   0 tom       (1000) tom       (1000)      889 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      964 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/segments.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6174 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.js
--rw-r--r--   0 tom       (1000) tom       (1000)      575 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      234 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.js
--rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/topology.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/topology.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/topology.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3731 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.js
--rw-r--r--   0 tom       (1000) tom       (1000)      726 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/has.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/has.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/has.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/index.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/index.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1416 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/index.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.989311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/
--rw-r--r--   0 tom       (1000) tom       (1000)      929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1777 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5948 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1390 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7979 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2243 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      369 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5507 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragPan.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3238 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2262 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      252 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)    20613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     3102 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    60848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6825 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    16223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5470 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1090 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5012 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2531 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      302 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.js
--rw-r--r--   0 tom       (1000) tom       (1000)    19642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2464 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    52422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7644 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      333 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.js
--rw-r--r--   0 tom       (1000) tom       (1000)      978 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6229 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.js
--rw-r--r--   0 tom       (1000) tom       (1000)      120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Property.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Property.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Property.js
--rw-r--r--   0 tom       (1000) tom       (1000)    15835 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2036 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8026 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    20211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.js
--rw-r--r--   0 tom       (1000) tom       (1000)    10173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/defaults.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1502 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1451 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.999311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/
--rw-r--r--   0 tom       (1000) tom       (1000)    11607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1896 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11672 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4914 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      257 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseImage.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8297 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9666 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      957 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.js
--rw-r--r--   0 tom       (1000) tom       (1000)    18432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1998 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    37037 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1067 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Image.js
--rw-r--r--   0 tom       (1000) tom       (1000)    14105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    15058 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.js
--rw-r--r--   0 tom       (1000) tom       (1000)    14310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9688 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.js
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Property.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Property.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      319 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Property.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1179 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      987 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Tile.js
--rw-r--r--   0 tom       (1000) tom       (1000)      171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/TileProperty.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/TileProperty.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/TileProperty.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1229 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Vector.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8265 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      375 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4741 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorImage.js
--rw-r--r--   0 tom       (1000) tom       (1000)    14538 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6068 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      471 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    17569 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)      739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      709 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/loadingstrategy.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3817 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/net.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/net.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3603 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/net.js
--rw-r--r--   0 tom       (1000) tom       (1000)      388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/obj.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/obj.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/obj.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ol.css
--rw-r--r--   0 tom       (1000) tom       (1000)      817 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/package.json
--rw-r--r--   0 tom       (1000) tom       (1000)      455 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pixel.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pixel.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pixel.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.999311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pointer/
--rw-r--r--   0 tom       (1000) tom       (1000)      344 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pointer/EventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pointer/EventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/pointer/EventType.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.999311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/
--rw-r--r--   0 tom       (1000) tom       (1000)     8986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1297 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8017 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.js
--rw-r--r--   0 tom       (1000) tom       (1000)      921 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1040 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Units.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1598 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      514 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3363 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.js
--rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg4326.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2019 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/proj4.js
--rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      775 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/projections.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1649 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      435 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/transforms.js
--rw-r--r--   0 tom       (1000) tom       (1000)    16859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    27310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.002644 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/
--rw-r--r--   0 tom       (1000) tom       (1000)     1408 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Box.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      488 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Box.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2992 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Box.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1690 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Event.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      319 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Event.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1458 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Event.js
--rw-r--r--   0 tom       (1000) tom       (1000)      411 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/EventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      178 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/EventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1606 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/EventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1592 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4053 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.009311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/
--rw-r--r--   0 tom       (1000) tom       (1000)     5941 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1658 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    19002 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      466 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9269 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1944 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    40772 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1058 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1958 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      548 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.js
--rw-r--r--   0 tom       (1000) tom       (1000)    10208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    34441 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.js
--rw-r--r--   0 tom       (1000) tom       (1000)      887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      298 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      742 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.js
--rw-r--r--   0 tom       (1000) tom       (1000)      460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4871 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.js
--rw-r--r--   0 tom       (1000) tom       (1000)      527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2706 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18880 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      419 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11093 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1951 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13928 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.012644 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/
--rw-r--r--   0 tom       (1000) tom       (1000)     4147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1021 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      234 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.js
--rw-r--r--   0 tom       (1000) tom       (1000)    13641 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    15253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.js
--rw-r--r--   0 tom       (1000) tom       (1000)      901 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.js
--rw-r--r--   0 tom       (1000) tom       (1000)      984 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3956 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1507 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/constants.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4610 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      718 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4667 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4979 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.015977 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/
--rw-r--r--   0 tom       (1000) tom       (1000)      609 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      252 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4045 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Composite.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5106 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1202 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5533 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4435 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.015977 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/
--rw-r--r--   0 tom       (1000) tom       (1000)      968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7381 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9121 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    23698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      431 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6481 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1093 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    23555 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3907 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      863 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    27833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    16654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.019311 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/
--rw-r--r--   0 tom       (1000) tom       (1000)     5062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      774 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11421 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1431 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    24796 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1056 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    27112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5373 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1306 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      423 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6336 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.022644 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/
--rw-r--r--   0 tom       (1000) tom       (1000)     4422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5963 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3377 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9619 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    15737 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.js
--rw-r--r--   0 tom       (1000) tom       (1000)      221 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/common.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      144 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/common.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      184 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/common.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      415 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/resolutionconstraint.js
--rw-r--r--   0 tom       (1000) tom       (1000)      853 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      413 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/rotationconstraint.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1406 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/size.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      300 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/size.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/size.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.042643 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/
--rw-r--r--   0 tom       (1000) tom       (1000)     7571 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      916 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10022 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5872 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1046 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9197 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8712 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12993 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)    13175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1097 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    31154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3440 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12907 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/IIIF.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7914 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      934 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     9476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6089 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4801 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6667 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1018 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      574 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5366 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14056 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3934 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      386 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4311 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OSM.js
--rw-r--r--   0 tom       (1000) tom       (1000)    15270 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2699 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    29965 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1276 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6064 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3520 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4240 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Stamen.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11482 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2520 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8601 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      224 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2504 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileDebug.js
--rw-r--r--   0 tom       (1000) tom       (1000)      282 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      150 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)    10583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      993 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      555 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11918 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    15573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)    30310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     3930 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    38214 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.js
--rw-r--r--   0 tom       (1000) tom       (1000)      492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      204 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1574 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      961 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18992 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.js
--rw-r--r--   0 tom       (1000) tom       (1000)    11081 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18733 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      371 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/XYZ.js
--rw-r--r--   0 tom       (1000) tom       (1000)     7798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      596 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    10426 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.js
--rw-r--r--   0 tom       (1000) tom       (1000)      164 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/common.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/common.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/common.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4415 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.js
--rw-r--r--   0 tom       (1000) tom       (1000)      659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/wms.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/wms.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      641 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/wms.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2913 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3784 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/sphere.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      482 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/sphere.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/sphere.js
--rw-r--r--   0 tom       (1000) tom       (1000)      682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/string.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      243 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/string.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/string.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.045977 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/
--rw-r--r--   0 tom       (1000) tom       (1000)     3770 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6273 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2903 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5202 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3207 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      875 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5157 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.052643 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/
--rw-r--r--   0 tom       (1000) tom       (1000)     2614 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2604 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Circle.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1806 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      404 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Fill.js
--rw-r--r--   0 tom       (1000) tom       (1000)    10407 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    16310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1069 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     7080 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1928 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1604 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.js
--rw-r--r--   0 tom       (1000) tom       (1000)     8242 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    17260 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5450 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1135 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4957 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.js
--rw-r--r--   0 tom       (1000) tom       (1000)    12707 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2067 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.js
--rw-r--r--   0 tom       (1000) tom       (1000)    16582 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    14673 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.js
--rw-r--r--   0 tom       (1000) tom       (1000)    13072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    33262 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.js
--rw-r--r--   0 tom       (1000) tom       (1000)    27824 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1036 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    17715 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2328 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/literal.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/literal.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/literal.js
--rw-r--r--   0 tom       (1000) tom       (1000)      532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1932 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      491 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2282 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilecoord.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.052643 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/
--rw-r--r--   0 tom       (1000) tom       (1000)    16618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2245 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    22965 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6106 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     6718 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.js
--rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/common.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      178 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/common.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/common.js
--rw-r--r--   0 tom       (1000) tom       (1000)     4352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      550 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     5910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1550 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.js
--rw-r--r--   0 tom       (1000) tom       (1000)     6147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      971 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     8826 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.js
--rw-r--r--   0 tom       (1000) tom       (1000)      414 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/uri.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      153 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/uri.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      841 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/uri.js
--rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/util.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      210 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/util.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      772 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/util.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.055976 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/
--rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      673 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/mat4.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.059310 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/
--rw-r--r--   0 tom       (1000) tom       (1000)     3149 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     3538 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.js
--rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)      156 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.js
--rw-r--r--   0 tom       (1000) tom       (1000)    22048 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    35286 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.js
--rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     1181 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.js
--rw-r--r--   0 tom       (1000) tom       (1000)     5700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    11869 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.js
--rw-r--r--   0 tom       (1000) tom       (1000)     2840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     4503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.js
--rw-r--r--   0 tom       (1000) tom       (1000)     9815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     1420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.js
--rw-r--r--   0 tom       (1000) tom       (1000)     3147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    12983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.js
--rw-r--r--   0 tom       (1000) tom       (1000)     1874 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      531 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)     2818 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.059310 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/worker/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/worker/webgl.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)      107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/worker/webgl.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    13749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/worker/webgl.js
--rw-r--r--   0 tom       (1000) tom       (1000)    13680 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.d.ts
--rw-r--r--   0 tom       (1000) tom       (1000)     2033 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.d.ts.map
--rw-r--r--   0 tom       (1000) tom       (1000)    18289 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.js
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.755983 localcosmos_app_kit-0.2.2/app_kit/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.059310 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.062643 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/
--rw-r--r--   0 tom       (1000) tom       (1000)     1108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/add_existing_generic_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/add_feature_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3139 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/app_card.html
--rw-r--r--   0 tom       (1000) tom       (1000)      460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/app_limit_reached.html
--rw-r--r--   0 tom       (1000) tom       (1000)      364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/build_errors.html
--rw-r--r--   0 tom       (1000) tom       (1000)      336 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/build_warnings.html
--rw-r--r--   0 tom       (1000) tom       (1000)      854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/change_generic_content_status.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/component_card.html
--rw-r--r--   0 tom       (1000) tom       (1000)      296 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/content_image_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      179 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/content_image_with_text_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/create_generic_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      246 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/delete_app_language.html
--rw-r--r--   0 tom       (1000) tom       (1000)       72 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/delete_content_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      747 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/delete_localized_content_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)      765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/edit_generic_content_name.html
--rw-r--r--   0 tom       (1000) tom       (1000)      479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/form_extended_with_content_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1087 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/get_content_image_suggestions.html
--rw-r--r--   0 tom       (1000) tom       (1000)      479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/get_translation.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/localized_content_image_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/manage_app_languages.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/manage_feature.html
--rw-r--r--   0 tom       (1000) tom       (1000)      485 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/mockbutton.html
--rw-r--r--   0 tom       (1000) tom       (1000)      715 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/options_form.html
--rw-r--r--   0 tom       (1000) tom       (1000)      215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/reload_appbar.html
--rw-r--r--   0 tom       (1000) tom       (1000)      311 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/remove_app_generic_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/tag_any_element.html
--rw-r--r--   0 tom       (1000) tom       (1000)      189 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/tags.html
--rw-r--r--   0 tom       (1000) tom       (1000)      764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/translate_app_pagination.html
--rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/upload_theme_image.html
--rw-r--r--   0 tom       (1000) tom       (1000)     4569 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/zip_import.html
--rw-r--r--   0 tom       (1000) tom       (1000)    15798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/base.html
--rw-r--r--   0 tom       (1000) tom       (1000)    13642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/build_app.html
--rw-r--r--   0 tom       (1000) tom       (1000)      164 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/content_images.html
--rw-r--r--   0 tom       (1000) tom       (1000)      239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/home.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.062643 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/legal/
--rw-r--r--   0 tom       (1000) tom       (1000)      551 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/legal/legal_notice.html
--rw-r--r--   0 tom       (1000) tom       (1000)    25354 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/legal/privacy_statement.html
--rw-r--r--   0 tom       (1000) tom       (1000)      789 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/list_manage_apps.html
--rw-r--r--   0 tom       (1000) tom       (1000)      751 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/list_manage_generic_content.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2960 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/manage_app.html
--rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/manage_app_design.html
--rw-r--r--   0 tom       (1000) tom       (1000)     3987 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/manage_generic_content.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/snippets/
--rw-r--r--   0 tom       (1000) tom       (1000)     1394 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/snippets/ckeditor_js_snippet.html
--rw-r--r--   0 tom       (1000) tom       (1000)      835 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/start_new_app.html
--rw-r--r--   0 tom       (1000) tom       (1000)     6172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/translate_app.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/templatetags/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templatetags/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/templatetags/app_tags.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:39.755983 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/
--rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/settings.json
--rw-r--r--   0 tom       (1000) tom       (1000)      678 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain.zip
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.065976 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/
--rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/settings.json
--rw-r--r--   0 tom       (1000) tom       (1000)      816 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain.zip
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.069310 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/
--rw-r--r--   0 tom       (1000) tom       (1000)    78900 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/Leaf-large.jpg
--rw-r--r--   0 tom       (1000) tom       (1000)    49349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/Leaf.jpg
--rw-r--r--   0 tom       (1000) tom       (1000)   274763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/app-background.jpg
--rw-r--r--   0 tom       (1000) tom       (1000)   409549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/localcosmos-logo.svg
--rw-r--r--   0 tom       (1000) tom       (1000)   156278 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/test-image-2560-1440.jpg
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/ipa_for_tests/
--rw-r--r--   0 tom       (1000) tom       (1000)    78900 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/ipa_for_tests/TestApp.ipa
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/templates/
--rw-r--r--   0 tom       (1000) tom       (1000)      147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/templates/neobiota.html
--rw-r--r--   0 tom       (1000) tom       (1000)     2693 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/cases.py
--rw-r--r--   0 tom       (1000) tom       (1000)    12293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)    17134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)    20463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/test_forms.py
--rw-r--r--   0 tom       (1000) tom       (1000)    48598 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/test_models.py
--rw-r--r--   0 tom       (1000) tom       (1000)    81265 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      511 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/validators.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/view_mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)    53553 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.2/app_kit/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     1170 2024-04-19 07:18:39.000000 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)    90617 2024-04-19 07:18:39.000000 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-19 07:18:39.000000 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      248 2024-04-19 07:18:39.000000 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        8 2024-04-19 07:18:39.000000 localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-19 07:18:40.072643 localcosmos_app_kit-0.2.2/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)     1275 2024-04-19 07:15:32.000000 localcosmos_app_kit-0.2.2/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit-0.2.3/LICENCE
+-rw-r--r--   0 tom       (1000) tom       (1000)     1156 2024-04-10 13:05:33.000000 localcosmos_app_kit-0.2.3/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     1170 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.417842 localcosmos_app_kit-0.2.3/app_kit/
+-rw-r--r--   0 tom       (1000) tom       (1000)       19 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      209 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/admin_urls.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.417842 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/
+-rw-r--r--   0 tom       (1000) tom       (1000)       64 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/apps.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.417842 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      255 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/permissions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3331 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.417842 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1070 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6796 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3814 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/app_kit_api/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.421176 localcosmos_app_kit-0.2.3/app_kit/appbuilder/
+-rw-r--r--   0 tom       (1000) tom       (1000)    28628 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppBuilderBase.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppPreviewBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   110094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppReleaseBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/ContentImageBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/GBIFlib.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.424509 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/BackboneTaxonomyJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3327 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/ButtonMatrixJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2735 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/FrontendJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6759 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/GenericFormJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/GlossaryJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6447 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/JSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2755 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/MapJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    25338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/NatureGuideJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    29123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/TaxonProfilesJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/TemplateContentJSONBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      152 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/precompile_fulltree.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.424509 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_ContentImageBuilder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2378 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_builder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14881 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_builder_base.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_preview_builder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    28055 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_release_builder.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       88 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      471 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/context_processors.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       82 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/definitions.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.424509 localcosmos_app_kit-0.2.3/app_kit/features/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      124 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1812 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2327 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/add_taxon_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1529 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbone_taxa_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbonetaxonomy.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      622 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_fulltree_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1206 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/remove_backbone_taxon.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2296 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/taxonlist.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1401 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      778 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget_search_only.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1743 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6504 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1028 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.427843 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    11368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      153 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/ajax/generic_form_exposed_field_options.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1315 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/buttonmatrix_button.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1084 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/delete_buttonmatrix_element.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_button.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_buttonmatrix.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1351 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templatetags/buttonmatrix_tags.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8015 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/frontend/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/PrivateFrontendImporter.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6636 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/0002_frontend_configuration.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/0003_alter_frontendtext_unique_together.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.431176 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      829 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/change_frontend.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      646 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/install_private_frontend.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/manage_frontend_settings.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1270 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/upload_private_frontend.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1587 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/manage_frontend.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.434510 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_PrivateFrontendImporter.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1702 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/frontend/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.434510 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13794 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.434510 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    13963 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.434510 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/generic_forms/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9793 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/generic_forms/datePicker.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      314 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/generic_forms/genericforms.css
+-rw-r--r--   0 tom       (1000) tom       (1000)      160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/generic_forms/genericforms.css~
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.434510 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.437843 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      923 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1562 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_value.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3847 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3462 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field_choices.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      546 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/generic_field.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1658 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/generic_field_modify.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     9240 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/manage_generic_form.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.437843 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templatetags/genericforms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.437843 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    15840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16038 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8369 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_templatetags_old.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    40955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1754 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/widgets.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.437843 localcosmos_app_kit-0.2.3/app_kit/features/glossary/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1410 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.441177 localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2295 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/0002_auto_20201207_1328.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2746 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.441177 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.441177 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1135 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/delete_glossary_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      754 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/glossary_entries.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/glossary_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/manage_glossary_entry.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      566 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/manage_glossary.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.441177 localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)      692 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10825 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      951 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6668 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8509 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/glossary/zip_import.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.441177 localcosmos_app_kit-0.2.3/app_kit/features/maps/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2692 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.444510 localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/0002_maptaxonomicfilter_filtertaxon.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2142 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.444510 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.444510 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      333 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/delete_filter_taxon.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     7840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/manage_project_area.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/manage_taxonomic_filter.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2665 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/taxonomic_filters.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     7838 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/manage_maps.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.444510 localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1227 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4821 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9019 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/maps/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.447844 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/fields.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14879 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7259 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filter_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filter_space_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    51676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filters.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.451177 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)    11025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      913 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0002_auto_20201013_0901.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0003_matrixfilterrestriction.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0004_auto_20210616_1315.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      391 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0005_metanode_settings.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0006_auto_20220503_0747.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0007_auto_20221110_0613.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0008_meta_node_description.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      411 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0009_meta_node_morphotype.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      403 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0010_matrix_filter_additional_data.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    52381 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.451177 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.454511 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4066 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes_page.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_keynodes_menu.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/copy_tree_branch.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      185 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_additional_matrix_filter_space_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      230 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_matrix_filter_value.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_nodelink.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      370 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/delete_overview_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_additional_matrix_filter_space_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_color_filter_space.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1421 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_restrictions.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4455 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_space.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_nodelink_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      610 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_overview_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     9986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/matrix_filters.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1644 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/move_natureguide_node.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node_small.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/node_loader.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2007 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/node_management_menu.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      608 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/nodelist.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/reload_matrix_filters.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     7146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/manage_nature_guide.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      360 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/manage_node.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1932 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/node_analysis.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      724 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/nodemenu_loader.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.454511 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_colors_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1009 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_description_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_numbers_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_range_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_text_description_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4250 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/grid_choices.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/horizontal_choices.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2633 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/range.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_colors.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_numbers.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_patterns.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_taxonfilters.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_texts.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_colors.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      623 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_numbers.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       62 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_patterns.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      480 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_taxonfilters.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      351 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_texts.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.457844 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    23054 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    87320 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_matrix_filters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    76980 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)   130947 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    57567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/widgets.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    44905 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/zip_import.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.461177 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.461177 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0002_taxontext_long_text.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0003_auto_20221021_0746.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      363 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0004_alter_taxontexttype_options.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0005_taxonprofile_tags.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      474 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0006_taxonprofile_publication_status.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      408 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0007_alter_taxonprofile_unique_together.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6874 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.464511 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.464511 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)      655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/batch_change_taxon_profiles_publication_status.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      596 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/change_taxon_profile_publication_status.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2591 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_images.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2470 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_traits.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/create_taxon_profile.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      689 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      342 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_text_type.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3373 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1141 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_type.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_types_order.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1997 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/nature_guide_taxonlist.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      628 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/non_nature_guide_taxonlist.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/taxonlist.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     5999 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profile.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     5593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profiles.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1353 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_texts.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.464511 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1064 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templatetags/taxon_profile_tags.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.464511 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    38014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3688 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    28498 2024-04-22 07:25:20.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8299 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/zip_import.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/generic.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/generic_content_validation.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    14647 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/generic_content_zip_import.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/global_urls.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/locale/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/locale/de/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.467844 localcosmos_app_kit-0.2.3/app_kit/locale/de/LC_MESSAGES/
+-rw-r--r--   0 tom       (1000) tom       (1000)    72219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 tom       (1000) tom       (1000)   121898 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.407842 localcosmos_app_kit-0.2.3/app_kit/locale/en/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.467844 localcosmos_app_kit-0.2.3/app_kit/locale/en/LC_MESSAGES/
+-rw-r--r--   0 tom       (1000) tom       (1000)      380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 tom       (1000) tom       (1000)    82354 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.467844 localcosmos_app_kit-0.2.3/app_kit/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/management/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1278 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/middleware.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.467844 localcosmos_app_kit-0.2.3/app_kit/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6766 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      378 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/0002_contentimage_features.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/0003_auto_20220520_0640.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1228 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/0004_auto_20220608_0717.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/0005_metaappgenericcontent_position.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    36009 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      182 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/commands/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/commands/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/commands/fix_staging_domains.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2821 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/middleware.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2495 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2822 2024-04-19 10:28:04.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1741 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/public_schema_urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/setup_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/setup_urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/setup_views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/
+-rw-r--r--   0 tom       (1000) tom       (1000)      887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/contact_us.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/delete_account.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      778 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/edit_account.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1328 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/my_account.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.471178 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/setup/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1678 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/setup/setup_initial_appkit.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.474511 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/multi_tenancy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/multi_tenancy/list_app_kits.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      750 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/tenant_schema_urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1016 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/permission_rules.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2490 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/server_side_cursors.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      267 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/settings.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.474511 localcosmos_app_kit-0.2.3/app_kit/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.474511 localcosmos_app_kit-0.2.3/app_kit/static/anycluster/openlayers/
+-rw-r--r--   0 tom       (1000) tom       (1000)   868865 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/anycluster/openlayers/anycluster-openlayers.js
+-rw-r--r--   0 tom       (1000) tom       (1000)  1366163 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/anycluster/openlayers/anycluster-openlayers.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.477845 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ButtonMatrix.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.487845 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)    64548 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   151749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    48488 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   108539 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4897 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    76483 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4021 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    32461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   192348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   492048 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   155758 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   625953 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.497845 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/
+-rw-r--r--   0 tom       (1000) tom       (1000)   222911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   402249 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    78635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   311949 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)   131637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   250568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    58072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   190253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.501179 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2079 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/Alphabetfilter.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3770 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/album.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3428 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/camera.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/observation.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     5892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/occurrence.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    10521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxon_detail.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.507846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/
+-rw-r--r--   0 tom       (1000) tom       (1000)     9500 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Amphibia.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    11925 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Animalia.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     5523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Anura.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    20432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Arachnida.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    37205 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Arthropoda.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3750 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Aves.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    10402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Chordata.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    16424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Coleoptera.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     2051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Customfilter.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Fungi.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     5158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    26448 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Insecta.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Lepidoptera.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     6444 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Mammalia.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Mollusca.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3896 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Odonata.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3489 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Plantae.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     7516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/no_filter.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3204 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/wikipedia_button.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.507846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/LICENSE.md
+-rw-r--r--   0 tom       (1000) tom       (1000)     3496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.507846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/
+-rw-r--r--   0 tom       (1000) tom       (1000)   524645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/ckeditor.js
+-rw-r--r--   0 tom       (1000) tom       (1000)   536734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/ckeditor.js.map
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.514513 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/
+-rw-r--r--   0 tom       (1000) tom       (1000)      290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/af.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ar.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ast.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/az.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/bg.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      279 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ca.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/cs.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/da.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      419 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/de-ch.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/de.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      680 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/el.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/en-au.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/en-gb.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      495 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/eo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      636 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/es.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/et.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      543 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/eu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fa.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      663 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      662 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/gl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/gu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      722 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/he.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hu.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      546 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/id.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/it.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ja.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      881 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/km.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      771 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/kn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ko.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ku.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      626 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/lt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      661 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/lv.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      518 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/nb.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      710 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ne.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/nl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/no.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/oc.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/pl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      661 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/pt-br.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      509 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/pt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ro.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ru.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/si.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      545 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sq.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sr-latn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      884 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sv.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      406 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/th.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      651 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/tk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/tr.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/tt.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      627 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ug.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/uk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/vi.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      599 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/zh-cn.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/zh.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1003 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/package.json
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.517846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/sample/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/sample/index.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     9567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/sample/styles.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.517846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/src/
+-rw-r--r--   0 tom       (1000) tom       (1000)      955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/src/ckeditor.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2118 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/webpack.config.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.517846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/css/
+-rw-r--r--   0 tom       (1000) tom       (1000)      637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/css/app.css
+-rw-r--r--   0 tom       (1000) tom       (1000)    16095 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/css/app_kit.css
+-rw-r--r--   0 tom       (1000) tom       (1000)   166813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/handlebars-v4.0.10.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.517846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/horizontal-slide/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3274 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/horizontal-slide/horizontal-slide.css
+-rw-r--r--   0 tom       (1000) tom       (1000)     1216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/horizontal-slide/horizontal-slide.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.521179 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3776 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/add_element.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     5082 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/auditory.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      429 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/burger.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4396 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/checkbox-off.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4496 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/checkbox-on.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)      815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/close.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.524513 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10402 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/BackboneTaxonomy.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     9239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/FactSheets.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    12414 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Frontend.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/GenericForm.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     5933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Glossary.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     5892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Map.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     7516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/NatureGuide.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    10521 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/TaxonProfiles.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    14005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/template_content.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3524 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/forward-arrow.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     8347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/gear.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)     4042 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/gustatory.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1000 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/lclogo32.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     3745 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/microscope.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     3434 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/olfactory.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    12200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/scalpel.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)    32016 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)    60165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner_huge.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)    13011 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner_old.gif
+-rw-r--r--   0 tom       (1000) tom       (1000)     3763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/tactile.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     4865 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/visual.svg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.524513 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/
+-rw-r--r--   0 tom       (1000) tom       (1000)    73792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/hammer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    86927 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/jquery-3.3.1.min.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6710 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/observatory_admin.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      457 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/polyfills.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    20337 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/popper.min.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.527846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2973 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Control.Draw.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.Draw.Event.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4728 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.draw.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9137 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Toolbar.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3005 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Tooltip.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/copyright.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.527846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2760 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/DrawToolbar.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.527846 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Circle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1063 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.CircleMarker.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2436 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Feature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3193 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Marker.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3279 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polygon.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    17648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polyline.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Rectangle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3273 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.SimpleShape.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.531180 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4605 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/EditToolbar.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.531180 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Circle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.CircleMarker.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Marker.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    13008 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Poly.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3306 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Rectangle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5387 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.SimpleShape.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4184 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Delete.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8232 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Edit.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.531180 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/GeometryUtil.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      757 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LatLngUtil.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      777 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LineUtil.Intersect.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      868 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polygon.Intersect.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3044 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polyline.Intersect.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7446 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/TouchEvents.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.531180 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet-2x.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     4975 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     7165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/leaflet.draw.css
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.534513 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/sortable/
+-rw-r--r--   0 tom       (1000) tom       (1000)    43303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/app_kit/sortable/Sortable.min.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.534513 localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/
+-rw-r--r--   0 tom       (1000) tom       (1000)    57236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/IdentificationMatrix.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    47183 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/IdentificationMatrix_beta.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/crosslink.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1248 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/jquery-searchfornode-autocomplete.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/noimage.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.571181 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/
+-rw-r--r--   0 tom       (1000) tom       (1000)      822 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/AssertionError.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7901 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/CollectionEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      125 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/CollectionEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/CollectionEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3248 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      752 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      511 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Disposable.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Disposable.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      540 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Disposable.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9073 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1652 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1816 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11371 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3779 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5665 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1675 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      430 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2133 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageCanvas.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageState.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageState.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      142 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageState.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      525 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4784 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1519 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      500 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2899 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Kinetic.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1337 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/LICENSE.md
+-rw-r--r--   0 tom       (1000) tom       (1000)    30833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     5845 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    58212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2473 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3156 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      572 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1506 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      838 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEvent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      339 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      933 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      201 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapProperty.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapProperty.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapProperty.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1232 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7563 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ObjectEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ObjectEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ObjectEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11257 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    16432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/README.md
+-rw-r--r--   0 tom       (1000) tom       (1000)     8274 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      499 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileCache.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileCache.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1015 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileCache.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2300 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      655 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2317 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      222 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileState.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileState.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileState.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3909 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      828 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3317 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    42492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     5572 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    72272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewHint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewHint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewHint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      182 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewProperty.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewProperty.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ViewProperty.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      645 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5897 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/asserts.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/asserts.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      304 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/asserts.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      437 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2911 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/centerconstraint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/color.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/color.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5110 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/color.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/colorlike.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      233 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/colorlike.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      800 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/colorlike.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/console.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      212 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/console.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/console.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.577848 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/
+-rw-r--r--   0 tom       (1000) tom       (1000)     6027 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      781 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9375 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      626 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6285 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1313 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8198 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1091 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18591 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      439 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5163 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Rotate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1483 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13760 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      286 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4863 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Zoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      743 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2114 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      309 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2714 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      193 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2124 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/defaults.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      723 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9638 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1017 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12576 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1711 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/css.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/css.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2779 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/css.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.577848 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dist/
+-rw-r--r--   0 tom       (1000) tom       (1000)   748708 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dist/ol.js
+-rw-r--r--   0 tom       (1000) tom       (1000)  4228748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dist/ol.js.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2452 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/easing.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/easing.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/easing.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.587848 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1522 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Event.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Event.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Event.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/EventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/KeyCode.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/KeyCode.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      141 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/KeyCode.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3003 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      612 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2990 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10962 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3855 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3526 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.587848 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent/
+-rw-r--r--   0 tom       (1000) tom       (1000)      256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent/Relationship.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent/Relationship.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      200 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent/Relationship.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    14578 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2724 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    24323 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      824 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5955 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.607849 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3632 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      823 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    17540 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11033 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9633 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      380 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      954 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8828 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2130 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    23660 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    14290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     3668 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    37006 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      245 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML32.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      121 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML32.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10213 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML32.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    12751 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    20323 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    26563 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GPX.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1007 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    15746 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IGC.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3832 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      670 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5305 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1615 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    93722 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      608 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11879 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OSMXML.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OSMXML.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5027 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OSMXML.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      115 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OWS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OWS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8683 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OWS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6011 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1042 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9920 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4959 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1000 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5165 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      623 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13534 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9753 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1575 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    43118 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4997 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    25384 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1084 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    21719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKT.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      309 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      185 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18326 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      383 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      308 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      671 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XML.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      242 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XML.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XML.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6403 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1346 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7814 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.614516 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/
+-rw-r--r--   0 tom       (1000) tom       (1000)      404 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/And.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      139 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/And.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      429 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/And.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      903 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      209 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      631 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      940 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      683 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      191 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      660 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Contains.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      966 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      689 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      191 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      666 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      639 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/During.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      570 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      603 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      226 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      571 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Filter.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      481 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      693 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      195 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      672 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      690 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      251 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1451 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      155 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsNull.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      469 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThan.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      505 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      261 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      774 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      477 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Not.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Not.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      449 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Not.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      582 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      196 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      599 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      393 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Or.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      136 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Or.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Or.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      345 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ResourceId.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1060 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      651 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Within.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9716 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10032 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8846 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/readme.md
+-rw-r--r--   0 tom       (1000) tom       (1000)      171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xlink.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      150 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xlink.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      290 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xlink.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2396 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3802 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1012 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)       99 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      972 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1132 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/functions.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      284 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/functions.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/functions.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.617849 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2294 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8576 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Circle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1449 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2020 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9203 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4585 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      892 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8304 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      510 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4679 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LinearRing.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      856 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1898 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5315 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1024 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12366 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      261 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3052 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Point.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1305 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3606 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      971 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.627850 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1581 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/area.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/center.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/center.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/center.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3731 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      964 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1712 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3487 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2002 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2609 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      206 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      873 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/flip.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1677 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      469 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5891 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1902 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      524 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2526 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1697 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      515 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2424 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5052 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      283 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/length.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1889 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3946 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      729 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6162 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      353 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      187 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      889 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      964 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/segments.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6174 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      575 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      234 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1355 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      417 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/topology.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/topology.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/topology.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3731 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      726 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/has.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/has.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/has.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/index.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/index.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1416 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/index.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.641183 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/
+-rw-r--r--   0 tom       (1000) tom       (1000)      929 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1777 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5948 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1390 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8674 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7979 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2243 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      369 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5507 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragPan.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3238 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2262 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      252 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2586 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    20613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     3102 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    60848 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6825 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1397 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    16223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5470 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1090 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5012 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2531 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      302 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4051 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      613 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9593 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    19642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2464 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    52422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7644 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      333 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      978 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      272 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3263 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6229 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6621 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Property.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Property.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Property.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    15835 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2036 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8026 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    20211 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    10173 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      216 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/defaults.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1502 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      109 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1451 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.647850 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/
+-rw-r--r--   0 tom       (1000) tom       (1000)    11607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1896 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11672 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4914 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      257 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2648 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseImage.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8297 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9666 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      957 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    18432 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1998 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    37037 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5629 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1177 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1067 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Image.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    14105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2316 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    15058 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    14310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      461 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9688 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Property.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      103 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Property.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      319 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Property.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1179 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      987 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Tile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/TileProperty.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      111 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/TileProperty.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      166 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/TileProperty.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1229 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Vector.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8265 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      375 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4741 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorImage.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    14538 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10171 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6068 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      471 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4643 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8303 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    17569 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      739 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      709 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2264 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/loadingstrategy.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3817 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      876 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5400 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1544 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/net.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      409 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/net.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3603 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/net.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      388 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/obj.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      161 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/obj.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/obj.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6217 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ol.css
+-rw-r--r--   0 tom       (1000) tom       (1000)      817 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/package.json
+-rw-r--r--   0 tom       (1000) tom       (1000)      455 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pixel.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pixel.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pixel.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.647850 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pointer/
+-rw-r--r--   0 tom       (1000) tom       (1000)      344 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pointer/EventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      105 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pointer/EventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      359 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/pointer/EventType.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.651184 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/
+-rw-r--r--   0 tom       (1000) tom       (1000)     8986 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1297 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8017 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      921 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      338 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1040 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Units.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1598 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      514 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3363 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      579 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg4326.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2019 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4219 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/proj4.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      611 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      775 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/projections.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1649 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      435 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2237 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/transforms.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    16859 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    27310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.654517 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1408 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Box.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      488 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Box.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2992 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Box.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1690 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Event.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      319 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Event.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1458 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Event.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      411 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/EventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      178 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/EventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1606 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/EventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1592 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4053 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.661184 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5941 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1658 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    19002 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1493 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      466 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2834 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9269 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1944 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    40772 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5116 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1058 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12379 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1958 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      548 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    10208 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    34441 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      298 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      742 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4871 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      527 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      176 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8194 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2706 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      748 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18880 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1694 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      419 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11093 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1951 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13928 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.661184 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7094 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1021 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      234 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3808 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    13641 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    15253 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      901 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      223 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3210 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      984 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      225 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3956 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1507 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      170 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/constants.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4610 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      718 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12100 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4667 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      584 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4979 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.664517 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/
+-rw-r--r--   0 tom       (1000) tom       (1000)      609 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      252 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4045 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Composite.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5106 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1202 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5533 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4435 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7392 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.667851 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/
+-rw-r--r--   0 tom       (1000) tom       (1000)      968 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      329 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7381 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1151 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9121 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6146 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    23698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1405 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      431 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6481 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1093 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    23555 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3907 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      863 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    27833 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    16654 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.671184 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      774 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7123 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11421 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1431 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    24796 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1056 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    27112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5373 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1306 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      423 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6336 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.674518 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4422 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      837 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14292 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5963 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3377 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      807 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9619 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    15737 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      221 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/common.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      144 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/common.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      184 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/common.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      721 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14062 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2117 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      415 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/resolutionconstraint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      853 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      413 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/rotationconstraint.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1406 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/size.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      300 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/size.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1637 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/size.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.694519 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/
+-rw-r--r--   0 tom       (1000) tom       (1000)     7571 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      916 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10022 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      624 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5872 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7341 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1046 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9197 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8712 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1158 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12993 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    13175 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1097 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    31154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3440 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12907 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/IIIF.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1568 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7914 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      934 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     9476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6089 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      653 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4801 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6667 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1018 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8287 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      574 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5366 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1160 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14056 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5235 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3934 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5635 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      386 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4311 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4523 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3476 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OSM.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    15270 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2699 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    29965 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1276 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6064 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3520 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      256 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4240 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Stamen.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11482 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2520 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8516 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      517 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8601 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2120 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      224 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2504 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileDebug.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      282 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      150 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      906 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    10583 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      993 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14744 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7350 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      555 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11918 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    15573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8254 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6034 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6607 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    30310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     3930 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    38214 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      492 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      204 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1574 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      961 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18992 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    11081 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18733 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8389 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      371 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/XYZ.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     7798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      596 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    10426 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      164 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/common.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/common.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      131 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/common.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4415 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11348 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      659 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/wms.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      188 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/wms.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      641 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/wms.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2913 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      288 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3368 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3784 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/sphere.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      482 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/sphere.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8922 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/sphere.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      682 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/string.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      243 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/string.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1190 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/string.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.694519 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3770 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1014 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6273 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2903 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5202 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3207 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      790 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6347 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3573 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      875 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5157 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.704519 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2614 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2604 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Circle.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1806 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      404 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1465 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Fill.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    10407 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1280 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    16310 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3730 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1069 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     7080 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1928 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6143 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1604 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6025 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     8242 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    17260 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5450 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1135 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4957 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    12707 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2067 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14567 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    16582 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2676 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    14673 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    13072 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1112 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    33262 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    27824 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1036 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    17715 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2328 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/literal.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/literal.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2092 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/literal.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      532 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)       97 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1932 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      491 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2282 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilecoord.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.704519 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/
+-rw-r--r--   0 tom       (1000) tom       (1000)    16618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2245 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    22965 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6106 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      445 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     6718 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      275 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/common.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      178 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/common.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      236 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/common.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     4352 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      550 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     5910 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1550 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      556 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3887 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     6147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      971 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     8826 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      414 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/uri.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      153 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/uri.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      841 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/uri.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      618 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/util.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      210 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/util.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      772 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/util.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.704519 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/
+-rw-r--r--   0 tom       (1000) tom       (1000)      549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      241 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      673 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/mat4.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.711186 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/
+-rw-r--r--   0 tom       (1000) tom       (1000)     3149 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      580 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     3538 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      154 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      119 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)      156 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ContextEventType.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    22048 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2719 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    35286 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.js
+-rw-r--r--   0 tom       (1000) tom       (1000)      617 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      277 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     1181 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     5700 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      813 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    11869 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     2840 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     4503 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     9815 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     1420 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18508 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     3147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      734 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    12983 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.js
+-rw-r--r--   0 tom       (1000) tom       (1000)     1874 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      531 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)     2818 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.711186 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/worker/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/worker/webgl.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)      107 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/worker/webgl.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    13749 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/worker/webgl.js
+-rw-r--r--   0 tom       (1000) tom       (1000)    13680 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.d.ts
+-rw-r--r--   0 tom       (1000) tom       (1000)     2033 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.d.ts.map
+-rw-r--r--   0 tom       (1000) tom       (1000)    18289 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.js
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.711186 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.714519 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1108 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/add_existing_generic_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      325 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/add_feature_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3139 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/app_card.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      460 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/app_limit_reached.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      364 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/build_errors.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      336 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/build_warnings.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      854 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/change_generic_content_status.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2589 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/component_card.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      296 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/content_image_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      179 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/content_image_with_text_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3001 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/create_generic_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      246 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/delete_app_language.html
+-rw-r--r--   0 tom       (1000) tom       (1000)       72 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/delete_content_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      747 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/delete_localized_content_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      765 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/edit_generic_content_name.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/form_extended_with_content_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1087 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/get_content_image_suggestions.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      479 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/get_translation.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1332 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/localized_content_image_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1361 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/manage_app_languages.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1792 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/manage_feature.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      485 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/mockbutton.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      715 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/options_form.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      215 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/reload_appbar.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      311 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/remove_app_generic_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      827 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/tag_any_element.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      189 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/tags.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      764 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/translate_app_pagination.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      101 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/upload_theme_image.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     4569 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/zip_import.html
+-rw-r--r--   0 tom       (1000) tom       (1000)    15798 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)    13642 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/build_app.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      164 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/content_images.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/home.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.714519 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/legal/
+-rw-r--r--   0 tom       (1000) tom       (1000)      551 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/legal/legal_notice.html
+-rw-r--r--   0 tom       (1000) tom       (1000)    25354 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/legal/privacy_statement.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      789 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/list_manage_apps.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      751 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/list_manage_generic_content.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2960 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/manage_app.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      374 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/manage_app_design.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     3987 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/manage_generic_content.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.714519 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/snippets/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1394 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/snippets/ckeditor_js_snippet.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      835 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/start_new_app.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     6172 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/translate_app.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.714519 localcosmos_app_kit-0.2.3/app_kit/templatetags/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templatetags/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7029 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/templatetags/app_tags.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.717853 localcosmos_app_kit-0.2.3/app_kit/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.411176 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.717853 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.717853 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/
+-rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/settings.json
+-rw-r--r--   0 tom       (1000) tom       (1000)      678 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain.zip
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.717853 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/
+-rw-r--r--   0 tom       (1000) tom       (1000)      564 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/settings.json
+-rw-r--r--   0 tom       (1000) tom       (1000)      816 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain.zip
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.721186 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)    78900 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/Leaf-large.jpg
+-rw-r--r--   0 tom       (1000) tom       (1000)    49349 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/Leaf.jpg
+-rw-r--r--   0 tom       (1000) tom       (1000)   274763 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/app-background.jpg
+-rw-r--r--   0 tom       (1000) tom       (1000)   409549 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/localcosmos-logo.svg
+-rw-r--r--   0 tom       (1000) tom       (1000)   156278 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/test-image-2560-1440.jpg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/ipa_for_tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)    78900 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/ipa_for_tests/TestApp.ipa
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/templates/
+-rw-r--r--   0 tom       (1000) tom       (1000)      147 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/templates/neobiota.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     2693 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/cases.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    12293 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    17134 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    20463 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/test_forms.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    48598 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/test_models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    81265 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      511 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2096 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      698 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/validators.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1399 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/view_mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    53553 2024-04-05 12:28:54.000000 localcosmos_app_kit-0.2.3/app_kit/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1170 2024-04-23 06:44:28.000000 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)    90617 2024-04-23 06:44:28.000000 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-23 06:44:28.000000 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      248 2024-04-23 06:44:28.000000 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        8 2024-04-23 06:44:28.000000 localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-23 06:44:28.724520 localcosmos_app_kit-0.2.3/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)     1275 2024-04-23 06:44:02.000000 localcosmos_app_kit-0.2.3/setup.py
```

### Comparing `localcosmos_app_kit-0.2.2/LICENCE` & `localcosmos_app_kit-0.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/MANIFEST.in` & `localcosmos_app_kit-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/PKG-INFO` & `localcosmos_app_kit-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit
-Version: 0.2.2
+Version: 0.2.3
 Summary: LocalCosmos App Kit. Web Portal to build Android and iOS apps
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity
 Platform: OS Independent
```

### Comparing `localcosmos_app_kit-0.2.2/app_kit/admin_urls.py` & `localcosmos_app_kit-0.2.3/app_kit/admin_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/models.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/serializers.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/serializers.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/mixins.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/test_serializers.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/app_kit_api/views.py` & `localcosmos_app_kit-0.2.3/app_kit/app_kit_api/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppBuilderBase.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppBuilderBase.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppPreviewBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppPreviewBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/AppReleaseBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/AppReleaseBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/ContentImageBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/ContentImageBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/GBIFlib.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/GBIFlib.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/BackboneTaxonomyJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/BackboneTaxonomyJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/ButtonMatrixJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/ButtonMatrixJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/FrontendJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/FrontendJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/GenericFormJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/GenericFormJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/GlossaryJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/GlossaryJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/JSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/JSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/MapJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/MapJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/NatureGuideJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/NatureGuideJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/TaxonProfilesJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/TaxonProfilesJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/JSONBuilders/TemplateContentJSONBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/JSONBuilders/TemplateContentJSONBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/precompile_fulltree.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/precompile_fulltree.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_ContentImageBuilder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_ContentImageBuilder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_builder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_builder_base.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_builder_base.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_preview_builder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_preview_builder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/appbuilder/tests/test_release_builder.py` & `localcosmos_app_kit-0.2.3/app_kit/appbuilder/tests/test_release_builder.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/add_taxon_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/add_taxon_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbone_taxa_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbone_taxa_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbonetaxonomy.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_backbonetaxonomy.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_fulltree_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/manage_fulltree_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/remove_backbone_taxon.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/remove_backbone_taxon.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/taxonlist.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/taxonlist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget_search_only.html` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/templates/backbonetaxonomy/widgets/backbone_taxon_autocomplete_widget_search_only.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/backbonetaxonomy/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/backbonetaxonomy/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/buttonmatrix_button.html` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/buttonmatrix_button.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/delete_buttonmatrix_element.html` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/delete_buttonmatrix_element.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_button.html` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_button.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_buttonmatrix.html` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templates/buttonmatrix/manage_buttonmatrix.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/templatetags/buttonmatrix_tags.py` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/templatetags/buttonmatrix_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/buttonmatrix/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/buttonmatrix/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/PrivateFrontendImporter.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/PrivateFrontendImporter.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/change_frontend.html` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/change_frontend.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/install_private_frontend.html` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/install_private_frontend.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/manage_frontend_settings.html` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/manage_frontend_settings.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/ajax/upload_private_frontend.html` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/ajax/upload_private_frontend.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/templates/frontend/manage_frontend.html` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/templates/frontend/manage_frontend.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/mixins.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_PrivateFrontendImporter.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_PrivateFrontendImporter.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/frontend/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/frontend/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/static/generic_forms/datePicker.js` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/static/generic_forms/datePicker.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_field.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_value.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/delete_generic_value.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field_choices.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/ajax/manage_generic_field_choices.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/generic_field.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/generic_field.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/generic_field_modify.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/generic_field_modify.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templates/generic_forms/manage_generic_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templates/generic_forms/manage_generic_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/templatetags/genericforms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/templatetags/genericforms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_templatetags_old.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_templatetags_old.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/generic_forms/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/generic_forms/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/migrations/0002_auto_20201207_1328.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/migrations/0002_auto_20201207_1328.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/add_glossary_entry_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/glossary_entries.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/glossary_entries.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/glossary_entry.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/glossary_entry.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/ajax/manage_glossary_entry.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/ajax/manage_glossary_entry.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/templates/glossary/manage_glossary.html` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/templates/glossary/manage_glossary.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/glossary/zip_import.py` & `localcosmos_app_kit-0.2.3/app_kit/features/glossary/zip_import.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/migrations/0002_maptaxonomicfilter_filtertaxon.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/migrations/0002_maptaxonomicfilter_filtertaxon.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/manage_project_area.html` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/manage_project_area.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/manage_taxonomic_filter.html` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/manage_taxonomic_filter.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/ajax/taxonomic_filters.html` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/ajax/taxonomic_filters.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/templates/maps/manage_maps.html` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/templates/maps/manage_maps.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/mixins.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/maps/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/maps/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/definitions.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/definitions.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/fields.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/fields.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filter_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filter_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filter_space_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filter_space_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/matrix_filters.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/matrix_filters.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0002_auto_20201013_0901.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0002_auto_20201013_0901.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0003_matrixfilterrestriction.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0003_matrixfilterrestriction.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/migrations/0007_auto_20221110_0613.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/migrations/0007_auto_20221110_0613.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes_page.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_existing_nodes_page.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/add_keynodes_menu.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/add_keynodes_menu.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/copy_tree_branch.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/copy_tree_branch.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_color_filter_space.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_color_filter_space.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_restrictions.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_restrictions.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_space.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_matrix_filter_space.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_nodelink_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_nodelink_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_overview_image.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/manage_overview_image.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/matrix_filters.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/matrix_filters.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/move_natureguide_node.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/move_natureguide_node.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node_small.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/natureguide_node_small.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/node_loader.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/node_loader.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/node_management_menu.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/node_management_menu.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/ajax/nodelist.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/ajax/nodelist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/manage_nature_guide.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/manage_nature_guide.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/node_analysis.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/node_analysis.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/nodemenu_loader.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/nodemenu_loader.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_colors_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_colors_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_description_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_description_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_numbers_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_numbers_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_range_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_range_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/define_text_description_widget.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/define_text_description_widget.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/grid_choices.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/grid_choices.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/horizontal_choices.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/horizontal_choices.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/range.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/range.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_colors.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_colors.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_numbers.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_numbers.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_patterns.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_patterns.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_taxonfilters.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/select_multiple_taxonfilters.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_colors.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_colors.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_numbers.html` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/templates/nature_guides/widgets/slider_select_multiple_numbers.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/common.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/common.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_matrix_filters.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_matrix_filters.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/widgets.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/widgets.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/nature_guides/zip_import.py` & `localcosmos_app_kit-0.2.3/app_kit/features/nature_guides/zip_import.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/migrations/0005_taxonprofile_tags.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/migrations/0005_taxonprofile_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/batch_change_taxon_profiles_publication_status.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/batch_change_taxon_profiles_publication_status.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/change_taxon_profile_publication_status.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/change_taxon_profile_publication_status.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_images.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_images.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_traits.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/collected_taxon_traits.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/create_taxon_profile.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/create_taxon_profile.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_profile.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_text_type.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/delete_taxon_text_type.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_form.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_image.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_taxon_profile_image.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_type.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_type.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_types_order.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/manage_text_types_order.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/nature_guide_taxonlist.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/nature_guide_taxonlist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/non_nature_guide_taxonlist.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/non_nature_guide_taxonlist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/taxonlist.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/ajax/taxonlist.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profile.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profile.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profiles.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_profiles.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_texts.html` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templates/taxon_profiles/manage_taxon_texts.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/templatetags/taxon_profile_tags.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/templatetags/taxon_profile_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/urls.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/views.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -702,17 +702,21 @@
         self.taxon = LazyTaxon(instance=taxon_profile)
 
 
     def get_taxon_traits(self):
 
         spaces = []
         
-        nodes = NatureGuidesTaxonTree.objects.filter(meta_node__taxon_source=self.taxon.taxon_source,
-                meta_node__taxon_latname=self.taxon.taxon_latname,
-                meta_node__taxon_author=self.taxon.taxon_author)
+        # sometimes taxon_athor=None is stored as taxon_author='' for unknown reasons
+        # as a tresult, this query fails for taxa without author
+        #nodes = NatureGuidesTaxonTree.objects.filter(meta_node__taxon_source=self.taxon.taxon_source,
+        #        meta_node__taxon_latname=self.taxon.taxon_latname,
+        #        meta_node__taxon_author=self.taxon.taxon_author)
+
+        nodes = NatureGuidesTaxonTree.objects.filter(meta_node__name_uuid=self.taxon.name_uuid)
         
         node_spaces = NodeFilterSpace.objects.filter(node__in=nodes)
 
         spaces += list(node_spaces)
 
         for node in nodes:
```

### Comparing `localcosmos_app_kit-0.2.2/app_kit/features/taxon_profiles/zip_import.py` & `localcosmos_app_kit-0.2.3/app_kit/features/taxon_profiles/zip_import.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/generic.py` & `localcosmos_app_kit-0.2.3/app_kit/generic.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/generic_content_validation.py` & `localcosmos_app_kit-0.2.3/app_kit/generic_content_validation.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/generic_content_zip_import.py` & `localcosmos_app_kit-0.2.3/app_kit/generic_content_zip_import.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/global_urls.py` & `localcosmos_app_kit-0.2.3/app_kit/global_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/locale/de/LC_MESSAGES/django.mo` & `localcosmos_app_kit-0.2.3/app_kit/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/locale/de/LC_MESSAGES/django.po` & `localcosmos_app_kit-0.2.3/app_kit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/locale/en/LC_MESSAGES/django.po` & `localcosmos_app_kit-0.2.3/app_kit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/middleware.py` & `localcosmos_app_kit-0.2.3/app_kit/middleware.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/migrations/0003_auto_20220520_0640.py` & `localcosmos_app_kit-0.2.3/app_kit/migrations/0003_auto_20220520_0640.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/migrations/0004_auto_20220608_0717.py` & `localcosmos_app_kit-0.2.3/app_kit/migrations/0004_auto_20220608_0717.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/models.py` & `localcosmos_app_kit-0.2.3/app_kit/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/forms.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/management/commands/fix_staging_domains.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/management/commands/fix_staging_domains.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/middleware.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/middleware.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/migrations/0001_initial.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/models.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext_lazy as _
+from django.urls import reverse
 
 from django_tenants.models import TenantMixin, DomainMixin
 
 from localcosmos_server.models import App
 
 from django_tenants.utils import tenant_context
```

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/public_schema_urls.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/public_schema_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/setup_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/setup_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/setup_views.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/setup_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/contact_us.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/contact_us.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/delete_account.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/delete_account.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/edit_account.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/edit_account.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/my_account.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/my_account.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/localcosmos/setup/setup_initial_appkit.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/localcosmos/setup/setup_initial_appkit.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/templates/multi_tenancy/list_app_kits.html` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/templates/multi_tenancy/list_app_kits.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/tenant_schema_urls.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/tenant_schema_urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/utils.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/multi_tenancy/views.py` & `localcosmos_app_kit-0.2.3/app_kit/multi_tenancy/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/permission_rules.py` & `localcosmos_app_kit-0.2.3/app_kit/permission_rules.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/server_side_cursors.py` & `localcosmos_app_kit-0.2.3/app_kit/server_side_cursors.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/anycluster/openlayers/anycluster-openlayers.js` & `localcosmos_app_kit-0.2.3/app_kit/static/anycluster/openlayers/anycluster-openlayers.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/anycluster/openlayers/anycluster-openlayers.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/anycluster/openlayers/anycluster-openlayers.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ButtonMatrix.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ButtonMatrix.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/bootstrap-4.3.1-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/Alphabetfilter.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/Alphabetfilter.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/album.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/album.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/camera.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/camera.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/observation.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/observation.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/occurrence.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/occurrence.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxon_detail.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxon_detail.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Amphibia.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Amphibia.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Animalia.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Animalia.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Anura.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Anura.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Arachnida.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Arachnida.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Arthropoda.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Arthropoda.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Aves.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Aves.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Chordata.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Chordata.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Coleoptera.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Coleoptera.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Customfilter.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Customfilter.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Fungi.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Fungi.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Holocephali,Elasmobranchii,Sarcopterygii,Actinopterygii.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Insecta.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Insecta.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Lepidoptera.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Lepidoptera.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Mammalia.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Mammalia.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Mollusca.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Mollusca.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Odonata.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Odonata.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/Plantae.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/Plantae.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/taxonfilters/no_filter.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/taxonfilters/no_filter.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/buttons/wikipedia_button.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/buttons/wikipedia_button.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/LICENSE.md` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/README.md` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/README.md`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/ckeditor.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/ckeditor.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/ckeditor.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/ckeditor.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ar.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ast.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ast.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/az.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/az.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/cs.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/cs.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/da.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/da.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/de.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/de.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/el.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/el.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/en-au.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/en-au.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/en-gb.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/en-gb.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/es.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/es.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/et.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/et.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/eu.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/eu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fa.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fa.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fi.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/fr.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/fr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/gl.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/gl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/he.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/he.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hi.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hr.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/hu.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/hu.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/id.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/id.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/it.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/it.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ja.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ja.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/km.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/km.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/kn.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/kn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ko.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ko.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ku.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ku.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/lt.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/lt.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/lv.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/lv.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/nb.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/nb.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ne.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ne.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/nl.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/nl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/no.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/no.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/pl.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/pl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/pt-br.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/pt-br.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ro.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ro.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ru.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ru.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sk.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sq.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sq.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sr-latn.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sr-latn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sr.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/sv.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/sv.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/tk.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/tk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/tr.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/tr.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/ug.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/ug.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/uk.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/uk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/vi.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/vi.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/zh-cn.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/zh-cn.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/build/translations/zh.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/build/translations/zh.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/package.json` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/package.json`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/sample/index.html` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/sample/index.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/sample/styles.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/sample/styles.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/src/ckeditor.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/src/ckeditor.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/ckeditor5/webpack.config.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/ckeditor5/webpack.config.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/css/app.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/css/app.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/css/app_kit.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/css/app_kit.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/handlebars-v4.0.10.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/handlebars-v4.0.10.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/horizontal-slide/horizontal-slide.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/horizontal-slide/horizontal-slide.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/horizontal-slide/horizontal-slide.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/horizontal-slide/horizontal-slide.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/add_element.png` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/add_element.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/auditory.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/auditory.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/checkbox-off.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/checkbox-off.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/checkbox-on.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/checkbox-on.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/close.png` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/close.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/BackboneTaxonomy.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/BackboneTaxonomy.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/FactSheets.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/FactSheets.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Frontend.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Frontend.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/GenericForm.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/GenericForm.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Glossary.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Glossary.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/Map.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/Map.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/NatureGuide.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/NatureGuide.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/TaxonProfiles.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/TaxonProfiles.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/features/template_content.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/features/template_content.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/forward-arrow.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/forward-arrow.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/gear.gif` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/gear.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/gustatory.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/gustatory.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/lclogo32.png` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/lclogo32.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/microscope.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/microscope.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/olfactory.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/olfactory.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/scalpel.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/scalpel.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner.gif` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner_huge.gif` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner_huge.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/spinner_old.gif` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/spinner_old.gif`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/tactile.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/tactile.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/images/visual.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/images/visual.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/hammer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/hammer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/jquery-3.3.1.min.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/observatory_admin.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/observatory_admin.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/js/popper.min.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Control.Draw.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Control.Draw.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.Draw.Event.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.Draw.Event.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.draw.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Leaflet.draw.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Toolbar.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Toolbar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/Tooltip.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/Tooltip.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/DrawToolbar.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/DrawToolbar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Circle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Circle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.CircleMarker.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.CircleMarker.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Feature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Feature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Marker.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Marker.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polygon.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polygon.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polyline.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Polyline.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Rectangle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.Rectangle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.SimpleShape.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/draw/handler/Draw.SimpleShape.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/EditToolbar.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/EditToolbar.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Circle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Circle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.CircleMarker.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.CircleMarker.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Marker.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Marker.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Poly.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Poly.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Rectangle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.Rectangle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.SimpleShape.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/Edit.SimpleShape.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Delete.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Delete.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Edit.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/edit/handler/EditToolbar.Edit.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/GeometryUtil.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/GeometryUtil.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LatLngUtil.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LatLngUtil.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LineUtil.Intersect.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/LineUtil.Intersect.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polygon.Intersect.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polygon.Intersect.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polyline.Intersect.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/Polyline.Intersect.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/TouchEvents.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/ext/TouchEvents.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet-2x.png` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet-2x.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.png` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/images/spritesheet.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/maps/Leaflet.draw/src/leaflet.draw.css` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/maps/Leaflet.draw/src/leaflet.draw.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/app_kit/sortable/Sortable.min.js` & `localcosmos_app_kit-0.2.3/app_kit/static/app_kit/sortable/Sortable.min.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/IdentificationMatrix.js` & `localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/IdentificationMatrix.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/IdentificationMatrix_beta.js` & `localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/IdentificationMatrix_beta.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/crosslink.svg` & `localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/crosslink.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/nature_guides/jquery-searchfornode-autocomplete.js` & `localcosmos_app_kit-0.2.3/app_kit/static/nature_guides/jquery-searchfornode-autocomplete.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/noimage.png` & `localcosmos_app_kit-0.2.3/app_kit/static/noimage.png`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/AssertionError.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/AssertionError.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/AssertionError.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Collection.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Collection.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/DataTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/DataTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Disposable.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Disposable.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Feature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Feature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Geolocation.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Geolocation.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Image.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Image.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageBase.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageBase.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageCanvas.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageCanvas.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageCanvas.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ImageTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ImageTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Kinetic.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Kinetic.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Kinetic.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/LICENSE.md` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Map.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Map.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEvent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventHandler.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapBrowserEventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEvent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEvent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEvent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/MapEventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/MapEventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Object.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Object.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Observable.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Observable.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Overlay.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Overlay.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/README.md` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/Tile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/Tile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileCache.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileCache.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileQueue.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileQueue.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/TileRange.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/TileRange.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorRenderTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorRenderTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/VectorTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/VectorTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/View.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/View.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/array.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/array.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/centerconstraint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/centerconstraint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/centerconstraint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/color.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/color.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/color.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/color.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/colorlike.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/colorlike.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/colorlike.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/colorlike.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/console.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/console.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/console.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/console.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Attribution.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Attribution.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Control.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Control.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/FullScreen.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/FullScreen.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/MousePosition.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/MousePosition.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/OverviewMap.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/OverviewMap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Rotate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Rotate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Rotate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ScaleLine.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ScaleLine.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Zoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/Zoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/Zoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomSlider.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/ZoomToExtent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/defaults.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control/defaults.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control/defaults.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/control.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/control.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/coordinate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/coordinate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/css.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/css.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/css.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/css.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dist/ol.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dist/ol.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dist/ol.js.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dist/ol.js.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/dom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/dom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/easing.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/easing.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/easing.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/easing.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Event.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Event.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Event.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Event.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/EventType.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/EventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/EventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/Target.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/Target.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events/condition.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events/condition.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/events.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/events.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/extent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/extent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/featureloader.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/featureloader.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/EsriJSON.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/EsriJSON.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Feature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Feature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML2.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML2.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML3.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML3.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GML32.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GML32.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GMLBase.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GMLBase.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GPX.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GPX.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GPX.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/GeoJSON.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/GeoJSON.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IGC.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IGC.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IGC.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/IIIFInfo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/JSONFeature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/JSONFeature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/KML.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/KML.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/MVT.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/MVT.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OSMXML.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OSMXML.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/OWS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/OWS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/Polyline.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/Polyline.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TextFeature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TextFeature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/TopoJSON.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/TopoJSON.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WFS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WFS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKB.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKB.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKT.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WKT.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WKT.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSCapabilities.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMSGetFeatureInfo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/WMTSCapabilities.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XML.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XML.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XML.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XML.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/XMLFeature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/XMLFeature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Bbox.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Comparison.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/ComparisonBinary.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Contains.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Contains.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Contains.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/DWithin.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Disjoint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/During.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/During.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/During.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/EqualTo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Filter.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Filter.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Filter.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThan.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/GreaterThanOrEqualTo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Intersects.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsBetween.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/IsLike.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LessThanOrEqualTo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/LogicalNary.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/NotEqualTo.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Spatial.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Within.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter/Within.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter/Within.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/filter.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/filter.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/readme.md` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/readme.md`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format/xsd.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format/xsd.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/format.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/format.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/functions.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/functions.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/functions.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/functions.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Circle.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Circle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Circle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Geometry.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Geometry.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/GeometryCollection.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LineString.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LineString.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LinearRing.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/LinearRing.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/LinearRing.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiLineString.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPoint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/MultiPolygon.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Point.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Point.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Point.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/Polygon.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/Polygon.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/SimpleGeometry.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/area.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/area.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/area.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/center.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/center.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/closest.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/closest.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/contains.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/contains.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/deflate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/flip.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/flip.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/flip.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/geodesic.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/inflate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interiorpoint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/interpolate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/intersectsextent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/length.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/length.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/length.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/linechunk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/orient.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/orient.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/reverse.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/segments.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/segments.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/segments.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/simplify.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/straightchunk.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/textpath.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/topology.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/topology.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom/flat/transform.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom/flat/transform.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/geom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/geom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/has.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/has.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/has.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/has.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/index.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/index.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/index.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/index.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DoubleClickZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragAndDrop.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragBox.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragBox.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragPan.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragPan.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragPan.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragRotateAndZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/DragZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Draw.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Draw.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Extent.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Extent.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Interaction.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Interaction.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardPan.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/KeyboardZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Link.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Link.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Modify.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Modify.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/MouseWheelZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchRotate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/PinchZoom.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Pointer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Pointer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Select.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Select.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Snap.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Snap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/Translate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/Translate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/defaults.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction/defaults.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction/defaults.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/interaction.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/interaction.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Base.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Base.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseImage.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseImage.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseImage.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/BaseVector.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/BaseVector.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Graticule.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Graticule.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Group.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Group.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Heatmap.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Heatmap.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Image.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Image.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Image.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Layer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Layer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/MapboxVector.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Tile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Tile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Tile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Vector.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/Vector.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/Vector.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorImage.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorImage.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorImage.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/VectorTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/VectorTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLPoints.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer/WebGLTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/layer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/layer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/loadingstrategy.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/loadingstrategy.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/loadingstrategy.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/math.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/math.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/net.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/net.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/net.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/net.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/ol.css` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/ol.css`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/package.json` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/package.json`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Projection.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Projection.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Units.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/Units.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/Units.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg3857.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg3857.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg4326.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/epsg4326.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/epsg4326.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/proj4.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/proj4.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/proj4.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/projections.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/projections.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/projections.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/transforms.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj/transforms.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj/transforms.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/proj.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/proj.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Box.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Box.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Box.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Box.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Event.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Event.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Event.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Event.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/EventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/EventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/Feature.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/Feature.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/VectorContext.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/VectorContext.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Builder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/BuilderGroup.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Executor.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ExecutorGroup.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/ImageBuilder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Immediate.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/Instruction.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/LineStringBuilder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/PolygonBuilder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/TextBuilder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas/hitdetect.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/canvas.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/canvas.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/BatchRenderer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/LineStringBatchRenderer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/MixedGeometryBatch.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PointBatchRenderer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/PolygonBatchRenderer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/constants.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/constants.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/constants.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render/webgl/utils.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render/webgl/utils.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/render.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/render.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Composite.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Composite.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Composite.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Layer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Layer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/Map.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/Map.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/ImageLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/Layer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/TileLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorImageLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/canvas/VectorTileLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/vector.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/vector.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/Layer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/PointsLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/TileLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/VectorLayer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/renderer/webgl/shaders.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/DataTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/DataTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Image.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Image.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Tile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Tile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj/Triangulation.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/reproj.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/reproj.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/resolutionconstraint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/resolutionconstraint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/resolutionconstraint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/rotationconstraint.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/rotationconstraint.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/rotationconstraint.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/size.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/size.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/size.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/size.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/BingMaps.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/BingMaps.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/CartoDB.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/CartoDB.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Cluster.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Cluster.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/DataTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/DataTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/GeoTIFF.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/IIIF.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/IIIF.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/IIIF.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Image.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Image.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageArcGISRest.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageCanvas.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageMapGuide.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageStatic.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageStatic.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ImageWMS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ImageWMS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCMapTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OGCVectorTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OSM.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/OSM.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/OSM.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Raster.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Raster.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Source.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Source.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Stamen.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Stamen.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Stamen.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Tile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Tile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileArcGISRest.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileDebug.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileDebug.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileDebug.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileEventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileEventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileImage.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileImage.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileJSON.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileJSON.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/TileWMS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/TileWMS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UTFGrid.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UTFGrid.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/UrlTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/UrlTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Vector.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Vector.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorEventType.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorEventType.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/VectorTile.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/VectorTile.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/WMTS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/WMTS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/XYZ.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/XYZ.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/XYZ.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/Zoomify.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/Zoomify.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/ogcTileUtil.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/wms.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/wms.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source/wms.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source/wms.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/source.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/source.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/sphere.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/sphere.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/sphere.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/sphere.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/string.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/string.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/string.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/string.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LRUCache.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LRUCache.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/LinkedList.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/LinkedList.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/PriorityQueue.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/structs/RBush.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/structs/RBush.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Circle.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Circle.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Circle.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Fill.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Fill.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Fill.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Icon.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Icon.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImage.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImage.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/IconImageCache.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/IconImageCache.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Image.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Image.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/RegularShape.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/RegularShape.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Stroke.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Stroke.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Style.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Style.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/Text.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/Text.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/expressions.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/expressions.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/flat.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/flat.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/literal.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/literal.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style/literal.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style/literal.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/style.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/style.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilecoord.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilecoord.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilecoord.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/TileGrid.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid/WMTS.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tilegrid.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tilegrid.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/tileurlfunction.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/tileurlfunction.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/transform.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/transform.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/uri.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/uri.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/util.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/util.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/util.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/util.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/mat4.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/vec/mat4.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/vec/mat4.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Buffer.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Buffer.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/Helper.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/Helper.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PaletteTexture.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/PostProcessingPass.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/RenderTarget.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/ShaderBuilder.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl/TileTexture.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/webgl.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/webgl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/worker/webgl.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/worker/webgl.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.d.ts` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.d.ts`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.d.ts.map` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.d.ts.map`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/static/openlayers/v7.3.0/xml.js` & `localcosmos_app_kit-0.2.3/app_kit/static/openlayers/v7.3.0/xml.js`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/add_existing_generic_content.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/add_existing_generic_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/app_card.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/app_card.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/change_generic_content_status.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/change_generic_content_status.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/component_card.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/component_card.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/create_generic_content.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/create_generic_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/delete_localized_content_image.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/delete_localized_content_image.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/edit_generic_content_name.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/edit_generic_content_name.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/get_content_image_suggestions.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/get_content_image_suggestions.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/localized_content_image_form.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/localized_content_image_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/manage_app_languages.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/manage_app_languages.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/manage_feature.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/manage_feature.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/options_form.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/options_form.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/tag_any_element.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/tag_any_element.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/translate_app_pagination.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/translate_app_pagination.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/ajax/zip_import.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/ajax/zip_import.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/base.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/build_app.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/build_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/legal/legal_notice.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/legal/legal_notice.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/legal/privacy_statement.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/legal/privacy_statement.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/list_manage_apps.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/list_manage_apps.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/list_manage_generic_content.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/list_manage_generic_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/manage_app.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/manage_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/manage_generic_content.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/manage_generic_content.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/snippets/ckeditor_js_snippet.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/snippets/ckeditor_js_snippet.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/start_new_app.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/start_new_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templates/app_kit/translate_app.html` & `localcosmos_app_kit-0.2.3/app_kit/templates/app_kit/translate_app.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/templatetags/app_tags.py` & `localcosmos_app_kit-0.2.3/app_kit/templatetags/app_tags.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/settings.json` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain/settings.json`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain.zip` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/InvalidMountain.zip`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/settings.json` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain/settings.json`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain.zip` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/frontends_for_testing/Mountain.zip`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/Leaf-large.jpg` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/Leaf-large.jpg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/Leaf.jpg` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/Leaf.jpg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/app-background.jpg` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/app-background.jpg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/localcosmos-logo.svg` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/localcosmos-logo.svg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/images/test-image-2560-1440.jpg` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/images/test-image-2560-1440.jpg`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/TESTS_ROOT/ipa_for_tests/TestApp.ipa` & `localcosmos_app_kit-0.2.3/app_kit/tests/TESTS_ROOT/ipa_for_tests/TestApp.ipa`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/cases.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/cases.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/common.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/common.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/mixins.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/test_forms.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/test_models.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/tests/test_views.py` & `localcosmos_app_kit-0.2.3/app_kit/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/utils.py` & `localcosmos_app_kit-0.2.3/app_kit/utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/validators.py` & `localcosmos_app_kit-0.2.3/app_kit/validators.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/view_mixins.py` & `localcosmos_app_kit-0.2.3/app_kit/view_mixins.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/app_kit/views.py` & `localcosmos_app_kit-0.2.3/app_kit/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/PKG-INFO` & `localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit
-Version: 0.2.2
+Version: 0.2.3
 Summary: LocalCosmos App Kit. Web Portal to build Android and iOS apps
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity
 Platform: OS Independent
```

### Comparing `localcosmos_app_kit-0.2.2/localcosmos_app_kit.egg-info/SOURCES.txt` & `localcosmos_app_kit-0.2.3/localcosmos_app_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit-0.2.2/setup.py` & `localcosmos_app_kit-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'opencv-python',
     'opencv-python-headless',
     'unidecode',
 ]
 
 setup(
     name='localcosmos_app_kit',
-    version='0.2.2',
+    version='0.2.3',
     description='LocalCosmos App Kit. Web Portal to build Android and iOS apps',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, localcosmos, localcosmos server, biodiversity',
     author='Thomas Uher',
```

