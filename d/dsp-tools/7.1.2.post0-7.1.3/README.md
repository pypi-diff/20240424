# Comparing `tmp/dsp_tools-7.1.2.post0.tar.gz` & `tmp/dsp_tools-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.1.2.post0.tar", max compression
+gzip compressed data, was "dsp_tools-7.1.3.tar", max compression
```

## Comparing `dsp_tools-7.1.2.post0.tar` & `dsp_tools-7.1.3.tar`

### file list

```diff
@@ -1,113 +1,115 @@
--rw-r--r--   0        0        0    35149 2024-04-11 14:31:12.870561 dsp_tools-7.1.2.post0/LICENSE
--rw-r--r--   0        0        0     4941 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/docs/index.md
--rw-r--r--   0        0        0     8363 2024-04-11 14:31:49.178882 dsp_tools-7.1.2.post0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     7360 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    12476 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9819 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0     8065 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0      501 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0     6313 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13147 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11830 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21350 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    75692 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-04-11 14:31:12.886562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19520 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28334 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     4200 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    14112 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0     1334 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     5428 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6751 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0      812 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      675 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     2236 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py
--rw-r--r--   0        0        0      548 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
--rw-r--r--   0        0        0     1437 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
--rw-r--r--   0        0        0     2026 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
--rw-r--r--   0        0        0     5164 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py
--rw-r--r--   0        0        0     4004 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
--rw-r--r--   0        0        0     3466 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3063 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    13023 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4585 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5724 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3068 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4237 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7727 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    22348 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0     2876 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2536 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    24360 2024-04-11 14:31:12.890562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    44347 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    33977 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3295 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0      893 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/json_ld_util.py
--rw-r--r--   0        0        0     1157 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0     4464 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7194 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-04-11 14:31:12.894562 dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6317 1970-01-01 00:00:00.000000 dsp_tools-7.1.2.post0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-24 07:07:52.677991 dsp_tools-7.1.3/LICENSE
+-rw-r--r--   0        0        0     4941 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/docs/index.md
+-rw-r--r--   0        0        0     8369 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     7360 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    12476 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9909 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0     8065 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0      501 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0     6313 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13738 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11830 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21324 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    76125 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    21090 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-04-24 07:07:52.693991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28334 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    14112 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0     1334 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     5428 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6751 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0      812 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      675 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     2236 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlallow.py
+-rw-r--r--   0        0        0      548 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1437 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlpermission.py
+-rw-r--r--   0        0        0     2026 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlproperty.py
+-rw-r--r--   0        0        0     5164 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlresource.py
+-rw-r--r--   0        0        0     4004 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlvalue.py
+-rw-r--r--   0        0        0     3466 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3063 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    13023 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4585 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5724 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3068 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4237 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7727 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    22348 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2536 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    24361 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    44347 2024-04-24 07:07:52.697991 dsp_tools-7.1.3/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    33977 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3281 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0      893 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/json_ld_util.py
+-rw-r--r--   0        0        0     1157 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      929 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4464 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     8219 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-04-24 07:07:52.701991 dsp_tools-7.1.3/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6311 1970-01-01 00:00:00.000000 dsp_tools-7.1.3/PKG-INFO
```

### Comparing `dsp_tools-7.1.2.post0/LICENSE` & `dsp_tools-7.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/docs/index.md` & `dsp_tools-7.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/pyproject.toml` & `dsp_tools-7.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.1.2.post0"
+version = "7.1.3"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -51,15 +51,15 @@
 types-lxml = "^2024.3.27"
 types-jsonschema = "^4.21.0.20240331"
 types-openpyxl = "^3.1.0.20240402"
 types-regex = "^2023.12.25.20240311"
 types-pyyaml = "^6.0.12.20240311"
 pytest-unordered = "^0.6.0"
 viztracer = "^0.16.2"
-ruff = "^0.3.5"
+ruff = "^0.3.7"
 pytest-sugar = "^1.0.0"
 pandas-stubs = "^2.2.1.240316"
 types-networkx = "^3.2.1.20240331"
 
 
 [tool.poetry.scripts]
 dsp-tools = "dsp_tools.cli.entry_point:main"  # definition of the CLI entry point
@@ -90,21 +90,19 @@
 """
 markdownlint = """
     docker run \
     -v $PWD:/workdir ghcr.io/igorshubovych/markdownlint-cli:latest \
     --config .markdownlint.yml \
     --ignore CHANGELOG.md "**/*.md"
 """
-
 ruff-check = "ruff check . --ignore=A002,D101,D102,PLR0913,PLR2004,PLW0603"
 ruff-check-github = """
     ruff check . --output-format=github --ignore=A002,D101,D102,PLR0913,PLR2004,PLW0603
-
 """
-ruff-format = "ruff format ."
+ruff-format-check = "ruff format --check ."
 mypy = "mypy ."
 unittests = "pytest test/unittests/"
 integration-tests = "pytest test/integration/"
 e2e-tests = "pytest test/e2e/"
 bump-version = """
     # get current version, append ".postN" (N=no. of commits since last release), write back into pyproject.toml
     version=$(git describe --tags --abbrev=0)
@@ -153,15 +151,15 @@
 [[tool.mypy.overrides]]
 module = ["jsonpath_ng.*", "viztracer.*"]  # For these packages, no type stubs are available yet
 ignore_missing_imports = true
 
 
 [tool.ruff]
 line-length = 120
-target-version = "py311"
+target-version = "py312"
 
 
 [tool.ruff.lint]
 select = [
     "RUF",      # ruff-specific rules
     "PL",       # pylint
     "I",        # isort
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.1.3/src/dsp_tools/cli/call_action.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.1.3/src/dsp_tools/cli/create_parsers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.1.3/src/dsp_tools/cli/entry_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from dsp_tools.cli.call_action import call_requested_action
 from dsp_tools.cli.create_parsers import make_parser
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.exceptions import InternalError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logger_config import logger_config
+from dsp_tools.utils.warnings_config import initialize_warnings
 
 
 def main() -> None:
     """
     Main entry point of the program as referenced in pyproject.toml
     """
     logger_config()
@@ -54,14 +55,15 @@
     )
     parsed_arguments = _parse_arguments(
         user_args=args,
         parser=parser,
     )
     _check_version()
     _log_cli_arguments(parsed_arguments)
+    initialize_warnings()
 
     try:
         parsed_arguments = _derive_sipi_url(
             parsed_arguments=parsed_arguments,
             default_dsp_api_url=default_dsp_api_url,
             default_sipi_url=default_sipi_url,
         )
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from dsp_tools.commands.excel2json.utils import check_required_values
 from dsp_tools.commands.excel2json.utils import col_must_or_not_empty_based_on_other_col
 from dsp_tools.commands.excel2json.utils import find_one_full_cell_in_cols
 from dsp_tools.commands.excel2json.utils import get_comments
 from dsp_tools.commands.excel2json.utils import get_labels
 from dsp_tools.commands.excel2json.utils import get_wrong_row_numbers
 from dsp_tools.commands.excel2json.utils import read_and_clean_all_sheets
+from dsp_tools.models.custom_warnings import DspToolsFutureWarning
 from dsp_tools.models.exceptions import InputError
 
 languages = ["en", "de", "fr", "it", "rm"]
 language_label_col = ["label_en", "label_de", "label_fr", "label_it", "label_rm"]
 mandatory_properties = ["name", "object", "gui_element"]
 
 
@@ -59,14 +60,16 @@
     property_df = _rename_deprecated_columnnames(df=property_df, excelfile=excelfile)
 
     # Not all columns have to be filled, users may delete some for ease of use, but it would generate an error later
     property_df = _add_optional_columns(df=property_df)
 
     _do_property_excel_compliance(df=property_df, excelfile=excelfile)
 
+    _check_for_deprecated_syntax(property_df)
+
     # transform every row into a property
     props = [
         _row2prop(
             df_row=row,
             row_num=int(str(index)) + 2,  # index is a label/index/hashable, but we need an int
             excelfile=excelfile,
         )
@@ -79,14 +82,27 @@
         with open(file=path_to_output_file, mode="w", encoding="utf-8") as file:
             json.dump(props, file, indent=4, ensure_ascii=False)
             print(f"properties section was created successfully and written to file '{path_to_output_file}'")
 
     return props, True
 
 
+def _check_for_deprecated_syntax(df: pd.DataFrame) -> None:
+    _check_for_deprecated_isSequenceOf(df)
+
+
+def _check_for_deprecated_isSequenceOf(df: pd.DataFrame) -> None:
+    if any(x in y for y in list(df["super"]) for x in ["isSequenceOf", "hasSequenceBounds"]):
+        msg = (
+            "Deprecation Warning: Your Excel file contains deprecated super-properties. "
+            "Support for the following super-properties will be removed soon: isSequenceOf, hasSequenceBounds"
+        )
+        warnings.warn(DspToolsFutureWarning(msg))
+
+
 def _read_check_property_df(excelfile: str) -> pd.DataFrame:
     sheets_df_dict = read_and_clean_all_sheets(excelfile=excelfile)
     if len(sheets_df_dict) != 1:
         msg = MoreThanOneSheetProblem("properties.xlsx", list(sheets_df_dict.keys())).execute_error_protocol()
         raise InputError(msg)
     return next(iter(sheets_df_dict.values()))
 
@@ -125,15 +141,14 @@
         df["hlist"] = df["hlist"].fillna(df["gui_attributes"])
         df.pop("gui_attributes")
     df = df.rename(columns={"hlist": "gui_attributes"})
     return df
 
 
 def _do_property_excel_compliance(df: pd.DataFrame, excelfile: str) -> None:
-    # If it does not pass any one of the tests, the function stops
     required_columns = {
         "name",
         "super",
         "object",
         "gui_element",
         "gui_attributes",
     }
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,16 +520,14 @@
         write_xml(root, output_file)
         if len(catched_warnings) > 0:
             success = False
             for warning in catched_warnings:
                 print(f"WARNING: {warning.message}")
 
     if success:
-        print(f"XML file successfully written to '{output_file!s}'")
+        print(f"XML file successfully written to '{output_file}'")
     else:
         red = "\033[31m"
         end = "\033[0m"
-        print(
-            f"{red}Some problems occurred. The XML file was written to '{output_file!s}', but it might be corrupt{end}"
-        )
+        print(f"{red}Some problems occurred. The XML file was written to '{output_file}', but it might be corrupt{end}")
 
     return success, catched_warnings
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,4713 +19,4740 @@
 00000120: 7274 2045 0a66 726f 6d20 7265 6765 7820  rt E.from regex 
 00000130: 696d 706f 7274 204d 6174 6368 0a0a 6672  import Match..fr
 00000140: 6f6d 2064 7370 5f74 6f6f 6c73 2e63 6f6d  om dsp_tools.com
 00000150: 6d61 6e64 732e 6578 6365 6c32 786d 6c2e  mands.excel2xml.
 00000160: 7072 6f70 6572 7479 656c 656d 656e 7420  propertyelement 
 00000170: 696d 706f 7274 2050 726f 7065 7274 7945  import PropertyE
 00000180: 6c65 6d65 6e74 0a66 726f 6d20 6473 705f  lement.from dsp_
-00000190: 746f 6f6c 732e 6d6f 6465 6c73 2e64 6174  tools.models.dat
-000001a0: 6574 696d 6573 7461 6d70 2069 6d70 6f72  etimestamp impor
-000001b0: 7420 4461 7465 5469 6d65 5374 616d 700a  t DateTimeStamp.
-000001c0: 6672 6f6d 2064 7370 5f74 6f6f 6c73 2e6d  from dsp_tools.m
-000001d0: 6f64 656c 732e 6578 6365 7074 696f 6e73  odels.exceptions
-000001e0: 2069 6d70 6f72 7420 4261 7365 4572 726f   import BaseErro
-000001f0: 720a 6672 6f6d 2064 7370 5f74 6f6f 6c73  r.from dsp_tools
-00000200: 2e75 7469 6c73 2e64 6174 655f 7574 696c  .utils.date_util
-00000210: 2069 6d70 6f72 7420 6973 5f66 756c 6c5f   import is_full_
-00000220: 6461 7465 0a66 726f 6d20 6473 705f 746f  date.from dsp_to
-00000230: 6f6c 732e 7574 696c 732e 7368 6172 6564  ols.utils.shared
-00000240: 2069 6d70 6f72 7420 6368 6563 6b5f 6e6f   import check_no
-00000250: 746e 610a 6672 6f6d 2064 7370 5f74 6f6f  tna.from dsp_too
-00000260: 6c73 2e75 7469 6c73 2e73 6861 7265 6420  ls.utils.shared 
-00000270: 696d 706f 7274 2073 696d 706c 6966 795f  import simplify_
-00000280: 6e61 6d65 0a66 726f 6d20 6473 705f 746f  name.from dsp_to
-00000290: 6f6c 732e 7574 696c 732e 7572 695f 7574  ols.utils.uri_ut
-000002a0: 696c 2069 6d70 6f72 7420 6973 5f75 7269  il import is_uri
-000002b0: 0a66 726f 6d20 6473 705f 746f 6f6c 732e  .from dsp_tools.
-000002c0: 7574 696c 732e 786d 6c5f 7661 6c69 6461  utils.xml_valida
-000002d0: 7469 6f6e 2069 6d70 6f72 7420 7661 6c69  tion import vali
-000002e0: 6461 7465 5f78 6d6c 0a0a 2320 7275 6666  date_xml..# ruff
-000002f0: 3a20 6e6f 7161 3a20 4535 3031 2028 6c69  : noqa: E501 (li
-00000300: 6e65 2d74 6f6f 2d6c 6f6e 6729 0a0a 0a78  ne-too-long)...x
-00000310: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-00000320: 203d 207b 4e6f 6e65 3a20 2268 7474 7073   = {None: "https
-00000330: 3a2f 2f64 6173 6368 2e73 7769 7373 2f73  ://dasch.swiss/s
-00000340: 6368 656d 6122 2c20 2278 7369 223a 2022  chema", "xsi": "
-00000350: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00000360: 672f 3230 3031 2f58 4d4c 5363 6865 6d61  g/2001/XMLSchema
-00000370: 2d69 6e73 7461 6e63 6522 7d0a 0a0a 6465  -instance"}...de
-00000380: 6620 6d61 6b65 5f78 7364 5f69 645f 636f  f make_xsd_id_co
-00000390: 6d70 6174 6962 6c65 2873 7472 696e 673a  mpatible(string:
-000003a0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-000003b0: 2020 2222 220a 2020 2020 4d61 6b65 2061    """.    Make a
-000003c0: 2073 7472 696e 6720 636f 6d70 6174 6962   string compatib
-000003d0: 6c65 2077 6974 6820 7468 6520 636f 6e73  le with the cons
-000003e0: 7472 6169 6e74 7320 6f66 2078 7364 3a49  traints of xsd:I
-000003f0: 442c 2073 6f20 7468 6174 2069 7420 6361  D, so that it ca
-00000400: 6e20 6265 2075 7365 6420 6173 2022 6964  n be used as "id
-00000410: 2220 6174 7472 6962 7574 6520 6f66 2061  " attribute of a
-00000420: 203c 7265 736f 7572 6365 3e0a 2020 2020   <resource>.    
-00000430: 7461 672e 2041 6e20 7873 643a 4944 206d  tag. An xsd:ID m
-00000440: 7573 7420 6e6f 7420 636f 6e74 6169 6e20  ust not contain 
-00000450: 7370 6563 6961 6c20 6368 6172 6163 7465  special characte
-00000460: 7273 2c20 616e 6420 6974 206d 7573 7420  rs, and it must 
-00000470: 6265 2075 6e69 7175 6520 696e 2074 6865  be unique in the
-00000480: 2064 6f63 756d 656e 742e 0a0a 2020 2020   document...    
-00000490: 5468 6973 206d 6574 686f 6420 7265 706c  This method repl
-000004a0: 6163 6573 2074 6865 2069 6c6c 6567 616c  aces the illegal
-000004b0: 2063 6861 7261 6374 6572 7320 6279 2022   characters by "
-000004c0: 5f22 2061 6e64 2061 7070 656e 6473 2061  _" and appends a
-000004d0: 2072 616e 646f 6d20 636f 6d70 6f6e 656e   random componen
-000004e0: 7420 746f 2074 6865 2073 7472 696e 6720  t to the string 
-000004f0: 746f 206d 616b 6520 6974 2075 6e69 7175  to make it uniqu
-00000500: 652e 0a0a 2020 2020 5468 6520 7374 7269  e...    The stri
-00000510: 6e67 206d 7573 7420 636f 6e74 6169 6e20  ng must contain 
-00000520: 6174 206c 6561 7374 206f 6e65 2055 6e69  at least one Uni
-00000530: 636f 6465 206c 6574 7465 7220 286d 6174  code letter (mat
-00000540: 6368 696e 6720 7468 6520 7265 6765 7820  ching the regex 
-00000550: 6060 5c5c 707b 4c7d 6060 292c 2075 6e64  ``\\p{L}``), und
-00000560: 6572 7363 6f72 652c 2021 2c20 3f2c 206f  erscore, !, ?, o
-00000570: 7220 6e75 6d62 6572 2c0a 2020 2020 6275  r number,.    bu
-00000580: 7420 6d75 7374 206e 6f74 2062 6520 224e  t must not be "N
-00000590: 6f6e 6522 2c20 223c 4e41 3e22 2c20 224e  one", "<NA>", "N
-000005a0: 2f41 222c 206f 7220 222d 222e 204f 7468  /A", or "-". Oth
-000005b0: 6572 7769 7365 2c20 6120 4261 7365 4572  erwise, a BaseEr
-000005c0: 726f 7220 7769 6c6c 2062 6520 7261 6973  ror will be rais
-000005d0: 6564 2e0a 0a20 2020 2041 7267 733a 0a20  ed...    Args:. 
-000005e0: 2020 2020 2020 2073 7472 696e 673a 2069         string: i
-000005f0: 6e70 7574 2073 7472 696e 670a 0a20 2020  nput string..   
-00000600: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00000610: 2042 6173 6545 7272 6f72 3a20 6966 2074   BaseError: if t
-00000620: 6865 2069 6e70 7574 2063 616e 6e6f 7420  he input cannot 
-00000630: 6265 2074 7261 6e73 666f 726d 6564 2074  be transformed t
-00000640: 6f20 616e 2078 7364 3a49 440a 0a20 2020  o an xsd:ID..   
-00000650: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000660: 2020 616e 2078 7364 2049 4420 6261 7365    an xsd ID base
-00000670: 6420 6f6e 2074 6865 2069 6e70 7574 2073  d on the input s
-00000680: 7472 696e 670a 2020 2020 2222 220a 0a20  tring.    """.. 
-00000690: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-000006a0: 616e 6365 2873 7472 696e 672c 2073 7472  ance(string, str
-000006b0: 2920 6f72 206e 6f74 2063 6865 636b 5f6e  ) or not check_n
-000006c0: 6f74 6e61 2873 7472 696e 6729 3a0a 2020  otna(string):.  
-000006d0: 2020 2020 2020 7261 6973 6520 4261 7365        raise Base
-000006e0: 4572 726f 7228 6622 5468 6520 696e 7075  Error(f"The inpu
-000006f0: 7420 277b 7374 7269 6e67 7d27 2063 616e  t '{string}' can
-00000700: 6e6f 7420 6265 2074 7261 6e73 666f 726d  not be transform
-00000710: 6564 2074 6f20 616e 2078 7364 3a49 4422  ed to an xsd:ID"
-00000720: 290a 0a20 2020 2023 2069 6620 7374 6172  )..    # if star
-00000730: 7420 6f66 2073 7472 696e 6720 6973 206e  t of string is n
-00000740: 6569 7468 6572 206c 6574 7465 7220 6e6f  either letter no
-00000750: 7220 756e 6465 7273 636f 7265 2c20 6164  r underscore, ad
-00000760: 6420 616e 2075 6e64 6572 7363 6f72 650a  d an underscore.
-00000770: 2020 2020 7265 7320 3d20 7265 6765 782e      res = regex.
-00000780: 7375 6228 7222 5e28 3f3d 5b5e 412d 5a61  sub(r"^(?=[^A-Za
-00000790: 2d7a 5f5d 2922 2c20 225f 222c 2073 7472  -z_])", "_", str
-000007a0: 696e 6729 0a0a 2020 2020 2320 7265 706c  ing)..    # repl
-000007b0: 6163 6520 616c 6c20 696c 6c65 6761 6c20  ace all illegal 
-000007c0: 6368 6172 6163 7465 7273 2062 7920 756e  characters by un
-000007d0: 6465 7273 636f 7265 0a20 2020 2072 6573  derscore.    res
-000007e0: 203d 2072 6567 6578 2e73 7562 2872 225b   = regex.sub(r"[
-000007f0: 5e5c 775f 5c2d 2e5d 222c 2022 5f22 2c20  ^\w_\-.]", "_", 
-00000800: 7265 732c 2066 6c61 6773 3d72 6567 6578  res, flags=regex
-00000810: 2e41 5343 4949 290a 0a20 2020 2023 2061  .ASCII)..    # a
-00000820: 6464 2075 7569 640a 2020 2020 5f75 7569  dd uuid.    _uui
-00000830: 6420 3d20 7575 6964 2e75 7569 6434 2829  d = uuid.uuid4()
-00000840: 0a20 2020 2072 6573 203d 2066 227b 7265  .    res = f"{re
-00000850: 737d 5f7b 5f75 7569 647d 220a 0a20 2020  s}_{_uuid}"..   
-00000860: 2072 6574 7572 6e20 7265 730a 0a0a 6465   return res...de
-00000870: 6620 5f66 696e 645f 6672 656e 6368 5f62  f _find_french_b
-00000880: 635f 6461 7465 280a 2020 2020 7374 7269  c_date(.    stri
-00000890: 6e67 3a20 7374 722c 0a20 2020 206c 6f6f  ng: str,.    loo
-000008a0: 6b62 6568 696e 643a 2073 7472 2c0a 2020  kbehind: str,.  
-000008b0: 2020 6c6f 6f6b 6168 6561 643a 2073 7472    lookahead: str
-000008c0: 2c0a 2920 2d3e 204f 7074 696f 6e61 6c5b  ,.) -> Optional[
-000008d0: 7374 725d 3a0a 2020 2020 6672 656e 6368  str]:.    french
-000008e0: 5f62 635f 7265 6765 7820 3d20 7222 6176  _bc_regex = r"av
-000008f0: 283f 3a5c 2e20 7c5c 2e7c 2029 4a5c 2e3f  (?:\. |\.| )J\.?
-00000900: 2d3f 435c 2e3f 220a 2020 2020 6966 206e  -?C\.?".    if n
-00000910: 6f74 2072 6567 6578 2e73 6561 7263 6828  ot regex.search(
-00000920: 6672 656e 6368 5f62 635f 7265 6765 782c  french_bc_regex,
-00000930: 2073 7472 696e 6729 3a0a 2020 2020 2020   string):.      
-00000940: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
-00000950: 2020 2079 6561 725f 7265 6765 7820 3d20     year_regex = 
-00000960: 7222 5c64 7b31 2c35 7d22 0a20 2020 2073  r"\d{1,5}".    s
-00000970: 6570 5f72 6567 6578 203d 2072 2220 3f2d  ep_regex = r" ?-
-00000980: 203f 220a 0a20 2020 2079 6561 725f 7261   ?"..    year_ra
-00000990: 6e67 655f 7265 6765 7820 3d20 7266 227b  nge_regex = rf"{
-000009a0: 6c6f 6f6b 6265 6869 6e64 7d28 7b79 6561  lookbehind}({yea
-000009b0: 725f 7265 6765 787d 297b 7365 705f 7265  r_regex}){sep_re
-000009c0: 6765 787d 287b 7965 6172 5f72 6567 6578  gex}({year_regex
-000009d0: 7d29 207b 6672 656e 6368 5f62 635f 7265  }) {french_bc_re
-000009e0: 6765 787d 7b6c 6f6f 6b61 6865 6164 7d22  gex}{lookahead}"
-000009f0: 0a20 2020 2079 6561 725f 7261 6e67 6520  .    year_range 
-00000a00: 3d20 7265 6765 782e 7365 6172 6368 2879  = regex.search(y
-00000a10: 6561 725f 7261 6e67 655f 7265 6765 782c  ear_range_regex,
-00000a20: 2073 7472 696e 6729 0a20 2020 2069 6620   string).    if 
-00000a30: 7965 6172 5f72 616e 6765 3a0a 2020 2020  year_range:.    
-00000a40: 2020 2020 7374 6172 745f 7965 6172 203d      start_year =
-00000a50: 2069 6e74 2879 6561 725f 7261 6e67 652e   int(year_range.
-00000a60: 6772 6f75 7028 3129 290a 2020 2020 2020  group(1)).      
-00000a70: 2020 656e 645f 7965 6172 203d 2069 6e74    end_year = int
-00000a80: 2879 6561 725f 7261 6e67 652e 6772 6f75  (year_range.grou
-00000a90: 7028 3229 290a 2020 2020 2020 2020 6966  p(2)).        if
-00000aa0: 2065 6e64 5f79 6561 7220 3e20 7374 6172   end_year > star
-00000ab0: 745f 7965 6172 3a0a 2020 2020 2020 2020  t_year:.        
-00000ac0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00000ad0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00000ae0: 2247 5245 474f 5249 414e 3a42 433a 7b73  "GREGORIAN:BC:{s
-00000af0: 7461 7274 5f79 6561 727d 3a42 433a 7b65  tart_year}:BC:{e
-00000b00: 6e64 5f79 6561 727d 220a 0a20 2020 2073  nd_year}"..    s
-00000b10: 696e 676c 655f 7965 6172 5f72 6567 6578  ingle_year_regex
-00000b20: 203d 2072 6622 7b6c 6f6f 6b62 6568 696e   = rf"{lookbehin
-00000b30: 647d 287b 7965 6172 5f72 6567 6578 7d29  d}({year_regex})
-00000b40: 207b 6672 656e 6368 5f62 635f 7265 6765   {french_bc_rege
-00000b50: 787d 7b6c 6f6f 6b61 6865 6164 7d22 0a20  x}{lookahead}". 
-00000b60: 2020 2073 696e 676c 655f 7965 6172 203d     single_year =
-00000b70: 2072 6567 6578 2e73 6561 7263 6828 7369   regex.search(si
-00000b80: 6e67 6c65 5f79 6561 725f 7265 6765 782c  ngle_year_regex,
-00000b90: 2073 7472 696e 6729 0a20 2020 2069 6620   string).    if 
-00000ba0: 7369 6e67 6c65 5f79 6561 723a 0a20 2020  single_year:.   
-00000bb0: 2020 2020 2073 7461 7274 5f79 6561 7220       start_year 
-00000bc0: 3d20 696e 7428 7369 6e67 6c65 5f79 6561  = int(single_yea
-00000bd0: 722e 6772 6f75 7028 3129 290a 2020 2020  r.group(1)).    
-00000be0: 2020 2020 7265 7475 726e 2066 2247 5245      return f"GRE
-00000bf0: 474f 5249 414e 3a42 433a 7b73 7461 7274  GORIAN:BC:{start
-00000c00: 5f79 6561 727d 3a42 433a 7b73 7461 7274  _year}:BC:{start
-00000c10: 5f79 6561 727d 220a 0a20 2020 2072 6574  _year}"..    ret
-00000c20: 7572 6e20 4e6f 6e65 0a0a 0a64 6566 2066  urn None...def f
-00000c30: 696e 645f 6461 7465 5f69 6e5f 7374 7269  ind_date_in_stri
-00000c40: 6e67 2873 7472 696e 673a 2073 7472 2920  ng(string: str) 
-00000c50: 2d3e 204f 7074 696f 6e61 6c5b 7374 725d  -> Optional[str]
-00000c60: 3a0a 2020 2020 2222 220a 2020 2020 4368  :.    """.    Ch
-00000c70: 6563 6b73 2069 6620 6120 7374 7269 6e67  ecks if a string
-00000c80: 2063 6f6e 7461 696e 7320 6120 6461 7465   contains a date
-00000c90: 2076 616c 7565 2028 7369 6e67 6c65 2064   value (single d
-00000ca0: 6174 652c 206f 7220 6461 7465 2072 616e  ate, or date ran
-00000cb0: 6765 292c 0a20 2020 2061 6e64 2072 6574  ge),.    and ret
-00000cc0: 7572 6e73 2074 6865 2066 6972 7374 2066  urns the first f
-00000cd0: 6f75 6e64 2064 6174 6520 6173 2044 5350  ound date as DSP
-00000ce0: 2d66 6f72 6d61 7474 6564 2073 7472 696e  -formatted strin
-00000cf0: 672e 0a20 2020 2052 6574 7572 6e73 204e  g..    Returns N
-00000d00: 6f6e 6520 6966 206e 6f20 6461 7465 2077  one if no date w
-00000d10: 6173 2066 6f75 6e64 2e0a 0a20 2020 204e  as found...    N
-00000d20: 6f74 6573 3a0a 2020 2020 2020 2020 2d20  otes:.        - 
-00000d30: 416c 6c20 6461 7465 7320 6172 6520 696e  All dates are in
-00000d40: 7465 7270 7265 7465 6420 696e 2074 6865  terpreted in the
-00000d50: 2043 6872 6973 7469 616e 2065 7261 2061   Christian era a
-00000d60: 6e64 2074 6865 2047 7265 676f 7269 616e  nd the Gregorian
-00000d70: 2063 616c 656e 6461 722e 0a20 2020 2020   calendar..     
-00000d80: 2020 202d 2042 4320 6461 7465 7320 6172     - BC dates ar
-00000d90: 6520 6f6e 6c79 2073 7570 706f 7274 6564  e only supported
-00000da0: 2069 6e20 4672 656e 6368 206e 6f74 6174   in French notat
-00000db0: 696f 6e20 2865 2e67 2e20 3130 3030 2d39  ion (e.g. 1000-9
-00000dc0: 3030 2061 762e 204a 2e2d 432e 292e 0a20  00 av. J.-C.).. 
-00000dd0: 2020 2020 2020 202d 2054 6865 2079 6561         - The yea
-00000de0: 7273 2030 3030 302d 3239 3939 2061 7265  rs 0000-2999 are
-00000df0: 2073 7570 706f 7274 6564 2c20 696e 2033   supported, in 3
-00000e00: 2f34 2d64 6967 6974 2066 6f72 6d2e 0a20  /4-digit form.. 
-00000e10: 2020 2020 2020 202d 2044 6174 6573 2077         - Dates w
-00000e20: 7269 7474 656e 2077 6974 6820 736c 6173  ritten with slas
-00000e30: 6865 7320 6172 6520 616c 7761 7973 2069  hes are always i
-00000e40: 6e74 6572 7072 6574 6564 2069 6e20 6120  nterpreted in a 
-00000e50: 4575 726f 7065 616e 206d 616e 6e65 723a  European manner:
-00000e60: 2035 2f31 312f 3230 3231 2069 7320 7468   5/11/2021 is th
-00000e70: 6520 3574 6820 6f66 204e 6f76 656d 6265  e 5th of Novembe
-00000e80: 722e 0a20 2020 2020 2020 202d 2049 6e20  r..        - In 
-00000e90: 7468 6520 4575 726f 7065 616e 206e 6f74  the European not
-00000ea0: 6174 696f 6e2c 2032 2d64 6967 6974 2079  ation, 2-digit y
-00000eb0: 6561 7273 2061 7265 2065 7870 616e 6465  ears are expande
-00000ec0: 6420 746f 2034 2064 6967 6974 732c 2077  d to 4 digits, w
-00000ed0: 6974 6820 7468 6520 6375 7272 656e 7420  ith the current 
-00000ee0: 7965 6172 2061 7320 7761 7465 7273 6865  year as watershe
-00000ef0: 643a 0a20 2020 2020 2020 2020 2020 202d  d:.            -
-00000f00: 2033 302e 342e 3234 202d 3e20 3330 2e30   30.4.24 -> 30.0
-00000f10: 342e 3230 3234 0a20 2020 2020 2020 2020  4.2024.         
-00000f20: 2020 202d 2033 302e 342e 3235 202d 3e20     - 30.4.25 -> 
-00000f30: 3330 2e30 342e 3139 3235 0a0a 2020 2020  30.04.1925..    
-00000f40: 4375 7272 656e 746c 7920 7375 7070 6f72  Currently suppor
-00000f50: 7465 6420 6461 7465 2066 6f72 6d61 7473  ted date formats
-00000f60: 3a0a 2020 2020 2020 2020 2d20 3034 3736  :.        - 0476
-00000f70: 2d30 392d 3034 202d 3e20 4752 4547 4f52  -09-04 -> GREGOR
-00000f80: 4941 4e3a 4345 3a30 3437 362d 3039 2d30  IAN:CE:0476-09-0
-00000f90: 343a 4345 3a30 3437 362d 3039 2d30 340a  4:CE:0476-09-04.
-00000fa0: 2020 2020 2020 2020 2d20 3034 3736 5f30          - 0476_0
-00000fb0: 395f 3034 202d 3e20 4752 4547 4f52 4941  9_04 -> GREGORIA
-00000fc0: 4e3a 4345 3a30 3437 362d 3039 2d30 343a  N:CE:0476-09-04:
-00000fd0: 4345 3a30 3437 362d 3039 2d30 340a 2020  CE:0476-09-04.  
-00000fe0: 2020 2020 2020 2d20 3330 2e34 2e32 3032        - 30.4.202
-00000ff0: 3120 2d3e 2047 5245 474f 5249 414e 3a43  1 -> GREGORIAN:C
-00001000: 453a 3230 3231 2d30 342d 3330 3a43 453a  E:2021-04-30:CE:
-00001010: 3230 3231 2d30 342d 3330 0a20 2020 2020  2021-04-30.     
-00001020: 2020 202d 2033 302e 342e 3231 202d 3e20     - 30.4.21 -> 
-00001030: 4752 4547 4f52 4941 4e3a 4345 3a32 3032  GREGORIAN:CE:202
-00001040: 312d 3034 2d33 303a 4345 3a32 3032 312d  1-04-30:CE:2021-
-00001050: 3034 2d33 300a 2020 2020 2020 2020 2d20  04-30.        - 
-00001060: 352f 3131 2f32 3032 3120 2d3e 2047 5245  5/11/2021 -> GRE
-00001070: 474f 5249 414e 3a43 453a 3230 3231 2d31  GORIAN:CE:2021-1
-00001080: 312d 3035 3a43 453a 3230 3231 2d31 312d  1-05:CE:2021-11-
-00001090: 3035 0a20 2020 2020 2020 202d 204a 616e  05.        - Jan
-000010a0: 2032 362c 2031 3939 3320 2d3e 2047 5245   26, 1993 -> GRE
-000010b0: 474f 5249 414e 3a43 453a 3139 3933 2d30  GORIAN:CE:1993-0
-000010c0: 312d 3236 3a43 453a 3139 3933 2d30 312d  1-26:CE:1993-01-
-000010d0: 3236 0a20 2020 2020 2020 202d 2032 382e  26.        - 28.
-000010e0: 322e 2d31 2e31 322e 3135 3135 202d 3e20  2.-1.12.1515 -> 
-000010f0: 4752 4547 4f52 4941 4e3a 4345 3a31 3531  GREGORIAN:CE:151
-00001100: 352d 3032 2d32 383a 4345 3a31 3531 352d  5-02-28:CE:1515-
-00001110: 3132 2d30 310a 2020 2020 2020 2020 2d20  12-01.        - 
-00001120: 3235 2e2d 3236 2e32 2e30 3830 3020 2d3e  25.-26.2.0800 ->
-00001130: 2047 5245 474f 5249 414e 3a43 453a 3038   GREGORIAN:CE:08
-00001140: 3030 2d30 322d 3235 3a43 453a 3038 3030  00-02-25:CE:0800
-00001150: 2d30 322d 3236 0a20 2020 2020 2020 202d  -02-26.        -
-00001160: 2031 2e39 2e32 3032 322d 332e 312e 3230   1.9.2022-3.1.20
-00001170: 3234 202d 3e20 4752 4547 4f52 4941 4e3a  24 -> GREGORIAN:
-00001180: 4345 3a32 3032 322d 3039 2d30 313a 4345  CE:2022-09-01:CE
-00001190: 3a32 3032 342d 3031 2d30 330a 2020 2020  :2024-01-03.    
-000011a0: 2020 2020 2d20 3138 3438 202d 3e20 4752      - 1848 -> GR
-000011b0: 4547 4f52 4941 4e3a 4345 3a31 3834 383a  EGORIAN:CE:1848:
-000011c0: 4345 3a31 3834 380a 2020 2020 2020 2020  CE:1848.        
-000011d0: 2d20 3138 3439 2f31 3835 3020 2d3e 2047  - 1849/1850 -> G
-000011e0: 5245 474f 5249 414e 3a43 453a 3138 3439  REGORIAN:CE:1849
-000011f0: 3a43 453a 3138 3530 0a20 2020 2020 2020  :CE:1850.       
-00001200: 202d 2031 3834 392f 3530 202d 3e20 4752   - 1849/50 -> GR
-00001210: 4547 4f52 4941 4e3a 4345 3a31 3834 393a  EGORIAN:CE:1849:
-00001220: 4345 3a31 3835 300a 2020 2020 2020 2020  CE:1850.        
-00001230: 2d20 3138 3435 2d35 3020 2d3e 2047 5245  - 1845-50 -> GRE
-00001240: 474f 5249 414e 3a43 453a 3138 3435 3a43  GORIAN:CE:1845:C
-00001250: 453a 3138 3530 0a20 2020 2020 2020 202d  E:1850.        -
-00001260: 2038 3430 2d35 3020 2d3e 2047 5245 474f   840-50 -> GREGO
-00001270: 5249 414e 3a43 453a 3834 303a 4345 3a38  RIAN:CE:840:CE:8
-00001280: 3530 0a20 2020 2020 2020 202d 2038 3430  50.        - 840
-00001290: 2d31 202d 3e20 4752 4547 4f52 4941 4e3a  -1 -> GREGORIAN:
-000012a0: 4345 3a38 3430 3a43 453a 3834 310a 2020  CE:840:CE:841.  
-000012b0: 2020 2020 2020 2d20 3130 3030 2d39 3030        - 1000-900
-000012c0: 2061 762e 204a 2e2d 432e 202d 3e20 4752   av. J.-C. -> GR
-000012d0: 4547 4f52 4941 4e3a 4243 3a31 3030 303a  EGORIAN:BC:1000:
-000012e0: 4243 3a39 3030 0a20 2020 2020 2020 202d  BC:900.        -
-000012f0: 2034 3520 6176 2e20 4a2e 2d43 2e20 2d3e   45 av. J.-C. ->
-00001300: 2047 5245 474f 5249 414e 3a42 433a 3435   GREGORIAN:BC:45
-00001310: 3a42 433a 3435 0a0a 2020 2020 4172 6773  :BC:45..    Args
-00001320: 3a0a 2020 2020 2020 2020 7374 7269 6e67  :.        string
-00001330: 3a20 7374 7269 6e67 2074 6f20 6368 6563  : string to chec
-00001340: 6b0a 0a20 2020 2052 6574 7572 6e73 3a0a  k..    Returns:.
-00001350: 2020 2020 2020 2020 4453 502d 666f 726d          DSP-form
-00001360: 6174 7465 6420 6461 7465 2073 7472 696e  atted date strin
-00001370: 672c 206f 7220 4e6f 6e65 0a0a 2020 2020  g, or None..    
-00001380: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-00001390: 2020 3e3e 3e20 6966 2066 696e 645f 6461    >>> if find_da
-000013a0: 7465 5f69 6e5f 7374 7269 6e67 2872 6f77  te_in_string(row
-000013b0: 5b22 4570 6f63 6822 5d29 3a0a 2020 2020  ["Epoch"]):.    
-000013c0: 2020 2020 3e3e 3e20 2020 2020 7265 736f      >>>     reso
-000013d0: 7572 6365 2e61 7070 656e 6428 6d61 6b65  urce.append(make
-000013e0: 5f64 6174 655f 7072 6f70 2822 3a68 6173  _date_prop(":has
-000013f0: 4461 7465 222c 2066 696e 645f 6461 7465  Date", find_date
-00001400: 5f69 6e5f 7374 7269 6e67 2872 6f77 5b22  _in_string(row["
-00001410: 4570 6f63 6822 5d29 290a 0a20 2020 2053  Epoch"]))..    S
-00001420: 6565 2068 7474 7073 3a2f 2f64 6f63 732e  ee https://docs.
-00001430: 6461 7363 682e 7377 6973 732f 6c61 7465  dasch.swiss/late
-00001440: 7374 2f44 5350 2d54 4f4f 4c53 2f66 696c  st/DSP-TOOLS/fil
-00001450: 652d 666f 726d 6174 732f 786d 6c2d 6461  e-formats/xml-da
-00001460: 7461 2d66 696c 652f 2364 6174 652d 7072  ta-file/#date-pr
-00001470: 6f70 0a20 2020 2022 2222 0a0a 2020 2020  op.    """..    
-00001480: 2320 7361 6e69 7469 7a65 2069 6e70 7574  # sanitize input
-00001490: 2c20 6a75 7374 2069 6e20 6361 7365 2074  , just in case t
-000014a0: 6861 7420 7468 6520 6d65 7468 6f64 2077  hat the method w
-000014b0: 6173 2063 616c 6c65 6420 6f6e 2061 6e20  as called on an 
-000014c0: 656d 7074 7920 6f72 204e 2f41 2063 656c  empty or N/A cel
-000014d0: 6c0a 2020 2020 6966 206e 6f74 2063 6865  l.    if not che
-000014e0: 636b 5f6e 6f74 6e61 2873 7472 696e 6729  ck_notna(string)
-000014f0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00001500: 204e 6f6e 650a 2020 2020 7472 793a 0a20   None.    try:. 
-00001510: 2020 2020 2020 2072 6574 7572 6e20 5f66         return _f
-00001520: 696e 645f 6461 7465 5f69 6e5f 7374 7269  ind_date_in_stri
-00001530: 6e67 5f74 6872 6f77 696e 6728 7374 7269  ng_throwing(stri
-00001540: 6e67 290a 2020 2020 6578 6365 7074 2056  ng).    except V
-00001550: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
-00001560: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
-00001570: 0a5f 6d6f 6e74 6873 5f64 6963 7420 3d20  ._months_dict = 
-00001580: 7b0a 2020 2020 224a 616e 7561 7279 223a  {.    "January":
-00001590: 2031 2c0a 2020 2020 224a 616e 223a 2031   1,.    "Jan": 1
-000015a0: 2c0a 2020 2020 2246 6562 7275 6172 7922  ,.    "February"
-000015b0: 3a20 322c 0a20 2020 2022 4665 6222 3a20  : 2,.    "Feb": 
-000015c0: 322c 0a20 2020 2022 4d61 7263 6822 3a20  2,.    "March": 
-000015d0: 332c 0a20 2020 2022 4d61 7222 3a20 332c  3,.    "Mar": 3,
-000015e0: 0a20 2020 2022 4170 7269 6c22 3a20 342c  .    "April": 4,
-000015f0: 0a20 2020 2022 4170 7222 3a20 342c 0a20  .    "Apr": 4,. 
-00001600: 2020 2022 4d61 7922 3a20 352c 0a20 2020     "May": 5,.   
-00001610: 2022 4a75 6e65 223a 2036 2c0a 2020 2020   "June": 6,.    
-00001620: 224a 756e 223a 2036 2c0a 2020 2020 224a  "Jun": 6,.    "J
-00001630: 756c 7922 3a20 372c 0a20 2020 2022 4a75  uly": 7,.    "Ju
-00001640: 6c22 3a20 372c 0a20 2020 2022 4175 6775  l": 7,.    "Augu
-00001650: 7374 223a 2038 2c0a 2020 2020 2241 7567  st": 8,.    "Aug
-00001660: 223a 2038 2c0a 2020 2020 2253 6570 7465  ": 8,.    "Septe
-00001670: 6d62 6572 223a 2039 2c0a 2020 2020 2253  mber": 9,.    "S
-00001680: 6570 7422 3a20 392c 0a20 2020 2022 4f63  ept": 9,.    "Oc
-00001690: 746f 6265 7222 3a20 3130 2c0a 2020 2020  tober": 10,.    
-000016a0: 224f 6374 223a 2031 302c 0a20 2020 2022  "Oct": 10,.    "
-000016b0: 4e6f 7665 6d62 6572 223a 2031 312c 0a20  November": 11,. 
-000016c0: 2020 2022 4e6f 7622 3a20 3131 2c0a 2020     "Nov": 11,.  
-000016d0: 2020 2244 6563 656d 6265 7222 3a20 3132    "December": 12
-000016e0: 2c0a 2020 2020 2244 6563 223a 2031 322c  ,.    "Dec": 12,
-000016f0: 0a7d 0a0a 0a64 6566 205f 6669 6e64 5f64  .}...def _find_d
-00001700: 6174 655f 696e 5f73 7472 696e 675f 7468  ate_in_string_th
-00001710: 726f 7769 6e67 2873 7472 696e 673a 2073  rowing(string: s
-00001720: 7472 2920 2d3e 2073 7472 207c 204e 6f6e  tr) -> str | Non
-00001730: 653a 0a20 2020 2022 2222 0a20 2020 2054  e:.    """.    T
-00001740: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
-00001750: 7468 6520 7361 6d65 2061 7320 6669 6e64  the same as find
-00001760: 5f64 6174 655f 696e 5f73 7472 696e 6728  _date_in_string(
-00001770: 292c 2062 7574 206d 6179 2072 6169 7365  ), but may raise
-00001780: 2061 2056 616c 7565 4572 726f 7220 696e   a ValueError in
-00001790: 7374 6561 6420 6f66 2072 6574 7572 6e69  stead of returni
-000017a0: 6e67 204e 6f6e 652e 0a20 2020 2022 2222  ng None..    """
-000017b0: 0a20 2020 2079 6561 725f 7265 6765 7820  .    year_regex 
-000017c0: 3d20 7222 285b 302d 325d 3f5b 302d 395d  = r"([0-2]?[0-9]
-000017d0: 5b30 2d39 5d5b 302d 395d 2922 0a20 2020  [0-9][0-9])".   
-000017e0: 2079 6561 725f 7265 6765 785f 325f 6f72   year_regex_2_or
-000017f0: 5f34 5f64 6967 6974 7320 3d20 7222 2828  _4_digits = r"((
-00001800: 3f3a 5b30 2d32 5d3f 5b30 2d39 5d29 3f5b  ?:[0-2]?[0-9])?[
-00001810: 302d 395d 5b30 2d39 5d29 220a 2020 2020  0-9][0-9])".    
-00001820: 6d6f 6e74 685f 7265 6765 7820 3d20 7222  month_regex = r"
-00001830: 285b 302d 315d 3f5b 302d 395d 2922 0a20  ([0-1]?[0-9])". 
-00001840: 2020 2064 6179 5f72 6567 6578 203d 2072     day_regex = r
-00001850: 2228 5b30 2d33 5d3f 5b30 2d39 5d29 220a  "([0-3]?[0-9])".
-00001860: 2020 2020 7365 705f 7265 6765 7820 3d20      sep_regex = 
-00001870: 7222 5b5c 2e2f 5d22 0a20 2020 206c 6f6f  r"[\./]".    loo
-00001880: 6b62 6568 696e 6420 3d20 7222 283f 3c21  kbehind = r"(?<!
-00001890: 5b30 2d39 412d 5a61 2d7a 5d29 220a 2020  [0-9A-Za-z])".  
-000018a0: 2020 6c6f 6f6b 6168 6561 6420 3d20 7222    lookahead = r"
-000018b0: 283f 215b 302d 3941 2d5a 612d 7a5d 2922  (?![0-9A-Za-z])"
-000018c0: 0a0a 2020 2020 6966 2066 7265 6e63 685f  ..    if french_
-000018d0: 6263 5f64 6174 6520 3a3d 205f 6669 6e64  bc_date := _find
-000018e0: 5f66 7265 6e63 685f 6263 5f64 6174 6528  _french_bc_date(
-000018f0: 7374 7269 6e67 3d73 7472 696e 672c 206c  string=string, l
-00001900: 6f6f 6b62 6568 696e 643d 6c6f 6f6b 6265  ookbehind=lookbe
-00001910: 6869 6e64 2c20 6c6f 6f6b 6168 6561 643d  hind, lookahead=
-00001920: 6c6f 6f6b 6168 6561 6429 3a0a 2020 2020  lookahead):.    
-00001930: 2020 2020 7265 7475 726e 2066 7265 6e63      return frenc
-00001940: 685f 6263 5f64 6174 650a 0a20 2020 2023  h_bc_date..    #
-00001950: 2074 656d 706c 6174 653a 2032 3032 312d   template: 2021-
-00001960: 3031 2d30 3120 7c20 3230 3135 5f30 315f  01-01 | 2015_01_
-00001970: 3032 0a20 2020 2069 736f 5f64 6174 6520  02.    iso_date 
-00001980: 3d20 7265 6765 782e 7365 6172 6368 2872  = regex.search(r
-00001990: 6622 7b6c 6f6f 6b62 6568 696e 647d 7b79  f"{lookbehind}{y
-000019a0: 6561 725f 7265 6765 787d 5b5f 2d5d 285b  ear_regex}[_-]([
-000019b0: 302d 315d 5b30 2d39 5d29 5b5f 2d5d 285b  0-1][0-9])[_-]([
-000019c0: 302d 335d 5b30 2d39 5d29 7b6c 6f6f 6b61  0-3][0-9]){looka
-000019d0: 6865 6164 7d22 2c20 7374 7269 6e67 290a  head}", string).
-000019e0: 0a20 2020 2023 2074 656d 706c 6174 653a  .    # template:
-000019f0: 2036 2e2d 382e 332e 3139 3438 207c 2036   6.-8.3.1948 | 6
-00001a00: 2f32 2f31 3934 3720 2d20 3234 2e30 332e  /2/1947 - 24.03.
-00001a10: 3139 3438 0a20 2020 2065 7572 5f64 6174  1948.    eur_dat
-00001a20: 655f 7261 6e67 655f 7265 6765 7820 3d20  e_range_regex = 
-00001a30: 280a 2020 2020 2020 2020 7266 227b 6c6f  (.        rf"{lo
-00001a40: 6f6b 6265 6869 6e64 7d22 0a20 2020 2020  okbehind}".     
-00001a50: 2020 2072 6622 7b64 6179 5f72 6567 6578     rf"{day_regex
-00001a60: 7d7b 7365 705f 7265 6765 787d 283f 3a7b  }{sep_regex}(?:{
-00001a70: 6d6f 6e74 685f 7265 6765 787d 7b73 6570  month_regex}{sep
-00001a80: 5f72 6567 6578 7d7b 7965 6172 5f72 6567  _regex}{year_reg
-00001a90: 6578 5f32 5f6f 725f 345f 6469 6769 7473  ex_2_or_4_digits
-00001aa0: 7d3f 293f 203f 283f 3a2d 7c3a 7c74 6f29  }?)? ?(?:-|:|to)
-00001ab0: 203f 220a 2020 2020 2020 2020 7266 227b   ?".        rf"{
-00001ac0: 6461 795f 7265 6765 787d 7b73 6570 5f72  day_regex}{sep_r
-00001ad0: 6567 6578 7d7b 6d6f 6e74 685f 7265 6765  egex}{month_rege
-00001ae0: 787d 7b73 6570 5f72 6567 6578 7d7b 7965  x}{sep_regex}{ye
-00001af0: 6172 5f72 6567 6578 5f32 5f6f 725f 345f  ar_regex_2_or_4_
-00001b00: 6469 6769 7473 7d22 0a20 2020 2020 2020  digits}".       
-00001b10: 2072 6622 7b6c 6f6f 6b61 6865 6164 7d22   rf"{lookahead}"
-00001b20: 0a20 2020 2029 0a20 2020 2065 7572 5f64  .    ).    eur_d
-00001b30: 6174 655f 7261 6e67 6520 3d20 7265 6765  ate_range = rege
-00001b40: 782e 7365 6172 6368 2865 7572 5f64 6174  x.search(eur_dat
-00001b50: 655f 7261 6e67 655f 7265 6765 782c 2073  e_range_regex, s
-00001b60: 7472 696e 6729 0a0a 2020 2020 2320 7465  tring)..    # te
-00001b70: 6d70 6c61 7465 3a20 312e 342e 3230 3231  mplate: 1.4.2021
-00001b80: 207c 2035 2f31 312f 3230 3231 0a20 2020   | 5/11/2021.   
-00001b90: 2065 7572 5f64 6174 655f 7265 6765 7820   eur_date_regex 
-00001ba0: 3d20 7266 227b 6c6f 6f6b 6265 6869 6e64  = rf"{lookbehind
-00001bb0: 7d7b 6461 795f 7265 6765 787d 7b73 6570  }{day_regex}{sep
-00001bc0: 5f72 6567 6578 7d7b 6d6f 6e74 685f 7265  _regex}{month_re
-00001bd0: 6765 787d 7b73 6570 5f72 6567 6578 7d7b  gex}{sep_regex}{
-00001be0: 7965 6172 5f72 6567 6578 5f32 5f6f 725f  year_regex_2_or_
-00001bf0: 345f 6469 6769 7473 7d7b 6c6f 6f6b 6168  4_digits}{lookah
-00001c00: 6561 647d 220a 2020 2020 6575 725f 6461  ead}".    eur_da
-00001c10: 7465 203d 2072 6567 6578 2e73 6561 7263  te = regex.searc
-00001c20: 6828 0a20 2020 2020 2020 2065 7572 5f64  h(.        eur_d
-00001c30: 6174 655f 7265 6765 782c 0a20 2020 2020  ate_regex,.     
-00001c40: 2020 2073 7472 696e 672c 0a20 2020 2029     string,.    )
-00001c50: 0a0a 2020 2020 2320 7465 6d70 6c61 7465  ..    # template
-00001c60: 3a20 4d61 7263 6820 392c 2031 3930 3820  : March 9, 1908 
-00001c70: 7c20 4d61 7263 6835 2c31 3930 3820 7c20  | March5,1908 | 
-00001c80: 4d61 7920 3131 2c20 3139 3036 0a20 2020  May 11, 1906.   
-00001c90: 2061 6c6c 5f6d 6f6e 7468 7320 3d20 227c   all_months = "|
-00001ca0: 222e 6a6f 696e 285f 6d6f 6e74 6873 5f64  ".join(_months_d
-00001cb0: 6963 7429 0a20 2020 206d 6f6e 7468 6e61  ict).    monthna
-00001cc0: 6d65 5f64 6174 655f 7265 6765 7820 3d20  me_date_regex = 
-00001cd0: 7266 227b 6c6f 6f6b 6265 6869 6e64 7d28  rf"{lookbehind}(
-00001ce0: 7b61 6c6c 5f6d 6f6e 7468 737d 2920 3f7b  {all_months}) ?{
-00001cf0: 6461 795f 7265 6765 787d 2c20 3f7b 7965  day_regex}, ?{ye
-00001d00: 6172 5f72 6567 6578 7d7b 6c6f 6f6b 6168  ar_regex}{lookah
-00001d10: 6561 647d 220a 2020 2020 6d6f 6e74 686e  ead}".    monthn
-00001d20: 616d 655f 6461 7465 203d 2072 6567 6578  ame_date = regex
-00001d30: 2e73 6561 7263 6828 6d6f 6e74 686e 616d  .search(monthnam
-00001d40: 655f 6461 7465 5f72 6567 6578 2c20 7374  e_date_regex, st
-00001d50: 7269 6e67 290a 0a20 2020 2023 2074 656d  ring)..    # tem
-00001d60: 706c 6174 653a 2031 3834 392f 3530 207c  plate: 1849/50 |
-00001d70: 2031 3834 392d 3530 207c 2031 3834 392f   1849-50 | 1849/
-00001d80: 3138 3530 0a20 2020 2079 6561 725f 7261  1850.    year_ra
-00001d90: 6e67 6520 3d20 7265 6765 782e 7365 6172  nge = regex.sear
-00001da0: 6368 286c 6f6f 6b62 6568 696e 6420 2b20  ch(lookbehind + 
-00001db0: 7965 6172 5f72 6567 6578 202b 2072 225b  year_regex + r"[
-00001dc0: 2f2d 5d28 5c64 7b31 2c34 7d29 2220 2b20  /-](\d{1,4})" + 
-00001dd0: 6c6f 6f6b 6168 6561 642c 2073 7472 696e  lookahead, strin
-00001de0: 6729 0a0a 2020 2020 2320 7465 6d70 6c61  g)..    # templa
-00001df0: 7465 3a20 3139 3037 0a20 2020 2079 6561  te: 1907.    yea
-00001e00: 725f 6f6e 6c79 203d 2072 6567 6578 2e73  r_only = regex.s
-00001e10: 6561 7263 6828 7266 227b 6c6f 6f6b 6265  earch(rf"{lookbe
-00001e20: 6869 6e64 7d7b 7965 6172 5f72 6567 6578  hind}{year_regex
-00001e30: 7d7b 6c6f 6f6b 6168 6561 647d 222c 2073  }{lookahead}", s
-00001e40: 7472 696e 6729 0a0a 2020 2020 7265 733a  tring)..    res:
-00001e50: 2073 7472 207c 204e 6f6e 6520 3d20 4e6f   str | None = No
-00001e60: 6e65 0a20 2020 2069 6620 6973 6f5f 6461  ne.    if iso_da
-00001e70: 7465 3a0a 2020 2020 2020 2020 7265 7320  te:.        res 
-00001e80: 3d20 5f66 726f 6d5f 6973 6f5f 6461 7465  = _from_iso_date
-00001e90: 2869 736f 5f64 6174 6529 0a20 2020 2065  (iso_date).    e
-00001ea0: 6c69 6620 6575 725f 6461 7465 5f72 616e  lif eur_date_ran
-00001eb0: 6765 3a0a 2020 2020 2020 2020 7265 7320  ge:.        res 
-00001ec0: 3d20 5f66 726f 6d5f 6575 725f 6461 7465  = _from_eur_date
-00001ed0: 5f72 616e 6765 2865 7572 5f64 6174 655f  _range(eur_date_
-00001ee0: 7261 6e67 6529 0a20 2020 2065 6c69 6620  range).    elif 
-00001ef0: 6575 725f 6461 7465 3a0a 2020 2020 2020  eur_date:.      
-00001f00: 2020 7265 7320 3d20 5f66 726f 6d5f 6575    res = _from_eu
-00001f10: 725f 6461 7465 2865 7572 5f64 6174 6529  r_date(eur_date)
-00001f20: 0a20 2020 2065 6c69 6620 6d6f 6e74 686e  .    elif monthn
-00001f30: 616d 655f 6461 7465 3a0a 2020 2020 2020  ame_date:.      
-00001f40: 2020 7265 7320 3d20 5f66 726f 6d5f 6d6f    res = _from_mo
-00001f50: 6e74 686e 616d 655f 6461 7465 286d 6f6e  nthname_date(mon
-00001f60: 7468 6e61 6d65 5f64 6174 6529 0a20 2020  thname_date).   
-00001f70: 2065 6c69 6620 7965 6172 5f72 616e 6765   elif year_range
-00001f80: 3a0a 2020 2020 2020 2020 7265 7320 3d20  :.        res = 
-00001f90: 5f66 726f 6d5f 7965 6172 5f72 616e 6765  _from_year_range
-00001fa0: 2879 6561 725f 7261 6e67 6529 0a20 2020  (year_range).   
-00001fb0: 2065 6c69 6620 7965 6172 5f6f 6e6c 793a   elif year_only:
-00001fc0: 0a20 2020 2020 2020 2079 6561 7220 3d20  .        year = 
-00001fd0: 696e 7428 7965 6172 5f6f 6e6c 792e 6772  int(year_only.gr
-00001fe0: 6f75 7028 3029 290a 2020 2020 2020 2020  oup(0)).        
-00001ff0: 7265 7320 3d20 6622 4752 4547 4f52 4941  res = f"GREGORIA
-00002000: 4e3a 4345 3a7b 7965 6172 7d3a 4345 3a7b  N:CE:{year}:CE:{
-00002010: 7965 6172 7d22 0a20 2020 2072 6574 7572  year}".    retur
-00002020: 6e20 7265 730a 0a0a 6465 6620 5f66 726f  n res...def _fro
-00002030: 6d5f 6973 6f5f 6461 7465 2869 736f 5f64  m_iso_date(iso_d
-00002040: 6174 653a 204d 6174 6368 5b73 7472 5d29  ate: Match[str])
-00002050: 202d 3e20 7374 723a 0a20 2020 2079 6561   -> str:.    yea
-00002060: 7220 3d20 696e 7428 6973 6f5f 6461 7465  r = int(iso_date
-00002070: 2e67 726f 7570 2831 2929 0a20 2020 206d  .group(1)).    m
-00002080: 6f6e 7468 203d 2069 6e74 2869 736f 5f64  onth = int(iso_d
-00002090: 6174 652e 6772 6f75 7028 3229 290a 2020  ate.group(2)).  
-000020a0: 2020 6461 7920 3d20 696e 7428 6973 6f5f    day = int(iso_
-000020b0: 6461 7465 2e67 726f 7570 2833 2929 0a20  date.group(3)). 
-000020c0: 2020 2064 6174 6520 3d20 6461 7465 7469     date = dateti
-000020d0: 6d65 2e64 6174 6528 7965 6172 2c20 6d6f  me.date(year, mo
-000020e0: 6e74 682c 2064 6179 290a 2020 2020 7265  nth, day).    re
-000020f0: 7475 726e 2066 2247 5245 474f 5249 414e  turn f"GREGORIAN
-00002100: 3a43 453a 7b64 6174 652e 6973 6f66 6f72  :CE:{date.isofor
-00002110: 6d61 7428 297d 3a43 453a 7b64 6174 652e  mat()}:CE:{date.
-00002120: 6973 6f66 6f72 6d61 7428 297d 220a 0a0a  isoformat()}"...
-00002130: 6465 6620 5f65 7870 616e 645f 325f 6469  def _expand_2_di
-00002140: 6769 745f 7965 6172 2879 6561 723a 2069  git_year(year: i
-00002150: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
-00002160: 6375 7272 656e 745f 7965 6172 203d 2064  current_year = d
-00002170: 6174 6574 696d 652e 6461 7465 2e74 6f64  atetime.date.tod
-00002180: 6179 2829 2e79 6561 7220 2d20 3230 3030  ay().year - 2000
-00002190: 0a20 2020 2069 6620 7965 6172 203c 3d20  .    if year <= 
-000021a0: 6375 7272 656e 745f 7965 6172 3a0a 2020  current_year:.  
-000021b0: 2020 2020 2020 7265 7475 726e 2079 6561        return yea
-000021c0: 7220 2b20 3230 3030 0a20 2020 2065 6c69  r + 2000.    eli
-000021d0: 6620 7965 6172 203c 3d20 3939 3a0a 2020  f year <= 99:.  
-000021e0: 2020 2020 2020 7265 7475 726e 2079 6561        return yea
-000021f0: 7220 2b20 3139 3030 0a20 2020 2065 6c73  r + 1900.    els
-00002200: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00002210: 6e20 7965 6172 0a0a 0a64 6566 205f 6672  n year...def _fr
-00002220: 6f6d 5f65 7572 5f64 6174 655f 7261 6e67  om_eur_date_rang
-00002230: 6528 6575 725f 6461 7465 5f72 616e 6765  e(eur_date_range
-00002240: 3a20 4d61 7463 685b 7374 725d 2920 2d3e  : Match[str]) ->
-00002250: 2073 7472 3a0a 2020 2020 7374 6172 7464   str:.    startd
-00002260: 6179 203d 2069 6e74 2865 7572 5f64 6174  ay = int(eur_dat
-00002270: 655f 7261 6e67 652e 6772 6f75 7028 3129  e_range.group(1)
-00002280: 290a 2020 2020 7374 6172 746d 6f6e 7468  ).    startmonth
-00002290: 203d 2069 6e74 2865 7572 5f64 6174 655f   = int(eur_date_
-000022a0: 7261 6e67 652e 6772 6f75 7028 3229 2920  range.group(2)) 
-000022b0: 6966 2065 7572 5f64 6174 655f 7261 6e67  if eur_date_rang
-000022c0: 652e 6772 6f75 7028 3229 2065 6c73 6520  e.group(2) else 
-000022d0: 696e 7428 6575 725f 6461 7465 5f72 616e  int(eur_date_ran
-000022e0: 6765 2e67 726f 7570 2835 2929 0a20 2020  ge.group(5)).   
-000022f0: 2073 7461 7274 7965 6172 203d 2069 6e74   startyear = int
-00002300: 2865 7572 5f64 6174 655f 7261 6e67 652e  (eur_date_range.
-00002310: 6772 6f75 7028 3329 2920 6966 2065 7572  group(3)) if eur
-00002320: 5f64 6174 655f 7261 6e67 652e 6772 6f75  _date_range.grou
-00002330: 7028 3329 2065 6c73 6520 696e 7428 6575  p(3) else int(eu
-00002340: 725f 6461 7465 5f72 616e 6765 2e67 726f  r_date_range.gro
-00002350: 7570 2836 2929 0a20 2020 2073 7461 7274  up(6)).    start
-00002360: 7965 6172 203d 205f 6578 7061 6e64 5f32  year = _expand_2
-00002370: 5f64 6967 6974 5f79 6561 7228 7374 6172  _digit_year(star
-00002380: 7479 6561 7229 0a20 2020 2065 6e64 6461  tyear).    endda
-00002390: 7920 3d20 696e 7428 6575 725f 6461 7465  y = int(eur_date
-000023a0: 5f72 616e 6765 2e67 726f 7570 2834 2929  _range.group(4))
-000023b0: 0a20 2020 2065 6e64 6d6f 6e74 6820 3d20  .    endmonth = 
-000023c0: 696e 7428 6575 725f 6461 7465 5f72 616e  int(eur_date_ran
-000023d0: 6765 2e67 726f 7570 2835 2929 0a20 2020  ge.group(5)).   
-000023e0: 2065 6e64 7965 6172 203d 2069 6e74 2865   endyear = int(e
-000023f0: 7572 5f64 6174 655f 7261 6e67 652e 6772  ur_date_range.gr
-00002400: 6f75 7028 3629 290a 2020 2020 656e 6479  oup(6)).    endy
-00002410: 6561 7220 3d20 5f65 7870 616e 645f 325f  ear = _expand_2_
-00002420: 6469 6769 745f 7965 6172 2865 6e64 7965  digit_year(endye
-00002430: 6172 290a 2020 2020 7374 6172 7464 6174  ar).    startdat
-00002440: 6520 3d20 6461 7465 7469 6d65 2e64 6174  e = datetime.dat
-00002450: 6528 7374 6172 7479 6561 722c 2073 7461  e(startyear, sta
-00002460: 7274 6d6f 6e74 682c 2073 7461 7274 6461  rtmonth, startda
-00002470: 7929 0a20 2020 2065 6e64 6461 7465 203d  y).    enddate =
-00002480: 2064 6174 6574 696d 652e 6461 7465 2865   datetime.date(e
-00002490: 6e64 7965 6172 2c20 656e 646d 6f6e 7468  ndyear, endmonth
-000024a0: 2c20 656e 6464 6179 290a 2020 2020 6966  , endday).    if
-000024b0: 2065 6e64 6461 7465 203c 2073 7461 7274   enddate < start
-000024c0: 6461 7465 3a0a 2020 2020 2020 2020 7261  date:.        ra
-000024d0: 6973 6520 5661 6c75 6545 7272 6f72 0a20  ise ValueError. 
-000024e0: 2020 2072 6574 7572 6e20 6622 4752 4547     return f"GREG
-000024f0: 4f52 4941 4e3a 4345 3a7b 7374 6172 7464  ORIAN:CE:{startd
-00002500: 6174 652e 6973 6f66 6f72 6d61 7428 297d  ate.isoformat()}
-00002510: 3a43 453a 7b65 6e64 6461 7465 2e69 736f  :CE:{enddate.iso
-00002520: 666f 726d 6174 2829 7d22 0a0a 0a64 6566  format()}"...def
-00002530: 205f 6672 6f6d 5f65 7572 5f64 6174 6528   _from_eur_date(
-00002540: 6575 725f 6461 7465 3a20 4d61 7463 685b  eur_date: Match[
-00002550: 7374 725d 2920 2d3e 2073 7472 3a0a 2020  str]) -> str:.  
-00002560: 2020 7374 6172 7464 6179 203d 2069 6e74    startday = int
-00002570: 2865 7572 5f64 6174 652e 6772 6f75 7028  (eur_date.group(
-00002580: 3129 290a 2020 2020 7374 6172 746d 6f6e  1)).    startmon
-00002590: 7468 203d 2069 6e74 2865 7572 5f64 6174  th = int(eur_dat
-000025a0: 652e 6772 6f75 7028 3229 290a 2020 2020  e.group(2)).    
-000025b0: 7374 6172 7479 6561 7220 3d20 696e 7428  startyear = int(
-000025c0: 6575 725f 6461 7465 2e67 726f 7570 2833  eur_date.group(3
-000025d0: 2929 0a20 2020 2073 7461 7274 7965 6172  )).    startyear
-000025e0: 203d 205f 6578 7061 6e64 5f32 5f64 6967   = _expand_2_dig
-000025f0: 6974 5f79 6561 7228 7374 6172 7479 6561  it_year(startyea
-00002600: 7229 0a20 2020 2064 6174 6520 3d20 6461  r).    date = da
-00002610: 7465 7469 6d65 2e64 6174 6528 7374 6172  tetime.date(star
-00002620: 7479 6561 722c 2073 7461 7274 6d6f 6e74  tyear, startmont
-00002630: 682c 2073 7461 7274 6461 7929 0a20 2020  h, startday).   
-00002640: 2072 6574 7572 6e20 6622 4752 4547 4f52   return f"GREGOR
-00002650: 4941 4e3a 4345 3a7b 6461 7465 2e69 736f  IAN:CE:{date.iso
-00002660: 666f 726d 6174 2829 7d3a 4345 3a7b 6461  format()}:CE:{da
-00002670: 7465 2e69 736f 666f 726d 6174 2829 7d22  te.isoformat()}"
-00002680: 0a0a 0a64 6566 205f 6672 6f6d 5f6d 6f6e  ...def _from_mon
-00002690: 7468 6e61 6d65 5f64 6174 6528 6d6f 6e74  thname_date(mont
-000026a0: 686e 616d 655f 6461 7465 3a20 4d61 7463  hname_date: Matc
-000026b0: 685b 7374 725d 2920 2d3e 2073 7472 3a0a  h[str]) -> str:.
-000026c0: 2020 2020 6461 7920 3d20 696e 7428 6d6f      day = int(mo
-000026d0: 6e74 686e 616d 655f 6461 7465 2e67 726f  nthname_date.gro
-000026e0: 7570 2832 2929 0a20 2020 206d 6f6e 7468  up(2)).    month
-000026f0: 203d 205f 6d6f 6e74 6873 5f64 6963 745b   = _months_dict[
-00002700: 6d6f 6e74 686e 616d 655f 6461 7465 2e67  monthname_date.g
-00002710: 726f 7570 2831 295d 0a20 2020 2079 6561  roup(1)].    yea
-00002720: 7220 3d20 696e 7428 6d6f 6e74 686e 616d  r = int(monthnam
-00002730: 655f 6461 7465 2e67 726f 7570 2833 2929  e_date.group(3))
-00002740: 0a20 2020 2064 6174 6520 3d20 6461 7465  .    date = date
-00002750: 7469 6d65 2e64 6174 6528 7965 6172 2c20  time.date(year, 
-00002760: 6d6f 6e74 682c 2064 6179 290a 2020 2020  month, day).    
-00002770: 7265 7475 726e 2066 2247 5245 474f 5249  return f"GREGORI
-00002780: 414e 3a43 453a 7b64 6174 652e 6973 6f66  AN:CE:{date.isof
-00002790: 6f72 6d61 7428 297d 3a43 453a 7b64 6174  ormat()}:CE:{dat
-000027a0: 652e 6973 6f66 6f72 6d61 7428 297d 220a  e.isoformat()}".
-000027b0: 0a0a 6465 6620 5f66 726f 6d5f 7965 6172  ..def _from_year
-000027c0: 5f72 616e 6765 2879 6561 725f 7261 6e67  _range(year_rang
-000027d0: 653a 204d 6174 6368 5b73 7472 5d29 202d  e: Match[str]) -
-000027e0: 3e20 7374 723a 0a20 2020 2073 7461 7274  > str:.    start
-000027f0: 7965 6172 203d 2069 6e74 2879 6561 725f  year = int(year_
-00002800: 7261 6e67 652e 6772 6f75 7028 3129 290a  range.group(1)).
-00002810: 2020 2020 656e 6479 6561 7220 3d20 696e      endyear = in
-00002820: 7428 7965 6172 5f72 616e 6765 2e67 726f  t(year_range.gro
-00002830: 7570 2832 2929 0a20 2020 2069 6620 656e  up(2)).    if en
-00002840: 6479 6561 7220 2f2f 2031 3020 3d3d 2030  dyear // 10 == 0
-00002850: 3a0a 2020 2020 2020 2020 2320 656e 6479  :.        # endy
-00002860: 6561 7220 6973 206f 6e6c 7920 312d 6469  ear is only 1-di
-00002870: 6769 743a 2061 6464 2074 6865 2066 6972  git: add the fir
-00002880: 7374 2032 2d33 2064 6967 6974 7320 6f66  st 2-3 digits of
-00002890: 2073 7461 7274 7965 6172 0a20 2020 2020   startyear.     
-000028a0: 2020 2065 6e64 7965 6172 203d 2073 7461     endyear = sta
-000028b0: 7274 7965 6172 202f 2f20 3130 202a 2031  rtyear // 10 * 1
-000028c0: 3020 2b20 656e 6479 6561 720a 2020 2020  0 + endyear.    
-000028d0: 656c 6966 2065 6e64 7965 6172 202f 2f20  elif endyear // 
-000028e0: 3130 3020 3d3d 2030 3a0a 2020 2020 2020  100 == 0:.      
-000028f0: 2020 2320 656e 6479 6561 7220 6973 206f    # endyear is o
-00002900: 6e6c 7920 322d 6469 6769 743a 2061 6464  nly 2-digit: add
-00002910: 2074 6865 2066 6972 7374 2031 2d32 2064   the first 1-2 d
-00002920: 6967 6974 7320 6f66 2073 7461 7274 7965  igits of startye
-00002930: 6172 0a20 2020 2020 2020 2065 6e64 7965  ar.        endye
-00002940: 6172 203d 2073 7461 7274 7965 6172 202f  ar = startyear /
-00002950: 2f20 3130 3020 2a20 3130 3020 2b20 656e  / 100 * 100 + en
-00002960: 6479 6561 720a 2020 2020 6966 2065 6e64  dyear.    if end
-00002970: 7965 6172 203c 3d20 7374 6172 7479 6561  year <= startyea
-00002980: 723a 0a20 2020 2020 2020 2072 6169 7365  r:.        raise
-00002990: 2056 616c 7565 4572 726f 720a 2020 2020   ValueError.    
-000029a0: 7265 7475 726e 2066 2247 5245 474f 5249  return f"GREGORI
-000029b0: 414e 3a43 453a 7b73 7461 7274 7965 6172  AN:CE:{startyear
-000029c0: 7d3a 4345 3a7b 656e 6479 6561 727d 220a  }:CE:{endyear}".
-000029d0: 0a0a 6465 6620 7072 6570 6172 655f 7661  ..def prepare_va
-000029e0: 6c75 6528 0a20 2020 2076 616c 7565 3a20  lue(.    value: 
-000029f0: 556e 696f 6e5b 5072 6f70 6572 7479 456c  Union[PropertyEl
-00002a00: 656d 656e 742c 2073 7472 2c20 696e 742c  ement, str, int,
-00002a10: 2066 6c6f 6174 2c20 626f 6f6c 2c20 4974   float, bool, It
-00002a20: 6572 6162 6c65 5b55 6e69 6f6e 5b50 726f  erable[Union[Pro
-00002a30: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
-00002a40: 722c 2069 6e74 2c20 666c 6f61 742c 2062  r, int, float, b
-00002a50: 6f6f 6c5d 5d5d 2c0a 2920 2d3e 206c 6973  ool]]],.) -> lis
-00002a60: 745b 5072 6f70 6572 7479 456c 656d 656e  t[PropertyElemen
-00002a70: 745d 3a0a 2020 2020 2222 220a 2020 2020  t]:.    """.    
-00002a80: 5468 6973 206d 6574 686f 6420 7472 616e  This method tran
-00002a90: 7366 6f72 6d73 2074 6865 2070 6172 616d  sforms the param
-00002aa0: 6574 6572 2022 7661 6c75 6522 2066 726f  eter "value" fro
-00002ab0: 6d20 6120 6d61 6b65 5f2a 5f70 726f 7028  m a make_*_prop(
-00002ac0: 2920 6d65 7468 6f64 2069 6e74 6f20 6120  ) method into a 
-00002ad0: 6c69 7374 206f 6620 5072 6f70 6572 7479  list of Property
-00002ae0: 456c 656d 656e 7473 2e20 2276 616c 7565  Elements. "value
-00002af0: 2220 6973 0a20 2020 2070 6173 7365 6420  " is.    passed 
-00002b00: 6f6e 2074 6f20 7468 6973 206d 6574 686f  on to this metho
-00002b10: 6420 6173 2069 7420 7761 7320 7265 6365  d as it was rece
-00002b20: 6976 6564 2e0a 0a20 2020 2041 7267 733a  ived...    Args:
-00002b30: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
-00002b40: 2276 616c 7565 2220 6173 2072 6563 6569  "value" as recei
-00002b50: 7665 6420 6672 6f6d 2074 6865 2063 616c  ved from the cal
-00002b60: 6c65 720a 0a20 2020 2052 6574 7572 6e73  ler..    Returns
-00002b70: 3a0a 2020 2020 2020 2020 6120 6c69 7374  :.        a list
-00002b80: 206f 6620 5072 6f70 6572 7479 456c 656d   of PropertyElem
-00002b90: 656e 7473 0a20 2020 2022 2222 0a20 2020  ents.    """.   
-00002ba0: 2023 206d 616b 6520 7375 7265 2074 6861   # make sure tha
-00002bb0: 7420 2276 616c 7565 2220 6973 206c 6973  t "value" is lis
-00002bc0: 742d 6c69 6b65 0a20 2020 2069 6620 6e6f  t-like.    if no
-00002bd0: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
-00002be0: 7565 2c20 4974 6572 6162 6c65 2920 6f72  ue, Iterable) or
-00002bf0: 2069 7369 6e73 7461 6e63 6528 7661 6c75   isinstance(valu
-00002c00: 652c 2073 7472 293a 0a20 2020 2020 2020  e, str):.       
-00002c10: 2076 616c 7565 203d 205b 7661 6c75 655d   value = [value]
-00002c20: 0a0a 2020 2020 2320 6d61 6b65 2061 2050  ..    # make a P
-00002c30: 726f 7065 7274 7945 6c65 6d65 6e74 206f  ropertyElement o
-00002c40: 7574 206f 6620 6974 7320 656c 656d 656e  ut of its elemen
-00002c50: 7473 2c20 6966 206e 6563 6573 7361 7279  ts, if necessary
-00002c60: 2e0a 2020 2020 7265 7475 726e 205b 7820  ..    return [x 
-00002c70: 6966 2069 7369 6e73 7461 6e63 6528 782c  if isinstance(x,
-00002c80: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00002c90: 2920 656c 7365 2050 726f 7065 7274 7945  ) else PropertyE
-00002ca0: 6c65 6d65 6e74 2878 2920 666f 7220 7820  lement(x) for x 
-00002cb0: 696e 2076 616c 7565 5d0a 0a0a 6465 6620  in value]...def 
-00002cc0: 6d61 6b65 5f72 6f6f 7428 0a20 2020 2073  make_root(.    s
-00002cd0: 686f 7274 636f 6465 3a20 7374 722c 0a20  hortcode: str,. 
-00002ce0: 2020 2064 6566 6175 6c74 5f6f 6e74 6f6c     default_ontol
-00002cf0: 6f67 793a 2073 7472 2c0a 2920 2d3e 2065  ogy: str,.) -> e
-00002d00: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
-00002d10: 2020 2022 2222 0a20 2020 2053 7461 7274     """.    Start
-00002d20: 2062 7569 6c64 696e 6720 796f 7572 2058   building your X
-00002d30: 4d4c 2064 6f63 756d 656e 7420 6279 2063  ML document by c
-00002d40: 7265 6174 696e 6720 7468 6520 726f 6f74  reating the root
-00002d50: 2065 6c65 6d65 6e74 203c 6b6e 6f72 613e   element <knora>
-00002d60: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00002d70: 2020 2020 2073 686f 7274 636f 6465 3a20       shortcode: 
-00002d80: 5468 6520 7368 6f72 7463 6f64 6520 6f66  The shortcode of
-00002d90: 2074 6869 7320 7072 6f6a 6563 7420 6173   this project as
-00002da0: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-00002db0: 4a53 4f4e 2070 726f 6a65 6374 2066 696c  JSON project fil
-00002dc0: 650a 2020 2020 2020 2020 6465 6661 756c  e.        defaul
-00002dd0: 745f 6f6e 746f 6c6f 6779 3a20 6f6e 6520  t_ontology: one 
-00002de0: 6f66 2074 6865 206f 6e74 6f6c 6f67 6965  of the ontologie
-00002df0: 7320 6f66 2074 6865 204a 534f 4e20 7072  s of the JSON pr
-00002e00: 6f6a 6563 7420 6669 6c65 0a0a 2020 2020  oject file..    
-00002e10: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00002e20: 2054 6865 2072 6f6f 7420 656c 656d 656e   The root elemen
-00002e30: 7420 3c6b 6e6f 7261 3e2e 0a0a 2020 2020  t <knora>...    
-00002e40: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-00002e50: 2020 3e3e 3e20 726f 6f74 203d 2065 7863    >>> root = exc
-00002e60: 656c 3278 6d6c 2e6d 616b 655f 726f 6f74  el2xml.make_root
-00002e70: 2873 686f 7274 636f 6465 3d73 686f 7274  (shortcode=short
-00002e80: 636f 6465 2c20 6465 6661 756c 745f 6f6e  code, default_on
-00002e90: 746f 6c6f 6779 3d64 6566 6175 6c74 5f6f  tology=default_o
-00002ea0: 6e74 6f6c 6f67 7929 0a20 2020 2020 2020  ntology).       
-00002eb0: 203e 3e3e 2072 6f6f 7420 3d20 6578 6365   >>> root = exce
-00002ec0: 6c32 786d 6c2e 6170 7065 6e64 5f70 6572  l2xml.append_per
-00002ed0: 6d69 7373 696f 6e73 2872 6f6f 7429 0a0a  missions(root)..
-00002ee0: 2020 2020 5365 6520 6874 7470 733a 2f2f      See https://
-00002ef0: 646f 6373 2e64 6173 6368 2e73 7769 7373  docs.dasch.swiss
-00002f00: 2f6c 6174 6573 742f 4453 502d 544f 4f4c  /latest/DSP-TOOL
-00002f10: 532f 6669 6c65 2d66 6f72 6d61 7473 2f78  S/file-formats/x
-00002f20: 6d6c 2d64 6174 612d 6669 6c65 2f23 7468  ml-data-file/#th
-00002f30: 652d 726f 6f74 2d65 6c65 6d65 6e74 2d6b  e-root-element-k
-00002f40: 6e6f 7261 0a20 2020 2022 2222 0a20 2020  nora.    """.   
-00002f50: 2073 6368 656d 615f 7572 6c20 3d20 2268   schema_url = "h
-00002f60: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-00002f70: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-00002f80: 2f64 6173 6368 2d73 7769 7373 2f64 7370  /dasch-swiss/dsp
-00002f90: 2d74 6f6f 6c73 2f6d 6169 6e2f 7372 632f  -tools/main/src/
-00002fa0: 6473 705f 746f 6f6c 732f 7265 736f 7572  dsp_tools/resour
-00002fb0: 6365 732f 7363 6865 6d61 2f64 6174 612e  ces/schema/data.
-00002fc0: 7873 6422 0a20 2020 2073 6368 656d 615f  xsd".    schema_
-00002fd0: 6c6f 6361 7469 6f6e 5f6b 6579 203d 2073  location_key = s
-00002fe0: 7472 2865 7472 6565 2e51 4e61 6d65 2822  tr(etree.QName("
-00002ff0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-00003000: 672f 3230 3031 2f58 4d4c 5363 6865 6d61  g/2001/XMLSchema
-00003010: 2d69 6e73 7461 6e63 6522 2c20 2273 6368  -instance", "sch
-00003020: 656d 614c 6f63 6174 696f 6e22 2929 0a20  emaLocation")). 
-00003030: 2020 2073 6368 656d 615f 6c6f 6361 7469     schema_locati
-00003040: 6f6e 5f76 616c 7565 203d 2066 2268 7474  on_value = f"htt
-00003050: 7073 3a2f 2f64 6173 6368 2e73 7769 7373  ps://dasch.swiss
-00003060: 2f73 6368 656d 6120 7b73 6368 656d 615f  /schema {schema_
-00003070: 7572 6c7d 220a 2020 2020 7265 7475 726e  url}".    return
-00003080: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-00003090: 2020 2020 2020 2020 227b 2573 7d6b 6e6f          "{%s}kno
-000030a0: 7261 2220 2520 786d 6c5f 6e61 6d65 7370  ra" % xml_namesp
-000030b0: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-000030c0: 2020 2020 2020 2061 7474 7269 623d 7b0a         attrib={.
-000030d0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
-000030e0: 6d61 5f6c 6f63 6174 696f 6e5f 6b65 793a  ma_location_key:
-000030f0: 2073 6368 656d 615f 6c6f 6361 7469 6f6e   schema_location
-00003100: 5f76 616c 7565 2c0a 2020 2020 2020 2020  _value,.        
-00003110: 2020 2020 2273 686f 7274 636f 6465 223a      "shortcode":
-00003120: 2073 686f 7274 636f 6465 2c0a 2020 2020   shortcode,.    
-00003130: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00003140: 2d6f 6e74 6f6c 6f67 7922 3a20 6465 6661  -ontology": defa
-00003150: 756c 745f 6f6e 746f 6c6f 6779 2c0a 2020  ult_ontology,.  
-00003160: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00003170: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-00003180: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
-00003190: 0a0a 6465 6620 6170 7065 6e64 5f70 6572  ..def append_per
-000031a0: 6d69 7373 696f 6e73 2872 6f6f 745f 656c  missions(root_el
-000031b0: 656d 656e 743a 2065 7472 6565 2e5f 456c  ement: etree._El
-000031c0: 656d 656e 7429 202d 3e20 6574 7265 652e  ement) -> etree.
-000031d0: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
-000031e0: 220a 2020 2020 4166 7465 7220 6861 7669  ".    After havi
-000031f0: 6e67 2063 7265 6174 6564 2061 2072 6f6f  ng created a roo
-00003200: 7420 656c 656d 656e 742c 2063 616c 6c20  t element, call 
-00003210: 7468 6973 206d 6574 686f 6420 746f 2061  this method to a
-00003220: 7070 656e 6420 7468 6520 666f 7572 2070  ppend the four p
-00003230: 6572 6d69 7373 696f 6e73 2022 7265 732d  ermissions "res-
-00003240: 6465 6661 756c 7422 2c0a 2020 2020 2272  default",.    "r
-00003250: 6573 2d72 6573 7472 6963 7465 6422 2c20  es-restricted", 
-00003260: 2270 726f 702d 6465 6661 756c 7422 2c20  "prop-default", 
-00003270: 616e 6420 2270 726f 702d 7265 7374 7269  and "prop-restri
-00003280: 6374 6564 2220 746f 2069 742e 2054 6865  cted" to it. The
-00003290: 7365 2066 6f75 7220 7065 726d 6973 7369  se four permissi
-000032a0: 6f6e 7320 6172 6520 6120 676f 6f64 2062  ons are a good b
-000032b0: 6173 6973 2074 6f0a 2020 2020 7374 6172  asis to.    star
-000032c0: 7420 7769 7468 2c20 6275 7420 7265 6d65  t with, but reme
-000032d0: 6d62 6572 2074 6861 7420 7468 6579 2063  mber that they c
-000032e0: 616e 2062 6520 6164 6170 7465 642c 2061  an be adapted, a
-000032f0: 6e64 2074 6861 7420 6f74 6865 7220 7065  nd that other pe
-00003300: 726d 6973 7369 6f6e 7320 6361 6e20 6265  rmissions can be
-00003310: 2064 6566 696e 6564 2069 6e73 7465 6164   defined instead
-00003320: 206f 6620 7468 6573 652e 0a0a 2020 2020   of these...    
-00003330: 4172 6773 3a0a 2020 2020 2020 2020 726f  Args:.        ro
-00003340: 6f74 5f65 6c65 6d65 6e74 3a20 5468 6520  ot_element: The 
-00003350: 584d 4c20 726f 6f74 2065 6c65 6d65 6e74  XML root element
-00003360: 203c 6b6e 6f72 613e 2063 7265 6174 6564   <knora> created
-00003370: 2062 7920 6d61 6b65 5f72 6f6f 7428 290a   by make_root().
-00003380: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00003390: 2020 2020 2020 5468 6520 726f 6f74 2065        The root e
-000033a0: 6c65 6d65 6e74 2077 6974 6820 7468 6520  lement with the 
-000033b0: 666f 7572 2070 6572 6d69 7373 696f 6e20  four permission 
-000033c0: 626c 6f63 6b73 2061 7070 656e 6465 640a  blocks appended.
-000033d0: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-000033e0: 2020 2020 2020 203e 3e3e 2072 6f6f 7420         >>> root 
-000033f0: 3d20 6578 6365 6c32 786d 6c2e 6d61 6b65  = excel2xml.make
-00003400: 5f72 6f6f 7428 7368 6f72 7463 6f64 653d  _root(shortcode=
-00003410: 7368 6f72 7463 6f64 652c 2064 6566 6175  shortcode, defau
-00003420: 6c74 5f6f 6e74 6f6c 6f67 793d 6465 6661  lt_ontology=defa
-00003430: 756c 745f 6f6e 746f 6c6f 6779 290a 2020  ult_ontology).  
-00003440: 2020 2020 2020 3e3e 3e20 726f 6f74 203d        >>> root =
-00003450: 2065 7863 656c 3278 6d6c 2e61 7070 656e   excel2xml.appen
-00003460: 645f 7065 726d 6973 7369 6f6e 7328 726f  d_permissions(ro
-00003470: 6f74 290a 0a20 2020 2053 6565 2068 7474  ot)..    See htt
-00003480: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-00003490: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
-000034a0: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
-000034b0: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
-000034c0: 652f 2364 6573 6372 6962 696e 672d 7065  e/#describing-pe
-000034d0: 726d 6973 7369 6f6e 732d 7769 7468 2d70  rmissions-with-p
-000034e0: 6572 6d69 7373 696f 6e73 2d65 6c65 6d65  ermissions-eleme
-000034f0: 6e74 730a 2020 2020 2222 220a 0a20 2020  nts.    """..   
-00003500: 2050 4552 4d49 5353 494f 4e53 203d 2045   PERMISSIONS = E
-00003510: 2e70 6572 6d69 7373 696f 6e73 0a20 2020  .permissions.   
-00003520: 2041 4c4c 4f57 203d 2045 2e61 6c6c 6f77   ALLOW = E.allow
-00003530: 0a20 2020 2023 206c 786d 6c2e 6275 696c  .    # lxml.buil
-00003540: 6465 722e 4520 6973 2061 206d 6f72 6520  der.E is a more 
-00003550: 736f 7068 6973 7469 6361 7465 6420 656c  sophisticated el
-00003560: 656d 656e 7420 6661 6374 6f72 7920 7468  ement factory th
-00003570: 616e 2065 7472 6565 2e45 6c65 6d65 6e74  an etree.Element
-00003580: 2e0a 2020 2020 2320 452e 7461 6720 6973  ..    # E.tag is
-00003590: 2065 7175 6976 616c 656e 7420 746f 2045   equivalent to E
-000035a0: 2822 7461 6722 2920 616e 6420 7265 7375  ("tag") and resu
-000035b0: 6c74 7320 696e 203c 7461 673e 0a0a 2020  lts in <tag>..  
-000035c0: 2020 7265 735f 6465 6661 756c 7420 3d20    res_default = 
-000035d0: 6574 7265 652e 456c 656d 656e 7428 227b  etree.Element("{
-000035e0: 2573 7d70 6572 6d69 7373 696f 6e73 2220  %s}permissions" 
-000035f0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-00003600: 6d61 705b 4e6f 6e65 5d2c 2069 643d 2272  map[None], id="r
-00003610: 6573 2d64 6566 6175 6c74 2229 0a20 2020  es-default").   
-00003620: 2072 6573 5f64 6566 6175 6c74 2e61 7070   res_default.app
-00003630: 656e 6428 414c 4c4f 5728 2256 222c 2067  end(ALLOW("V", g
-00003640: 726f 7570 3d22 556e 6b6e 6f77 6e55 7365  roup="UnknownUse
-00003650: 7222 2929 0a20 2020 2072 6573 5f64 6566  r")).    res_def
-00003660: 6175 6c74 2e61 7070 656e 6428 414c 4c4f  ault.append(ALLO
-00003670: 5728 2256 222c 2067 726f 7570 3d22 4b6e  W("V", group="Kn
-00003680: 6f77 6e55 7365 7222 2929 0a20 2020 2072  ownUser")).    r
-00003690: 6573 5f64 6566 6175 6c74 2e61 7070 656e  es_default.appen
-000036a0: 6428 414c 4c4f 5728 2244 222c 2067 726f  d(ALLOW("D", gro
-000036b0: 7570 3d22 5072 6f6a 6563 744d 656d 6265  up="ProjectMembe
-000036c0: 7222 2929 0a20 2020 2072 6573 5f64 6566  r")).    res_def
-000036d0: 6175 6c74 2e61 7070 656e 6428 414c 4c4f  ault.append(ALLO
-000036e0: 5728 2243 5222 2c20 6772 6f75 703d 2250  W("CR", group="P
-000036f0: 726f 6a65 6374 4164 6d69 6e22 2929 0a20  rojectAdmin")). 
-00003700: 2020 2072 6573 5f64 6566 6175 6c74 2e61     res_default.a
-00003710: 7070 656e 6428 414c 4c4f 5728 2243 5222  ppend(ALLOW("CR"
-00003720: 2c20 6772 6f75 703d 2243 7265 6174 6f72  , group="Creator
-00003730: 2229 290a 2020 2020 726f 6f74 5f65 6c65  ")).    root_ele
-00003740: 6d65 6e74 2e61 7070 656e 6428 7265 735f  ment.append(res_
-00003750: 6465 6661 756c 7429 0a0a 2020 2020 7265  default)..    re
-00003760: 735f 7265 7374 7269 6374 6564 203d 2050  s_restricted = P
-00003770: 4552 4d49 5353 494f 4e53 2869 643d 2272  ERMISSIONS(id="r
-00003780: 6573 2d72 6573 7472 6963 7465 6422 290a  es-restricted").
-00003790: 2020 2020 7265 735f 7265 7374 7269 6374      res_restrict
-000037a0: 6564 2e61 7070 656e 6428 414c 4c4f 5728  ed.append(ALLOW(
-000037b0: 224d 222c 2067 726f 7570 3d22 5072 6f6a  "M", group="Proj
-000037c0: 6563 744d 656d 6265 7222 2929 0a20 2020  ectMember")).   
-000037d0: 2072 6573 5f72 6573 7472 6963 7465 642e   res_restricted.
-000037e0: 6170 7065 6e64 2841 4c4c 4f57 2822 4352  append(ALLOW("CR
-000037f0: 222c 2067 726f 7570 3d22 5072 6f6a 6563  ", group="Projec
-00003800: 7441 646d 696e 2229 290a 2020 2020 7265  tAdmin")).    re
-00003810: 735f 7265 7374 7269 6374 6564 2e61 7070  s_restricted.app
-00003820: 656e 6428 414c 4c4f 5728 2243 5222 2c20  end(ALLOW("CR", 
-00003830: 6772 6f75 703d 2243 7265 6174 6f72 2229  group="Creator")
-00003840: 290a 2020 2020 726f 6f74 5f65 6c65 6d65  ).    root_eleme
-00003850: 6e74 2e61 7070 656e 6428 7265 735f 7265  nt.append(res_re
-00003860: 7374 7269 6374 6564 290a 0a20 2020 2070  stricted)..    p
-00003870: 726f 705f 6465 6661 756c 7420 3d20 5045  rop_default = PE
-00003880: 524d 4953 5349 4f4e 5328 6964 3d22 7072  RMISSIONS(id="pr
-00003890: 6f70 2d64 6566 6175 6c74 2229 0a20 2020  op-default").   
-000038a0: 2070 726f 705f 6465 6661 756c 742e 6170   prop_default.ap
-000038b0: 7065 6e64 2841 4c4c 4f57 2822 5622 2c20  pend(ALLOW("V", 
-000038c0: 6772 6f75 703d 2255 6e6b 6e6f 776e 5573  group="UnknownUs
-000038d0: 6572 2229 290a 2020 2020 7072 6f70 5f64  er")).    prop_d
-000038e0: 6566 6175 6c74 2e61 7070 656e 6428 414c  efault.append(AL
-000038f0: 4c4f 5728 2256 222c 2067 726f 7570 3d22  LOW("V", group="
-00003900: 4b6e 6f77 6e55 7365 7222 2929 0a20 2020  KnownUser")).   
-00003910: 2070 726f 705f 6465 6661 756c 742e 6170   prop_default.ap
-00003920: 7065 6e64 2841 4c4c 4f57 2822 4422 2c20  pend(ALLOW("D", 
-00003930: 6772 6f75 703d 2250 726f 6a65 6374 4d65  group="ProjectMe
-00003940: 6d62 6572 2229 290a 2020 2020 7072 6f70  mber")).    prop
-00003950: 5f64 6566 6175 6c74 2e61 7070 656e 6428  _default.append(
-00003960: 414c 4c4f 5728 2243 5222 2c20 6772 6f75  ALLOW("CR", grou
-00003970: 703d 2250 726f 6a65 6374 4164 6d69 6e22  p="ProjectAdmin"
-00003980: 2929 0a20 2020 2070 726f 705f 6465 6661  )).    prop_defa
-00003990: 756c 742e 6170 7065 6e64 2841 4c4c 4f57  ult.append(ALLOW
-000039a0: 2822 4352 222c 2067 726f 7570 3d22 4372  ("CR", group="Cr
-000039b0: 6561 746f 7222 2929 0a20 2020 2072 6f6f  eator")).    roo
-000039c0: 745f 656c 656d 656e 742e 6170 7065 6e64  t_element.append
-000039d0: 2870 726f 705f 6465 6661 756c 7429 0a0a  (prop_default)..
-000039e0: 2020 2020 7072 6f70 5f72 6573 7472 6963      prop_restric
-000039f0: 7465 6420 3d20 5045 524d 4953 5349 4f4e  ted = PERMISSION
-00003a00: 5328 6964 3d22 7072 6f70 2d72 6573 7472  S(id="prop-restr
-00003a10: 6963 7465 6422 290a 2020 2020 7072 6f70  icted").    prop
-00003a20: 5f72 6573 7472 6963 7465 642e 6170 7065  _restricted.appe
-00003a30: 6e64 2841 4c4c 4f57 2822 4d22 2c20 6772  nd(ALLOW("M", gr
-00003a40: 6f75 703d 2250 726f 6a65 6374 4d65 6d62  oup="ProjectMemb
-00003a50: 6572 2229 290a 2020 2020 7072 6f70 5f72  er")).    prop_r
-00003a60: 6573 7472 6963 7465 642e 6170 7065 6e64  estricted.append
-00003a70: 2841 4c4c 4f57 2822 4352 222c 2067 726f  (ALLOW("CR", gro
-00003a80: 7570 3d22 5072 6f6a 6563 7441 646d 696e  up="ProjectAdmin
-00003a90: 2229 290a 2020 2020 7072 6f70 5f72 6573  ")).    prop_res
-00003aa0: 7472 6963 7465 642e 6170 7065 6e64 2841  tricted.append(A
-00003ab0: 4c4c 4f57 2822 4352 222c 2067 726f 7570  LLOW("CR", group
-00003ac0: 3d22 4372 6561 746f 7222 2929 0a20 2020  ="Creator")).   
-00003ad0: 2072 6f6f 745f 656c 656d 656e 742e 6170   root_element.ap
-00003ae0: 7065 6e64 2870 726f 705f 7265 7374 7269  pend(prop_restri
-00003af0: 6374 6564 290a 0a20 2020 2072 6574 7572  cted)..    retur
-00003b00: 6e20 726f 6f74 5f65 6c65 6d65 6e74 0a0a  n root_element..
-00003b10: 0a64 6566 206d 616b 655f 7265 736f 7572  .def make_resour
-00003b20: 6365 2820 2023 206e 6f71 613a 2044 3431  ce(  # noqa: D41
-00003b30: 3720 2875 6e64 6f63 756d 656e 7465 642d  7 (undocumented-
-00003b40: 7061 7261 6d29 0a20 2020 206c 6162 656c  param).    label
-00003b50: 3a20 7374 722c 0a20 2020 2072 6573 7479  : str,.    resty
-00003b60: 7065 3a20 7374 722c 0a20 2020 2069 643a  pe: str,.    id:
-00003b70: 2073 7472 2c0a 2020 2020 7065 726d 6973   str,.    permis
-00003b80: 7369 6f6e 733a 2073 7472 203d 2022 7265  sions: str = "re
-00003b90: 732d 6465 6661 756c 7422 2c0a 2020 2020  s-default",.    
-00003ba0: 6172 6b3a 204f 7074 696f 6e61 6c5b 7374  ark: Optional[st
-00003bb0: 725d 203d 204e 6f6e 652c 0a20 2020 2069  r] = None,.    i
-00003bc0: 7269 3a20 4f70 7469 6f6e 616c 5b73 7472  ri: Optional[str
-00003bd0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6372  ] = None,.    cr
-00003be0: 6561 7469 6f6e 5f64 6174 653a 204f 7074  eation_date: Opt
-00003bf0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-00003c00: 652c 0a29 202d 3e20 6574 7265 652e 5f45  e,.) -> etree._E
-00003c10: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
-00003c20: 2020 2020 4372 6561 7465 7320 616e 2065      Creates an e
-00003c30: 6d70 7479 2072 6573 6f75 7263 6520 656c  mpty resource el
-00003c40: 656d 656e 742c 2077 6974 6820 7468 6520  ement, with the 
-00003c50: 6174 7472 6962 7574 6573 2061 7320 7370  attributes as sp
-00003c60: 6563 6966 6965 6420 6279 2074 6865 2061  ecified by the a
-00003c70: 7267 756d 656e 7473 0a0a 2020 2020 4172  rguments..    Ar
-00003c80: 6773 3a0a 2020 2020 2020 2020 5468 6520  gs:.        The 
-00003c90: 6172 6775 6d65 6e74 7320 636f 7272 6573  arguments corres
-00003ca0: 706f 6e64 2074 6f20 7468 6520 6174 7472  pond to the attr
-00003cb0: 6962 7574 6573 206f 6620 7468 6520 3c72  ibutes of the <r
-00003cc0: 6573 6f75 7263 653e 2065 6c65 6d65 6e74  esource> element
-00003cd0: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
-00003ce0: 2020 2020 2020 2020 5468 6520 7265 736f          The reso
-00003cf0: 7572 6365 2065 6c65 6d65 6e74 2c20 7769  urce element, wi
-00003d00: 7468 6f75 7420 616e 7920 6368 696c 6472  thout any childr
-00003d10: 656e 2c20 6275 7420 7769 7468 2074 6865  en, but with the
-00003d20: 2061 7474 7269 6275 7465 730a 2020 2020   attributes.    
-00003d30: 2020 2020 6060 3c72 6573 6f75 7263 6520      ``<resource 
-00003d40: 6c61 6265 6c3d 6c61 6265 6c20 7265 7374  label=label rest
-00003d50: 7970 653d 7265 7374 7970 6520 6964 3d69  ype=restype id=i
-00003d60: 6420 7065 726d 6973 7369 6f6e 733d 7065  d permissions=pe
-00003d70: 726d 6973 7369 6f6e 7320 6172 6b3d 6172  rmissions ark=ar
-00003d80: 6b20 6972 693d 6972 693e 3c2f 7265 736f  k iri=iri></reso
-00003d90: 7572 6365 3e60 600a 0a20 2020 2052 6169  urce>``..    Rai
-00003da0: 7365 733a 0a20 2020 2020 2020 2057 6172  ses:.        War
-00003db0: 6e69 6e67 3a20 6966 2062 6f74 6820 616e  ning: if both an
-00003dc0: 2041 524b 2061 6e64 2061 6e20 4952 4920   ARK and an IRI 
-00003dd0: 6172 6520 7072 6f76 6964 6564 0a20 2020  are provided.   
-00003de0: 2020 2020 2042 6173 6545 7272 6f72 3a20       BaseError: 
-00003df0: 6966 2074 6865 2063 7265 6174 696f 6e20  if the creation 
-00003e00: 6461 7465 2069 7320 696e 7661 6c69 640a  date is invalid.
-00003e10: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-00003e20: 2020 2020 2020 203e 3e3e 2072 6573 6f75         >>> resou
-00003e30: 7263 6520 3d20 6578 6365 6c32 786d 6c2e  rce = excel2xml.
-00003e40: 6d61 6b65 5f72 6573 6f75 7263 6528 2e2e  make_resource(..
-00003e50: 2e29 0a20 2020 2020 2020 203e 3e3e 2072  .).        >>> r
-00003e60: 6573 6f75 7263 652e 6170 7065 6e64 2865  esource.append(e
-00003e70: 7863 656c 3278 6d6c 2e6d 616b 655f 7465  xcel2xml.make_te
-00003e80: 7874 5f70 726f 7028 2e2e 2e29 290a 2020  xt_prop(...)).  
-00003e90: 2020 2020 2020 3e3e 3e20 726f 6f74 2e61        >>> root.a
-00003ea0: 7070 656e 6428 7265 736f 7572 6365 290a  ppend(resource).
-00003eb0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-00003ec0: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
-00003ed0: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
-00003ee0: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
-00003ef0: 786d 6c2d 6461 7461 2d66 696c 652f 2364  xml-data-file/#d
-00003f00: 6573 6372 6962 696e 672d 7265 736f 7572  escribing-resour
-00003f10: 6365 732d 7769 7468 2d74 6865 2d72 6573  ces-with-the-res
-00003f20: 6f75 7263 652d 656c 656d 656e 740a 2020  ource-element.  
-00003f30: 2020 2222 220a 2020 2020 6966 206e 6f74    """.    if not
-00003f40: 2063 6865 636b 5f6e 6f74 6e61 286c 6162   check_notna(lab
-00003f50: 656c 293a 0a20 2020 2020 2020 2077 6172  el):.        war
-00003f60: 6e69 6e67 732e 7761 726e 2866 2257 4152  nings.warn(f"WAR
-00003f70: 4e49 4e47 3a20 596f 7572 2072 6573 6f75  NING: Your resou
-00003f80: 7263 6527 7320 6c61 6265 6c20 6c6f 6f6b  rce's label look
-00003f90: 7320 7375 7370 6963 696f 7573 2028 7265  s suspicious (re
-00003fa0: 736f 7572 6365 2077 6974 6820 6964 2027  source with id '
-00003fb0: 7b69 647d 2720 616e 6420 6c61 6265 6c20  {id}' and label 
-00003fc0: 277b 6c61 6265 6c7d 2729 2229 0a20 2020  '{label}')").   
-00003fd0: 2069 6620 6e6f 7420 6368 6563 6b5f 6e6f   if not check_no
-00003fe0: 746e 6128 6964 293a 0a20 2020 2020 2020  tna(id):.       
-00003ff0: 2077 6172 6e69 6e67 732e 7761 726e 2866   warnings.warn(f
-00004000: 2257 4152 4e49 4e47 3a20 596f 7572 2072  "WARNING: Your r
-00004010: 6573 6f75 7263 6527 7320 6964 206c 6f6f  esource's id loo
-00004020: 6b73 2073 7573 7069 6369 6f75 7320 2872  ks suspicious (r
-00004030: 6573 6f75 7263 6520 7769 7468 2069 6420  esource with id 
-00004040: 277b 6964 7d27 2061 6e64 206c 6162 656c  '{id}' and label
-00004050: 2027 7b6c 6162 656c 7d27 2229 0a20 2020   '{label}'").   
-00004060: 206b 7761 7267 7320 3d20 7b22 6c61 6265   kwargs = {"labe
-00004070: 6c22 3a20 6c61 6265 6c2c 2022 7265 7374  l": label, "rest
-00004080: 7970 6522 3a20 7265 7374 7970 652c 2022  ype": restype, "
-00004090: 6964 223a 2069 642c 2022 7065 726d 6973  id": id, "permis
-000040a0: 7369 6f6e 7322 3a20 7065 726d 6973 7369  sions": permissi
-000040b0: 6f6e 732c 2022 6e73 6d61 7022 3a20 786d  ons, "nsmap": xm
-000040c0: 6c5f 6e61 6d65 7370 6163 655f 6d61 707d  l_namespace_map}
-000040d0: 0a20 2020 2069 6620 6172 6b3a 0a20 2020  .    if ark:.   
-000040e0: 2020 2020 206b 7761 7267 735b 2261 726b       kwargs["ark
-000040f0: 225d 203d 2061 726b 0a20 2020 2069 6620  "] = ark.    if 
-00004100: 6972 693a 0a20 2020 2020 2020 206b 7761  iri:.        kwa
-00004110: 7267 735b 2269 7269 225d 203d 2069 7269  rgs["iri"] = iri
-00004120: 0a20 2020 2069 6620 6172 6b20 616e 6420  .    if ark and 
-00004130: 6972 693a 0a20 2020 2020 2020 2077 6172  iri:.        war
-00004140: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
-00004150: 2020 2020 2020 2020 6622 426f 7468 2041          f"Both A
-00004160: 524b 2061 6e64 2049 5249 2077 6572 6520  RK and IRI were 
-00004170: 7072 6f76 6964 6564 2066 6f72 2072 6573  provided for res
-00004180: 6f75 7263 6520 277b 6c61 6265 6c7d 2720  ource '{label}' 
-00004190: 287b 6964 7d29 2e20 5468 6520 4152 4b20  ({id}). The ARK 
-000041a0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
-000041b0: 6520 4952 492e 222c 0a20 2020 2020 2020  e IRI.",.       
-000041c0: 2020 2020 2073 7461 636b 6c65 7665 6c3d       stacklevel=
-000041d0: 322c 0a20 2020 2020 2020 2029 0a20 2020  2,.        ).   
-000041e0: 2069 6620 6372 6561 7469 6f6e 5f64 6174   if creation_dat
-000041f0: 653a 0a20 2020 2020 2020 2074 7279 3a0a  e:.        try:.
-00004200: 2020 2020 2020 2020 2020 2020 4461 7465              Date
-00004210: 5469 6d65 5374 616d 7028 6372 6561 7469  TimeStamp(creati
-00004220: 6f6e 5f64 6174 6529 0a20 2020 2020 2020  on_date).       
-00004230: 2065 7863 6570 7420 4261 7365 4572 726f   except BaseErro
-00004240: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00004250: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
-00004260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004270: 6622 5468 6520 7265 736f 7572 6365 2027  f"The resource '
-00004280: 7b6c 6162 656c 7d27 2028 4944 3a20 7b69  {label}' (ID: {i
-00004290: 647d 2920 6861 7320 616e 2069 6e76 616c  d}) has an inval
-000042a0: 6964 2063 7265 6174 696f 6e20 6461 7465  id creation date
-000042b0: 2027 7b63 7265 6174 696f 6e5f 6461 7465   '{creation_date
-000042c0: 7d27 2e20 220a 2020 2020 2020 2020 2020  }'. ".          
-000042d0: 2020 2020 2020 6622 4469 6420 796f 7520        f"Did you 
-000042e0: 7065 7268 6170 7320 666f 7267 6574 2074  perhaps forget t
-000042f0: 6865 2074 696d 657a 6f6e 653f 220a 2020  he timezone?".  
-00004300: 2020 2020 2020 2020 2020 2920 6672 6f6d            ) from
-00004310: 204e 6f6e 650a 2020 2020 2020 2020 6b77   None.        kw
-00004320: 6172 6773 5b22 6372 6561 7469 6f6e 5f64  args["creation_d
-00004330: 6174 6522 5d20 3d20 6372 6561 7469 6f6e  ate"] = creation
-00004340: 5f64 6174 650a 0a20 2020 2072 6574 7572  _date..    retur
-00004350: 6e20 6574 7265 652e 456c 656d 656e 7428  n etree.Element(
-00004360: 227b 2573 7d72 6573 6f75 7263 6522 2025  "{%s}resource" %
-00004370: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-00004380: 6170 5b4e 6f6e 655d 2c20 2a2a 6b77 6172  ap[None], **kwar
-00004390: 6773 2920 2023 2074 7970 653a 2069 676e  gs)  # type: ign
-000043a0: 6f72 655b 6172 672d 7479 7065 5d0a 0a0a  ore[arg-type]...
-000043b0: 6465 6620 6d61 6b65 5f62 6974 7374 7265  def make_bitstre
-000043c0: 616d 5f70 726f 7028 0a20 2020 2070 6174  am_prop(.    pat
-000043d0: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
-000043e0: 2e50 6174 684c 696b 655b 416e 795d 5d2c  .PathLike[Any]],
-000043f0: 0a20 2020 2070 6572 6d69 7373 696f 6e73  .    permissions
-00004400: 3a20 7374 7220 3d20 2270 726f 702d 6465  : str = "prop-de
-00004410: 6661 756c 7422 2c0a 2020 2020 6368 6563  fault",.    chec
-00004420: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 652c  k: bool = False,
-00004430: 0a20 2020 2063 616c 6c69 6e67 5f72 6573  .    calling_res
-00004440: 6f75 7263 653a 2073 7472 203d 2022 222c  ource: str = "",
-00004450: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-00004460: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-00004470: 2020 4372 6561 7465 7320 6120 6269 7473    Creates a bits
-00004480: 7472 6561 6d20 656c 656d 656e 7420 7468  tream element th
-00004490: 6174 2070 6f69 6e74 7320 746f 2022 7061  at points to "pa
-000044a0: 7468 222e 0a0a 2020 2020 4172 6773 3a0a  th"...    Args:.
-000044b0: 2020 2020 2020 2020 7061 7468 3a20 7061          path: pa
-000044c0: 7468 2074 6f20 6120 7661 6c69 6420 6669  th to a valid fi
-000044d0: 6c65 2074 6861 7420 7769 6c6c 2062 6520  le that will be 
-000044e0: 7570 6c6f 6164 6564 0a20 2020 2020 2020  uploaded.       
-000044f0: 2070 6572 6d69 7373 696f 6e73 3a20 7065   permissions: pe
-00004500: 726d 6973 7369 6f6e 7320 7374 7269 6e67  rmissions string
-00004510: 0a20 2020 2020 2020 2063 6865 636b 3a20  .        check: 
-00004520: 6966 2054 7275 652c 2069 7373 7565 2061  if True, issue a
-00004530: 2077 6172 6e69 6e67 2069 6620 7468 6520   warning if the 
-00004540: 7061 7468 2064 6f65 736e 2774 2070 6f69  path doesn't poi
-00004550: 6e74 2074 6f20 616e 2065 7869 7374 696e  nt to an existin
-00004560: 6720 6669 6c65 0a20 2020 2020 2020 2063  g file.        c
-00004570: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
-00004580: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
-00004590: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
-000045a0: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
-000045b0: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
-000045c0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-000045d0: 2020 5761 726e 696e 673a 2069 6620 7468    Warning: if th
-000045e0: 6520 7061 7468 2064 6f65 736e 2774 2070  e path doesn't p
-000045f0: 6f69 6e74 2074 6f20 616e 2065 7869 7374  oint to an exist
-00004600: 696e 6720 6669 6c65 2028 6f6e 6c79 2069  ing file (only i
-00004610: 6620 6368 6563 6b3d 5472 7565 290a 0a20  f check=True).. 
-00004620: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00004630: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
-00004640: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
-00004650: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
-00004660: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00004670: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
-00004680: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
-00004690: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
-000046a0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-000046b0: 3e3e 3e20 7265 736f 7572 6365 203d 2065  >>> resource = e
-000046c0: 7863 656c 3278 6d6c 2e6d 616b 655f 7265  xcel2xml.make_re
-000046d0: 736f 7572 6365 282e 2e2e 290a 2020 2020  source(...).    
-000046e0: 2020 2020 3e3e 3e20 7265 736f 7572 6365      >>> resource
-000046f0: 2e61 7070 656e 6428 6578 6365 6c32 786d  .append(excel2xm
-00004700: 6c2e 6d61 6b65 5f62 6974 7374 7265 616d  l.make_bitstream
-00004710: 5f70 726f 7028 2264 6174 612f 696d 6167  _prop("data/imag
-00004720: 6573 2f74 7265 652e 6a70 6722 2929 0a20  es/tree.jpg")). 
-00004730: 2020 2020 2020 203e 3e3e 2072 6f6f 742e         >>> root.
-00004740: 6170 7065 6e64 2872 6573 6f75 7263 6529  append(resource)
-00004750: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-00004760: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
-00004770: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
-00004780: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
-00004790: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
-000047a0: 6269 7473 7472 6561 6d0a 2020 2020 2222  bitstream.    ""
-000047b0: 220a 0a20 2020 2069 6620 6368 6563 6b20  "..    if check 
-000047c0: 616e 6420 6e6f 7420 5061 7468 2870 6174  and not Path(pat
-000047d0: 6829 2e69 735f 6669 6c65 2829 3a0a 2020  h).is_file():.  
-000047e0: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-000047f0: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00004800: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
-00004810: 7469 6f6e 2069 6e20 6269 7473 7472 6561  tion in bitstrea
-00004820: 6d20 7461 6720 6f66 2072 6573 6f75 7263  m tag of resourc
-00004830: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
-00004840: 7572 6365 7d27 3a20 220a 2020 2020 2020  urce}': ".      
-00004850: 2020 2020 2020 6622 5468 6520 666f 6c6c        f"The foll
-00004860: 6f77 696e 6720 7061 7468 2064 6f65 736e  owing path doesn
-00004870: 2774 2070 6f69 6e74 2074 6f20 6120 6669  't point to a fi
-00004880: 6c65 3a20 7b70 6174 687d 222c 0a20 2020  le: {path}",.   
-00004890: 2020 2020 2020 2020 2073 7461 636b 6c65           stackle
-000048a0: 7665 6c3d 322c 0a20 2020 2020 2020 2029  vel=2,.        )
-000048b0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-000048c0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-000048d0: 2020 2020 227b 2573 7d62 6974 7374 7265      "{%s}bitstre
-000048e0: 616d 2220 2520 786d 6c5f 6e61 6d65 7370  am" % xml_namesp
-000048f0: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-00004900: 2020 2020 2020 2070 6572 6d69 7373 696f         permissio
-00004910: 6e73 3d70 6572 6d69 7373 696f 6e73 2c0a  ns=permissions,.
-00004920: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-00004930: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-00004940: 0a20 2020 2029 0a20 2020 2070 726f 705f  .    ).    prop_
-00004950: 2e74 6578 7420 3d20 7374 7228 7061 7468  .text = str(path
-00004960: 290a 2020 2020 7265 7475 726e 2070 726f  ).    return pro
-00004970: 705f 0a0a 0a64 6566 205f 666f 726d 6174  p_...def _format
-00004980: 5f62 6f6f 6c28 0a20 2020 2075 6e66 6f72  _bool(.    unfor
-00004990: 6d61 7474 6564 3a20 556e 696f 6e5b 626f  matted: Union[bo
-000049a0: 6f6c 2c20 7374 722c 2069 6e74 2c20 666c  ol, str, int, fl
-000049b0: 6f61 745d 2c0a 2020 2020 6e61 6d65 3a20  oat],.    name: 
-000049c0: 7374 722c 0a20 2020 2063 616c 6c69 6e67  str,.    calling
-000049d0: 5f72 6573 6f75 7263 653a 2073 7472 2c0a  _resource: str,.
-000049e0: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-000049f0: 220a 2020 2020 5468 6973 206d 6574 686f  ".    This metho
-00004a00: 6420 7461 6b65 7320 616e 2075 6e66 6f72  d takes an unfor
-00004a10: 6d61 7474 6564 2062 6f6f 6c65 616e 2d6c  matted boolean-l
-00004a20: 696b 6520 7661 6c75 652c 2061 6e64 2074  ike value, and t
-00004a30: 7261 6e73 666f 726d 7320 6974 2069 6e74  ransforms it int
-00004a40: 6f20 7468 6520 7374 7269 6e67 2076 616c  o the string val
-00004a50: 7565 7320 2274 7275 6522 206f 7220 2266  ues "true" or "f
-00004a60: 616c 7365 222e 0a0a 2020 2020 4172 6773  alse"...    Args
-00004a70: 3a0a 2020 2020 2020 2020 756e 666f 726d  :.        unform
-00004a80: 6174 7465 643a 2062 6f6f 6c65 616e 2d6c  atted: boolean-l
-00004a90: 696b 6520 7661 6c75 650a 2020 2020 2020  ike value.      
-00004aa0: 2020 6e61 6d65 3a20 7072 6f70 6572 7479    name: property
-00004ab0: 206e 616d 652c 2066 6f72 2062 6574 7465   name, for bette
-00004ac0: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
-00004ad0: 0a20 2020 2020 2020 2063 616c 6c69 6e67  .        calling
-00004ae0: 5f72 6573 6f75 7263 653a 2072 6573 6f75  _resource: resou
-00004af0: 7263 6520 6e61 6d65 2c20 666f 7220 6265  rce name, for be
+00000190: 746f 6f6c 732e 6d6f 6465 6c73 2e63 7573  tools.models.cus
+000001a0: 746f 6d5f 7761 726e 696e 6773 2069 6d70  tom_warnings imp
+000001b0: 6f72 7420 4473 7054 6f6f 6c73 4675 7475  ort DspToolsFutu
+000001c0: 7265 5761 726e 696e 670a 6672 6f6d 2064  reWarning.from d
+000001d0: 7370 5f74 6f6f 6c73 2e6d 6f64 656c 732e  sp_tools.models.
+000001e0: 6461 7465 7469 6d65 7374 616d 7020 696d  datetimestamp im
+000001f0: 706f 7274 2044 6174 6554 696d 6553 7461  port DateTimeSta
+00000200: 6d70 0a66 726f 6d20 6473 705f 746f 6f6c  mp.from dsp_tool
+00000210: 732e 6d6f 6465 6c73 2e65 7863 6570 7469  s.models.excepti
+00000220: 6f6e 7320 696d 706f 7274 2042 6173 6545  ons import BaseE
+00000230: 7272 6f72 0a66 726f 6d20 6473 705f 746f  rror.from dsp_to
+00000240: 6f6c 732e 7574 696c 732e 6461 7465 5f75  ols.utils.date_u
+00000250: 7469 6c20 696d 706f 7274 2069 735f 6675  til import is_fu
+00000260: 6c6c 5f64 6174 650a 6672 6f6d 2064 7370  ll_date.from dsp
+00000270: 5f74 6f6f 6c73 2e75 7469 6c73 2e73 6861  _tools.utils.sha
+00000280: 7265 6420 696d 706f 7274 2063 6865 636b  red import check
+00000290: 5f6e 6f74 6e61 0a66 726f 6d20 6473 705f  _notna.from dsp_
+000002a0: 746f 6f6c 732e 7574 696c 732e 7368 6172  tools.utils.shar
+000002b0: 6564 2069 6d70 6f72 7420 7369 6d70 6c69  ed import simpli
+000002c0: 6679 5f6e 616d 650a 6672 6f6d 2064 7370  fy_name.from dsp
+000002d0: 5f74 6f6f 6c73 2e75 7469 6c73 2e75 7269  _tools.utils.uri
+000002e0: 5f75 7469 6c20 696d 706f 7274 2069 735f  _util import is_
+000002f0: 7572 690a 6672 6f6d 2064 7370 5f74 6f6f  uri.from dsp_too
+00000300: 6c73 2e75 7469 6c73 2e78 6d6c 5f76 616c  ls.utils.xml_val
+00000310: 6964 6174 696f 6e20 696d 706f 7274 2076  idation import v
+00000320: 616c 6964 6174 655f 786d 6c0a 0a23 2072  alidate_xml..# r
+00000330: 7566 663a 206e 6f71 613a 2045 3530 3120  uff: noqa: E501 
+00000340: 286c 696e 652d 746f 6f2d 6c6f 6e67 290a  (line-too-long).
+00000350: 0a0a 786d 6c5f 6e61 6d65 7370 6163 655f  ..xml_namespace_
+00000360: 6d61 7020 3d20 7b4e 6f6e 653a 2022 6874  map = {None: "ht
+00000370: 7470 733a 2f2f 6461 7363 682e 7377 6973  tps://dasch.swis
+00000380: 732f 7363 6865 6d61 222c 2022 7873 6922  s/schema", "xsi"
+00000390: 3a20 2268 7474 703a 2f2f 7777 772e 7733  : "http://www.w3
+000003a0: 2e6f 7267 2f32 3030 312f 584d 4c53 6368  .org/2001/XMLSch
+000003b0: 656d 612d 696e 7374 616e 6365 227d 0a0a  ema-instance"}..
+000003c0: 0a64 6566 206d 616b 655f 7873 645f 6964  .def make_xsd_id
+000003d0: 5f63 6f6d 7061 7469 626c 6528 7374 7269  _compatible(stri
+000003e0: 6e67 3a20 7374 7229 202d 3e20 7374 723a  ng: str) -> str:
+000003f0: 0a20 2020 2022 2222 0a20 2020 204d 616b  .    """.    Mak
+00000400: 6520 6120 7374 7269 6e67 2063 6f6d 7061  e a string compa
+00000410: 7469 626c 6520 7769 7468 2074 6865 2063  tible with the c
+00000420: 6f6e 7374 7261 696e 7473 206f 6620 7873  onstraints of xs
+00000430: 643a 4944 2c20 736f 2074 6861 7420 6974  d:ID, so that it
+00000440: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
+00000450: 2269 6422 2061 7474 7269 6275 7465 206f  "id" attribute o
+00000460: 6620 6120 3c72 6573 6f75 7263 653e 0a20  f a <resource>. 
+00000470: 2020 2074 6167 2e20 416e 2078 7364 3a49     tag. An xsd:I
+00000480: 4420 6d75 7374 206e 6f74 2063 6f6e 7461  D must not conta
+00000490: 696e 2073 7065 6369 616c 2063 6861 7261  in special chara
+000004a0: 6374 6572 732c 2061 6e64 2069 7420 6d75  cters, and it mu
+000004b0: 7374 2062 6520 756e 6971 7565 2069 6e20  st be unique in 
+000004c0: 7468 6520 646f 6375 6d65 6e74 2e0a 0a20  the document... 
+000004d0: 2020 2054 6869 7320 6d65 7468 6f64 2072     This method r
+000004e0: 6570 6c61 6365 7320 7468 6520 696c 6c65  eplaces the ille
+000004f0: 6761 6c20 6368 6172 6163 7465 7273 2062  gal characters b
+00000500: 7920 225f 2220 616e 6420 6170 7065 6e64  y "_" and append
+00000510: 7320 6120 7261 6e64 6f6d 2063 6f6d 706f  s a random compo
+00000520: 6e65 6e74 2074 6f20 7468 6520 7374 7269  nent to the stri
+00000530: 6e67 2074 6f20 6d61 6b65 2069 7420 756e  ng to make it un
+00000540: 6971 7565 2e0a 0a20 2020 2054 6865 2073  ique...    The s
+00000550: 7472 696e 6720 6d75 7374 2063 6f6e 7461  tring must conta
+00000560: 696e 2061 7420 6c65 6173 7420 6f6e 6520  in at least one 
+00000570: 556e 6963 6f64 6520 6c65 7474 6572 2028  Unicode letter (
+00000580: 6d61 7463 6869 6e67 2074 6865 2072 6567  matching the reg
+00000590: 6578 2060 605c 5c70 7b4c 7d60 6029 2c20  ex ``\\p{L}``), 
+000005a0: 756e 6465 7273 636f 7265 2c20 212c 203f  underscore, !, ?
+000005b0: 2c20 6f72 206e 756d 6265 722c 0a20 2020  , or number,.   
+000005c0: 2062 7574 206d 7573 7420 6e6f 7420 6265   but must not be
+000005d0: 2022 4e6f 6e65 222c 2022 3c4e 413e 222c   "None", "<NA>",
+000005e0: 2022 4e2f 4122 2c20 6f72 2022 2d22 2e20   "N/A", or "-". 
+000005f0: 4f74 6865 7277 6973 652c 2061 2042 6173  Otherwise, a Bas
+00000600: 6545 7272 6f72 2077 696c 6c20 6265 2072  eError will be r
+00000610: 6169 7365 642e 0a0a 2020 2020 4172 6773  aised...    Args
+00000620: 3a0a 2020 2020 2020 2020 7374 7269 6e67  :.        string
+00000630: 3a20 696e 7075 7420 7374 7269 6e67 0a0a  : input string..
+00000640: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00000650: 2020 2020 4261 7365 4572 726f 723a 2069      BaseError: i
+00000660: 6620 7468 6520 696e 7075 7420 6361 6e6e  f the input cann
+00000670: 6f74 2062 6520 7472 616e 7366 6f72 6d65  ot be transforme
+00000680: 6420 746f 2061 6e20 7873 643a 4944 0a0a  d to an xsd:ID..
+00000690: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000006a0: 2020 2020 2061 6e20 7873 6420 4944 2062       an xsd ID b
+000006b0: 6173 6564 206f 6e20 7468 6520 696e 7075  ased on the inpu
+000006c0: 7420 7374 7269 6e67 0a20 2020 2022 2222  t string.    """
+000006d0: 0a0a 2020 2020 6966 206e 6f74 2069 7369  ..    if not isi
+000006e0: 6e73 7461 6e63 6528 7374 7269 6e67 2c20  nstance(string, 
+000006f0: 7374 7229 206f 7220 6e6f 7420 6368 6563  str) or not chec
+00000700: 6b5f 6e6f 746e 6128 7374 7269 6e67 293a  k_notna(string):
+00000710: 0a20 2020 2020 2020 2072 6169 7365 2042  .        raise B
+00000720: 6173 6545 7272 6f72 2866 2254 6865 2069  aseError(f"The i
+00000730: 6e70 7574 2027 7b73 7472 696e 677d 2720  nput '{string}' 
+00000740: 6361 6e6e 6f74 2062 6520 7472 616e 7366  cannot be transf
+00000750: 6f72 6d65 6420 746f 2061 6e20 7873 643a  ormed to an xsd:
+00000760: 4944 2229 0a0a 2020 2020 2320 6966 2073  ID")..    # if s
+00000770: 7461 7274 206f 6620 7374 7269 6e67 2069  tart of string i
+00000780: 7320 6e65 6974 6865 7220 6c65 7474 6572  s neither letter
+00000790: 206e 6f72 2075 6e64 6572 7363 6f72 652c   nor underscore,
+000007a0: 2061 6464 2061 6e20 756e 6465 7273 636f   add an undersco
+000007b0: 7265 0a20 2020 2072 6573 203d 2072 6567  re.    res = reg
+000007c0: 6578 2e73 7562 2872 225e 283f 3d5b 5e41  ex.sub(r"^(?=[^A
+000007d0: 2d5a 612d 7a5f 5d29 222c 2022 5f22 2c20  -Za-z_])", "_", 
+000007e0: 7374 7269 6e67 290a 0a20 2020 2023 2072  string)..    # r
+000007f0: 6570 6c61 6365 2061 6c6c 2069 6c6c 6567  eplace all illeg
+00000800: 616c 2063 6861 7261 6374 6572 7320 6279  al characters by
+00000810: 2075 6e64 6572 7363 6f72 650a 2020 2020   underscore.    
+00000820: 7265 7320 3d20 7265 6765 782e 7375 6228  res = regex.sub(
+00000830: 7222 5b5e 5c77 5f5c 2d2e 5d22 2c20 225f  r"[^\w_\-.]", "_
+00000840: 222c 2072 6573 2c20 666c 6167 733d 7265  ", res, flags=re
+00000850: 6765 782e 4153 4349 4929 0a0a 2020 2020  gex.ASCII)..    
+00000860: 2320 6164 6420 7575 6964 0a20 2020 205f  # add uuid.    _
+00000870: 7575 6964 203d 2075 7569 642e 7575 6964  uuid = uuid.uuid
+00000880: 3428 290a 2020 2020 7265 7320 3d20 6622  4().    res = f"
+00000890: 7b72 6573 7d5f 7b5f 7575 6964 7d22 0a0a  {res}_{_uuid}"..
+000008a0: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+000008b0: 0a64 6566 205f 6669 6e64 5f66 7265 6e63  .def _find_frenc
+000008c0: 685f 6263 5f64 6174 6528 0a20 2020 2073  h_bc_date(.    s
+000008d0: 7472 696e 673a 2073 7472 2c0a 2020 2020  tring: str,.    
+000008e0: 6c6f 6f6b 6265 6869 6e64 3a20 7374 722c  lookbehind: str,
+000008f0: 0a20 2020 206c 6f6f 6b61 6865 6164 3a20  .    lookahead: 
+00000900: 7374 722c 0a29 202d 3e20 4f70 7469 6f6e  str,.) -> Option
+00000910: 616c 5b73 7472 5d3a 0a20 2020 2066 7265  al[str]:.    fre
+00000920: 6e63 685f 6263 5f72 6567 6578 203d 2072  nch_bc_regex = r
+00000930: 2261 7628 3f3a 5c2e 207c 5c2e 7c20 294a  "av(?:\. |\.| )J
+00000940: 5c2e 3f2d 3f43 5c2e 3f22 0a20 2020 2069  \.?-?C\.?".    i
+00000950: 6620 6e6f 7420 7265 6765 782e 7365 6172  f not regex.sear
+00000960: 6368 2866 7265 6e63 685f 6263 5f72 6567  ch(french_bc_reg
+00000970: 6578 2c20 7374 7269 6e67 293a 0a20 2020  ex, string):.   
+00000980: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00000990: 0a0a 2020 2020 7965 6172 5f72 6567 6578  ..    year_regex
+000009a0: 203d 2072 225c 647b 312c 357d 220a 2020   = r"\d{1,5}".  
+000009b0: 2020 7365 705f 7265 6765 7820 3d20 7222    sep_regex = r"
+000009c0: 203f 2d20 3f22 0a0a 2020 2020 7965 6172   ?- ?"..    year
+000009d0: 5f72 616e 6765 5f72 6567 6578 203d 2072  _range_regex = r
+000009e0: 6622 7b6c 6f6f 6b62 6568 696e 647d 287b  f"{lookbehind}({
+000009f0: 7965 6172 5f72 6567 6578 7d29 7b73 6570  year_regex}){sep
+00000a00: 5f72 6567 6578 7d28 7b79 6561 725f 7265  _regex}({year_re
+00000a10: 6765 787d 2920 7b66 7265 6e63 685f 6263  gex}) {french_bc
+00000a20: 5f72 6567 6578 7d7b 6c6f 6f6b 6168 6561  _regex}{lookahea
+00000a30: 647d 220a 2020 2020 7965 6172 5f72 616e  d}".    year_ran
+00000a40: 6765 203d 2072 6567 6578 2e73 6561 7263  ge = regex.searc
+00000a50: 6828 7965 6172 5f72 616e 6765 5f72 6567  h(year_range_reg
+00000a60: 6578 2c20 7374 7269 6e67 290a 2020 2020  ex, string).    
+00000a70: 6966 2079 6561 725f 7261 6e67 653a 0a20  if year_range:. 
+00000a80: 2020 2020 2020 2073 7461 7274 5f79 6561         start_yea
+00000a90: 7220 3d20 696e 7428 7965 6172 5f72 616e  r = int(year_ran
+00000aa0: 6765 2e67 726f 7570 2831 2929 0a20 2020  ge.group(1)).   
+00000ab0: 2020 2020 2065 6e64 5f79 6561 7220 3d20       end_year = 
+00000ac0: 696e 7428 7965 6172 5f72 616e 6765 2e67  int(year_range.g
+00000ad0: 726f 7570 2832 2929 0a20 2020 2020 2020  roup(2)).       
+00000ae0: 2069 6620 656e 645f 7965 6172 203e 2073   if end_year > s
+00000af0: 7461 7274 5f79 6561 723a 0a20 2020 2020  tart_year:.     
+00000b00: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00000b10: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+00000b20: 6e20 6622 4752 4547 4f52 4941 4e3a 4243  n f"GREGORIAN:BC
+00000b30: 3a7b 7374 6172 745f 7965 6172 7d3a 4243  :{start_year}:BC
+00000b40: 3a7b 656e 645f 7965 6172 7d22 0a0a 2020  :{end_year}"..  
+00000b50: 2020 7369 6e67 6c65 5f79 6561 725f 7265    single_year_re
+00000b60: 6765 7820 3d20 7266 227b 6c6f 6f6b 6265  gex = rf"{lookbe
+00000b70: 6869 6e64 7d28 7b79 6561 725f 7265 6765  hind}({year_rege
+00000b80: 787d 2920 7b66 7265 6e63 685f 6263 5f72  x}) {french_bc_r
+00000b90: 6567 6578 7d7b 6c6f 6f6b 6168 6561 647d  egex}{lookahead}
+00000ba0: 220a 2020 2020 7369 6e67 6c65 5f79 6561  ".    single_yea
+00000bb0: 7220 3d20 7265 6765 782e 7365 6172 6368  r = regex.search
+00000bc0: 2873 696e 676c 655f 7965 6172 5f72 6567  (single_year_reg
+00000bd0: 6578 2c20 7374 7269 6e67 290a 2020 2020  ex, string).    
+00000be0: 6966 2073 696e 676c 655f 7965 6172 3a0a  if single_year:.
+00000bf0: 2020 2020 2020 2020 7374 6172 745f 7965          start_ye
+00000c00: 6172 203d 2069 6e74 2873 696e 676c 655f  ar = int(single_
+00000c10: 7965 6172 2e67 726f 7570 2831 2929 0a20  year.group(1)). 
+00000c20: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+00000c30: 4752 4547 4f52 4941 4e3a 4243 3a7b 7374  GREGORIAN:BC:{st
+00000c40: 6172 745f 7965 6172 7d3a 4243 3a7b 7374  art_year}:BC:{st
+00000c50: 6172 745f 7965 6172 7d22 0a0a 2020 2020  art_year}"..    
+00000c60: 7265 7475 726e 204e 6f6e 650a 0a0a 6465  return None...de
+00000c70: 6620 6669 6e64 5f64 6174 655f 696e 5f73  f find_date_in_s
+00000c80: 7472 696e 6728 7374 7269 6e67 3a20 7374  tring(string: st
+00000c90: 7229 202d 3e20 4f70 7469 6f6e 616c 5b73  r) -> Optional[s
+00000ca0: 7472 5d3a 0a20 2020 2022 2222 0a20 2020  tr]:.    """.   
+00000cb0: 2043 6865 636b 7320 6966 2061 2073 7472   Checks if a str
+00000cc0: 696e 6720 636f 6e74 6169 6e73 2061 2064  ing contains a d
+00000cd0: 6174 6520 7661 6c75 6520 2873 696e 676c  ate value (singl
+00000ce0: 6520 6461 7465 2c20 6f72 2064 6174 6520  e date, or date 
+00000cf0: 7261 6e67 6529 2c0a 2020 2020 616e 6420  range),.    and 
+00000d00: 7265 7475 726e 7320 7468 6520 6669 7273  returns the firs
+00000d10: 7420 666f 756e 6420 6461 7465 2061 7320  t found date as 
+00000d20: 4453 502d 666f 726d 6174 7465 6420 7374  DSP-formatted st
+00000d30: 7269 6e67 2e0a 2020 2020 5265 7475 726e  ring..    Return
+00000d40: 7320 4e6f 6e65 2069 6620 6e6f 2064 6174  s None if no dat
+00000d50: 6520 7761 7320 666f 756e 642e 0a0a 2020  e was found...  
+00000d60: 2020 4e6f 7465 733a 0a20 2020 2020 2020    Notes:.       
+00000d70: 202d 2041 6c6c 2064 6174 6573 2061 7265   - All dates are
+00000d80: 2069 6e74 6572 7072 6574 6564 2069 6e20   interpreted in 
+00000d90: 7468 6520 4368 7269 7374 6961 6e20 6572  the Christian er
+00000da0: 6120 616e 6420 7468 6520 4772 6567 6f72  a and the Gregor
+00000db0: 6961 6e20 6361 6c65 6e64 6172 2e0a 2020  ian calendar..  
+00000dc0: 2020 2020 2020 2d20 4243 2064 6174 6573        - BC dates
+00000dd0: 2061 7265 206f 6e6c 7920 7375 7070 6f72   are only suppor
+00000de0: 7465 6420 696e 2046 7265 6e63 6820 6e6f  ted in French no
+00000df0: 7461 7469 6f6e 2028 652e 672e 2031 3030  tation (e.g. 100
+00000e00: 302d 3930 3020 6176 2e20 4a2e 2d43 2e29  0-900 av. J.-C.)
+00000e10: 2e0a 2020 2020 2020 2020 2d20 5468 6520  ..        - The 
+00000e20: 7965 6172 7320 3030 3030 2d32 3939 3920  years 0000-2999 
+00000e30: 6172 6520 7375 7070 6f72 7465 642c 2069  are supported, i
+00000e40: 6e20 332f 342d 6469 6769 7420 666f 726d  n 3/4-digit form
+00000e50: 2e0a 2020 2020 2020 2020 2d20 4461 7465  ..        - Date
+00000e60: 7320 7772 6974 7465 6e20 7769 7468 2073  s written with s
+00000e70: 6c61 7368 6573 2061 7265 2061 6c77 6179  lashes are alway
+00000e80: 7320 696e 7465 7270 7265 7465 6420 696e  s interpreted in
+00000e90: 2061 2045 7572 6f70 6561 6e20 6d61 6e6e   a European mann
+00000ea0: 6572 3a20 352f 3131 2f32 3032 3120 6973  er: 5/11/2021 is
+00000eb0: 2074 6865 2035 7468 206f 6620 4e6f 7665   the 5th of Nove
+00000ec0: 6d62 6572 2e0a 2020 2020 2020 2020 2d20  mber..        - 
+00000ed0: 496e 2074 6865 2045 7572 6f70 6561 6e20  In the European 
+00000ee0: 6e6f 7461 7469 6f6e 2c20 322d 6469 6769  notation, 2-digi
+00000ef0: 7420 7965 6172 7320 6172 6520 6578 7061  t years are expa
+00000f00: 6e64 6564 2074 6f20 3420 6469 6769 7473  nded to 4 digits
+00000f10: 2c20 7769 7468 2074 6865 2063 7572 7265  , with the curre
+00000f20: 6e74 2079 6561 7220 6173 2077 6174 6572  nt year as water
+00000f30: 7368 6564 3a0a 2020 2020 2020 2020 2020  shed:.          
+00000f40: 2020 2d20 3330 2e34 2e32 3420 2d3e 2033    - 30.4.24 -> 3
+00000f50: 302e 3034 2e32 3032 340a 2020 2020 2020  0.04.2024.      
+00000f60: 2020 2020 2020 2d20 3330 2e34 2e32 3520        - 30.4.25 
+00000f70: 2d3e 2033 302e 3034 2e31 3932 350a 0a20  -> 30.04.1925.. 
+00000f80: 2020 2043 7572 7265 6e74 6c79 2073 7570     Currently sup
+00000f90: 706f 7274 6564 2064 6174 6520 666f 726d  ported date form
+00000fa0: 6174 733a 0a20 2020 2020 2020 202d 2030  ats:.        - 0
+00000fb0: 3437 362d 3039 2d30 3420 2d3e 2047 5245  476-09-04 -> GRE
+00000fc0: 474f 5249 414e 3a43 453a 3034 3736 2d30  GORIAN:CE:0476-0
+00000fd0: 392d 3034 3a43 453a 3034 3736 2d30 392d  9-04:CE:0476-09-
+00000fe0: 3034 0a20 2020 2020 2020 202d 2030 3437  04.        - 047
+00000ff0: 365f 3039 5f30 3420 2d3e 2047 5245 474f  6_09_04 -> GREGO
+00001000: 5249 414e 3a43 453a 3034 3736 2d30 392d  RIAN:CE:0476-09-
+00001010: 3034 3a43 453a 3034 3736 2d30 392d 3034  04:CE:0476-09-04
+00001020: 0a20 2020 2020 2020 202d 2033 302e 342e  .        - 30.4.
+00001030: 3230 3231 202d 3e20 4752 4547 4f52 4941  2021 -> GREGORIA
+00001040: 4e3a 4345 3a32 3032 312d 3034 2d33 303a  N:CE:2021-04-30:
+00001050: 4345 3a32 3032 312d 3034 2d33 300a 2020  CE:2021-04-30.  
+00001060: 2020 2020 2020 2d20 3330 2e34 2e32 3120        - 30.4.21 
+00001070: 2d3e 2047 5245 474f 5249 414e 3a43 453a  -> GREGORIAN:CE:
+00001080: 3230 3231 2d30 342d 3330 3a43 453a 3230  2021-04-30:CE:20
+00001090: 3231 2d30 342d 3330 0a20 2020 2020 2020  21-04-30.       
+000010a0: 202d 2035 2f31 312f 3230 3231 202d 3e20   - 5/11/2021 -> 
+000010b0: 4752 4547 4f52 4941 4e3a 4345 3a32 3032  GREGORIAN:CE:202
+000010c0: 312d 3131 2d30 353a 4345 3a32 3032 312d  1-11-05:CE:2021-
+000010d0: 3131 2d30 350a 2020 2020 2020 2020 2d20  11-05.        - 
+000010e0: 4a61 6e20 3236 2c20 3139 3933 202d 3e20  Jan 26, 1993 -> 
+000010f0: 4752 4547 4f52 4941 4e3a 4345 3a31 3939  GREGORIAN:CE:199
+00001100: 332d 3031 2d32 363a 4345 3a31 3939 332d  3-01-26:CE:1993-
+00001110: 3031 2d32 360a 2020 2020 2020 2020 2d20  01-26.        - 
+00001120: 3238 2e32 2e2d 312e 3132 2e31 3531 3520  28.2.-1.12.1515 
+00001130: 2d3e 2047 5245 474f 5249 414e 3a43 453a  -> GREGORIAN:CE:
+00001140: 3135 3135 2d30 322d 3238 3a43 453a 3135  1515-02-28:CE:15
+00001150: 3135 2d31 322d 3031 0a20 2020 2020 2020  15-12-01.       
+00001160: 202d 2032 352e 2d32 362e 322e 3038 3030   - 25.-26.2.0800
+00001170: 202d 3e20 4752 4547 4f52 4941 4e3a 4345   -> GREGORIAN:CE
+00001180: 3a30 3830 302d 3032 2d32 353a 4345 3a30  :0800-02-25:CE:0
+00001190: 3830 302d 3032 2d32 360a 2020 2020 2020  800-02-26.      
+000011a0: 2020 2d20 312e 392e 3230 3232 2d33 2e31    - 1.9.2022-3.1
+000011b0: 2e32 3032 3420 2d3e 2047 5245 474f 5249  .2024 -> GREGORI
+000011c0: 414e 3a43 453a 3230 3232 2d30 392d 3031  AN:CE:2022-09-01
+000011d0: 3a43 453a 3230 3234 2d30 312d 3033 0a20  :CE:2024-01-03. 
+000011e0: 2020 2020 2020 202d 2031 3834 3820 2d3e         - 1848 ->
+000011f0: 2047 5245 474f 5249 414e 3a43 453a 3138   GREGORIAN:CE:18
+00001200: 3438 3a43 453a 3138 3438 0a20 2020 2020  48:CE:1848.     
+00001210: 2020 202d 2031 3834 392f 3138 3530 202d     - 1849/1850 -
+00001220: 3e20 4752 4547 4f52 4941 4e3a 4345 3a31  > GREGORIAN:CE:1
+00001230: 3834 393a 4345 3a31 3835 300a 2020 2020  849:CE:1850.    
+00001240: 2020 2020 2d20 3138 3439 2f35 3020 2d3e      - 1849/50 ->
+00001250: 2047 5245 474f 5249 414e 3a43 453a 3138   GREGORIAN:CE:18
+00001260: 3439 3a43 453a 3138 3530 0a20 2020 2020  49:CE:1850.     
+00001270: 2020 202d 2031 3834 352d 3530 202d 3e20     - 1845-50 -> 
+00001280: 4752 4547 4f52 4941 4e3a 4345 3a31 3834  GREGORIAN:CE:184
+00001290: 353a 4345 3a31 3835 300a 2020 2020 2020  5:CE:1850.      
+000012a0: 2020 2d20 3834 302d 3530 202d 3e20 4752    - 840-50 -> GR
+000012b0: 4547 4f52 4941 4e3a 4345 3a38 3430 3a43  EGORIAN:CE:840:C
+000012c0: 453a 3835 300a 2020 2020 2020 2020 2d20  E:850.        - 
+000012d0: 3834 302d 3120 2d3e 2047 5245 474f 5249  840-1 -> GREGORI
+000012e0: 414e 3a43 453a 3834 303a 4345 3a38 3431  AN:CE:840:CE:841
+000012f0: 0a20 2020 2020 2020 202d 2031 3030 302d  .        - 1000-
+00001300: 3930 3020 6176 2e20 4a2e 2d43 2e20 2d3e  900 av. J.-C. ->
+00001310: 2047 5245 474f 5249 414e 3a42 433a 3130   GREGORIAN:BC:10
+00001320: 3030 3a42 433a 3930 300a 2020 2020 2020  00:BC:900.      
+00001330: 2020 2d20 3435 2061 762e 204a 2e2d 432e    - 45 av. J.-C.
+00001340: 202d 3e20 4752 4547 4f52 4941 4e3a 4243   -> GREGORIAN:BC
+00001350: 3a34 353a 4243 3a34 350a 0a20 2020 2041  :45:BC:45..    A
+00001360: 7267 733a 0a20 2020 2020 2020 2073 7472  rgs:.        str
+00001370: 696e 673a 2073 7472 696e 6720 746f 2063  ing: string to c
+00001380: 6865 636b 0a0a 2020 2020 5265 7475 726e  heck..    Return
+00001390: 733a 0a20 2020 2020 2020 2044 5350 2d66  s:.        DSP-f
+000013a0: 6f72 6d61 7474 6564 2064 6174 6520 7374  ormatted date st
+000013b0: 7269 6e67 2c20 6f72 204e 6f6e 650a 0a20  ring, or None.. 
+000013c0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+000013d0: 2020 2020 203e 3e3e 2069 6620 6669 6e64       >>> if find
+000013e0: 5f64 6174 655f 696e 5f73 7472 696e 6728  _date_in_string(
+000013f0: 726f 775b 2245 706f 6368 225d 293a 0a20  row["Epoch"]):. 
+00001400: 2020 2020 2020 203e 3e3e 2020 2020 2072         >>>     r
+00001410: 6573 6f75 7263 652e 6170 7065 6e64 286d  esource.append(m
+00001420: 616b 655f 6461 7465 5f70 726f 7028 223a  ake_date_prop(":
+00001430: 6861 7344 6174 6522 2c20 6669 6e64 5f64  hasDate", find_d
+00001440: 6174 655f 696e 5f73 7472 696e 6728 726f  ate_in_string(ro
+00001450: 775b 2245 706f 6368 225d 2929 0a0a 2020  w["Epoch"]))..  
+00001460: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
+00001470: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
+00001480: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
+00001490: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
+000014a0: 2d64 6174 612d 6669 6c65 2f23 6461 7465  -data-file/#date
+000014b0: 2d70 726f 700a 2020 2020 2222 220a 0a20  -prop.    """.. 
+000014c0: 2020 2023 2073 616e 6974 697a 6520 696e     # sanitize in
+000014d0: 7075 742c 206a 7573 7420 696e 2063 6173  put, just in cas
+000014e0: 6520 7468 6174 2074 6865 206d 6574 686f  e that the metho
+000014f0: 6420 7761 7320 6361 6c6c 6564 206f 6e20  d was called on 
+00001500: 616e 2065 6d70 7479 206f 7220 4e2f 4120  an empty or N/A 
+00001510: 6365 6c6c 0a20 2020 2069 6620 6e6f 7420  cell.    if not 
+00001520: 6368 6563 6b5f 6e6f 746e 6128 7374 7269  check_notna(stri
+00001530: 6e67 293a 0a20 2020 2020 2020 2072 6574  ng):.        ret
+00001540: 7572 6e20 4e6f 6e65 0a20 2020 2074 7279  urn None.    try
+00001550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001560: 205f 6669 6e64 5f64 6174 655f 696e 5f73   _find_date_in_s
+00001570: 7472 696e 675f 7468 726f 7769 6e67 2873  tring_throwing(s
+00001580: 7472 696e 6729 0a20 2020 2065 7863 6570  tring).    excep
+00001590: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
+000015a0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+000015b0: 650a 0a0a 5f6d 6f6e 7468 735f 6469 6374  e..._months_dict
+000015c0: 203d 207b 0a20 2020 2022 4a61 6e75 6172   = {.    "Januar
+000015d0: 7922 3a20 312c 0a20 2020 2022 4a61 6e22  y": 1,.    "Jan"
+000015e0: 3a20 312c 0a20 2020 2022 4665 6272 7561  : 1,.    "Februa
+000015f0: 7279 223a 2032 2c0a 2020 2020 2246 6562  ry": 2,.    "Feb
+00001600: 223a 2032 2c0a 2020 2020 224d 6172 6368  ": 2,.    "March
+00001610: 223a 2033 2c0a 2020 2020 224d 6172 223a  ": 3,.    "Mar":
+00001620: 2033 2c0a 2020 2020 2241 7072 696c 223a   3,.    "April":
+00001630: 2034 2c0a 2020 2020 2241 7072 223a 2034   4,.    "Apr": 4
+00001640: 2c0a 2020 2020 224d 6179 223a 2035 2c0a  ,.    "May": 5,.
+00001650: 2020 2020 224a 756e 6522 3a20 362c 0a20      "June": 6,. 
+00001660: 2020 2022 4a75 6e22 3a20 362c 0a20 2020     "Jun": 6,.   
+00001670: 2022 4a75 6c79 223a 2037 2c0a 2020 2020   "July": 7,.    
+00001680: 224a 756c 223a 2037 2c0a 2020 2020 2241  "Jul": 7,.    "A
+00001690: 7567 7573 7422 3a20 382c 0a20 2020 2022  ugust": 8,.    "
+000016a0: 4175 6722 3a20 382c 0a20 2020 2022 5365  Aug": 8,.    "Se
+000016b0: 7074 656d 6265 7222 3a20 392c 0a20 2020  ptember": 9,.   
+000016c0: 2022 5365 7074 223a 2039 2c0a 2020 2020   "Sept": 9,.    
+000016d0: 224f 6374 6f62 6572 223a 2031 302c 0a20  "October": 10,. 
+000016e0: 2020 2022 4f63 7422 3a20 3130 2c0a 2020     "Oct": 10,.  
+000016f0: 2020 224e 6f76 656d 6265 7222 3a20 3131    "November": 11
+00001700: 2c0a 2020 2020 224e 6f76 223a 2031 312c  ,.    "Nov": 11,
+00001710: 0a20 2020 2022 4465 6365 6d62 6572 223a  .    "December":
+00001720: 2031 322c 0a20 2020 2022 4465 6322 3a20   12,.    "Dec": 
+00001730: 3132 2c0a 7d0a 0a0a 6465 6620 5f66 696e  12,.}...def _fin
+00001740: 645f 6461 7465 5f69 6e5f 7374 7269 6e67  d_date_in_string
+00001750: 5f74 6872 6f77 696e 6728 7374 7269 6e67  _throwing(string
+00001760: 3a20 7374 7229 202d 3e20 7374 7220 7c20  : str) -> str | 
+00001770: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+00001780: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+00001790: 6973 2074 6865 2073 616d 6520 6173 2066  is the same as f
+000017a0: 696e 645f 6461 7465 5f69 6e5f 7374 7269  ind_date_in_stri
+000017b0: 6e67 2829 2c20 6275 7420 6d61 7920 7261  ng(), but may ra
+000017c0: 6973 6520 6120 5661 6c75 6545 7272 6f72  ise a ValueError
+000017d0: 2069 6e73 7465 6164 206f 6620 7265 7475   instead of retu
+000017e0: 726e 696e 6720 4e6f 6e65 2e0a 2020 2020  rning None..    
+000017f0: 2222 220a 2020 2020 7965 6172 5f72 6567  """.    year_reg
+00001800: 6578 203d 2072 2228 5b30 2d32 5d3f 5b30  ex = r"([0-2]?[0
+00001810: 2d39 5d5b 302d 395d 5b30 2d39 5d29 220a  -9][0-9][0-9])".
+00001820: 2020 2020 7965 6172 5f72 6567 6578 5f32      year_regex_2
+00001830: 5f6f 725f 345f 6469 6769 7473 203d 2072  _or_4_digits = r
+00001840: 2228 283f 3a5b 302d 325d 3f5b 302d 395d  "((?:[0-2]?[0-9]
+00001850: 293f 5b30 2d39 5d5b 302d 395d 2922 0a20  )?[0-9][0-9])". 
+00001860: 2020 206d 6f6e 7468 5f72 6567 6578 203d     month_regex =
+00001870: 2072 2228 5b30 2d31 5d3f 5b30 2d39 5d29   r"([0-1]?[0-9])
+00001880: 220a 2020 2020 6461 795f 7265 6765 7820  ".    day_regex 
+00001890: 3d20 7222 285b 302d 335d 3f5b 302d 395d  = r"([0-3]?[0-9]
+000018a0: 2922 0a20 2020 2073 6570 5f72 6567 6578  )".    sep_regex
+000018b0: 203d 2072 225b 5c2e 2f5d 220a 2020 2020   = r"[\./]".    
+000018c0: 6c6f 6f6b 6265 6869 6e64 203d 2072 2228  lookbehind = r"(
+000018d0: 3f3c 215b 302d 3941 2d5a 612d 7a5d 2922  ?<![0-9A-Za-z])"
+000018e0: 0a20 2020 206c 6f6f 6b61 6865 6164 203d  .    lookahead =
+000018f0: 2072 2228 3f21 5b30 2d39 412d 5a61 2d7a   r"(?![0-9A-Za-z
+00001900: 5d29 220a 0a20 2020 2069 6620 6672 656e  ])"..    if fren
+00001910: 6368 5f62 635f 6461 7465 203a 3d20 5f66  ch_bc_date := _f
+00001920: 696e 645f 6672 656e 6368 5f62 635f 6461  ind_french_bc_da
+00001930: 7465 2873 7472 696e 673d 7374 7269 6e67  te(string=string
+00001940: 2c20 6c6f 6f6b 6265 6869 6e64 3d6c 6f6f  , lookbehind=loo
+00001950: 6b62 6568 696e 642c 206c 6f6f 6b61 6865  kbehind, lookahe
+00001960: 6164 3d6c 6f6f 6b61 6865 6164 293a 0a20  ad=lookahead):. 
+00001970: 2020 2020 2020 2072 6574 7572 6e20 6672         return fr
+00001980: 656e 6368 5f62 635f 6461 7465 0a0a 2020  ench_bc_date..  
+00001990: 2020 2320 7465 6d70 6c61 7465 3a20 3230    # template: 20
+000019a0: 3231 2d30 312d 3031 207c 2032 3031 355f  21-01-01 | 2015_
+000019b0: 3031 5f30 320a 2020 2020 6973 6f5f 6461  01_02.    iso_da
+000019c0: 7465 203d 2072 6567 6578 2e73 6561 7263  te = regex.searc
+000019d0: 6828 7266 227b 6c6f 6f6b 6265 6869 6e64  h(rf"{lookbehind
+000019e0: 7d7b 7965 6172 5f72 6567 6578 7d5b 5f2d  }{year_regex}[_-
+000019f0: 5d28 5b30 2d31 5d5b 302d 395d 295b 5f2d  ]([0-1][0-9])[_-
+00001a00: 5d28 5b30 2d33 5d5b 302d 395d 297b 6c6f  ]([0-3][0-9]){lo
+00001a10: 6f6b 6168 6561 647d 222c 2073 7472 696e  okahead}", strin
+00001a20: 6729 0a0a 2020 2020 2320 7465 6d70 6c61  g)..    # templa
+00001a30: 7465 3a20 362e 2d38 2e33 2e31 3934 3820  te: 6.-8.3.1948 
+00001a40: 7c20 362f 322f 3139 3437 202d 2032 342e  | 6/2/1947 - 24.
+00001a50: 3033 2e31 3934 380a 2020 2020 6575 725f  03.1948.    eur_
+00001a60: 6461 7465 5f72 616e 6765 5f72 6567 6578  date_range_regex
+00001a70: 203d 2028 0a20 2020 2020 2020 2072 6622   = (.        rf"
+00001a80: 7b6c 6f6f 6b62 6568 696e 647d 220a 2020  {lookbehind}".  
+00001a90: 2020 2020 2020 7266 227b 6461 795f 7265        rf"{day_re
+00001aa0: 6765 787d 7b73 6570 5f72 6567 6578 7d28  gex}{sep_regex}(
+00001ab0: 3f3a 7b6d 6f6e 7468 5f72 6567 6578 7d7b  ?:{month_regex}{
+00001ac0: 7365 705f 7265 6765 787d 7b79 6561 725f  sep_regex}{year_
+00001ad0: 7265 6765 785f 325f 6f72 5f34 5f64 6967  regex_2_or_4_dig
+00001ae0: 6974 737d 3f29 3f20 3f28 3f3a 2d7c 3a7c  its}?)? ?(?:-|:|
+00001af0: 746f 2920 3f22 0a20 2020 2020 2020 2072  to) ?".        r
+00001b00: 6622 7b64 6179 5f72 6567 6578 7d7b 7365  f"{day_regex}{se
+00001b10: 705f 7265 6765 787d 7b6d 6f6e 7468 5f72  p_regex}{month_r
+00001b20: 6567 6578 7d7b 7365 705f 7265 6765 787d  egex}{sep_regex}
+00001b30: 7b79 6561 725f 7265 6765 785f 325f 6f72  {year_regex_2_or
+00001b40: 5f34 5f64 6967 6974 737d 220a 2020 2020  _4_digits}".    
+00001b50: 2020 2020 7266 227b 6c6f 6f6b 6168 6561      rf"{lookahea
+00001b60: 647d 220a 2020 2020 290a 2020 2020 6575  d}".    ).    eu
+00001b70: 725f 6461 7465 5f72 616e 6765 203d 2072  r_date_range = r
+00001b80: 6567 6578 2e73 6561 7263 6828 6575 725f  egex.search(eur_
+00001b90: 6461 7465 5f72 616e 6765 5f72 6567 6578  date_range_regex
+00001ba0: 2c20 7374 7269 6e67 290a 0a20 2020 2023  , string)..    #
+00001bb0: 2074 656d 706c 6174 653a 2031 2e34 2e32   template: 1.4.2
+00001bc0: 3032 3120 7c20 352f 3131 2f32 3032 310a  021 | 5/11/2021.
+00001bd0: 2020 2020 6575 725f 6461 7465 5f72 6567      eur_date_reg
+00001be0: 6578 203d 2072 6622 7b6c 6f6f 6b62 6568  ex = rf"{lookbeh
+00001bf0: 696e 647d 7b64 6179 5f72 6567 6578 7d7b  ind}{day_regex}{
+00001c00: 7365 705f 7265 6765 787d 7b6d 6f6e 7468  sep_regex}{month
+00001c10: 5f72 6567 6578 7d7b 7365 705f 7265 6765  _regex}{sep_rege
+00001c20: 787d 7b79 6561 725f 7265 6765 785f 325f  x}{year_regex_2_
+00001c30: 6f72 5f34 5f64 6967 6974 737d 7b6c 6f6f  or_4_digits}{loo
+00001c40: 6b61 6865 6164 7d22 0a20 2020 2065 7572  kahead}".    eur
+00001c50: 5f64 6174 6520 3d20 7265 6765 782e 7365  _date = regex.se
+00001c60: 6172 6368 280a 2020 2020 2020 2020 6575  arch(.        eu
+00001c70: 725f 6461 7465 5f72 6567 6578 2c0a 2020  r_date_regex,.  
+00001c80: 2020 2020 2020 7374 7269 6e67 2c0a 2020        string,.  
+00001c90: 2020 290a 0a20 2020 2023 2074 656d 706c    )..    # templ
+00001ca0: 6174 653a 204d 6172 6368 2039 2c20 3139  ate: March 9, 19
+00001cb0: 3038 207c 204d 6172 6368 352c 3139 3038  08 | March5,1908
+00001cc0: 207c 204d 6179 2031 312c 2031 3930 360a   | May 11, 1906.
+00001cd0: 2020 2020 616c 6c5f 6d6f 6e74 6873 203d      all_months =
+00001ce0: 2022 7c22 2e6a 6f69 6e28 5f6d 6f6e 7468   "|".join(_month
+00001cf0: 735f 6469 6374 290a 2020 2020 6d6f 6e74  s_dict).    mont
+00001d00: 686e 616d 655f 6461 7465 5f72 6567 6578  hname_date_regex
+00001d10: 203d 2072 6622 7b6c 6f6f 6b62 6568 696e   = rf"{lookbehin
+00001d20: 647d 287b 616c 6c5f 6d6f 6e74 6873 7d29  d}({all_months})
+00001d30: 203f 7b64 6179 5f72 6567 6578 7d2c 203f   ?{day_regex}, ?
+00001d40: 7b79 6561 725f 7265 6765 787d 7b6c 6f6f  {year_regex}{loo
+00001d50: 6b61 6865 6164 7d22 0a20 2020 206d 6f6e  kahead}".    mon
+00001d60: 7468 6e61 6d65 5f64 6174 6520 3d20 7265  thname_date = re
+00001d70: 6765 782e 7365 6172 6368 286d 6f6e 7468  gex.search(month
+00001d80: 6e61 6d65 5f64 6174 655f 7265 6765 782c  name_date_regex,
+00001d90: 2073 7472 696e 6729 0a0a 2020 2020 2320   string)..    # 
+00001da0: 7465 6d70 6c61 7465 3a20 3138 3439 2f35  template: 1849/5
+00001db0: 3020 7c20 3138 3439 2d35 3020 7c20 3138  0 | 1849-50 | 18
+00001dc0: 3439 2f31 3835 300a 2020 2020 7965 6172  49/1850.    year
+00001dd0: 5f72 616e 6765 203d 2072 6567 6578 2e73  _range = regex.s
+00001de0: 6561 7263 6828 6c6f 6f6b 6265 6869 6e64  earch(lookbehind
+00001df0: 202b 2079 6561 725f 7265 6765 7820 2b20   + year_regex + 
+00001e00: 7222 5b2f 2d5d 285c 647b 312c 347d 2922  r"[/-](\d{1,4})"
+00001e10: 202b 206c 6f6f 6b61 6865 6164 2c20 7374   + lookahead, st
+00001e20: 7269 6e67 290a 0a20 2020 2023 2074 656d  ring)..    # tem
+00001e30: 706c 6174 653a 2031 3930 370a 2020 2020  plate: 1907.    
+00001e40: 7965 6172 5f6f 6e6c 7920 3d20 7265 6765  year_only = rege
+00001e50: 782e 7365 6172 6368 2872 6622 7b6c 6f6f  x.search(rf"{loo
+00001e60: 6b62 6568 696e 647d 7b79 6561 725f 7265  kbehind}{year_re
+00001e70: 6765 787d 7b6c 6f6f 6b61 6865 6164 7d22  gex}{lookahead}"
+00001e80: 2c20 7374 7269 6e67 290a 0a20 2020 2072  , string)..    r
+00001e90: 6573 3a20 7374 7220 7c20 4e6f 6e65 203d  es: str | None =
+00001ea0: 204e 6f6e 650a 2020 2020 6966 2069 736f   None.    if iso
+00001eb0: 5f64 6174 653a 0a20 2020 2020 2020 2072  _date:.        r
+00001ec0: 6573 203d 205f 6672 6f6d 5f69 736f 5f64  es = _from_iso_d
+00001ed0: 6174 6528 6973 6f5f 6461 7465 290a 2020  ate(iso_date).  
+00001ee0: 2020 656c 6966 2065 7572 5f64 6174 655f    elif eur_date_
+00001ef0: 7261 6e67 653a 0a20 2020 2020 2020 2072  range:.        r
+00001f00: 6573 203d 205f 6672 6f6d 5f65 7572 5f64  es = _from_eur_d
+00001f10: 6174 655f 7261 6e67 6528 6575 725f 6461  ate_range(eur_da
+00001f20: 7465 5f72 616e 6765 290a 2020 2020 656c  te_range).    el
+00001f30: 6966 2065 7572 5f64 6174 653a 0a20 2020  if eur_date:.   
+00001f40: 2020 2020 2072 6573 203d 205f 6672 6f6d       res = _from
+00001f50: 5f65 7572 5f64 6174 6528 6575 725f 6461  _eur_date(eur_da
+00001f60: 7465 290a 2020 2020 656c 6966 206d 6f6e  te).    elif mon
+00001f70: 7468 6e61 6d65 5f64 6174 653a 0a20 2020  thname_date:.   
+00001f80: 2020 2020 2072 6573 203d 205f 6672 6f6d       res = _from
+00001f90: 5f6d 6f6e 7468 6e61 6d65 5f64 6174 6528  _monthname_date(
+00001fa0: 6d6f 6e74 686e 616d 655f 6461 7465 290a  monthname_date).
+00001fb0: 2020 2020 656c 6966 2079 6561 725f 7261      elif year_ra
+00001fc0: 6e67 653a 0a20 2020 2020 2020 2072 6573  nge:.        res
+00001fd0: 203d 205f 6672 6f6d 5f79 6561 725f 7261   = _from_year_ra
+00001fe0: 6e67 6528 7965 6172 5f72 616e 6765 290a  nge(year_range).
+00001ff0: 2020 2020 656c 6966 2079 6561 725f 6f6e      elif year_on
+00002000: 6c79 3a0a 2020 2020 2020 2020 7965 6172  ly:.        year
+00002010: 203d 2069 6e74 2879 6561 725f 6f6e 6c79   = int(year_only
+00002020: 2e67 726f 7570 2830 2929 0a20 2020 2020  .group(0)).     
+00002030: 2020 2072 6573 203d 2066 2247 5245 474f     res = f"GREGO
+00002040: 5249 414e 3a43 453a 7b79 6561 727d 3a43  RIAN:CE:{year}:C
+00002050: 453a 7b79 6561 727d 220a 2020 2020 7265  E:{year}".    re
+00002060: 7475 726e 2072 6573 0a0a 0a64 6566 205f  turn res...def _
+00002070: 6672 6f6d 5f69 736f 5f64 6174 6528 6973  from_iso_date(is
+00002080: 6f5f 6461 7465 3a20 4d61 7463 685b 7374  o_date: Match[st
+00002090: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
+000020a0: 7965 6172 203d 2069 6e74 2869 736f 5f64  year = int(iso_d
+000020b0: 6174 652e 6772 6f75 7028 3129 290a 2020  ate.group(1)).  
+000020c0: 2020 6d6f 6e74 6820 3d20 696e 7428 6973    month = int(is
+000020d0: 6f5f 6461 7465 2e67 726f 7570 2832 2929  o_date.group(2))
+000020e0: 0a20 2020 2064 6179 203d 2069 6e74 2869  .    day = int(i
+000020f0: 736f 5f64 6174 652e 6772 6f75 7028 3329  so_date.group(3)
+00002100: 290a 2020 2020 6461 7465 203d 2064 6174  ).    date = dat
+00002110: 6574 696d 652e 6461 7465 2879 6561 722c  etime.date(year,
+00002120: 206d 6f6e 7468 2c20 6461 7929 0a20 2020   month, day).   
+00002130: 2072 6574 7572 6e20 6622 4752 4547 4f52   return f"GREGOR
+00002140: 4941 4e3a 4345 3a7b 6461 7465 2e69 736f  IAN:CE:{date.iso
+00002150: 666f 726d 6174 2829 7d3a 4345 3a7b 6461  format()}:CE:{da
+00002160: 7465 2e69 736f 666f 726d 6174 2829 7d22  te.isoformat()}"
+00002170: 0a0a 0a64 6566 205f 6578 7061 6e64 5f32  ...def _expand_2
+00002180: 5f64 6967 6974 5f79 6561 7228 7965 6172  _digit_year(year
+00002190: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+000021a0: 2020 2063 7572 7265 6e74 5f79 6561 7220     current_year 
+000021b0: 3d20 6461 7465 7469 6d65 2e64 6174 652e  = datetime.date.
+000021c0: 746f 6461 7928 292e 7965 6172 202d 2032  today().year - 2
+000021d0: 3030 300a 2020 2020 6966 2079 6561 7220  000.    if year 
+000021e0: 3c3d 2063 7572 7265 6e74 5f79 6561 723a  <= current_year:
+000021f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002200: 7965 6172 202b 2032 3030 300a 2020 2020  year + 2000.    
+00002210: 656c 6966 2079 6561 7220 3c3d 2039 393a  elif year <= 99:
+00002220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002230: 7965 6172 202b 2031 3930 300a 2020 2020  year + 1900.    
+00002240: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00002250: 7475 726e 2079 6561 720a 0a0a 6465 6620  turn year...def 
+00002260: 5f66 726f 6d5f 6575 725f 6461 7465 5f72  _from_eur_date_r
+00002270: 616e 6765 2865 7572 5f64 6174 655f 7261  ange(eur_date_ra
+00002280: 6e67 653a 204d 6174 6368 5b73 7472 5d29  nge: Match[str])
+00002290: 202d 3e20 7374 723a 0a20 2020 2073 7461   -> str:.    sta
+000022a0: 7274 6461 7920 3d20 696e 7428 6575 725f  rtday = int(eur_
+000022b0: 6461 7465 5f72 616e 6765 2e67 726f 7570  date_range.group
+000022c0: 2831 2929 0a20 2020 2073 7461 7274 6d6f  (1)).    startmo
+000022d0: 6e74 6820 3d20 696e 7428 6575 725f 6461  nth = int(eur_da
+000022e0: 7465 5f72 616e 6765 2e67 726f 7570 2832  te_range.group(2
+000022f0: 2929 2069 6620 6575 725f 6461 7465 5f72  )) if eur_date_r
+00002300: 616e 6765 2e67 726f 7570 2832 2920 656c  ange.group(2) el
+00002310: 7365 2069 6e74 2865 7572 5f64 6174 655f  se int(eur_date_
+00002320: 7261 6e67 652e 6772 6f75 7028 3529 290a  range.group(5)).
+00002330: 2020 2020 7374 6172 7479 6561 7220 3d20      startyear = 
+00002340: 696e 7428 6575 725f 6461 7465 5f72 616e  int(eur_date_ran
+00002350: 6765 2e67 726f 7570 2833 2929 2069 6620  ge.group(3)) if 
+00002360: 6575 725f 6461 7465 5f72 616e 6765 2e67  eur_date_range.g
+00002370: 726f 7570 2833 2920 656c 7365 2069 6e74  roup(3) else int
+00002380: 2865 7572 5f64 6174 655f 7261 6e67 652e  (eur_date_range.
+00002390: 6772 6f75 7028 3629 290a 2020 2020 7374  group(6)).    st
+000023a0: 6172 7479 6561 7220 3d20 5f65 7870 616e  artyear = _expan
+000023b0: 645f 325f 6469 6769 745f 7965 6172 2873  d_2_digit_year(s
+000023c0: 7461 7274 7965 6172 290a 2020 2020 656e  tartyear).    en
+000023d0: 6464 6179 203d 2069 6e74 2865 7572 5f64  dday = int(eur_d
+000023e0: 6174 655f 7261 6e67 652e 6772 6f75 7028  ate_range.group(
+000023f0: 3429 290a 2020 2020 656e 646d 6f6e 7468  4)).    endmonth
+00002400: 203d 2069 6e74 2865 7572 5f64 6174 655f   = int(eur_date_
+00002410: 7261 6e67 652e 6772 6f75 7028 3529 290a  range.group(5)).
+00002420: 2020 2020 656e 6479 6561 7220 3d20 696e      endyear = in
+00002430: 7428 6575 725f 6461 7465 5f72 616e 6765  t(eur_date_range
+00002440: 2e67 726f 7570 2836 2929 0a20 2020 2065  .group(6)).    e
+00002450: 6e64 7965 6172 203d 205f 6578 7061 6e64  ndyear = _expand
+00002460: 5f32 5f64 6967 6974 5f79 6561 7228 656e  _2_digit_year(en
+00002470: 6479 6561 7229 0a20 2020 2073 7461 7274  dyear).    start
+00002480: 6461 7465 203d 2064 6174 6574 696d 652e  date = datetime.
+00002490: 6461 7465 2873 7461 7274 7965 6172 2c20  date(startyear, 
+000024a0: 7374 6172 746d 6f6e 7468 2c20 7374 6172  startmonth, star
+000024b0: 7464 6179 290a 2020 2020 656e 6464 6174  tday).    enddat
+000024c0: 6520 3d20 6461 7465 7469 6d65 2e64 6174  e = datetime.dat
+000024d0: 6528 656e 6479 6561 722c 2065 6e64 6d6f  e(endyear, endmo
+000024e0: 6e74 682c 2065 6e64 6461 7929 0a20 2020  nth, endday).   
+000024f0: 2069 6620 656e 6464 6174 6520 3c20 7374   if enddate < st
+00002500: 6172 7464 6174 653a 0a20 2020 2020 2020  artdate:.       
+00002510: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002520: 720a 2020 2020 7265 7475 726e 2066 2247  r.    return f"G
+00002530: 5245 474f 5249 414e 3a43 453a 7b73 7461  REGORIAN:CE:{sta
+00002540: 7274 6461 7465 2e69 736f 666f 726d 6174  rtdate.isoformat
+00002550: 2829 7d3a 4345 3a7b 656e 6464 6174 652e  ()}:CE:{enddate.
+00002560: 6973 6f66 6f72 6d61 7428 297d 220a 0a0a  isoformat()}"...
+00002570: 6465 6620 5f66 726f 6d5f 6575 725f 6461  def _from_eur_da
+00002580: 7465 2865 7572 5f64 6174 653a 204d 6174  te(eur_date: Mat
+00002590: 6368 5b73 7472 5d29 202d 3e20 7374 723a  ch[str]) -> str:
+000025a0: 0a20 2020 2073 7461 7274 6461 7920 3d20  .    startday = 
+000025b0: 696e 7428 6575 725f 6461 7465 2e67 726f  int(eur_date.gro
+000025c0: 7570 2831 2929 0a20 2020 2073 7461 7274  up(1)).    start
+000025d0: 6d6f 6e74 6820 3d20 696e 7428 6575 725f  month = int(eur_
+000025e0: 6461 7465 2e67 726f 7570 2832 2929 0a20  date.group(2)). 
+000025f0: 2020 2073 7461 7274 7965 6172 203d 2069     startyear = i
+00002600: 6e74 2865 7572 5f64 6174 652e 6772 6f75  nt(eur_date.grou
+00002610: 7028 3329 290a 2020 2020 7374 6172 7479  p(3)).    starty
+00002620: 6561 7220 3d20 5f65 7870 616e 645f 325f  ear = _expand_2_
+00002630: 6469 6769 745f 7965 6172 2873 7461 7274  digit_year(start
+00002640: 7965 6172 290a 2020 2020 6461 7465 203d  year).    date =
+00002650: 2064 6174 6574 696d 652e 6461 7465 2873   datetime.date(s
+00002660: 7461 7274 7965 6172 2c20 7374 6172 746d  tartyear, startm
+00002670: 6f6e 7468 2c20 7374 6172 7464 6179 290a  onth, startday).
+00002680: 2020 2020 7265 7475 726e 2066 2247 5245      return f"GRE
+00002690: 474f 5249 414e 3a43 453a 7b64 6174 652e  GORIAN:CE:{date.
+000026a0: 6973 6f66 6f72 6d61 7428 297d 3a43 453a  isoformat()}:CE:
+000026b0: 7b64 6174 652e 6973 6f66 6f72 6d61 7428  {date.isoformat(
+000026c0: 297d 220a 0a0a 6465 6620 5f66 726f 6d5f  )}"...def _from_
+000026d0: 6d6f 6e74 686e 616d 655f 6461 7465 286d  monthname_date(m
+000026e0: 6f6e 7468 6e61 6d65 5f64 6174 653a 204d  onthname_date: M
+000026f0: 6174 6368 5b73 7472 5d29 202d 3e20 7374  atch[str]) -> st
+00002700: 723a 0a20 2020 2064 6179 203d 2069 6e74  r:.    day = int
+00002710: 286d 6f6e 7468 6e61 6d65 5f64 6174 652e  (monthname_date.
+00002720: 6772 6f75 7028 3229 290a 2020 2020 6d6f  group(2)).    mo
+00002730: 6e74 6820 3d20 5f6d 6f6e 7468 735f 6469  nth = _months_di
+00002740: 6374 5b6d 6f6e 7468 6e61 6d65 5f64 6174  ct[monthname_dat
+00002750: 652e 6772 6f75 7028 3129 5d0a 2020 2020  e.group(1)].    
+00002760: 7965 6172 203d 2069 6e74 286d 6f6e 7468  year = int(month
+00002770: 6e61 6d65 5f64 6174 652e 6772 6f75 7028  name_date.group(
+00002780: 3329 290a 2020 2020 6461 7465 203d 2064  3)).    date = d
+00002790: 6174 6574 696d 652e 6461 7465 2879 6561  atetime.date(yea
+000027a0: 722c 206d 6f6e 7468 2c20 6461 7929 0a20  r, month, day). 
+000027b0: 2020 2072 6574 7572 6e20 6622 4752 4547     return f"GREG
+000027c0: 4f52 4941 4e3a 4345 3a7b 6461 7465 2e69  ORIAN:CE:{date.i
+000027d0: 736f 666f 726d 6174 2829 7d3a 4345 3a7b  soformat()}:CE:{
+000027e0: 6461 7465 2e69 736f 666f 726d 6174 2829  date.isoformat()
+000027f0: 7d22 0a0a 0a64 6566 205f 6672 6f6d 5f79  }"...def _from_y
+00002800: 6561 725f 7261 6e67 6528 7965 6172 5f72  ear_range(year_r
+00002810: 616e 6765 3a20 4d61 7463 685b 7374 725d  ange: Match[str]
+00002820: 2920 2d3e 2073 7472 3a0a 2020 2020 7374  ) -> str:.    st
+00002830: 6172 7479 6561 7220 3d20 696e 7428 7965  artyear = int(ye
+00002840: 6172 5f72 616e 6765 2e67 726f 7570 2831  ar_range.group(1
+00002850: 2929 0a20 2020 2065 6e64 7965 6172 203d  )).    endyear =
+00002860: 2069 6e74 2879 6561 725f 7261 6e67 652e   int(year_range.
+00002870: 6772 6f75 7028 3229 290a 2020 2020 6966  group(2)).    if
+00002880: 2065 6e64 7965 6172 202f 2f20 3130 203d   endyear // 10 =
+00002890: 3d20 303a 0a20 2020 2020 2020 2023 2065  = 0:.        # e
+000028a0: 6e64 7965 6172 2069 7320 6f6e 6c79 2031  ndyear is only 1
+000028b0: 2d64 6967 6974 3a20 6164 6420 7468 6520  -digit: add the 
+000028c0: 6669 7273 7420 322d 3320 6469 6769 7473  first 2-3 digits
+000028d0: 206f 6620 7374 6172 7479 6561 720a 2020   of startyear.  
+000028e0: 2020 2020 2020 656e 6479 6561 7220 3d20        endyear = 
+000028f0: 7374 6172 7479 6561 7220 2f2f 2031 3020  startyear // 10 
+00002900: 2a20 3130 202b 2065 6e64 7965 6172 0a20  * 10 + endyear. 
+00002910: 2020 2065 6c69 6620 656e 6479 6561 7220     elif endyear 
+00002920: 2f2f 2031 3030 203d 3d20 303a 0a20 2020  // 100 == 0:.   
+00002930: 2020 2020 2023 2065 6e64 7965 6172 2069       # endyear i
+00002940: 7320 6f6e 6c79 2032 2d64 6967 6974 3a20  s only 2-digit: 
+00002950: 6164 6420 7468 6520 6669 7273 7420 312d  add the first 1-
+00002960: 3220 6469 6769 7473 206f 6620 7374 6172  2 digits of star
+00002970: 7479 6561 720a 2020 2020 2020 2020 656e  tyear.        en
+00002980: 6479 6561 7220 3d20 7374 6172 7479 6561  dyear = startyea
+00002990: 7220 2f2f 2031 3030 202a 2031 3030 202b  r // 100 * 100 +
+000029a0: 2065 6e64 7965 6172 0a20 2020 2069 6620   endyear.    if 
+000029b0: 656e 6479 6561 7220 3c3d 2073 7461 7274  endyear <= start
+000029c0: 7965 6172 3a0a 2020 2020 2020 2020 7261  year:.        ra
+000029d0: 6973 6520 5661 6c75 6545 7272 6f72 0a20  ise ValueError. 
+000029e0: 2020 2072 6574 7572 6e20 6622 4752 4547     return f"GREG
+000029f0: 4f52 4941 4e3a 4345 3a7b 7374 6172 7479  ORIAN:CE:{starty
+00002a00: 6561 727d 3a43 453a 7b65 6e64 7965 6172  ear}:CE:{endyear
+00002a10: 7d22 0a0a 0a64 6566 2070 7265 7061 7265  }"...def prepare
+00002a20: 5f76 616c 7565 280a 2020 2020 7661 6c75  _value(.    valu
+00002a30: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
+00002a40: 7945 6c65 6d65 6e74 2c20 7374 722c 2069  yElement, str, i
+00002a50: 6e74 2c20 666c 6f61 742c 2062 6f6f 6c2c  nt, float, bool,
+00002a60: 2049 7465 7261 626c 655b 556e 696f 6e5b   Iterable[Union[
+00002a70: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
+00002a80: 2073 7472 2c20 696e 742c 2066 6c6f 6174   str, int, float
+00002a90: 2c20 626f 6f6c 5d5d 5d2c 0a29 202d 3e20  , bool]]],.) -> 
+00002aa0: 6c69 7374 5b50 726f 7065 7274 7945 6c65  list[PropertyEle
+00002ab0: 6d65 6e74 5d3a 0a20 2020 2022 2222 0a20  ment]:.    """. 
+00002ac0: 2020 2054 6869 7320 6d65 7468 6f64 2074     This method t
+00002ad0: 7261 6e73 666f 726d 7320 7468 6520 7061  ransforms the pa
+00002ae0: 7261 6d65 7465 7220 2276 616c 7565 2220  rameter "value" 
+00002af0: 6672 6f6d 2061 206d 616b 655f 2a5f 7072  from a make_*_pr
+00002b00: 6f70 2829 206d 6574 686f 6420 696e 746f  op() method into
+00002b10: 2061 206c 6973 7420 6f66 2050 726f 7065   a list of Prope
+00002b20: 7274 7945 6c65 6d65 6e74 732e 2022 7661  rtyElements. "va
+00002b30: 6c75 6522 2069 730a 2020 2020 7061 7373  lue" is.    pass
+00002b40: 6564 206f 6e20 746f 2074 6869 7320 6d65  ed on to this me
+00002b50: 7468 6f64 2061 7320 6974 2077 6173 2072  thod as it was r
+00002b60: 6563 6569 7665 642e 0a0a 2020 2020 4172  eceived...    Ar
+00002b70: 6773 3a0a 2020 2020 2020 2020 7661 6c75  gs:.        valu
+00002b80: 653a 2022 7661 6c75 6522 2061 7320 7265  e: "value" as re
+00002b90: 6365 6976 6564 2066 726f 6d20 7468 6520  ceived from the 
+00002ba0: 6361 6c6c 6572 0a0a 2020 2020 5265 7475  caller..    Retu
+00002bb0: 726e 733a 0a20 2020 2020 2020 2061 206c  rns:.        a l
+00002bc0: 6973 7420 6f66 2050 726f 7065 7274 7945  ist of PropertyE
+00002bd0: 6c65 6d65 6e74 730a 2020 2020 2222 220a  lements.    """.
+00002be0: 2020 2020 2320 6d61 6b65 2073 7572 6520      # make sure 
+00002bf0: 7468 6174 2022 7661 6c75 6522 2069 7320  that "value" is 
+00002c00: 6c69 7374 2d6c 696b 650a 2020 2020 6966  list-like.    if
+00002c10: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00002c20: 7661 6c75 652c 2049 7465 7261 626c 6529  value, Iterable)
+00002c30: 206f 7220 6973 696e 7374 616e 6365 2876   or isinstance(v
+00002c40: 616c 7565 2c20 7374 7229 3a0a 2020 2020  alue, str):.    
+00002c50: 2020 2020 7661 6c75 6520 3d20 5b76 616c      value = [val
+00002c60: 7565 5d0a 0a20 2020 2023 206d 616b 6520  ue]..    # make 
+00002c70: 6120 5072 6f70 6572 7479 456c 656d 656e  a PropertyElemen
+00002c80: 7420 6f75 7420 6f66 2069 7473 2065 6c65  t out of its ele
+00002c90: 6d65 6e74 732c 2069 6620 6e65 6365 7373  ments, if necess
+00002ca0: 6172 792e 0a20 2020 2072 6574 7572 6e20  ary..    return 
+00002cb0: 5b78 2069 6620 6973 696e 7374 616e 6365  [x if isinstance
+00002cc0: 2878 2c20 5072 6f70 6572 7479 456c 656d  (x, PropertyElem
+00002cd0: 656e 7429 2065 6c73 6520 5072 6f70 6572  ent) else Proper
+00002ce0: 7479 456c 656d 656e 7428 7829 2066 6f72  tyElement(x) for
+00002cf0: 2078 2069 6e20 7661 6c75 655d 0a0a 0a64   x in value]...d
+00002d00: 6566 206d 616b 655f 726f 6f74 280a 2020  ef make_root(.  
+00002d10: 2020 7368 6f72 7463 6f64 653a 2073 7472    shortcode: str
+00002d20: 2c0a 2020 2020 6465 6661 756c 745f 6f6e  ,.    default_on
+00002d30: 746f 6c6f 6779 3a20 7374 722c 0a29 202d  tology: str,.) -
+00002d40: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
+00002d50: 3a0a 2020 2020 2222 220a 2020 2020 5374  :.    """.    St
+00002d60: 6172 7420 6275 696c 6469 6e67 2079 6f75  art building you
+00002d70: 7220 584d 4c20 646f 6375 6d65 6e74 2062  r XML document b
+00002d80: 7920 6372 6561 7469 6e67 2074 6865 2072  y creating the r
+00002d90: 6f6f 7420 656c 656d 656e 7420 3c6b 6e6f  oot element <kno
+00002da0: 7261 3e2e 0a0a 2020 2020 4172 6773 3a0a  ra>...    Args:.
+00002db0: 2020 2020 2020 2020 7368 6f72 7463 6f64          shortcod
+00002dc0: 653a 2054 6865 2073 686f 7274 636f 6465  e: The shortcode
+00002dd0: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
+00002de0: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
+00002df0: 6865 204a 534f 4e20 7072 6f6a 6563 7420  he JSON project 
+00002e00: 6669 6c65 0a20 2020 2020 2020 2064 6566  file.        def
+00002e10: 6175 6c74 5f6f 6e74 6f6c 6f67 793a 206f  ault_ontology: o
+00002e20: 6e65 206f 6620 7468 6520 6f6e 746f 6c6f  ne of the ontolo
+00002e30: 6769 6573 206f 6620 7468 6520 4a53 4f4e  gies of the JSON
+00002e40: 2070 726f 6a65 6374 2066 696c 650a 0a20   project file.. 
+00002e50: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002e60: 2020 2020 5468 6520 726f 6f74 2065 6c65      The root ele
+00002e70: 6d65 6e74 203c 6b6e 6f72 613e 2e0a 0a20  ment <knora>... 
+00002e80: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00002e90: 2020 2020 203e 3e3e 2072 6f6f 7420 3d20       >>> root = 
+00002ea0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f72  excel2xml.make_r
+00002eb0: 6f6f 7428 7368 6f72 7463 6f64 653d 7368  oot(shortcode=sh
+00002ec0: 6f72 7463 6f64 652c 2064 6566 6175 6c74  ortcode, default
+00002ed0: 5f6f 6e74 6f6c 6f67 793d 6465 6661 756c  _ontology=defaul
+00002ee0: 745f 6f6e 746f 6c6f 6779 290a 2020 2020  t_ontology).    
+00002ef0: 2020 2020 3e3e 3e20 726f 6f74 203d 2065      >>> root = e
+00002f00: 7863 656c 3278 6d6c 2e61 7070 656e 645f  xcel2xml.append_
+00002f10: 7065 726d 6973 7369 6f6e 7328 726f 6f74  permissions(root
+00002f20: 290a 0a20 2020 2053 6565 2068 7474 7073  )..    See https
+00002f30: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+00002f40: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+00002f50: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+00002f60: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+00002f70: 2374 6865 2d72 6f6f 742d 656c 656d 656e  #the-root-elemen
+00002f80: 742d 6b6e 6f72 610a 2020 2020 2222 220a  t-knora.    """.
+00002f90: 2020 2020 7363 6865 6d61 5f75 726c 203d      schema_url =
+00002fa0: 2022 6874 7470 733a 2f2f 7261 772e 6769   "https://raw.gi
+00002fb0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00002fc0: 636f 6d2f 6461 7363 682d 7377 6973 732f  com/dasch-swiss/
+00002fd0: 6473 702d 746f 6f6c 732f 6d61 696e 2f73  dsp-tools/main/s
+00002fe0: 7263 2f64 7370 5f74 6f6f 6c73 2f72 6573  rc/dsp_tools/res
+00002ff0: 6f75 7263 6573 2f73 6368 656d 612f 6461  ources/schema/da
+00003000: 7461 2e78 7364 220a 2020 2020 7363 6865  ta.xsd".    sche
+00003010: 6d61 5f6c 6f63 6174 696f 6e5f 6b65 7920  ma_location_key 
+00003020: 3d20 7374 7228 6574 7265 652e 514e 616d  = str(etree.QNam
+00003030: 6528 2268 7474 703a 2f2f 7777 772e 7733  e("http://www.w3
+00003040: 2e6f 7267 2f32 3030 312f 584d 4c53 6368  .org/2001/XMLSch
+00003050: 656d 612d 696e 7374 616e 6365 222c 2022  ema-instance", "
+00003060: 7363 6865 6d61 4c6f 6361 7469 6f6e 2229  schemaLocation")
+00003070: 290a 2020 2020 7363 6865 6d61 5f6c 6f63  ).    schema_loc
+00003080: 6174 696f 6e5f 7661 6c75 6520 3d20 6622  ation_value = f"
+00003090: 6874 7470 733a 2f2f 6461 7363 682e 7377  https://dasch.sw
+000030a0: 6973 732f 7363 6865 6d61 207b 7363 6865  iss/schema {sche
+000030b0: 6d61 5f75 726c 7d22 0a20 2020 2072 6574  ma_url}".    ret
+000030c0: 7572 6e20 6574 7265 652e 456c 656d 656e  urn etree.Elemen
+000030d0: 7428 0a20 2020 2020 2020 2022 7b25 737d  t(.        "{%s}
+000030e0: 6b6e 6f72 6122 2025 2078 6d6c 5f6e 616d  knora" % xml_nam
+000030f0: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+00003100: 2c0a 2020 2020 2020 2020 6174 7472 6962  ,.        attrib
+00003110: 3d7b 0a20 2020 2020 2020 2020 2020 2073  ={.            s
+00003120: 6368 656d 615f 6c6f 6361 7469 6f6e 5f6b  chema_location_k
+00003130: 6579 3a20 7363 6865 6d61 5f6c 6f63 6174  ey: schema_locat
+00003140: 696f 6e5f 7661 6c75 652c 0a20 2020 2020  ion_value,.     
+00003150: 2020 2020 2020 2022 7368 6f72 7463 6f64         "shortcod
+00003160: 6522 3a20 7368 6f72 7463 6f64 652c 0a20  e": shortcode,. 
+00003170: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00003180: 756c 742d 6f6e 746f 6c6f 6779 223a 2064  ult-ontology": d
+00003190: 6566 6175 6c74 5f6f 6e74 6f6c 6f67 792c  efault_ontology,
+000031a0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000031b0: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
+000031c0: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
+000031d0: 2029 0a0a 0a64 6566 2061 7070 656e 645f   )...def append_
+000031e0: 7065 726d 6973 7369 6f6e 7328 726f 6f74  permissions(root
+000031f0: 5f65 6c65 6d65 6e74 3a20 6574 7265 652e  _element: etree.
+00003200: 5f45 6c65 6d65 6e74 2920 2d3e 2065 7472  _Element) -> etr
+00003210: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
+00003220: 2022 2222 0a20 2020 2041 6674 6572 2068   """.    After h
+00003230: 6176 696e 6720 6372 6561 7465 6420 6120  aving created a 
+00003240: 726f 6f74 2065 6c65 6d65 6e74 2c20 6361  root element, ca
+00003250: 6c6c 2074 6869 7320 6d65 7468 6f64 2074  ll this method t
+00003260: 6f20 6170 7065 6e64 2074 6865 2066 6f75  o append the fou
+00003270: 7220 7065 726d 6973 7369 6f6e 7320 2272  r permissions "r
+00003280: 6573 2d64 6566 6175 6c74 222c 0a20 2020  es-default",.   
+00003290: 2022 7265 732d 7265 7374 7269 6374 6564   "res-restricted
+000032a0: 222c 2022 7072 6f70 2d64 6566 6175 6c74  ", "prop-default
+000032b0: 222c 2061 6e64 2022 7072 6f70 2d72 6573  ", and "prop-res
+000032c0: 7472 6963 7465 6422 2074 6f20 6974 2e20  tricted" to it. 
+000032d0: 5468 6573 6520 666f 7572 2070 6572 6d69  These four permi
+000032e0: 7373 696f 6e73 2061 7265 2061 2067 6f6f  ssions are a goo
+000032f0: 6420 6261 7369 7320 746f 0a20 2020 2073  d basis to.    s
+00003300: 7461 7274 2077 6974 682c 2062 7574 2072  tart with, but r
+00003310: 656d 656d 6265 7220 7468 6174 2074 6865  emember that the
+00003320: 7920 6361 6e20 6265 2061 6461 7074 6564  y can be adapted
+00003330: 2c20 616e 6420 7468 6174 206f 7468 6572  , and that other
+00003340: 2070 6572 6d69 7373 696f 6e73 2063 616e   permissions can
+00003350: 2062 6520 6465 6669 6e65 6420 696e 7374   be defined inst
+00003360: 6561 6420 6f66 2074 6865 7365 2e0a 0a20  ead of these... 
+00003370: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00003380: 2072 6f6f 745f 656c 656d 656e 743a 2054   root_element: T
+00003390: 6865 2058 4d4c 2072 6f6f 7420 656c 656d  he XML root elem
+000033a0: 656e 7420 3c6b 6e6f 7261 3e20 6372 6561  ent <knora> crea
+000033b0: 7465 6420 6279 206d 616b 655f 726f 6f74  ted by make_root
+000033c0: 2829 0a0a 2020 2020 5265 7475 726e 733a  ()..    Returns:
+000033d0: 0a20 2020 2020 2020 2054 6865 2072 6f6f  .        The roo
+000033e0: 7420 656c 656d 656e 7420 7769 7468 2074  t element with t
+000033f0: 6865 2066 6f75 7220 7065 726d 6973 7369  he four permissi
+00003400: 6f6e 2062 6c6f 636b 7320 6170 7065 6e64  on blocks append
+00003410: 6564 0a0a 2020 2020 4578 616d 706c 6573  ed..    Examples
+00003420: 3a0a 2020 2020 2020 2020 3e3e 3e20 726f  :.        >>> ro
+00003430: 6f74 203d 2065 7863 656c 3278 6d6c 2e6d  ot = excel2xml.m
+00003440: 616b 655f 726f 6f74 2873 686f 7274 636f  ake_root(shortco
+00003450: 6465 3d73 686f 7274 636f 6465 2c20 6465  de=shortcode, de
+00003460: 6661 756c 745f 6f6e 746f 6c6f 6779 3d64  fault_ontology=d
+00003470: 6566 6175 6c74 5f6f 6e74 6f6c 6f67 7929  efault_ontology)
+00003480: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
+00003490: 7420 3d20 6578 6365 6c32 786d 6c2e 6170  t = excel2xml.ap
+000034a0: 7065 6e64 5f70 6572 6d69 7373 696f 6e73  pend_permissions
+000034b0: 2872 6f6f 7429 0a0a 2020 2020 5365 6520  (root)..    See 
+000034c0: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+000034d0: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+000034e0: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+000034f0: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+00003500: 6669 6c65 2f23 6465 7363 7269 6269 6e67  file/#describing
+00003510: 2d70 6572 6d69 7373 696f 6e73 2d77 6974  -permissions-wit
+00003520: 682d 7065 726d 6973 7369 6f6e 732d 656c  h-permissions-el
+00003530: 656d 656e 7473 0a20 2020 2022 2222 0a0a  ements.    """..
+00003540: 2020 2020 5045 524d 4953 5349 4f4e 5320      PERMISSIONS 
+00003550: 3d20 452e 7065 726d 6973 7369 6f6e 730a  = E.permissions.
+00003560: 2020 2020 414c 4c4f 5720 3d20 452e 616c      ALLOW = E.al
+00003570: 6c6f 770a 2020 2020 2320 6c78 6d6c 2e62  low.    # lxml.b
+00003580: 7569 6c64 6572 2e45 2069 7320 6120 6d6f  uilder.E is a mo
+00003590: 7265 2073 6f70 6869 7374 6963 6174 6564  re sophisticated
+000035a0: 2065 6c65 6d65 6e74 2066 6163 746f 7279   element factory
+000035b0: 2074 6861 6e20 6574 7265 652e 456c 656d   than etree.Elem
+000035c0: 656e 742e 0a20 2020 2023 2045 2e74 6167  ent..    # E.tag
+000035d0: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
+000035e0: 6f20 4528 2274 6167 2229 2061 6e64 2072  o E("tag") and r
+000035f0: 6573 756c 7473 2069 6e20 3c74 6167 3e0a  esults in <tag>.
+00003600: 0a20 2020 2072 6573 5f64 6566 6175 6c74  .    res_default
+00003610: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+00003620: 2822 7b25 737d 7065 726d 6973 7369 6f6e  ("{%s}permission
+00003630: 7322 2025 2078 6d6c 5f6e 616d 6573 7061  s" % xml_namespa
+00003640: 6365 5f6d 6170 5b4e 6f6e 655d 2c20 6964  ce_map[None], id
+00003650: 3d22 7265 732d 6465 6661 756c 7422 290a  ="res-default").
+00003660: 2020 2020 7265 735f 6465 6661 756c 742e      res_default.
+00003670: 6170 7065 6e64 2841 4c4c 4f57 2822 5622  append(ALLOW("V"
+00003680: 2c20 6772 6f75 703d 2255 6e6b 6e6f 776e  , group="Unknown
+00003690: 5573 6572 2229 290a 2020 2020 7265 735f  User")).    res_
+000036a0: 6465 6661 756c 742e 6170 7065 6e64 2841  default.append(A
+000036b0: 4c4c 4f57 2822 5622 2c20 6772 6f75 703d  LLOW("V", group=
+000036c0: 224b 6e6f 776e 5573 6572 2229 290a 2020  "KnownUser")).  
+000036d0: 2020 7265 735f 6465 6661 756c 742e 6170    res_default.ap
+000036e0: 7065 6e64 2841 4c4c 4f57 2822 4422 2c20  pend(ALLOW("D", 
+000036f0: 6772 6f75 703d 2250 726f 6a65 6374 4d65  group="ProjectMe
+00003700: 6d62 6572 2229 290a 2020 2020 7265 735f  mber")).    res_
+00003710: 6465 6661 756c 742e 6170 7065 6e64 2841  default.append(A
+00003720: 4c4c 4f57 2822 4352 222c 2067 726f 7570  LLOW("CR", group
+00003730: 3d22 5072 6f6a 6563 7441 646d 696e 2229  ="ProjectAdmin")
+00003740: 290a 2020 2020 7265 735f 6465 6661 756c  ).    res_defaul
+00003750: 742e 6170 7065 6e64 2841 4c4c 4f57 2822  t.append(ALLOW("
+00003760: 4352 222c 2067 726f 7570 3d22 4372 6561  CR", group="Crea
+00003770: 746f 7222 2929 0a20 2020 2072 6f6f 745f  tor")).    root_
+00003780: 656c 656d 656e 742e 6170 7065 6e64 2872  element.append(r
+00003790: 6573 5f64 6566 6175 6c74 290a 0a20 2020  es_default)..   
+000037a0: 2072 6573 5f72 6573 7472 6963 7465 6420   res_restricted 
+000037b0: 3d20 5045 524d 4953 5349 4f4e 5328 6964  = PERMISSIONS(id
+000037c0: 3d22 7265 732d 7265 7374 7269 6374 6564  ="res-restricted
+000037d0: 2229 0a20 2020 2072 6573 5f72 6573 7472  ").    res_restr
+000037e0: 6963 7465 642e 6170 7065 6e64 2841 4c4c  icted.append(ALL
+000037f0: 4f57 2822 4d22 2c20 6772 6f75 703d 2250  OW("M", group="P
+00003800: 726f 6a65 6374 4d65 6d62 6572 2229 290a  rojectMember")).
+00003810: 2020 2020 7265 735f 7265 7374 7269 6374      res_restrict
+00003820: 6564 2e61 7070 656e 6428 414c 4c4f 5728  ed.append(ALLOW(
+00003830: 2243 5222 2c20 6772 6f75 703d 2250 726f  "CR", group="Pro
+00003840: 6a65 6374 4164 6d69 6e22 2929 0a20 2020  jectAdmin")).   
+00003850: 2072 6573 5f72 6573 7472 6963 7465 642e   res_restricted.
+00003860: 6170 7065 6e64 2841 4c4c 4f57 2822 4352  append(ALLOW("CR
+00003870: 222c 2067 726f 7570 3d22 4372 6561 746f  ", group="Creato
+00003880: 7222 2929 0a20 2020 2072 6f6f 745f 656c  r")).    root_el
+00003890: 656d 656e 742e 6170 7065 6e64 2872 6573  ement.append(res
+000038a0: 5f72 6573 7472 6963 7465 6429 0a0a 2020  _restricted)..  
+000038b0: 2020 7072 6f70 5f64 6566 6175 6c74 203d    prop_default =
+000038c0: 2050 4552 4d49 5353 494f 4e53 2869 643d   PERMISSIONS(id=
+000038d0: 2270 726f 702d 6465 6661 756c 7422 290a  "prop-default").
+000038e0: 2020 2020 7072 6f70 5f64 6566 6175 6c74      prop_default
+000038f0: 2e61 7070 656e 6428 414c 4c4f 5728 2256  .append(ALLOW("V
+00003900: 222c 2067 726f 7570 3d22 556e 6b6e 6f77  ", group="Unknow
+00003910: 6e55 7365 7222 2929 0a20 2020 2070 726f  nUser")).    pro
+00003920: 705f 6465 6661 756c 742e 6170 7065 6e64  p_default.append
+00003930: 2841 4c4c 4f57 2822 5622 2c20 6772 6f75  (ALLOW("V", grou
+00003940: 703d 224b 6e6f 776e 5573 6572 2229 290a  p="KnownUser")).
+00003950: 2020 2020 7072 6f70 5f64 6566 6175 6c74      prop_default
+00003960: 2e61 7070 656e 6428 414c 4c4f 5728 2244  .append(ALLOW("D
+00003970: 222c 2067 726f 7570 3d22 5072 6f6a 6563  ", group="Projec
+00003980: 744d 656d 6265 7222 2929 0a20 2020 2070  tMember")).    p
+00003990: 726f 705f 6465 6661 756c 742e 6170 7065  rop_default.appe
+000039a0: 6e64 2841 4c4c 4f57 2822 4352 222c 2067  nd(ALLOW("CR", g
+000039b0: 726f 7570 3d22 5072 6f6a 6563 7441 646d  roup="ProjectAdm
+000039c0: 696e 2229 290a 2020 2020 7072 6f70 5f64  in")).    prop_d
+000039d0: 6566 6175 6c74 2e61 7070 656e 6428 414c  efault.append(AL
+000039e0: 4c4f 5728 2243 5222 2c20 6772 6f75 703d  LOW("CR", group=
+000039f0: 2243 7265 6174 6f72 2229 290a 2020 2020  "Creator")).    
+00003a00: 726f 6f74 5f65 6c65 6d65 6e74 2e61 7070  root_element.app
+00003a10: 656e 6428 7072 6f70 5f64 6566 6175 6c74  end(prop_default
+00003a20: 290a 0a20 2020 2070 726f 705f 7265 7374  )..    prop_rest
+00003a30: 7269 6374 6564 203d 2050 4552 4d49 5353  ricted = PERMISS
+00003a40: 494f 4e53 2869 643d 2270 726f 702d 7265  IONS(id="prop-re
+00003a50: 7374 7269 6374 6564 2229 0a20 2020 2070  stricted").    p
+00003a60: 726f 705f 7265 7374 7269 6374 6564 2e61  rop_restricted.a
+00003a70: 7070 656e 6428 414c 4c4f 5728 224d 222c  ppend(ALLOW("M",
+00003a80: 2067 726f 7570 3d22 5072 6f6a 6563 744d   group="ProjectM
+00003a90: 656d 6265 7222 2929 0a20 2020 2070 726f  ember")).    pro
+00003aa0: 705f 7265 7374 7269 6374 6564 2e61 7070  p_restricted.app
+00003ab0: 656e 6428 414c 4c4f 5728 2243 5222 2c20  end(ALLOW("CR", 
+00003ac0: 6772 6f75 703d 2250 726f 6a65 6374 4164  group="ProjectAd
+00003ad0: 6d69 6e22 2929 0a20 2020 2070 726f 705f  min")).    prop_
+00003ae0: 7265 7374 7269 6374 6564 2e61 7070 656e  restricted.appen
+00003af0: 6428 414c 4c4f 5728 2243 5222 2c20 6772  d(ALLOW("CR", gr
+00003b00: 6f75 703d 2243 7265 6174 6f72 2229 290a  oup="Creator")).
+00003b10: 2020 2020 726f 6f74 5f65 6c65 6d65 6e74      root_element
+00003b20: 2e61 7070 656e 6428 7072 6f70 5f72 6573  .append(prop_res
+00003b30: 7472 6963 7465 6429 0a0a 2020 2020 7265  tricted)..    re
+00003b40: 7475 726e 2072 6f6f 745f 656c 656d 656e  turn root_elemen
+00003b50: 740a 0a0a 6465 6620 6d61 6b65 5f72 6573  t...def make_res
+00003b60: 6f75 7263 6528 2020 2320 6e6f 7161 3a20  ource(  # noqa: 
+00003b70: 4434 3137 2028 756e 646f 6375 6d65 6e74  D417 (undocument
+00003b80: 6564 2d70 6172 616d 290a 2020 2020 6c61  ed-param).    la
+00003b90: 6265 6c3a 2073 7472 2c0a 2020 2020 7265  bel: str,.    re
+00003ba0: 7374 7970 653a 2073 7472 2c0a 2020 2020  stype: str,.    
+00003bb0: 6964 3a20 7374 722c 0a20 2020 2070 6572  id: str,.    per
+00003bc0: 6d69 7373 696f 6e73 3a20 7374 7220 3d20  missions: str = 
+00003bd0: 2272 6573 2d64 6566 6175 6c74 222c 0a20  "res-default",. 
+00003be0: 2020 2061 726b 3a20 4f70 7469 6f6e 616c     ark: Optional
+00003bf0: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00003c00: 2020 6972 693a 204f 7074 696f 6e61 6c5b    iri: Optional[
+00003c10: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00003c20: 2063 7265 6174 696f 6e5f 6461 7465 3a20   creation_date: 
+00003c30: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00003c40: 4e6f 6e65 2c0a 2920 2d3e 2065 7472 6565  None,.) -> etree
+00003c50: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
+00003c60: 2222 0a20 2020 2043 7265 6174 6573 2061  "".    Creates a
+00003c70: 6e20 656d 7074 7920 7265 736f 7572 6365  n empty resource
+00003c80: 2065 6c65 6d65 6e74 2c20 7769 7468 2074   element, with t
+00003c90: 6865 2061 7474 7269 6275 7465 7320 6173  he attributes as
+00003ca0: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+00003cb0: 6520 6172 6775 6d65 6e74 730a 0a20 2020  e arguments..   
+00003cc0: 2041 7267 733a 0a20 2020 2020 2020 2054   Args:.        T
+00003cd0: 6865 2061 7267 756d 656e 7473 2063 6f72  he arguments cor
+00003ce0: 7265 7370 6f6e 6420 746f 2074 6865 2061  respond to the a
+00003cf0: 7474 7269 6275 7465 7320 6f66 2074 6865  ttributes of the
+00003d00: 203c 7265 736f 7572 6365 3e20 656c 656d   <resource> elem
+00003d10: 656e 742e 0a0a 2020 2020 5265 7475 726e  ent...    Return
+00003d20: 733a 0a20 2020 2020 2020 2054 6865 2072  s:.        The r
+00003d30: 6573 6f75 7263 6520 656c 656d 656e 742c  esource element,
+00003d40: 2077 6974 686f 7574 2061 6e79 2063 6869   without any chi
+00003d50: 6c64 7265 6e2c 2062 7574 2077 6974 6820  ldren, but with 
+00003d60: 7468 6520 6174 7472 6962 7574 6573 0a20  the attributes. 
+00003d70: 2020 2020 2020 2060 603c 7265 736f 7572         ``<resour
+00003d80: 6365 206c 6162 656c 3d6c 6162 656c 2072  ce label=label r
+00003d90: 6573 7479 7065 3d72 6573 7479 7065 2069  estype=restype i
+00003da0: 643d 6964 2070 6572 6d69 7373 696f 6e73  d=id permissions
+00003db0: 3d70 6572 6d69 7373 696f 6e73 2061 726b  =permissions ark
+00003dc0: 3d61 726b 2069 7269 3d69 7269 3e3c 2f72  =ark iri=iri></r
+00003dd0: 6573 6f75 7263 653e 6060 0a0a 2020 2020  esource>``..    
+00003de0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00003df0: 5761 726e 696e 673a 2069 6620 626f 7468  Warning: if both
+00003e00: 2061 6e20 4152 4b20 616e 6420 616e 2049   an ARK and an I
+00003e10: 5249 2061 7265 2070 726f 7669 6465 640a  RI are provided.
+00003e20: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+00003e30: 723a 2069 6620 7468 6520 6372 6561 7469  r: if the creati
+00003e40: 6f6e 2064 6174 6520 6973 2069 6e76 616c  on date is inval
+00003e50: 6964 0a0a 2020 2020 4578 616d 706c 6573  id..    Examples
+00003e60: 3a0a 2020 2020 2020 2020 3e3e 3e20 7265  :.        >>> re
+00003e70: 736f 7572 6365 203d 2065 7863 656c 3278  source = excel2x
+00003e80: 6d6c 2e6d 616b 655f 7265 736f 7572 6365  ml.make_resource
+00003e90: 282e 2e2e 290a 2020 2020 2020 2020 3e3e  (...).        >>
+00003ea0: 3e20 7265 736f 7572 6365 2e61 7070 656e  > resource.appen
+00003eb0: 6428 6578 6365 6c32 786d 6c2e 6d61 6b65  d(excel2xml.make
+00003ec0: 5f74 6578 745f 7072 6f70 282e 2e2e 2929  _text_prop(...))
+00003ed0: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
+00003ee0: 742e 6170 7065 6e64 2872 6573 6f75 7263  t.append(resourc
+00003ef0: 6529 0a0a 2020 2020 5365 6520 6874 7470  e)..    See http
+00003f00: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+00003f10: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+00003f20: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+00003f30: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+00003f40: 2f23 6465 7363 7269 6269 6e67 2d72 6573  /#describing-res
+00003f50: 6f75 7263 6573 2d77 6974 682d 7468 652d  ources-with-the-
+00003f60: 7265 736f 7572 6365 2d65 6c65 6d65 6e74  resource-element
+00003f70: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
+00003f80: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
+00003f90: 6c61 6265 6c29 3a0a 2020 2020 2020 2020  label):.        
+00003fa0: 7761 726e 696e 6773 2e77 6172 6e28 6622  warnings.warn(f"
+00003fb0: 5741 524e 494e 473a 2059 6f75 7220 7265  WARNING: Your re
+00003fc0: 736f 7572 6365 2773 206c 6162 656c 206c  source's label l
+00003fd0: 6f6f 6b73 2073 7573 7069 6369 6f75 7320  ooks suspicious 
+00003fe0: 2872 6573 6f75 7263 6520 7769 7468 2069  (resource with i
+00003ff0: 6420 277b 6964 7d27 2061 6e64 206c 6162  d '{id}' and lab
+00004000: 656c 2027 7b6c 6162 656c 7d27 2922 290a  el '{label}')").
+00004010: 2020 2020 6966 206e 6f74 2063 6865 636b      if not check
+00004020: 5f6e 6f74 6e61 2869 6429 3a0a 2020 2020  _notna(id):.    
+00004030: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+00004040: 6e28 6622 5741 524e 494e 473a 2059 6f75  n(f"WARNING: You
+00004050: 7220 7265 736f 7572 6365 2773 2069 6420  r resource's id 
+00004060: 6c6f 6f6b 7320 7375 7370 6963 696f 7573  looks suspicious
+00004070: 2028 7265 736f 7572 6365 2077 6974 6820   (resource with 
+00004080: 6964 2027 7b69 647d 2720 616e 6420 6c61  id '{id}' and la
+00004090: 6265 6c20 277b 6c61 6265 6c7d 2722 290a  bel '{label}'").
+000040a0: 2020 2020 6b77 6172 6773 203d 207b 226c      kwargs = {"l
+000040b0: 6162 656c 223a 206c 6162 656c 2c20 2272  abel": label, "r
+000040c0: 6573 7479 7065 223a 2072 6573 7479 7065  estype": restype
+000040d0: 2c20 2269 6422 3a20 6964 2c20 2270 6572  , "id": id, "per
+000040e0: 6d69 7373 696f 6e73 223a 2070 6572 6d69  missions": permi
+000040f0: 7373 696f 6e73 2c20 226e 736d 6170 223a  ssions, "nsmap":
+00004100: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+00004110: 6170 7d0a 2020 2020 6966 2061 726b 3a0a  ap}.    if ark:.
+00004120: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+00004130: 6172 6b22 5d20 3d20 6172 6b0a 2020 2020  ark"] = ark.    
+00004140: 6966 2069 7269 3a0a 2020 2020 2020 2020  if iri:.        
+00004150: 6b77 6172 6773 5b22 6972 6922 5d20 3d20  kwargs["iri"] = 
+00004160: 6972 690a 2020 2020 6966 2061 726b 2061  iri.    if ark a
+00004170: 6e64 2069 7269 3a0a 2020 2020 2020 2020  nd iri:.        
+00004180: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+00004190: 2020 2020 2020 2020 2020 2066 2242 6f74             f"Bot
+000041a0: 6820 4152 4b20 616e 6420 4952 4920 7765  h ARK and IRI we
+000041b0: 7265 2070 726f 7669 6465 6420 666f 7220  re provided for 
+000041c0: 7265 736f 7572 6365 2027 7b6c 6162 656c  resource '{label
+000041d0: 7d27 2028 7b69 647d 292e 2054 6865 2041  }' ({id}). The A
+000041e0: 524b 2077 696c 6c20 6f76 6572 7269 6465  RK will override
+000041f0: 2074 6865 2049 5249 2e22 2c0a 2020 2020   the IRI.",.    
+00004200: 2020 2020 2020 2020 7374 6163 6b6c 6576          stacklev
+00004210: 656c 3d32 2c0a 2020 2020 2020 2020 290a  el=2,.        ).
+00004220: 2020 2020 6966 2063 7265 6174 696f 6e5f      if creation_
+00004230: 6461 7465 3a0a 2020 2020 2020 2020 7472  date:.        tr
+00004240: 793a 0a20 2020 2020 2020 2020 2020 2044  y:.            D
+00004250: 6174 6554 696d 6553 7461 6d70 2863 7265  ateTimeStamp(cre
+00004260: 6174 696f 6e5f 6461 7465 290a 2020 2020  ation_date).    
+00004270: 2020 2020 6578 6365 7074 2042 6173 6545      except BaseE
+00004280: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00004290: 2020 7261 6973 6520 4261 7365 4572 726f    raise BaseErro
+000042a0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+000042b0: 2020 2066 2254 6865 2072 6573 6f75 7263     f"The resourc
+000042c0: 6520 277b 6c61 6265 6c7d 2720 2849 443a  e '{label}' (ID:
+000042d0: 207b 6964 7d29 2068 6173 2061 6e20 696e   {id}) has an in
+000042e0: 7661 6c69 6420 6372 6561 7469 6f6e 2064  valid creation d
+000042f0: 6174 6520 277b 6372 6561 7469 6f6e 5f64  ate '{creation_d
+00004300: 6174 657d 272e 2022 0a20 2020 2020 2020  ate}'. ".       
+00004310: 2020 2020 2020 2020 2066 2244 6964 2079           f"Did y
+00004320: 6f75 2070 6572 6861 7073 2066 6f72 6765  ou perhaps forge
+00004330: 7420 7468 6520 7469 6d65 7a6f 6e65 3f22  t the timezone?"
+00004340: 0a20 2020 2020 2020 2020 2020 2029 2066  .            ) f
+00004350: 726f 6d20 4e6f 6e65 0a20 2020 2020 2020  rom None.       
+00004360: 206b 7761 7267 735b 2263 7265 6174 696f   kwargs["creatio
+00004370: 6e5f 6461 7465 225d 203d 2063 7265 6174  n_date"] = creat
+00004380: 696f 6e5f 6461 7465 0a0a 2020 2020 7265  ion_date..    re
+00004390: 7475 726e 2065 7472 6565 2e45 6c65 6d65  turn etree.Eleme
+000043a0: 6e74 2822 7b25 737d 7265 736f 7572 6365  nt("{%s}resource
+000043b0: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
+000043c0: 655f 6d61 705b 4e6f 6e65 5d2c 202a 2a6b  e_map[None], **k
+000043d0: 7761 7267 7329 2020 2320 7479 7065 3a20  wargs)  # type: 
+000043e0: 6967 6e6f 7265 5b61 7267 2d74 7970 655d  ignore[arg-type]
+000043f0: 0a0a 0a64 6566 206d 616b 655f 6269 7473  ...def make_bits
+00004400: 7472 6561 6d5f 7072 6f70 280a 2020 2020  tream_prop(.    
+00004410: 7061 7468 3a20 556e 696f 6e5b 7374 722c  path: Union[str,
+00004420: 206f 732e 5061 7468 4c69 6b65 5b41 6e79   os.PathLike[Any
+00004430: 5d5d 2c0a 2020 2020 7065 726d 6973 7369  ]],.    permissi
+00004440: 6f6e 733a 2073 7472 203d 2022 7072 6f70  ons: str = "prop
+00004450: 2d64 6566 6175 6c74 222c 0a20 2020 2063  -default",.    c
+00004460: 6865 636b 3a20 626f 6f6c 203d 2046 616c  heck: bool = Fal
+00004470: 7365 2c0a 2020 2020 6361 6c6c 696e 675f  se,.    calling_
+00004480: 7265 736f 7572 6365 3a20 7374 7220 3d20  resource: str = 
+00004490: 2222 2c0a 2920 2d3e 2065 7472 6565 2e5f  "",.) -> etree._
+000044a0: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
+000044b0: 0a20 2020 2043 7265 6174 6573 2061 2062  .    Creates a b
+000044c0: 6974 7374 7265 616d 2065 6c65 6d65 6e74  itstream element
+000044d0: 2074 6861 7420 706f 696e 7473 2074 6f20   that points to 
+000044e0: 2270 6174 6822 2e0a 0a20 2020 2041 7267  "path"...    Arg
+000044f0: 733a 0a20 2020 2020 2020 2070 6174 683a  s:.        path:
+00004500: 2070 6174 6820 746f 2061 2076 616c 6964   path to a valid
+00004510: 2066 696c 6520 7468 6174 2077 696c 6c20   file that will 
+00004520: 6265 2075 706c 6f61 6465 640a 2020 2020  be uploaded.    
+00004530: 2020 2020 7065 726d 6973 7369 6f6e 733a      permissions:
+00004540: 2070 6572 6d69 7373 696f 6e73 2073 7472   permissions str
+00004550: 696e 670a 2020 2020 2020 2020 6368 6563  ing.        chec
+00004560: 6b3a 2069 6620 5472 7565 2c20 6973 7375  k: if True, issu
+00004570: 6520 6120 7761 726e 696e 6720 6966 2074  e a warning if t
+00004580: 6865 2070 6174 6820 646f 6573 6e27 7420  he path doesn't 
+00004590: 706f 696e 7420 746f 2061 6e20 6578 6973  point to an exis
+000045a0: 7469 6e67 2066 696c 650a 2020 2020 2020  ting file.      
+000045b0: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+000045c0: 6365 3a20 7468 6520 6e61 6d65 206f 6620  ce: the name of 
+000045d0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+000045e0: 7263 6520 2866 6f72 2062 6574 7465 7220  rce (for better 
+000045f0: 6572 726f 7220 6d65 7373 6167 6573 290a  error messages).
+00004600: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+00004610: 2020 2020 2057 6172 6e69 6e67 3a20 6966       Warning: if
+00004620: 2074 6865 2070 6174 6820 646f 6573 6e27   the path doesn'
+00004630: 7420 706f 696e 7420 746f 2061 6e20 6578  t point to an ex
+00004640: 6973 7469 6e67 2066 696c 6520 286f 6e6c  isting file (onl
+00004650: 7920 6966 2063 6865 636b 3d54 7275 6529  y if check=True)
+00004660: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00004670: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
+00004680: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
+00004690: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
+000046a0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+000046b0: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
+000046c0: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
+000046d0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
+000046e0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+000046f0: 2020 203e 3e3e 2072 6573 6f75 7263 6520     >>> resource 
+00004700: 3d20 6578 6365 6c32 786d 6c2e 6d61 6b65  = excel2xml.make
+00004710: 5f72 6573 6f75 7263 6528 2e2e 2e29 0a20  _resource(...). 
+00004720: 2020 2020 2020 203e 3e3e 2072 6573 6f75         >>> resou
+00004730: 7263 652e 6170 7065 6e64 2865 7863 656c  rce.append(excel
+00004740: 3278 6d6c 2e6d 616b 655f 6269 7473 7472  2xml.make_bitstr
+00004750: 6561 6d5f 7072 6f70 2822 6461 7461 2f69  eam_prop("data/i
+00004760: 6d61 6765 732f 7472 6565 2e6a 7067 2229  mages/tree.jpg")
+00004770: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
+00004780: 6f74 2e61 7070 656e 6428 7265 736f 7572  ot.append(resour
+00004790: 6365 290a 0a20 2020 2053 6565 2068 7474  ce)..    See htt
+000047a0: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
+000047b0: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
+000047c0: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
+000047d0: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
+000047e0: 652f 2362 6974 7374 7265 616d 0a20 2020  e/#bitstream.   
+000047f0: 2022 2222 0a0a 2020 2020 6966 2063 6865   """..    if che
+00004800: 636b 2061 6e64 206e 6f74 2050 6174 6828  ck and not Path(
+00004810: 7061 7468 292e 6973 5f66 696c 6528 293a  path).is_file():
+00004820: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
+00004830: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00004840: 2020 2020 6622 4661 696c 6564 2076 616c      f"Failed val
+00004850: 6964 6174 696f 6e20 696e 2062 6974 7374  idation in bitst
+00004860: 7265 616d 2074 6167 206f 6620 7265 736f  ream tag of reso
+00004870: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
+00004880: 6573 6f75 7263 657d 273a 2022 0a20 2020  esource}': ".   
+00004890: 2020 2020 2020 2020 2066 2254 6865 2066           f"The f
+000048a0: 6f6c 6c6f 7769 6e67 2070 6174 6820 646f  ollowing path do
+000048b0: 6573 6e27 7420 706f 696e 7420 746f 2061  esn't point to a
+000048c0: 2066 696c 653a 207b 7061 7468 7d22 2c0a   file: {path}",.
+000048d0: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+000048e0: 6b6c 6576 656c 3d32 2c0a 2020 2020 2020  klevel=2,.      
+000048f0: 2020 290a 2020 2020 7072 6f70 5f20 3d20    ).    prop_ = 
+00004900: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
+00004910: 2020 2020 2020 2022 7b25 737d 6269 7473         "{%s}bits
+00004920: 7472 6561 6d22 2025 2078 6d6c 5f6e 616d  tream" % xml_nam
+00004930: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+00004940: 2c0a 2020 2020 2020 2020 7065 726d 6973  ,.        permis
+00004950: 7369 6f6e 733d 7065 726d 6973 7369 6f6e  sions=permission
+00004960: 732c 0a20 2020 2020 2020 206e 736d 6170  s,.        nsmap
+00004970: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
+00004980: 6170 2c0a 2020 2020 290a 2020 2020 7072  ap,.    ).    pr
+00004990: 6f70 5f2e 7465 7874 203d 2073 7472 2870  op_.text = str(p
+000049a0: 6174 6829 0a20 2020 2072 6574 7572 6e20  ath).    return 
+000049b0: 7072 6f70 5f0a 0a0a 6465 6620 5f66 6f72  prop_...def _for
+000049c0: 6d61 745f 626f 6f6c 280a 2020 2020 756e  mat_bool(.    un
+000049d0: 666f 726d 6174 7465 643a 2055 6e69 6f6e  formatted: Union
+000049e0: 5b62 6f6f 6c2c 2073 7472 2c20 696e 742c  [bool, str, int,
+000049f0: 2066 6c6f 6174 5d2c 0a20 2020 206e 616d   float],.    nam
+00004a00: 653a 2073 7472 2c0a 2020 2020 6361 6c6c  e: str,.    call
+00004a10: 696e 675f 7265 736f 7572 6365 3a20 7374  ing_resource: st
+00004a20: 722c 0a29 202d 3e20 7374 723a 0a20 2020  r,.) -> str:.   
+00004a30: 2022 2222 0a20 2020 2054 6869 7320 6d65   """.    This me
+00004a40: 7468 6f64 2074 616b 6573 2061 6e20 756e  thod takes an un
+00004a50: 666f 726d 6174 7465 6420 626f 6f6c 6561  formatted boolea
+00004a60: 6e2d 6c69 6b65 2076 616c 7565 2c20 616e  n-like value, an
+00004a70: 6420 7472 616e 7366 6f72 6d73 2069 7420  d transforms it 
+00004a80: 696e 746f 2074 6865 2073 7472 696e 6720  into the string 
+00004a90: 7661 6c75 6573 2022 7472 7565 2220 6f72  values "true" or
+00004aa0: 2022 6661 6c73 6522 2e0a 0a20 2020 2041   "false"...    A
+00004ab0: 7267 733a 0a20 2020 2020 2020 2075 6e66  rgs:.        unf
+00004ac0: 6f72 6d61 7474 6564 3a20 626f 6f6c 6561  ormatted: boolea
+00004ad0: 6e2d 6c69 6b65 2076 616c 7565 0a20 2020  n-like value.   
+00004ae0: 2020 2020 206e 616d 653a 2070 726f 7065       name: prope
+00004af0: 7274 7920 6e61 6d65 2c20 666f 7220 6265  rty name, for be
 00004b00: 7474 6572 2065 7272 6f72 206d 6573 7361  tter error messa
-00004b10: 6765 730a 0a20 2020 2052 6169 7365 733a  ges..    Raises:
-00004b20: 0a20 2020 2020 2020 2042 6173 6545 7272  .        BaseErr
-00004b30: 6f72 3a20 6966 2074 6865 2069 6e70 7574  or: if the input
-00004b40: 2063 616e 6e6f 7420 6265 2074 7261 6e73   cannot be trans
-00004b50: 666f 726d 6564 2069 6e74 6f20 2274 7275  formed into "tru
-00004b60: 6522 2f22 6661 6c73 6522 0a0a 2020 2020  e"/"false"..    
-00004b70: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00004b80: 2022 7472 7565 2220 6966 2074 6865 2069   "true" if the i
-00004b90: 6e70 7574 2069 7320 696e 2028 5472 7565  nput is in (True
-00004ba0: 2c20 2274 7275 6522 2c20 2231 222c 2031  , "true", "1", 1
-00004bb0: 2c20 2279 6573 2229 3b20 2266 616c 7365  , "yes"); "false
-00004bc0: 2220 6966 2069 6e70 7574 2069 7320 696e  " if input is in
-00004bd0: 2028 4661 6c73 652c 2022 6661 6c73 6522   (False, "false"
-00004be0: 2c20 2230 222c 2030 2c20 226e 6f22 290a  , "0", 0, "no").
-00004bf0: 2020 2020 2222 220a 2020 2020 6966 2069      """.    if i
-00004c00: 7369 6e73 7461 6e63 6528 756e 666f 726d  sinstance(unform
-00004c10: 6174 7465 642c 2073 7472 293a 0a20 2020  atted, str):.   
-00004c20: 2020 2020 2075 6e66 6f72 6d61 7474 6564       unformatted
-00004c30: 203d 2075 6e66 6f72 6d61 7474 6564 2e6c   = unformatted.l
-00004c40: 6f77 6572 2829 0a20 2020 2069 6620 756e  ower().    if un
-00004c50: 666f 726d 6174 7465 6420 696e 2028 4661  formatted in (Fa
-00004c60: 6c73 652c 2022 6661 6c73 6522 2c20 2230  lse, "false", "0
-00004c70: 222c 2030 2c20 302e 302c 2022 6e6f 2229  ", 0, 0.0, "no")
-00004c80: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00004c90: 2022 6661 6c73 6522 0a20 2020 2065 6c69   "false".    eli
-00004ca0: 6620 756e 666f 726d 6174 7465 6420 696e  f unformatted in
-00004cb0: 2028 5472 7565 2c20 2274 7275 6522 2c20   (True, "true", 
-00004cc0: 2231 222c 2031 2c20 312e 302c 2022 7965  "1", 1, 1.0, "ye
-00004cd0: 7322 293a 0a20 2020 2020 2020 2072 6574  s"):.        ret
-00004ce0: 7572 6e20 2274 7275 6522 0a20 2020 2065  urn "true".    e
-00004cf0: 6c73 653a 0a20 2020 2020 2020 2072 6169  lse:.        rai
-00004d00: 7365 2042 6173 6545 7272 6f72 280a 2020  se BaseError(.  
-00004d10: 2020 2020 2020 2020 2020 6622 4661 696c            f"Fail
-00004d20: 6564 2076 616c 6964 6174 696f 6e20 696e  ed validation in
-00004d30: 2072 6573 6f75 7263 6520 277b 6361 6c6c   resource '{call
-00004d40: 696e 675f 7265 736f 7572 6365 7d27 2c20  ing_resource}', 
-00004d50: 7072 6f70 6572 7479 2027 7b6e 616d 657d  property '{name}
-00004d60: 273a 2022 0a20 2020 2020 2020 2020 2020  ': ".           
-00004d70: 2066 2227 7b75 6e66 6f72 6d61 7474 6564   f"'{unformatted
-00004d80: 7d27 2069 7320 6e6f 7420 6120 7661 6c69  }' is not a vali
-00004d90: 6420 626f 6f6c 6561 6e2e 220a 2020 2020  d boolean.".    
-00004da0: 2020 2020 290a 0a0a 6465 6620 6d61 6b65      )...def make
-00004db0: 5f62 6f6f 6c65 616e 5f70 726f 7028 0a20  _boolean_prop(. 
-00004dc0: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
-00004dd0: 2020 7661 6c75 653a 2055 6e69 6f6e 5b50    value: Union[P
-00004de0: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-00004df0: 7374 722c 2069 6e74 2c20 626f 6f6c 5d2c  str, int, bool],
-00004e00: 0a20 2020 2063 616c 6c69 6e67 5f72 6573  .    calling_res
-00004e10: 6f75 7263 653a 2073 7472 203d 2022 222c  ource: str = "",
-00004e20: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-00004e30: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-00004e40: 2020 4d61 6b65 2061 203c 626f 6f6c 6561    Make a <boolea
-00004e50: 6e2d 7072 6f70 3e20 6672 6f6d 2061 2062  n-prop> from a b
-00004e60: 6f6f 6c65 616e 2076 616c 7565 2e20 5468  oolean value. Th
-00004e70: 6520 7661 6c75 6520 6361 6e20 6265 2070  e value can be p
-00004e80: 726f 7669 6465 6420 6469 7265 6374 6c79  rovided directly
-00004e90: 206f 7220 696e 7369 6465 2061 2050 726f   or inside a Pro
-00004ea0: 7065 7274 7945 6c65 6d65 6e74 2e20 5468  pertyElement. Th
-00004eb0: 650a 2020 2020 666f 6c6c 6f77 696e 6720  e.    following 
-00004ec0: 666f 726d 6174 7320 6172 6520 7375 7070  formats are supp
-00004ed0: 6f72 7465 643a 0a20 2020 2020 2d20 7472  orted:.     - tr
-00004ee0: 7565 3a20 2854 7275 652c 2022 7472 7565  ue: (True, "true
-00004ef0: 222c 2022 5472 7565 222c 2022 3122 2c20  ", "True", "1", 
-00004f00: 312c 2022 7965 7322 2c20 2259 6573 2229  1, "yes", "Yes")
-00004f10: 0a20 2020 2020 2d20 6661 6c73 653a 2028  .     - false: (
-00004f20: 4661 6c73 652c 2022 6661 6c73 6522 2c20  False, "false", 
-00004f30: 2246 616c 7365 222c 2022 3022 2c20 302c  "False", "0", 0,
-00004f40: 2022 6e6f 222c 2022 4e6f 2229 0a0a 2020   "no", "No")..  
-00004f50: 2020 556e 6c65 7373 2070 726f 7669 6465    Unless provide
-00004f60: 6420 6173 2050 726f 7065 7274 7945 6c65  d as PropertyEle
-00004f70: 6d65 6e74 2c20 7468 6520 7065 726d 6973  ment, the permis
-00004f80: 7369 6f6e 7320 6f66 2074 6865 2076 616c  sions of the val
-00004f90: 7565 2064 6566 6175 6c74 2074 6f20 2270  ue default to "p
-00004fa0: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
-00004fb0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00004fc0: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
-00004fd0: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
-00004fe0: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
-00004ff0: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
-00005000: 7661 6c75 653a 2061 2062 6f6f 6c65 616e  value: a boolean
-00005010: 2076 616c 7565 2061 7320 7374 722f 626f   value as str/bo
-00005020: 6f6c 2f69 6e74 2c20 6f72 2061 7320 7374  ol/int, or as st
-00005030: 722f 626f 6f6c 2f69 6e74 2069 6e73 6964  r/bool/int insid
-00005040: 6520 6120 5072 6f70 6572 7479 456c 656d  e a PropertyElem
-00005050: 656e 740a 2020 2020 2020 2020 6361 6c6c  ent.        call
-00005060: 696e 675f 7265 736f 7572 6365 3a20 7468  ing_resource: th
-00005070: 6520 6e61 6d65 206f 6620 7468 6520 7061  e name of the pa
-00005080: 7265 6e74 2072 6573 6f75 7263 6520 2866  rent resource (f
-00005090: 6f72 2062 6574 7465 7220 6572 726f 7220  or better error 
-000050a0: 6d65 7373 6167 6573 290a 0a20 2020 2052  messages)..    R
-000050b0: 6169 7365 733a 0a20 2020 2020 2020 2042  aises:.        B
-000050c0: 6173 6545 7272 6f72 3a20 6966 2074 6865  aseError: if the
-000050d0: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
-000050e0: 7661 6c69 6420 626f 6f6c 6561 6e0a 0a20  valid boolean.. 
-000050f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00005100: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
-00005110: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
-00005120: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
-00005130: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00005140: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
-00005150: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
-00005160: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
-00005170: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00005180: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-00005190: 6b65 5f62 6f6f 6c65 616e 5f70 726f 7028  ke_boolean_prop(
-000051a0: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-000051b0: 2022 6e6f 2229 0a20 2020 2020 2020 2020   "no").         
-000051c0: 2020 2020 2020 203c 626f 6f6c 6561 6e2d         <boolean-
-000051d0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
-000051e0: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
-000051f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00005200: 626f 6f6c 6561 6e20 7065 726d 6973 7369  boolean permissi
-00005210: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-00005220: 7422 3e66 616c 7365 3c2f 626f 6f6c 6561  t">false</boolea
-00005230: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
-00005240: 2020 203c 2f62 6f6f 6c65 616e 2d70 726f     </boolean-pro
-00005250: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-00005260: 7863 656c 3278 6d6c 2e6d 616b 655f 626f  xcel2xml.make_bo
-00005270: 6f6c 6561 6e5f 7072 6f70 2822 3a74 6573  olean_prop(":tes
-00005280: 7470 726f 7065 7274 7922 2c20 6578 6365  tproperty", exce
-00005290: 6c32 786d 6c2e 5072 6f70 6572 7479 456c  l2xml.PropertyEl
-000052a0: 656d 656e 7428 2231 222c 2070 6572 6d69  ement("1", permi
-000052b0: 7373 696f 6e73 3d22 7072 6f70 2d72 6573  ssions="prop-res
-000052c0: 7472 6963 7465 6422 2c20 636f 6d6d 656e  tricted", commen
-000052d0: 743d 2265 7861 6d70 6c65 2229 290a 2020  t="example")).  
-000052e0: 2020 2020 2020 2020 2020 2020 2020 3c62                <b
-000052f0: 6f6f 6c65 616e 2d70 726f 7020 6e61 6d65  oolean-prop name
-00005300: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-00005310: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005320: 2020 2020 2020 3c62 6f6f 6c65 616e 2070        <boolean p
-00005330: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00005340: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
-00005350: 6d65 6e74 3d22 6578 616d 706c 6522 3e74  ment="example">t
-00005360: 7275 653c 2f62 6f6f 6c65 616e 3e0a 2020  rue</boolean>.  
-00005370: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00005380: 626f 6f6c 6561 6e2d 7072 6f70 3e0a 0a20  boolean-prop>.. 
-00005390: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
-000053a0: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
-000053b0: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
-000053c0: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
-000053d0: 6c2d 6461 7461 2d66 696c 652f 2362 6f6f  l-data-file/#boo
-000053e0: 6c65 616e 2d70 726f 700a 2020 2020 2222  lean-prop.    ""
-000053f0: 220a 0a20 2020 2023 2076 616c 6964 6174  "..    # validat
-00005400: 6520 696e 7075 740a 2020 2020 6966 2069  e input.    if i
-00005410: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
-00005420: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00005430: 293a 0a20 2020 2020 2020 2076 616c 7565  ):.        value
-00005440: 5f6e 6577 203d 2064 6174 6163 6c61 7373  _new = dataclass
-00005450: 6573 2e72 6570 6c61 6365 2876 616c 7565  es.replace(value
-00005460: 2c20 7661 6c75 653d 5f66 6f72 6d61 745f  , value=_format_
-00005470: 626f 6f6c 2876 616c 7565 2e76 616c 7565  bool(value.value
-00005480: 2c20 6e61 6d65 2c20 6361 6c6c 696e 675f  , name, calling_
-00005490: 7265 736f 7572 6365 2929 0a20 2020 2065  resource)).    e
-000054a0: 6c69 6620 6973 696e 7374 616e 6365 2876  lif isinstance(v
-000054b0: 616c 7565 2c20 2873 7472 2c20 626f 6f6c  alue, (str, bool
-000054c0: 2c20 696e 7429 293a 0a20 2020 2020 2020  , int)):.       
-000054d0: 2076 616c 7565 5f6e 6577 203d 2050 726f   value_new = Pro
-000054e0: 7065 7274 7945 6c65 6d65 6e74 285f 666f  pertyElement(_fo
-000054f0: 726d 6174 5f62 6f6f 6c28 7661 6c75 652c  rmat_bool(value,
-00005500: 206e 616d 652c 2063 616c 6c69 6e67 5f72   name, calling_r
-00005510: 6573 6f75 7263 6529 290a 2020 2020 656c  esource)).    el
-00005520: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
-00005530: 6520 4261 7365 4572 726f 7228 0a20 2020  e BaseError(.   
-00005540: 2020 2020 2020 2020 2066 2246 6169 6c65           f"Faile
-00005550: 6420 7661 6c69 6461 7469 6f6e 2069 6e20  d validation in 
-00005560: 7265 736f 7572 6365 2027 7b63 616c 6c69  resource '{calli
-00005570: 6e67 5f72 6573 6f75 7263 657d 272c 2070  ng_resource}', p
-00005580: 726f 7065 7274 7920 277b 6e61 6d65 7d27  roperty '{name}'
-00005590: 3a20 277b 7661 6c75 657d 2720 6973 206e  : '{value}' is n
-000055a0: 6f74 2061 2076 616c 6964 2062 6f6f 6c65  ot a valid boole
-000055b0: 616e 2e22 0a20 2020 2020 2020 2029 0a0a  an.".        )..
-000055c0: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
-000055d0: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
-000055e0: 7661 6c75 650a 2020 2020 7072 6f70 5f20  value.    prop_ 
-000055f0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-00005600: 0a20 2020 2020 2020 2022 7b25 737d 626f  .        "{%s}bo
-00005610: 6f6c 6561 6e2d 7072 6f70 2220 2520 786d  olean-prop" % xm
-00005620: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
-00005630: 4e6f 6e65 5d2c 0a20 2020 2020 2020 206e  None],.        n
-00005640: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
-00005650: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
-00005660: 7370 6163 655f 6d61 702c 0a20 2020 2029  space_map,.    )
-00005670: 0a20 2020 206b 7761 7267 7320 3d20 7b22  .    kwargs = {"
-00005680: 7065 726d 6973 7369 6f6e 7322 3a20 7661  permissions": va
-00005690: 6c75 655f 6e65 772e 7065 726d 6973 7369  lue_new.permissi
-000056a0: 6f6e 737d 0a20 2020 2069 6620 7661 6c75  ons}.    if valu
-000056b0: 655f 6e65 772e 636f 6d6d 656e 7420 616e  e_new.comment an
-000056c0: 6420 6368 6563 6b5f 6e6f 746e 6128 7661  d check_notna(va
-000056d0: 6c75 655f 6e65 772e 636f 6d6d 656e 7429  lue_new.comment)
-000056e0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
-000056f0: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
-00005700: 6c75 655f 6e65 772e 636f 6d6d 656e 740a  lue_new.comment.
-00005710: 2020 2020 7661 6c75 655f 203d 2065 7472      value_ = etr
-00005720: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-00005730: 2020 2020 227b 2573 7d62 6f6f 6c65 616e      "{%s}boolean
-00005740: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-00005750: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-00005760: 2020 2020 202a 2a6b 7761 7267 732c 2020       **kwargs,  
-00005770: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
-00005780: 7267 2d74 7970 655d 0a20 2020 2020 2020  rg-type].       
-00005790: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-000057a0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
-000057b0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
-000057c0: 3d20 7374 7228 7661 6c75 655f 6e65 772e  = str(value_new.
-000057d0: 7661 6c75 6529 0a20 2020 2070 726f 705f  value).    prop_
-000057e0: 2e61 7070 656e 6428 7661 6c75 655f 290a  .append(value_).
-000057f0: 0a20 2020 2072 6574 7572 6e20 7072 6f70  .    return prop
-00005800: 5f0a 0a0a 6465 6620 6d61 6b65 5f63 6f6c  _...def make_col
-00005810: 6f72 5f70 726f 7028 0a20 2020 206e 616d  or_prop(.    nam
-00005820: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
-00005830: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
-00005840: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
-00005850: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
-00005860: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-00005870: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
-00005880: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
-00005890: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
-000058a0: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
-000058b0: 2222 220a 2020 2020 4d61 6b65 2061 203c  """.    Make a <
-000058c0: 636f 6c6f 722d 7072 6f70 3e20 6672 6f6d  color-prop> from
-000058d0: 206f 6e65 206f 7220 6d6f 7265 2063 6f6c   one or more col
-000058e0: 6f72 732e 2054 6865 2063 6f6c 6f72 2873  ors. The color(s
-000058f0: 2920 6361 6e20 6265 2070 726f 7669 6465  ) can be provide
-00005900: 6420 6173 2073 7472 696e 6720 6f72 2061  d as string or a
-00005910: 7320 5072 6f70 6572 7479 456c 656d 656e  s PropertyElemen
-00005920: 7420 7769 7468 2061 0a20 2020 2073 7472  t with a.    str
-00005930: 696e 6720 696e 7369 6465 2e20 4966 2070  ing inside. If p
-00005940: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
-00005950: 672c 2074 6865 2070 6572 6d69 7373 696f  g, the permissio
-00005960: 6e73 2064 6566 6175 6c74 2074 6f20 2270  ns default to "p
-00005970: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
-00005980: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00005990: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
-000059a0: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
-000059b0: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
-000059c0: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
-000059d0: 7661 6c75 653a 206f 6e65 206f 7220 6d6f  value: one or mo
-000059e0: 7265 2044 5350 2063 6f6c 6f72 2873 292c  re DSP color(s),
-000059f0: 2061 7320 7374 7269 6e67 2f50 726f 7065   as string/Prope
-00005a00: 7274 7945 6c65 6d65 6e74 2c20 6f72 2061  rtyElement, or a
-00005a10: 7320 6974 6572 6162 6c65 206f 6620 7374  s iterable of st
-00005a20: 7269 6e67 732f 5072 6f70 6572 7479 456c  rings/PropertyEl
-00005a30: 656d 656e 7473 0a20 2020 2020 2020 2063  ements.        c
-00005a40: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
-00005a50: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
-00005a60: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
-00005a70: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
-00005a80: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
-00005a90: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00005aa0: 2020 4261 7365 4572 726f 723a 2049 6620    BaseError: If 
-00005ab0: 7468 6520 7661 6c75 6520 6973 206e 6f74  the value is not
-00005ac0: 2061 2076 616c 6964 2063 6f6c 6f72 0a0a   a valid color..
-00005ad0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00005ae0: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
-00005af0: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
-00005b00: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
-00005b10: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
-00005b20: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
-00005b30: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
-00005b40: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
-00005b50: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-00005b60: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-00005b70: 616b 655f 636f 6c6f 725f 7072 6f70 2822  ake_color_prop("
-00005b80: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-00005b90: 2223 3030 6666 3636 2229 0a20 2020 2020  "#00ff66").     
-00005ba0: 2020 2020 2020 2020 2020 203c 636f 6c6f             <colo
-00005bb0: 722d 7072 6f70 206e 616d 653d 223a 7465  r-prop name=":te
-00005bc0: 7374 7072 6f70 6572 7479 223e 0a20 2020  stproperty">.   
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005be0: 203c 636f 6c6f 7220 7065 726d 6973 7369   <color permissi
-00005bf0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-00005c00: 7422 3e23 3030 6666 3636 3c2f 636f 6c6f  t">#00ff66</colo
-00005c10: 723e 0a20 2020 2020 2020 2020 2020 2020  r>.             
-00005c20: 2020 203c 2f63 6f6c 6f72 2d70 726f 703e     </color-prop>
-00005c30: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
-00005c40: 656c 3278 6d6c 2e6d 616b 655f 636f 6c6f  el2xml.make_colo
-00005c50: 725f 7072 6f70 2822 3a74 6573 7470 726f  r_prop(":testpro
-00005c60: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
-00005c70: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
-00005c80: 7428 2223 3030 6666 3636 222c 2070 6572  t("#00ff66", per
-00005c90: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
-00005ca0: 6573 7472 6963 7465 6422 2c20 636f 6d6d  estricted", comm
-00005cb0: 656e 743d 2265 7861 6d70 6c65 2229 290a  ent="example")).
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 3c63 6f6c 6f72 2d70 726f 7020 6e61 6d65  <color-prop name
-00005ce0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-00005cf0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005d00: 2020 2020 2020 3c63 6f6c 6f72 2070 6572        <color per
-00005d10: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
-00005d20: 6573 7472 6963 7465 6422 2063 6f6d 6d65  estricted" comme
-00005d30: 6e74 3d22 6578 616d 706c 6522 3e23 3030  nt="example">#00
-00005d40: 6666 3636 3c2f 636f 6c6f 723e 0a20 2020  ff66</color>.   
-00005d50: 2020 2020 2020 2020 2020 2020 203c 2f63               </c
-00005d60: 6f6c 6f72 2d70 726f 703e 0a20 2020 2020  olor-prop>.     
-00005d70: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-00005d80: 2e6d 616b 655f 636f 6c6f 725f 7072 6f70  .make_color_prop
-00005d90: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-00005da0: 2c20 5b22 2330 3066 6636 3622 2c20 2223  , ["#00ff66", "#
-00005db0: 3030 3030 3030 225d 290a 2020 2020 2020  000000"]).      
-00005dc0: 2020 2020 2020 2020 2020 3c63 6f6c 6f72            <color
-00005dd0: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
-00005de0: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
-00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e00: 3c63 6f6c 6f72 2070 6572 6d69 7373 696f  <color permissio
-00005e10: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
-00005e20: 223e 2330 3066 6636 363c 2f63 6f6c 6f72  ">#00ff66</color
-00005e30: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005e40: 2020 2020 2020 3c63 6f6c 6f72 2070 6572        <color per
-00005e50: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-00005e60: 6566 6175 6c74 223e 2330 3030 3030 303c  efault">#000000<
-00005e70: 2f63 6f6c 6f72 3e0a 2020 2020 2020 2020  /color>.        
-00005e80: 2020 2020 2020 2020 3c2f 636f 6c6f 722d          </color-
-00005e90: 7072 6f70 3e0a 0a20 2020 2053 6565 2068  prop>..    See h
-00005ea0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
-00005eb0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
-00005ec0: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
-00005ed0: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
-00005ee0: 696c 652f 2363 6f6c 6f72 2d70 726f 700a  ile/#color-prop.
-00005ef0: 2020 2020 2222 220a 0a20 2020 2023 2063      """..    # c
-00005f00: 6865 636b 2074 6865 2069 6e70 7574 3a20  heck the input: 
-00005f10: 7072 6570 6172 6520 6120 6c69 7374 2077  prepare a list w
-00005f20: 6974 6820 7661 6c69 6420 7661 6c75 6573  ith valid values
-00005f30: 0a20 2020 2076 616c 7565 7320 3d20 7072  .    values = pr
-00005f40: 6570 6172 655f 7661 6c75 6528 7661 6c75  epare_value(valu
-00005f50: 6529 0a0a 2020 2020 2320 6368 6563 6b20  e)..    # check 
-00005f60: 7661 6c75 6520 7479 7065 0a20 2020 2066  value type.    f
-00005f70: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
-00005f80: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-00005f90: 2072 6567 6578 2e73 6561 7263 6828 7222   regex.search(r"
-00005fa0: 5e23 5b30 2d39 612d 665d 7b36 7d24 222c  ^#[0-9a-f]{6}$",
-00005fb0: 2073 7472 2876 616c 2e76 616c 7565 292e   str(val.value).
-00005fc0: 7374 7269 7028 292c 2066 6c61 6773 3d72  strip(), flags=r
-00005fd0: 6567 6578 2e49 474e 4f52 4543 4153 4529  egex.IGNORECASE)
-00005fe0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00005ff0: 6973 6520 4261 7365 4572 726f 7228 0a20  ise BaseError(. 
-00006000: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00006010: 2246 6169 6c65 6420 7661 6c69 6461 7469  "Failed validati
-00006020: 6f6e 2069 6e20 7265 736f 7572 6365 2027  on in resource '
-00006030: 7b63 616c 6c69 6e67 5f72 6573 6f75 7263  {calling_resourc
-00006040: 657d 272c 2070 726f 7065 7274 7920 277b  e}', property '{
-00006050: 6e61 6d65 7d27 3a20 220a 2020 2020 2020  name}': ".      
-00006060: 2020 2020 2020 2020 2020 6622 277b 7661            f"'{va
-00006070: 6c2e 7661 6c75 657d 2720 6973 206e 6f74  l.value}' is not
-00006080: 2061 2076 616c 6964 2063 6f6c 6f72 2e22   a valid color."
-00006090: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000060a0: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
-000060b0: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
-000060c0: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-000060d0: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
-000060e0: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-000060f0: 227b 2573 7d63 6f6c 6f72 2d70 726f 7022  "{%s}color-prop"
-00006100: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
-00006110: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
-00006120: 2020 2020 6e61 6d65 3d6e 616d 652c 0a20      name=name,. 
-00006130: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
-00006140: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
-00006150: 2020 2020 290a 2020 2020 666f 7220 7661      ).    for va
-00006160: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
-00006170: 2020 2020 206b 7761 7267 7320 3d20 7b22       kwargs = {"
-00006180: 7065 726d 6973 7369 6f6e 7322 3a20 7661  permissions": va
-00006190: 6c2e 7065 726d 6973 7369 6f6e 737d 0a20  l.permissions}. 
-000061a0: 2020 2020 2020 2069 6620 7661 6c2e 636f         if val.co
-000061b0: 6d6d 656e 7420 616e 6420 6368 6563 6b5f  mment and check_
-000061c0: 6e6f 746e 6128 7661 6c2e 636f 6d6d 656e  notna(val.commen
-000061d0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000061e0: 6b77 6172 6773 5b22 636f 6d6d 656e 7422  kwargs["comment"
-000061f0: 5d20 3d20 7661 6c2e 636f 6d6d 656e 740a  ] = val.comment.
-00006200: 2020 2020 2020 2020 7661 6c75 655f 203d          value_ =
-00006210: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-00006220: 2020 2020 2020 2020 2020 2020 227b 2573              "{%s
-00006230: 7d63 6f6c 6f72 2220 2520 786d 6c5f 6e61  }color" % xml_na
-00006240: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-00006250: 5d2c 0a20 2020 2020 2020 2020 2020 202a  ],.            *
-00006260: 2a6b 7761 7267 732c 2020 2320 7479 7065  *kwargs,  # type
-00006270: 3a20 6967 6e6f 7265 5b61 7267 2d74 7970  : ignore[arg-typ
-00006280: 655d 0a20 2020 2020 2020 2020 2020 206e  e].            n
-00006290: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
-000062a0: 6365 5f6d 6170 2c0a 2020 2020 2020 2020  ce_map,.        
-000062b0: 290a 2020 2020 2020 2020 7661 6c75 655f  ).        value_
-000062c0: 2e74 6578 7420 3d20 7374 7228 7661 6c2e  .text = str(val.
-000062d0: 7661 6c75 6529 2e73 7472 6970 2829 0a20  value).strip(). 
-000062e0: 2020 2020 2020 2070 726f 705f 2e61 7070         prop_.app
-000062f0: 656e 6428 7661 6c75 655f 290a 0a20 2020  end(value_)..   
-00006300: 2072 6574 7572 6e20 7072 6f70 5f0a 0a0a   return prop_...
-00006310: 6465 6620 6d61 6b65 5f64 6174 655f 7072  def make_date_pr
-00006320: 6f70 280a 2020 2020 6e61 6d65 3a20 7374  op(.    name: st
-00006330: 722c 0a20 2020 2076 616c 7565 3a20 556e  r,.    value: Un
-00006340: 696f 6e5b 5072 6f70 6572 7479 456c 656d  ion[PropertyElem
-00006350: 656e 742c 2073 7472 2c20 4974 6572 6162  ent, str, Iterab
-00006360: 6c65 5b55 6e69 6f6e 5b50 726f 7065 7274  le[Union[Propert
-00006370: 7945 6c65 6d65 6e74 2c20 7374 725d 5d5d  yElement, str]]]
-00006380: 2c0a 2020 2020 6361 6c6c 696e 675f 7265  ,.    calling_re
-00006390: 736f 7572 6365 3a20 7374 7220 3d20 2222  source: str = ""
-000063a0: 2c0a 2920 2d3e 2065 7472 6565 2e5f 456c  ,.) -> etree._El
-000063b0: 656d 656e 743a 0a20 2020 2022 2222 0a20  ement:.    """. 
-000063c0: 2020 204d 616b 6520 6120 3c64 6174 652d     Make a <date-
-000063d0: 7072 6f70 3e20 6672 6f6d 206f 6e65 206f  prop> from one o
-000063e0: 7220 6d6f 7265 2064 6174 6573 2f64 6174  r more dates/dat
-000063f0: 6520 7261 6e67 6573 2e20 5468 6520 6461  e ranges. The da
-00006400: 7465 2873 2920 6361 6e20 6265 2070 726f  te(s) can be pro
-00006410: 7669 6465 6420 6173 2073 7472 696e 6720  vided as string 
-00006420: 6f72 2061 7320 5072 6f70 6572 7479 456c  or as PropertyEl
-00006430: 656d 656e 740a 2020 2020 7769 7468 2061  ement.    with a
-00006440: 2073 7472 696e 6720 696e 7369 6465 2e20   string inside. 
-00006450: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
-00006460: 7472 696e 672c 2074 6865 2070 6572 6d69  tring, the permi
-00006470: 7373 696f 6e73 2064 6566 6175 6c74 2074  ssions default t
-00006480: 6f20 2270 726f 702d 6465 6661 756c 7422  o "prop-default"
-00006490: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000064a0: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-000064b0: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-000064c0: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
-000064d0: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
-000064e0: 2020 2020 7661 6c75 653a 206f 6e65 206f      value: one o
-000064f0: 7220 6d6f 7265 2044 5350 2064 6174 6573  r more DSP dates
-00006500: 2c20 6173 2073 7472 696e 672f 5072 6f70  , as string/Prop
-00006510: 6572 7479 456c 656d 656e 742c 206f 7220  ertyElement, or 
-00006520: 6173 2069 7465 7261 626c 6520 6f66 2073  as iterable of s
-00006530: 7472 696e 6773 2f50 726f 7065 7274 7945  trings/PropertyE
-00006540: 6c65 6d65 6e74 730a 2020 2020 2020 2020  lements.        
-00006550: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-00006560: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-00006570: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00006580: 6520 2866 6f72 2062 6574 7465 7220 6572  e (for better er
-00006590: 726f 7220 6d65 7373 6167 6573 290a 0a20  ror messages).. 
-000065a0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-000065b0: 2020 2042 6173 6545 7272 6f72 3a20 4966     BaseError: If
-000065c0: 2074 6865 2076 616c 7565 2069 7320 6e6f   the value is no
-000065d0: 7420 6120 7661 6c69 6420 4453 5020 6461  t a valid DSP da
-000065e0: 7465 0a0a 2020 2020 5265 7475 726e 733a  te..    Returns:
-000065f0: 0a20 2020 2020 2020 2061 6e20 6574 7265  .        an etre
-00006600: 652e 5f45 6c65 6d65 6e74 2074 6861 7420  e._Element that 
-00006610: 6361 6e20 6265 2061 7070 656e 6465 6420  can be appended 
-00006620: 746f 2074 6865 2070 6172 656e 7420 7265  to the parent re
-00006630: 736f 7572 6365 2077 6974 6820 7265 736f  source with reso
-00006640: 7572 6365 2e61 7070 656e 6428 6d61 6b65  urce.append(make
-00006650: 5f2a 5f70 726f 7028 2e2e 2e29 290a 0a20  _*_prop(...)).. 
-00006660: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-00006670: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-00006680: 6d6c 2e6d 616b 655f 6461 7465 5f70 726f  ml.make_date_pro
-00006690: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-000066a0: 222c 2022 4752 4547 4f52 4941 4e3a 4345  ", "GREGORIAN:CE
-000066b0: 3a32 3031 342d 3031 2d33 3122 290a 2020  :2014-01-31").  
-000066c0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000066d0: 6174 652d 7072 6f70 206e 616d 653d 223a  ate-prop name=":
-000066e0: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 203c 6461 7465 2070 6572 6d69 7373     <date permiss
-00006710: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-00006720: 6c74 223e 4752 4547 4f52 4941 4e3a 4345  lt">GREGORIAN:CE
-00006730: 3a32 3031 342d 3031 2d33 313c 2f64 6174  :2014-01-31</dat
-00006740: 653e 0a20 2020 2020 2020 2020 2020 2020  e>.             
-00006750: 2020 203c 2f64 6174 652d 7072 6f70 3e0a     </date-prop>.
-00006760: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
-00006770: 6c32 786d 6c2e 6d61 6b65 5f64 6174 655f  l2xml.make_date_
-00006780: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
-00006790: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
-000067a0: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
-000067b0: 2247 5245 474f 5249 414e 3a43 453a 3230  "GREGORIAN:CE:20
-000067c0: 3134 2d30 312d 3331 222c 2070 6572 6d69  14-01-31", permi
-000067d0: 7373 696f 6e73 3d22 7072 6f70 2d72 6573  ssions="prop-res
-000067e0: 7472 6963 7465 6422 2c20 636f 6d6d 656e  tricted", commen
-000067f0: 743d 2265 7861 6d70 6c65 2229 290a 2020  t="example")).  
-00006800: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00006810: 6174 652d 7072 6f70 206e 616d 653d 223a  ate-prop name=":
-00006820: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 203c 6461 7465 2070 6572 6d69 7373     <date permiss
-00006850: 696f 6e73 3d22 7072 6f70 2d72 6573 7472  ions="prop-restr
-00006860: 6963 7465 6422 2063 6f6d 6d65 6e74 3d22  icted" comment="
-00006870: 6578 616d 706c 6522 3e0a 2020 2020 2020  example">.      
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 4752 4547 4f52 4941 4e3a 4345 3a32    GREGORIAN:CE:2
-000068a0: 3031 342d 3031 2d33 310a 2020 2020 2020  014-01-31.      
-000068b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000068c0: 6461 7465 3e0a 2020 2020 2020 2020 2020  date>.          
-000068d0: 2020 2020 2020 3c2f 6461 7465 2d70 726f        </date-pro
-000068e0: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-000068f0: 7863 656c 3278 6d6c 2e6d 616b 655f 6461  xcel2xml.make_da
-00006900: 7465 5f70 726f 7028 223a 7465 7374 7072  te_prop(":testpr
-00006910: 6f70 6572 7479 222c 205b 2247 5245 474f  operty", ["GREGO
-00006920: 5249 414e 3a43 453a 3139 3330 2d30 392d  RIAN:CE:1930-09-
-00006930: 3032 3a43 453a 3139 3330 2d30 392d 3033  02:CE:1930-09-03
-00006940: 222c 2022 4752 4547 4f52 4941 4e3a 4345  ", "GREGORIAN:CE
-00006950: 3a31 3933 302d 3039 2d30 323a 4345 3a31  :1930-09-02:CE:1
-00006960: 3933 302d 3039 2d30 3322 5d29 0a20 2020  930-09-03"]).   
-00006970: 2020 2020 2020 2020 2020 2020 203c 6461               <da
-00006980: 7465 2d70 726f 7020 6e61 6d65 3d22 3a74  te-prop name=":t
-00006990: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2020 3c64 6174 6520 7065 726d 6973 7369    <date permissi
-000069c0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-000069d0: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-000069e0: 2020 2020 2020 2020 2020 2020 4752 4547              GREG
-000069f0: 4f52 4941 4e3a 4345 3a31 3933 302d 3039  ORIAN:CE:1930-09
-00006a00: 2d30 323a 4345 3a31 3933 302d 3039 2d30  -02:CE:1930-09-0
-00006a10: 330a 2020 2020 2020 2020 2020 2020 2020  3.              
-00006a20: 2020 2020 2020 3c2f 6461 7465 3e0a 2020        </date>.  
-00006a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a40: 2020 3c64 6174 6520 7065 726d 6973 7369    <date permissi
-00006a50: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-00006a60: 7422 3e0a 2020 2020 2020 2020 2020 2020  t">.            
-00006a70: 2020 2020 2020 2020 2020 2020 4752 4547              GREG
-00006a80: 4f52 4941 4e3a 4345 3a31 3933 302d 3039  ORIAN:CE:1930-09
-00006a90: 2d30 323a 4345 3a31 3933 302d 3039 2d30  -02:CE:1930-09-0
-00006aa0: 330a 2020 2020 2020 2020 2020 2020 2020  3.              
-00006ab0: 2020 2020 2020 3c2f 6461 7465 3e0a 2020        </date>.  
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00006ad0: 6461 7465 2d70 726f 703e 0a0a 2020 2020  date-prop>..    
-00006ae0: 5365 6520 6874 7470 733a 2f2f 646f 6373  See https://docs
-00006af0: 2e64 6173 6368 2e73 7769 7373 2f6c 6174  .dasch.swiss/lat
-00006b00: 6573 742f 4453 502d 544f 4f4c 532f 6669  est/DSP-TOOLS/fi
-00006b10: 6c65 2d66 6f72 6d61 7473 2f78 6d6c 2d64  le-formats/xml-d
-00006b20: 6174 612d 6669 6c65 2f23 6461 7465 2d70  ata-file/#date-p
-00006b30: 726f 700a 2020 2020 2222 220a 0a20 2020  rop.    """..   
-00006b40: 2023 2063 6865 636b 2074 6865 2069 6e70   # check the inp
-00006b50: 7574 3a20 7072 6570 6172 6520 6120 6c69  ut: prepare a li
-00006b60: 7374 2077 6974 6820 7661 6c69 6420 7661  st with valid va
-00006b70: 6c75 6573 0a20 2020 2076 616c 7565 7320  lues.    values 
-00006b80: 3d20 7072 6570 6172 655f 7661 6c75 6528  = prepare_value(
-00006b90: 7661 6c75 6529 0a0a 2020 2020 2320 6368  value)..    # ch
-00006ba0: 6563 6b20 7661 6c75 6520 7479 7065 0a20  eck value type. 
-00006bb0: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
-00006bc0: 6c75 6573 3a0a 2020 2020 2020 2020 6966  lues:.        if
-00006bd0: 206e 6f74 2069 735f 6675 6c6c 5f64 6174   not is_full_dat
-00006be0: 6528 7374 7228 7661 6c2e 7661 6c75 6529  e(str(val.value)
-00006bf0: 2e73 7472 6970 2829 293a 0a20 2020 2020  .strip()):.     
-00006c00: 2020 2020 2020 2072 6169 7365 2042 6173         raise Bas
-00006c10: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00006c20: 2020 2020 2020 2020 6622 4661 696c 6564          f"Failed
-00006c30: 2076 616c 6964 6174 696f 6e20 696e 2072   validation in r
-00006c40: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
-00006c50: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
-00006c60: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
-00006c70: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00006c80: 2020 2066 2227 7b76 616c 2e76 616c 7565     f"'{val.value
-00006c90: 7d27 2069 7320 6e6f 7420 6120 7661 6c69  }' is not a vali
-00006ca0: 6420 4453 5020 6461 7465 2e22 0a20 2020  d DSP date.".   
-00006cb0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00006cc0: 2320 6d61 6b65 2078 6d6c 2073 7472 7563  # make xml struc
-00006cd0: 7475 7265 206f 6620 7468 6520 7661 6c69  ture of the vali
-00006ce0: 6420 7661 6c75 6573 0a20 2020 2070 726f  d values.    pro
-00006cf0: 705f 203d 2065 7472 6565 2e45 6c65 6d65  p_ = etree.Eleme
-00006d00: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
-00006d10: 7d64 6174 652d 7072 6f70 2220 2520 786d  }date-prop" % xm
-00006d20: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
-00006d30: 4e6f 6e65 5d2c 0a20 2020 2020 2020 206e  None],.        n
-00006d40: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
-00006d50: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
-00006d60: 7370 6163 655f 6d61 702c 0a20 2020 2029  space_map,.    )
-00006d70: 0a20 2020 2066 6f72 2076 616c 2069 6e20  .    for val in 
-00006d80: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
-00006d90: 6b77 6172 6773 203d 207b 2270 6572 6d69  kwargs = {"permi
-00006da0: 7373 696f 6e73 223a 2076 616c 2e70 6572  ssions": val.per
-00006db0: 6d69 7373 696f 6e73 7d0a 2020 2020 2020  missions}.      
-00006dc0: 2020 6966 2076 616c 2e63 6f6d 6d65 6e74    if val.comment
-00006dd0: 2061 6e64 2063 6865 636b 5f6e 6f74 6e61   and check_notna
-00006de0: 2876 616c 2e63 6f6d 6d65 6e74 293a 0a20  (val.comment):. 
-00006df0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00006e00: 735b 2263 6f6d 6d65 6e74 225d 203d 2076  s["comment"] = v
-00006e10: 616c 2e63 6f6d 6d65 6e74 0a20 2020 2020  al.comment.     
-00006e20: 2020 2076 616c 7565 5f20 3d20 6574 7265     value_ = etre
-00006e30: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
-00006e40: 2020 2020 2020 2022 7b25 737d 6461 7465         "{%s}date
-00006e50: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-00006e60: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-00006e70: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-00006e80: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-00006e90: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-00006ea0: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
-00006eb0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-00006ec0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00006ed0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
-00006ee0: 3d20 7374 7228 7661 6c2e 7661 6c75 6529  = str(val.value)
-00006ef0: 2e73 7472 6970 2829 0a20 2020 2020 2020  .strip().       
-00006f00: 2070 726f 705f 2e61 7070 656e 6428 7661   prop_.append(va
-00006f10: 6c75 655f 290a 0a20 2020 2072 6574 7572  lue_)..    retur
-00006f20: 6e20 7072 6f70 5f0a 0a0a 6465 6620 6d61  n prop_...def ma
-00006f30: 6b65 5f64 6563 696d 616c 5f70 726f 7028  ke_decimal_prop(
-00006f40: 0a20 2020 206e 616d 653a 2073 7472 2c0a  .    name: str,.
-00006f50: 2020 2020 7661 6c75 653a 2055 6e69 6f6e      value: Union
-00006f60: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
-00006f70: 2c20 7374 722c 2049 7465 7261 626c 655b  , str, Iterable[
-00006f80: 556e 696f 6e5b 5072 6f70 6572 7479 456c  Union[PropertyEl
-00006f90: 656d 656e 742c 2073 7472 5d5d 5d2c 0a20  ement, str]]],. 
-00006fa0: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
-00006fb0: 7263 653a 2073 7472 203d 2022 222c 0a29  rce: str = "",.)
-00006fc0: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
-00006fd0: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
-00006fe0: 4d61 6b65 2061 203c 6465 6369 6d61 6c2d  Make a <decimal-
-00006ff0: 7072 6f70 3e20 6672 6f6d 206f 6e65 206f  prop> from one o
-00007000: 7220 6d6f 7265 2064 6563 696d 616c 206e  r more decimal n
-00007010: 756d 6265 7273 2e20 5468 6520 6465 6369  umbers. The deci
-00007020: 6d61 6c28 7329 2063 616e 2062 6520 7072  mal(s) can be pr
-00007030: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
-00007040: 2c20 666c 6f61 742c 206f 7220 6173 0a20  , float, or as. 
-00007050: 2020 2050 726f 7065 7274 7945 6c65 6d65     PropertyEleme
-00007060: 6e74 2077 6974 6820 6120 7374 7269 6e67  nt with a string
-00007070: 2f66 6c6f 6174 2069 6e73 6964 652e 2049  /float inside. I
-00007080: 6620 7072 6f76 6964 6564 2061 7320 7374  f provided as st
-00007090: 7269 6e67 2f66 6c6f 6174 2c20 7468 6520  ring/float, the 
-000070a0: 7065 726d 6973 7369 6f6e 7320 6465 6661  permissions defa
-000070b0: 756c 7420 746f 0a20 2020 2022 7072 6f70  ult to.    "prop
-000070c0: 2d64 6566 6175 6c74 222e 0a0a 2020 2020  -default"...    
-000070d0: 4172 6773 3a0a 2020 2020 2020 2020 6e61  Args:.        na
-000070e0: 6d65 3a20 7468 6520 6e61 6d65 206f 6620  me: the name of 
-000070f0: 7468 6973 2070 726f 7065 7274 7920 6173  this property as
-00007100: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-00007110: 6f6e 746f 0a20 2020 2020 2020 2076 616c  onto.        val
-00007120: 7565 3a20 6f6e 6520 6f72 206d 6f72 6520  ue: one or more 
-00007130: 6465 6369 6d61 6c20 6e75 6d62 6572 732c  decimal numbers,
-00007140: 2061 7320 7374 7269 6e67 2f66 6c6f 6174   as string/float
-00007150: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-00007160: 2c20 6f72 2061 7320 6974 6572 6162 6c65  , or as iterable
-00007170: 206f 6620 7374 7269 6e67 732f 5072 6f70   of strings/Prop
-00007180: 6572 7479 456c 656d 656e 7473 0a20 2020  ertyElements.   
-00007190: 2020 2020 2063 616c 6c69 6e67 5f72 6573       calling_res
-000071a0: 6f75 7263 653a 2074 6865 206e 616d 6520  ource: the name 
-000071b0: 6f66 2074 6865 2070 6172 656e 7420 7265  of the parent re
-000071c0: 736f 7572 6365 2028 666f 7220 6265 7474  source (for bett
-000071d0: 6572 2065 7272 6f72 206d 6573 7361 6765  er error message
-000071e0: 7329 0a0a 2020 2020 5261 6973 6573 3a0a  s)..    Raises:.
-000071f0: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
-00007200: 723a 2049 6620 7468 6520 7661 6c75 6520  r: If the value 
-00007210: 6973 206e 6f74 2061 2076 616c 6964 2064  is not a valid d
-00007220: 6563 696d 616c 206e 756d 6265 720a 0a20  ecimal number.. 
-00007230: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00007240: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
-00007250: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
-00007260: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
-00007270: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00007280: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
-00007290: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
-000072a0: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
-000072b0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-000072c0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-000072d0: 6b65 5f64 6563 696d 616c 5f70 726f 7028  ke_decimal_prop(
-000072e0: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-000072f0: 2022 332e 3134 3135 3922 290a 2020 2020   "3.14159").    
-00007300: 2020 2020 2020 2020 2020 2020 3c64 6563              <dec
-00007310: 696d 616c 2d70 726f 7020 6e61 6d65 3d22  imal-prop name="
-00007320: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 3c64 6563 696d 616c 2070 6572      <decimal per
-00007350: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-00007360: 6566 6175 6c74 223e 332e 3134 3135 393c  efault">3.14159<
-00007370: 2f64 6563 696d 616c 3e0a 2020 2020 2020  /decimal>.      
-00007380: 2020 2020 2020 2020 2020 3c2f 6465 6369            </deci
-00007390: 6d61 6c2d 7072 6f70 3e0a 2020 2020 2020  mal-prop>.      
-000073a0: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
-000073b0: 6d61 6b65 5f64 6563 696d 616c 5f70 726f  make_decimal_pro
-000073c0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-000073d0: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
-000073e0: 7065 7274 7945 6c65 6d65 6e74 2822 332e  pertyElement("3.
-000073f0: 3134 3135 3922 2c20 7065 726d 6973 7369  14159", permissi
-00007400: 6f6e 733d 2270 726f 702d 7265 7374 7269  ons="prop-restri
-00007410: 6374 6564 222c 2063 6f6d 6d65 6e74 3d22  cted", comment="
-00007420: 6578 616d 706c 6522 2929 0a20 2020 2020  example")).     
-00007430: 2020 2020 2020 2020 2020 203c 6465 6369             <deci
-00007440: 6d61 6c2d 7072 6f70 206e 616d 653d 223a  mal-prop name=":
-00007450: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007470: 2020 203c 6465 6369 6d61 6c20 7065 726d     <decimal perm
-00007480: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-00007490: 7374 7269 6374 6564 2220 636f 6d6d 656e  stricted" commen
-000074a0: 743d 2265 7861 6d70 6c65 223e 332e 3134  t="example">3.14
-000074b0: 3135 393c 2f64 6563 696d 616c 3e0a 2020  159</decimal>.  
-000074c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-000074d0: 6465 6369 6d61 6c2d 7072 6f70 3e0a 2020  decimal-prop>.  
-000074e0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-000074f0: 786d 6c2e 6d61 6b65 5f64 6563 696d 616c  xml.make_decimal
-00007500: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
-00007510: 6572 7479 222c 205b 2233 2e31 3431 3539  erty", ["3.14159
-00007520: 222c 2022 322e 3731 3822 5d29 0a20 2020  ", "2.718"]).   
-00007530: 2020 2020 2020 2020 2020 2020 203c 6465               <de
-00007540: 6369 6d61 6c2d 7072 6f70 206e 616d 653d  cimal-prop name=
-00007550: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
-00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007570: 2020 2020 203c 6465 6369 6d61 6c20 7065       <decimal pe
-00007580: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-00007590: 6465 6661 756c 7422 3e33 2e31 3431 3539  default">3.14159
-000075a0: 3c2f 6465 6369 6d61 6c3e 0a20 2020 2020  </decimal>.     
-000075b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000075c0: 6465 6369 6d61 6c20 7065 726d 6973 7369  decimal permissi
-000075d0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-000075e0: 7422 3e32 2e37 3138 3c2f 6465 6369 6d61  t">2.718</decima
-000075f0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-00007600: 2020 203c 2f64 6563 696d 616c 2d70 726f     </decimal-pro
-00007610: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
-00007620: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
-00007630: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
-00007640: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
-00007650: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
-00007660: 2f23 6465 6369 6d61 6c2d 7072 6f70 0a20  /#decimal-prop. 
-00007670: 2020 2022 2222 0a0a 2020 2020 2320 6368     """..    # ch
-00007680: 6563 6b20 7468 6520 696e 7075 743a 2070  eck the input: p
-00007690: 7265 7061 7265 2061 206c 6973 7420 7769  repare a list wi
-000076a0: 7468 2076 616c 6964 2076 616c 7565 730a  th valid values.
-000076b0: 2020 2020 7661 6c75 6573 203d 2070 7265      values = pre
-000076c0: 7061 7265 5f76 616c 7565 2876 616c 7565  pare_value(value
-000076d0: 290a 0a20 2020 2023 2063 6865 636b 2076  )..    # check v
-000076e0: 616c 7565 2074 7970 650a 2020 2020 666f  alue type.    fo
-000076f0: 7220 7661 6c20 696e 2076 616c 7565 733a  r val in values:
-00007700: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00007710: 2020 2020 2020 2020 2020 666c 6f61 7428            float(
-00007720: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
-00007730: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
-00007740: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
-00007750: 2020 7261 6973 6520 4261 7365 4572 726f    raise BaseErro
-00007760: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00007770: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
-00007780: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
-00007790: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
-000077a0: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
-000077b0: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
-000077c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000077d0: 277b 7661 6c2e 7661 6c75 657d 2720 6973  '{val.value}' is
-000077e0: 206e 6f74 2061 2076 616c 6964 2064 6563   not a valid dec
-000077f0: 696d 616c 206e 756d 6265 722e 220a 2020  imal number.".  
-00007800: 2020 2020 2020 2020 2020 2920 6672 6f6d            ) from
-00007810: 204e 6f6e 650a 0a20 2020 2023 206d 616b   None..    # mak
-00007820: 6520 786d 6c20 7374 7275 6374 7572 6520  e xml structure 
-00007830: 6f66 2074 6865 2076 616c 6964 2076 616c  of the valid val
-00007840: 7565 730a 2020 2020 7072 6f70 5f20 3d20  ues.    prop_ = 
-00007850: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-00007860: 2020 2020 2020 2022 7b25 737d 6465 6369         "{%s}deci
-00007870: 6d61 6c2d 7072 6f70 2220 2520 786d 6c5f  mal-prop" % xml_
-00007880: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
-00007890: 6e65 5d2c 0a20 2020 2020 2020 206e 616d  ne],.        nam
-000078a0: 653d 6e61 6d65 2c0a 2020 2020 2020 2020  e=name,.        
-000078b0: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
-000078c0: 6163 655f 6d61 702c 0a20 2020 2029 0a20  ace_map,.    ). 
-000078d0: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
-000078e0: 6c75 6573 3a0a 2020 2020 2020 2020 6b77  lues:.        kw
-000078f0: 6172 6773 203d 207b 2270 6572 6d69 7373  args = {"permiss
-00007900: 696f 6e73 223a 2076 616c 2e70 6572 6d69  ions": val.permi
-00007910: 7373 696f 6e73 7d0a 2020 2020 2020 2020  ssions}.        
-00007920: 6966 2076 616c 2e63 6f6d 6d65 6e74 2061  if val.comment a
-00007930: 6e64 2063 6865 636b 5f6e 6f74 6e61 2876  nd check_notna(v
-00007940: 616c 2e63 6f6d 6d65 6e74 293a 0a20 2020  al.comment):.   
-00007950: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
-00007960: 2263 6f6d 6d65 6e74 225d 203d 2076 616c  "comment"] = val
-00007970: 2e63 6f6d 6d65 6e74 0a20 2020 2020 2020  .comment.       
-00007980: 2076 616c 7565 5f20 3d20 6574 7265 652e   value_ = etree.
-00007990: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
-000079a0: 2020 2020 2022 7b25 737d 6465 6369 6d61       "{%s}decima
-000079b0: 6c22 2025 2078 6d6c 5f6e 616d 6573 7061  l" % xml_namespa
-000079c0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
-000079d0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-000079e0: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
-000079f0: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
-00007a00: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
-00007a10: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-00007a20: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
-00007a30: 2020 2020 2076 616c 7565 5f2e 7465 7874       value_.text
-00007a40: 203d 2073 7472 2866 6c6f 6174 2876 616c   = str(float(val
-00007a50: 2e76 616c 7565 2929 0a20 2020 2020 2020  .value)).       
-00007a60: 2070 726f 705f 2e61 7070 656e 6428 7661   prop_.append(va
-00007a70: 6c75 655f 290a 0a20 2020 2072 6574 7572  lue_)..    retur
-00007a80: 6e20 7072 6f70 5f0a 0a0a 6465 6620 6d61  n prop_...def ma
-00007a90: 6b65 5f67 656f 6d65 7472 795f 7072 6f70  ke_geometry_prop
-00007aa0: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-00007ab0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-00007ac0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-00007ad0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
-00007ae0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
-00007af0: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
-00007b00: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-00007b10: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-00007b20: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-00007b30: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-00007b40: 204d 616b 6520 6120 3c67 656f 6d65 7472   Make a <geometr
-00007b50: 792d 7072 6f70 3e20 6672 6f6d 206f 6e65  y-prop> from one
-00007b60: 206f 7220 6d6f 7265 2061 7265 6173 206f   or more areas o
-00007b70: 6620 616e 2069 6d61 6765 2e20 5468 6520  f an image. The 
-00007b80: 6172 6561 2873 2920 6361 6e20 6265 2070  area(s) can be p
-00007b90: 726f 7669 6465 6420 6173 204a 534f 4e2d  rovided as JSON-
-00007ba0: 7374 7269 6e67 206f 7220 6173 0a20 2020  string or as.   
-00007bb0: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00007bc0: 2077 6974 6820 7468 6520 4a53 4f4e 2d73   with the JSON-s
-00007bd0: 7472 696e 6720 696e 7369 6465 2e20 4966  tring inside. If
-00007be0: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
-00007bf0: 696e 672c 2074 6865 2070 6572 6d69 7373  ing, the permiss
-00007c00: 696f 6e73 2064 6566 6175 6c74 2074 6f20  ions default to 
-00007c10: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
-00007c20: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00007c30: 2020 206e 616d 653a 2074 6865 206e 616d     name: the nam
-00007c40: 6520 6f66 2074 6869 7320 7072 6f70 6572  e of this proper
-00007c50: 7479 2061 7320 6465 6669 6e65 6420 696e  ty as defined in
-00007c60: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
-00007c70: 2020 7661 6c75 653a 206f 6e65 206f 7220    value: one or 
-00007c80: 6d6f 7265 204a 534f 4e20 6765 6f6d 6574  more JSON geomet
-00007c90: 7279 206f 626a 6563 7473 2c20 6173 2073  ry objects, as s
-00007ca0: 7472 696e 672f 5072 6f70 6572 7479 456c  tring/PropertyEl
-00007cb0: 656d 656e 742c 206f 7220 6173 2069 7465  ement, or as ite
-00007cc0: 7261 626c 6520 6f66 2073 7472 696e 6773  rable of strings
-00007cd0: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-00007ce0: 730a 2020 2020 2020 2020 6361 6c6c 696e  s.        callin
-00007cf0: 675f 7265 736f 7572 6365 3a20 7468 6520  g_resource: the 
-00007d00: 6e61 6d65 206f 6620 7468 6520 7061 7265  name of the pare
-00007d10: 6e74 2072 6573 6f75 7263 6520 2866 6f72  nt resource (for
-00007d20: 2062 6574 7465 7220 6572 726f 7220 6d65   better error me
-00007d30: 7373 6167 6573 290a 0a20 2020 2052 6169  ssages)..    Rai
-00007d40: 7365 733a 0a20 2020 2020 2020 2042 6173  ses:.        Bas
-00007d50: 6545 7272 6f72 3a20 4966 2074 6865 2076  eError: If the v
-00007d60: 616c 7565 2069 7320 6e6f 7420 6120 7661  alue is not a va
-00007d70: 6c69 6420 4a53 4f4e 2067 656f 6d65 7472  lid JSON geometr
-00007d80: 7920 6f62 6a65 6374 0a0a 2020 2020 5265  y object..    Re
-00007d90: 7475 726e 733a 0a20 2020 2020 2020 2061  turns:.        a
-00007da0: 6e20 6574 7265 652e 5f45 6c65 6d65 6e74  n etree._Element
-00007db0: 2074 6861 7420 6361 6e20 6265 2061 7070   that can be app
-00007dc0: 656e 6465 6420 746f 2074 6865 2070 6172  ended to the par
-00007dd0: 656e 7420 7265 736f 7572 6365 2077 6974  ent resource wit
-00007de0: 6820 7265 736f 7572 6365 2e61 7070 656e  h resource.appen
-00007df0: 6428 6d61 6b65 5f2a 5f70 726f 7028 2e2e  d(make_*_prop(..
-00007e00: 2e29 290a 0a20 2020 2045 7861 6d70 6c65  .))..    Example
-00007e10: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
-00007e20: 7863 656c 3278 6d6c 2e6d 616b 655f 6765  xcel2xml.make_ge
-00007e30: 6f6d 6574 7279 5f70 726f 7028 223a 7465  ometry_prop(":te
-00007e40: 7374 7072 6f70 6572 7479 222c 206a 736f  stproperty", jso
-00007e50: 6e5f 7374 7269 6e67 290a 2020 2020 2020  n_string).      
-00007e60: 2020 2020 2020 2020 2020 3c67 656f 6d65            <geome
-00007e70: 7472 792d 7072 6f70 206e 616d 653d 223a  try-prop name=":
-00007e80: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 203c 6765 6f6d 6574 7279 2070 6572     <geometry per
-00007eb0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-00007ec0: 6566 6175 6c74 223e 7b4a 534f 4e7d 3c2f  efault">{JSON}</
-00007ed0: 6765 6f6d 6574 7279 3e0a 2020 2020 2020  geometry>.      
-00007ee0: 2020 2020 2020 2020 2020 3c2f 6765 6f6d            </geom
-00007ef0: 6574 7279 2d70 726f 703e 0a20 2020 2020  etry-prop>.     
-00007f00: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-00007f10: 2e6d 616b 655f 6765 6f6d 6574 7279 5f70  .make_geometry_p
-00007f20: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-00007f30: 7479 222c 2065 7863 656c 3278 6d6c 2e50  ty", excel2xml.P
-00007f40: 726f 7065 7274 7945 6c65 6d65 6e74 286a  ropertyElement(j
-00007f50: 736f 6e5f 7374 7269 6e67 2c20 7065 726d  son_string, perm
-00007f60: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-00007f70: 7374 7269 6374 6564 222c 2063 6f6d 6d65  stricted", comme
-00007f80: 6e74 3d22 6578 616d 706c 6522 2929 0a20  nt="example")). 
-00007f90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00007fa0: 6765 6f6d 6574 7279 2d70 726f 7020 6e61  geometry-prop na
-00007fb0: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-00007fc0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-00007fd0: 2020 2020 2020 2020 3c67 656f 6d65 7472          <geometr
-00007fe0: 7920 7065 726d 6973 7369 6f6e 733d 2270  y permissions="p
-00007ff0: 726f 702d 7265 7374 7269 6374 6564 2220  rop-restricted" 
-00008000: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
-00008010: 223e 7b4a 534f 4e7d 3c2f 6765 6f6d 6574  ">{JSON}</geomet
-00008020: 7279 3e0a 2020 2020 2020 2020 2020 2020  ry>.            
-00008030: 2020 2020 3c2f 6765 6f6d 6574 7279 2d70      </geometry-p
-00008040: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
-00008050: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
-00008060: 6765 6f6d 6574 7279 5f70 726f 7028 223a  geometry_prop(":
-00008070: 7465 7374 7072 6f70 6572 7479 222c 205b  testproperty", [
-00008080: 6a73 6f6e 5f73 7472 696e 6731 2c20 6a73  json_string1, js
-00008090: 6f6e 5f73 7472 696e 6732 5d29 0a20 2020  on_string2]).   
-000080a0: 2020 2020 2020 2020 2020 2020 203c 6765               <ge
-000080b0: 6f6d 6574 7279 2d70 726f 7020 6e61 6d65  ometry-prop name
-000080c0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-000080d0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000080e0: 2020 2020 2020 3c67 656f 6d65 7472 7920        <geometry 
-000080f0: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-00008100: 702d 6465 6661 756c 7422 3e7b 4a53 4f4e  p-default">{JSON
-00008110: 7d3c 2f67 656f 6d65 7472 793e 0a20 2020  }</geometry>.   
-00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008130: 203c 6765 6f6d 6574 7279 2070 6572 6d69   <geometry permi
-00008140: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-00008150: 6175 6c74 223e 7b4a 534f 4e7d 3c2f 6765  ault">{JSON}</ge
-00008160: 6f6d 6574 7279 3e0a 2020 2020 2020 2020  ometry>.        
-00008170: 2020 2020 2020 2020 3c2f 6765 6f6d 6574          </geomet
-00008180: 7279 2d70 726f 703e 0a0a 2020 2020 5365  ry-prop>..    Se
-00008190: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
-000081a0: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
-000081b0: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
-000081c0: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
-000081d0: 612d 6669 6c65 2f23 6765 6f6d 6574 7279  a-file/#geometry
-000081e0: 2d70 726f 700a 2020 2020 2222 220a 0a20  -prop.    """.. 
-000081f0: 2020 2023 2063 6865 636b 2074 6865 2069     # check the i
-00008200: 6e70 7574 3a20 7072 6570 6172 6520 6120  nput: prepare a 
-00008210: 6c69 7374 2077 6974 6820 7661 6c69 6420  list with valid 
-00008220: 7661 6c75 6573 0a20 2020 2076 616c 7565  values.    value
-00008230: 7320 3d20 7072 6570 6172 655f 7661 6c75  s = prepare_valu
-00008240: 6528 7661 6c75 6529 0a0a 2020 2020 2320  e(value)..    # 
-00008250: 6368 6563 6b20 7661 6c75 6520 7479 7065  check value type
-00008260: 0a20 2020 2066 6f72 2076 616c 2069 6e20  .    for val in 
-00008270: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
-00008280: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00008290: 2076 616c 7565 5f61 735f 6469 6374 203d   value_as_dict =
-000082a0: 206a 736f 6e2e 6c6f 6164 7328 7374 7228   json.loads(str(
-000082b0: 7661 6c2e 7661 6c75 6529 290a 2020 2020  val.value)).    
-000082c0: 2020 2020 2020 2020 6966 2076 616c 7565          if value
-000082d0: 5f61 735f 6469 6374 5b22 7479 7065 225d  _as_dict["type"]
-000082e0: 206e 6f74 2069 6e20 5b22 7265 6374 616e   not in ["rectan
-000082f0: 676c 6522 2c20 2263 6972 636c 6522 2c20  gle", "circle", 
-00008300: 2270 6f6c 7967 6f6e 225d 3a0a 2020 2020  "polygon"]:.    
-00008310: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00008320: 6520 4261 7365 4572 726f 7228 0a20 2020  e BaseError(.   
-00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008340: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
-00008350: 7469 6f6e 2069 6e20 7265 736f 7572 6365  tion in resource
-00008360: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
-00008370: 7263 657d 272c 2070 726f 7065 7274 7920  rce}', property 
-00008380: 277b 6e61 6d65 7d27 3a20 220a 2020 2020  '{name}': ".    
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 6622 5468 6520 2774 7970 6527 206f 6620  f"The 'type' of 
-000083b0: 7468 6520 4a53 4f4e 2067 656f 6d65 7472  the JSON geometr
-000083c0: 7920 6f62 6a65 6374 206d 7573 7420 6265  y object must be
-000083d0: 2027 7265 6374 616e 676c 6527 2c20 2763   'rectangle', 'c
-000083e0: 6972 636c 6527 2c20 6f72 2027 706f 6c79  ircle', or 'poly
-000083f0: 676f 6e27 2e22 0a20 2020 2020 2020 2020  gon'.".         
-00008400: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00008410: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00008420: 7374 616e 6365 2876 616c 7565 5f61 735f  stance(value_as_
-00008430: 6469 6374 5b22 706f 696e 7473 225d 2c20  dict["points"], 
-00008440: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-00008450: 2020 2020 2020 2072 6169 7365 2042 6173         raise Bas
-00008460: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00008470: 2020 2020 2020 2020 2020 2020 6622 4661              f"Fa
-00008480: 696c 6564 2076 616c 6964 6174 696f 6e20  iled validation 
-00008490: 696e 2072 6573 6f75 7263 6520 277b 6361  in resource '{ca
-000084a0: 6c6c 696e 675f 7265 736f 7572 6365 7d27  lling_resource}'
-000084b0: 2c20 7072 6f70 6572 7479 2027 7b6e 616d  , property '{nam
-000084c0: 657d 273a 2022 0a20 2020 2020 2020 2020  e}': ".         
-000084d0: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
-000084e0: 2027 706f 696e 7473 276f 6620 7468 6520   'points'of the 
-000084f0: 4a53 4f4e 2067 656f 6d65 7472 7920 6f62  JSON geometry ob
-00008500: 6a65 6374 206d 7573 7420 6265 2061 206c  ject must be a l
-00008510: 6973 7420 6f66 2070 6f69 6e74 732e 220a  ist of points.".
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00008540: 2028 6a73 6f6e 2e4a 534f 4e44 6563 6f64   (json.JSONDecod
-00008550: 6545 7272 6f72 2c20 5479 7065 4572 726f  eError, TypeErro
-00008560: 722c 2049 6e64 6578 4572 726f 722c 204b  r, IndexError, K
-00008570: 6579 4572 726f 722c 2041 7373 6572 7469  eyError, Asserti
-00008580: 6f6e 4572 726f 7229 3a0a 2020 2020 2020  onError):.      
-00008590: 2020 2020 2020 7261 6973 6520 4261 7365        raise Base
-000085a0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000085b0: 2020 2020 2020 2066 2246 6169 6c65 6420         f"Failed 
-000085c0: 7661 6c69 6461 7469 6f6e 2069 6e20 7265  validation in re
-000085d0: 736f 7572 6365 2027 7b63 616c 6c69 6e67  source '{calling
-000085e0: 5f72 6573 6f75 7263 657d 272c 2070 726f  _resource}', pro
-000085f0: 7065 7274 7920 277b 6e61 6d65 7d27 3a20  perty '{name}': 
-00008600: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00008610: 2020 6622 277b 7661 6c2e 7661 6c75 657d    f"'{val.value}
-00008620: 2720 6973 206e 6f74 2061 2076 616c 6964  ' is not a valid
-00008630: 204a 534f 4e20 6765 6f6d 6574 7279 206f   JSON geometry o
-00008640: 626a 6563 742e 220a 2020 2020 2020 2020  bject.".        
-00008650: 2020 2020 2920 6672 6f6d 204e 6f6e 650a      ) from None.
-00008660: 0a20 2020 2023 206d 616b 6520 786d 6c20  .    # make xml 
-00008670: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
-00008680: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
-00008690: 2020 7072 6f70 5f20 3d20 6574 7265 652e    prop_ = etree.
-000086a0: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
-000086b0: 2022 7b25 737d 6765 6f6d 6574 7279 2d70   "{%s}geometry-p
-000086c0: 726f 7022 2025 2078 6d6c 5f6e 616d 6573  rop" % xml_names
-000086d0: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
-000086e0: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
-000086f0: 652c 0a20 2020 2020 2020 206e 736d 6170  e,.        nsmap
-00008700: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
-00008710: 6170 2c0a 2020 2020 290a 2020 2020 666f  ap,.    ).    fo
-00008720: 7220 7661 6c20 696e 2076 616c 7565 733a  r val in values:
-00008730: 0a20 2020 2020 2020 206b 7761 7267 7320  .        kwargs 
-00008740: 3d20 7b22 7065 726d 6973 7369 6f6e 7322  = {"permissions"
-00008750: 3a20 7661 6c2e 7065 726d 6973 7369 6f6e  : val.permission
-00008760: 737d 0a20 2020 2020 2020 2069 6620 7661  s}.        if va
-00008770: 6c2e 636f 6d6d 656e 7420 616e 6420 6368  l.comment and ch
-00008780: 6563 6b5f 6e6f 746e 6128 7661 6c2e 636f  eck_notna(val.co
-00008790: 6d6d 656e 7429 3a0a 2020 2020 2020 2020  mment):.        
-000087a0: 2020 2020 6b77 6172 6773 5b22 636f 6d6d      kwargs["comm
-000087b0: 656e 7422 5d20 3d20 7661 6c2e 636f 6d6d  ent"] = val.comm
-000087c0: 656e 740a 2020 2020 2020 2020 7661 6c75  ent.        valu
-000087d0: 655f 203d 2065 7472 6565 2e45 6c65 6d65  e_ = etree.Eleme
-000087e0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-000087f0: 227b 2573 7d67 656f 6d65 7472 7922 2025  "{%s}geometry" %
-00008800: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-00008810: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
-00008820: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
-00008830: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
-00008840: 6172 672d 7479 7065 5d0a 2020 2020 2020  arg-type].      
-00008850: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-00008860: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-00008870: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00008880: 2076 616c 7565 5f2e 7465 7874 203d 2073   value_.text = s
-00008890: 7472 2876 616c 2e76 616c 7565 290a 2020  tr(val.value).  
-000088a0: 2020 2020 2020 7072 6f70 5f2e 6170 7065        prop_.appe
-000088b0: 6e64 2876 616c 7565 5f29 0a20 2020 2072  nd(value_).    r
-000088c0: 6574 7572 6e20 7072 6f70 5f0a 0a0a 6465  eturn prop_...de
-000088d0: 6620 6d61 6b65 5f67 656f 6e61 6d65 5f70  f make_geoname_p
-000088e0: 726f 7028 0a20 2020 206e 616d 653a 2073  rop(.    name: s
-000088f0: 7472 2c0a 2020 2020 7661 6c75 653a 2055  tr,.    value: U
-00008900: 6e69 6f6e 5b50 726f 7065 7274 7945 6c65  nion[PropertyEle
-00008910: 6d65 6e74 2c20 7374 722c 2069 6e74 2c20  ment, str, int, 
-00008920: 4974 6572 6162 6c65 5b55 6e69 6f6e 5b50  Iterable[Union[P
-00008930: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-00008940: 7374 722c 2069 6e74 5d5d 5d2c 0a20 2020  str, int]]],.   
-00008950: 2063 616c 6c69 6e67 5f72 6573 6f75 7263   calling_resourc
-00008960: 653a 2073 7472 203d 2022 222c 0a29 202d  e: str = "",.) -
-00008970: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
-00008980: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
-00008990: 6b65 2061 203c 6765 6f6e 616d 652d 7072  ke a <geoname-pr
-000089a0: 6f70 3e20 6672 6f6d 206f 6e65 206f 7220  op> from one or 
-000089b0: 6d6f 7265 2067 656f 6e61 6d65 732e 6f72  more geonames.or
-000089c0: 6720 4944 732e 2054 6865 2049 4428 7329  g IDs. The ID(s)
-000089d0: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
-000089e0: 2061 7320 7374 7269 6e67 2c20 696e 7465   as string, inte
-000089f0: 6765 722c 206f 7220 6173 0a20 2020 2050  ger, or as.    P
-00008a00: 726f 7065 7274 7945 6c65 6d65 6e74 2077  ropertyElement w
-00008a10: 6974 6820 6120 7374 7269 6e67 2f69 6e74  ith a string/int
-00008a20: 6567 6572 2069 6e73 6964 652e 2049 6620  eger inside. If 
-00008a30: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-00008a40: 6e67 2f69 6e74 6567 6572 2c20 7468 6520  ng/integer, the 
-00008a50: 7065 726d 6973 7369 6f6e 7320 6465 6661  permissions defa
-00008a60: 756c 7420 746f 0a20 2020 2022 7072 6f70  ult to.    "prop
-00008a70: 2d64 6566 6175 6c74 222e 0a0a 2020 2020  -default"...    
-00008a80: 4172 6773 3a0a 2020 2020 2020 2020 6e61  Args:.        na
-00008a90: 6d65 3a20 7468 6520 6e61 6d65 206f 6620  me: the name of 
-00008aa0: 7468 6973 2070 726f 7065 7274 7920 6173  this property as
-00008ab0: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-00008ac0: 6f6e 746f 0a20 2020 2020 2020 2076 616c  onto.        val
-00008ad0: 7565 3a20 6f6e 6520 6f72 206d 6f72 6520  ue: one or more 
-00008ae0: 6765 6f6e 616d 6573 2e6f 7267 2049 4473  geonames.org IDs
-00008af0: 2c20 6173 2073 7472 2f69 6e74 2f50 726f  , as str/int/Pro
-00008b00: 7065 7274 7945 6c65 6d65 6e74 2c20 6f72  pertyElement, or
-00008b10: 2061 7320 6974 6572 6162 6c65 206f 6620   as iterable of 
-00008b20: 7374 722f 696e 742f 5072 6f70 6572 7479  str/int/Property
-00008b30: 456c 656d 656e 740a 2020 2020 2020 2020  Element.        
-00008b40: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-00008b50: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-00008b60: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00008b70: 6520 2866 6f72 2062 6574 7465 7220 6572  e (for better er
-00008b80: 726f 7220 6d65 7373 6167 6573 290a 0a20  ror messages).. 
-00008b90: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-00008ba0: 2020 2042 6173 6545 7272 6f72 3a20 4966     BaseError: If
-00008bb0: 2074 6865 2076 616c 7565 2069 7320 6e6f   the value is no
-00008bc0: 7420 6120 7661 6c69 6420 6765 6f6e 616d  t a valid geonam
-00008bd0: 6573 2e6f 7267 2069 6465 6e74 6966 6965  es.org identifie
-00008be0: 720a 0a20 2020 2052 6574 7572 6e73 3a0a  r..    Returns:.
-00008bf0: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
-00008c00: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
-00008c10: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
-00008c20: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
-00008c30: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
-00008c40: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
-00008c50: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
-00008c60: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
-00008c70: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
-00008c80: 6c2e 6d61 6b65 5f67 656f 6e61 6d65 5f70  l.make_geoname_p
-00008c90: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-00008ca0: 7479 222c 2022 3237 3631 3336 3922 290a  ty", "2761369").
-00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cc0: 3c67 656f 6e61 6d65 2d70 726f 7020 6e61  <geoname-prop na
-00008cd0: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-00008ce0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-00008cf0: 2020 2020 2020 2020 3c67 656f 6e61 6d65          <geoname
-00008d00: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-00008d10: 6f70 2d64 6566 6175 6c74 223e 3237 3631  op-default">2761
-00008d20: 3336 393c 2f67 656f 6e61 6d65 3e0a 2020  369</geoname>.  
-00008d30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00008d40: 6765 6f6e 616d 652d 7072 6f70 3e0a 2020  geoname-prop>.  
-00008d50: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-00008d60: 786d 6c2e 6d61 6b65 5f67 656f 6e61 6d65  xml.make_geoname
-00008d70: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
-00008d80: 6572 7479 222c 2065 7863 656c 3278 6d6c  erty", excel2xml
-00008d90: 2e50 726f 7065 7274 7945 6c65 6d65 6e74  .PropertyElement
-00008da0: 2822 3237 3631 3336 3922 2c20 7065 726d  ("2761369", perm
-00008db0: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-00008dc0: 7374 7269 6374 6564 222c 2063 6f6d 6d65  stricted", comme
-00008dd0: 6e74 3d22 6578 616d 706c 6522 2929 0a20  nt="example")). 
-00008de0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008df0: 6765 6f6e 616d 652d 7072 6f70 206e 616d  geoname-prop nam
-00008e00: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
-00008e10: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00008e20: 2020 2020 2020 203c 6765 6f6e 616d 6520         <geoname 
-00008e30: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-00008e40: 702d 7265 7374 7269 6374 6564 2220 636f  p-restricted" co
-00008e50: 6d6d 656e 743d 2265 7861 6d70 6c65 223e  mment="example">
-00008e60: 3237 3631 3336 393c 2f67 656f 6e61 6d65  2761369</geoname
-00008e70: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00008e80: 2020 3c2f 6765 6f6e 616d 652d 7072 6f70    </geoname-prop
-00008e90: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
-00008ea0: 6365 6c32 786d 6c2e 6d61 6b65 5f67 656f  cel2xml.make_geo
-00008eb0: 6e61 6d65 5f70 726f 7028 223a 7465 7374  name_prop(":test
-00008ec0: 7072 6f70 6572 7479 222c 205b 2232 3736  property", ["276
-00008ed0: 3133 3639 222c 2022 3130 3130 3130 3122  1369", "1010101"
-00008ee0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00008ef0: 2020 203c 6765 6f6e 616d 652d 7072 6f70     <geoname-prop
-00008f00: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-00008f10: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-00008f20: 2020 2020 2020 2020 2020 203c 6765 6f6e             <geon
-00008f30: 616d 6520 7065 726d 6973 7369 6f6e 733d  ame permissions=
-00008f40: 2270 726f 702d 6465 6661 756c 7422 3e32  "prop-default">2
-00008f50: 3736 3133 3639 3c2f 6765 6f6e 616d 653e  761369</geoname>
-00008f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f70: 2020 2020 203c 6765 6f6e 616d 6520 7065       <geoname pe
-00008f80: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-00008f90: 6465 6661 756c 7422 3e31 3031 3031 3031  default">1010101
-00008fa0: 3c2f 6765 6f6e 616d 653e 0a20 2020 2020  </geoname>.     
-00008fb0: 2020 2020 2020 2020 2020 203c 2f67 656f             </geo
-00008fc0: 6e61 6d65 2d70 726f 703e 0a0a 2020 2020  name-prop>..    
-00008fd0: 5365 6520 6874 7470 733a 2f2f 646f 6373  See https://docs
-00008fe0: 2e64 6173 6368 2e73 7769 7373 2f6c 6174  .dasch.swiss/lat
-00008ff0: 6573 742f 4453 502d 544f 4f4c 532f 6669  est/DSP-TOOLS/fi
-00009000: 6c65 2d66 6f72 6d61 7473 2f78 6d6c 2d64  le-formats/xml-d
-00009010: 6174 612d 6669 6c65 2f23 6765 6f6e 616d  ata-file/#geonam
-00009020: 652d 7072 6f70 0a20 2020 2022 2222 0a0a  e-prop.    """..
-00009030: 2020 2020 2320 6368 6563 6b20 7468 6520      # check the 
-00009040: 696e 7075 743a 2070 7265 7061 7265 2061  input: prepare a
-00009050: 206c 6973 7420 7769 7468 2076 616c 6964   list with valid
-00009060: 2076 616c 7565 730a 2020 2020 7661 6c75   values.    valu
-00009070: 6573 203d 2070 7265 7061 7265 5f76 616c  es = prepare_val
-00009080: 7565 2876 616c 7565 290a 0a20 2020 2023  ue(value)..    #
-00009090: 2063 6865 636b 2076 616c 7565 2074 7970   check value typ
-000090a0: 650a 2020 2020 666f 7220 7661 6c20 696e  e.    for val in
-000090b0: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
-000090c0: 2069 6620 6e6f 7420 7265 6765 782e 7365   if not regex.se
-000090d0: 6172 6368 2872 225e 5b30 2d39 5d2b 2422  arch(r"^[0-9]+$"
-000090e0: 2c20 7374 7228 7661 6c2e 7661 6c75 6529  , str(val.value)
-000090f0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00009100: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
-00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009120: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-00009130: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
-00009140: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
-00009150: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
-00009160: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
-00009170: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
-00009180: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
-00009190: 7420 6120 6765 6f6e 616d 6573 2e6f 7267  t a geonames.org
-000091a0: 2069 6465 6e74 6966 6965 722e 220a 2020   identifier.".  
-000091b0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000091c0: 2023 206d 616b 6520 786d 6c20 7374 7275   # make xml stru
-000091d0: 6374 7572 6520 6f66 2074 6865 2076 616c  cture of the val
-000091e0: 6964 2076 616c 7565 730a 2020 2020 7072  id values.    pr
-000091f0: 6f70 5f20 3d20 6574 7265 652e 456c 656d  op_ = etree.Elem
-00009200: 656e 7428 0a20 2020 2020 2020 2022 7b25  ent(.        "{%
-00009210: 737d 6765 6f6e 616d 652d 7072 6f70 2220  s}geoname-prop" 
-00009220: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-00009230: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-00009240: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
-00009250: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-00009260: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-00009270: 2020 2029 0a20 2020 2066 6f72 2076 616c     ).    for val
-00009280: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-00009290: 2020 2020 6b77 6172 6773 203d 207b 2270      kwargs = {"p
-000092a0: 6572 6d69 7373 696f 6e73 223a 2076 616c  ermissions": val
-000092b0: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
-000092c0: 2020 2020 2020 6966 2076 616c 2e63 6f6d        if val.com
-000092d0: 6d65 6e74 2061 6e64 2063 6865 636b 5f6e  ment and check_n
-000092e0: 6f74 6e61 2876 616c 2e63 6f6d 6d65 6e74  otna(val.comment
-000092f0: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
-00009300: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
-00009310: 203d 2076 616c 2e63 6f6d 6d65 6e74 0a20   = val.comment. 
-00009320: 2020 2020 2020 2076 616c 7565 5f20 3d20         value_ = 
-00009330: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-00009340: 2020 2020 2020 2020 2020 2022 7b25 737d             "{%s}
-00009350: 6765 6f6e 616d 6522 2025 2078 6d6c 5f6e  geoname" % xml_n
-00009360: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-00009370: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00009380: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
-00009390: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
-000093a0: 7065 5d0a 2020 2020 2020 2020 2020 2020  pe].            
-000093b0: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
-000093c0: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
-000093d0: 2029 0a20 2020 2020 2020 2076 616c 7565   ).        value
-000093e0: 5f2e 7465 7874 203d 2073 7472 2876 616c  _.text = str(val
-000093f0: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
-00009400: 7072 6f70 5f2e 6170 7065 6e64 2876 616c  prop_.append(val
-00009410: 7565 5f29 0a0a 2020 2020 7265 7475 726e  ue_)..    return
-00009420: 2070 726f 705f 0a0a 0a64 6566 206d 616b   prop_...def mak
-00009430: 655f 696e 7465 6765 725f 7072 6f70 280a  e_integer_prop(.
-00009440: 2020 2020 6e61 6d65 3a20 7374 722c 0a20      name: str,. 
-00009450: 2020 2076 616c 7565 3a20 556e 696f 6e5b     value: Union[
-00009460: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-00009470: 2073 7472 2c20 696e 742c 2049 7465 7261   str, int, Itera
-00009480: 626c 655b 556e 696f 6e5b 5072 6f70 6572  ble[Union[Proper
-00009490: 7479 456c 656d 656e 742c 2073 7472 2c20  tyElement, str, 
-000094a0: 696e 745d 5d5d 2c0a 2020 2020 6361 6c6c  int]]],.    call
-000094b0: 696e 675f 7265 736f 7572 6365 3a20 7374  ing_resource: st
-000094c0: 7220 3d20 2222 2c0a 2920 2d3e 2065 7472  r = "",.) -> etr
-000094d0: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-000094e0: 2022 2222 0a20 2020 204d 616b 6520 6120   """.    Make a 
-000094f0: 3c69 6e74 6567 6572 2d70 726f 703e 2066  <integer-prop> f
-00009500: 726f 6d20 6f6e 6520 6f72 206d 6f72 6520  rom one or more 
-00009510: 696e 7465 6765 7273 2e20 5468 6520 696e  integers. The in
-00009520: 7465 6765 7273 2063 616e 2062 6520 7072  tegers can be pr
-00009530: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
-00009540: 2c20 696e 7465 6765 722c 206f 7220 6173  , integer, or as
-00009550: 0a20 2020 2050 726f 7065 7274 7945 6c65  .    PropertyEle
-00009560: 6d65 6e74 2077 6974 6820 6120 7374 7269  ment with a stri
-00009570: 6e67 2f69 6e74 6567 6572 2069 6e73 6964  ng/integer insid
-00009580: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
-00009590: 7320 7374 7269 6e67 2f69 6e74 6567 6572  s string/integer
-000095a0: 2c20 7468 6520 7065 726d 6973 7369 6f6e  , the permission
-000095b0: 7320 6465 6661 756c 7420 746f 0a20 2020  s default to.   
-000095c0: 2022 7072 6f70 2d64 6566 6175 6c74 222e   "prop-default".
-000095d0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-000095e0: 2020 2020 6e61 6d65 3a20 7468 6520 6e61      name: the na
-000095f0: 6d65 206f 6620 7468 6973 2070 726f 7065  me of this prope
-00009600: 7274 7920 6173 2064 6566 696e 6564 2069  rty as defined i
-00009610: 6e20 7468 6520 6f6e 746f 0a20 2020 2020  n the onto.     
-00009620: 2020 2076 616c 7565 3a20 6f6e 6520 6f72     value: one or
-00009630: 206d 6f72 6520 696e 7465 6765 7273 2c20   more integers, 
-00009640: 6173 2073 7472 696e 672f 696e 742f 5072  as string/int/Pr
-00009650: 6f70 6572 7479 456c 656d 656e 742c 206f  opertyElement, o
-00009660: 7220 6173 2069 7465 7261 626c 6520 6f66  r as iterable of
-00009670: 2073 7472 696e 6773 2f69 6e74 732f 5072   strings/ints/Pr
-00009680: 6f70 6572 7479 456c 656d 656e 7473 0a20  opertyElements. 
-00009690: 2020 2020 2020 2063 616c 6c69 6e67 5f72         calling_r
-000096a0: 6573 6f75 7263 653a 2074 6865 206e 616d  esource: the nam
-000096b0: 6520 6f66 2074 6865 2070 6172 656e 7420  e of the parent 
-000096c0: 7265 736f 7572 6365 2028 666f 7220 6265  resource (for be
-000096d0: 7474 6572 2065 7272 6f72 206d 6573 7361  tter error messa
-000096e0: 6765 7329 0a0a 2020 2020 5261 6973 6573  ges)..    Raises
-000096f0: 3a0a 2020 2020 2020 2020 4261 7365 4572  :.        BaseEr
-00009700: 726f 723a 2049 6620 7468 6520 7661 6c75  ror: If the valu
-00009710: 6520 6973 206e 6f74 2061 2076 616c 6964  e is not a valid
-00009720: 2069 6e74 6567 6572 0a0a 2020 2020 5265   integer..    Re
-00009730: 7475 726e 733a 0a20 2020 2020 2020 2061  turns:.        a
-00009740: 6e20 6574 7265 652e 5f45 6c65 6d65 6e74  n etree._Element
-00009750: 2074 6861 7420 6361 6e20 6265 2061 7070   that can be app
-00009760: 656e 6465 6420 746f 2074 6865 2070 6172  ended to the par
-00009770: 656e 7420 7265 736f 7572 6365 2077 6974  ent resource wit
-00009780: 6820 7265 736f 7572 6365 2e61 7070 656e  h resource.appen
-00009790: 6428 6d61 6b65 5f2a 5f70 726f 7028 2e2e  d(make_*_prop(..
-000097a0: 2e29 290a 0a20 2020 2045 7861 6d70 6c65  .))..    Example
-000097b0: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
-000097c0: 7863 656c 3278 6d6c 2e6d 616b 655f 696e  xcel2xml.make_in
-000097d0: 7465 6765 725f 7072 6f70 2822 3a74 6573  teger_prop(":tes
-000097e0: 7470 726f 7065 7274 7922 2c20 2232 3736  tproperty", "276
-000097f0: 3133 3639 2229 0a20 2020 2020 2020 2020  1369").         
-00009800: 2020 2020 2020 203c 696e 7465 6765 722d         <integer-
-00009810: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
-00009820: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
-00009830: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009840: 696e 7465 6765 7220 7065 726d 6973 7369  integer permissi
-00009850: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-00009860: 7422 3e32 3736 3133 3639 3c2f 696e 7465  t">2761369</inte
-00009870: 6765 723e 0a20 2020 2020 2020 2020 2020  ger>.           
-00009880: 2020 2020 203c 2f69 6e74 6567 6572 2d70       </integer-p
-00009890: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
-000098a0: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
-000098b0: 696e 7465 6765 725f 7072 6f70 2822 3a74  integer_prop(":t
-000098c0: 6573 7470 726f 7065 7274 7922 2c20 6578  estproperty", ex
-000098d0: 6365 6c32 786d 6c2e 5072 6f70 6572 7479  cel2xml.Property
-000098e0: 456c 656d 656e 7428 2232 3736 3133 3639  Element("2761369
-000098f0: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
-00009900: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
-00009910: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
-00009920: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
-00009930: 2020 2020 2020 3c69 6e74 6567 6572 2d70        <integer-p
-00009940: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
-00009950: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
-00009960: 2020 2020 2020 2020 2020 2020 2020 3c69                <i
-00009970: 6e74 6567 6572 2070 6572 6d69 7373 696f  nteger permissio
-00009980: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
-00009990: 7465 6422 2063 6f6d 6d65 6e74 3d22 6578  ted" comment="ex
-000099a0: 616d 706c 6522 3e32 3736 3133 3639 3c2f  ample">2761369</
-000099b0: 696e 7465 6765 723e 0a20 2020 2020 2020  integer>.       
-000099c0: 2020 2020 2020 2020 203c 2f69 6e74 6567           </integ
-000099d0: 6572 2d70 726f 703e 0a20 2020 2020 2020  er-prop>.       
-000099e0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-000099f0: 616b 655f 696e 7465 6765 725f 7072 6f70  ake_integer_prop
-00009a00: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-00009a10: 2c20 5b22 3237 3631 3336 3922 2c20 2231  , ["2761369", "1
-00009a20: 3031 3031 3031 225d 290a 2020 2020 2020  010101"]).      
-00009a30: 2020 2020 2020 2020 2020 3c69 6e74 6567            <integ
-00009a40: 6572 2d70 726f 7020 6e61 6d65 3d22 3a74  er-prop name=":t
-00009a50: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 3c69 6e74 6567 6572 2070 6572 6d69    <integer permi
-00009a80: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-00009a90: 6175 6c74 223e 3237 3631 3336 393c 2f69  ault">2761369</i
-00009aa0: 6e74 6567 6572 3e0a 2020 2020 2020 2020  nteger>.        
-00009ab0: 2020 2020 2020 2020 2020 2020 3c69 6e74              <int
-00009ac0: 6567 6572 2070 6572 6d69 7373 696f 6e73  eger permissions
-00009ad0: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-00009ae0: 3130 3130 3130 313c 2f69 6e74 6567 6572  1010101</integer
-00009af0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00009b00: 2020 3c2f 696e 7465 6765 722d 7072 6f70    </integer-prop
-00009b10: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-00009b20: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-00009b30: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-00009b40: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-00009b50: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-00009b60: 2369 6e74 6567 6572 2d70 726f 700a 2020  #integer-prop.  
-00009b70: 2020 2222 220a 0a20 2020 2023 2063 6865    """..    # che
-00009b80: 636b 2074 6865 2069 6e70 7574 3a20 7072  ck the input: pr
-00009b90: 6570 6172 6520 6120 6c69 7374 2077 6974  epare a list wit
-00009ba0: 6820 7661 6c69 6420 7661 6c75 6573 0a20  h valid values. 
-00009bb0: 2020 2076 616c 7565 7320 3d20 7072 6570     values = prep
-00009bc0: 6172 655f 7661 6c75 6528 7661 6c75 6529  are_value(value)
-00009bd0: 0a0a 2020 2020 2320 6368 6563 6b20 7661  ..    # check va
-00009be0: 6c75 6520 7479 7065 0a20 2020 2066 6f72  lue type.    for
-00009bf0: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
-00009c00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00009c10: 2020 2020 2020 2020 2069 6e74 2876 616c           int(val
-00009c20: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
-00009c30: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00009c40: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-00009c50: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
-00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c70: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-00009c80: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
-00009c90: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
-00009ca0: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
-00009cb0: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
-00009cc0: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
-00009cd0: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
-00009ce0: 7420 6120 7661 6c69 6420 696e 7465 6765  t a valid intege
-00009cf0: 722e 220a 2020 2020 2020 2020 2020 2020  r.".            
-00009d00: 2920 6672 6f6d 204e 6f6e 650a 0a20 2020  ) from None..   
-00009d10: 2023 206d 616b 6520 786d 6c20 7374 7275   # make xml stru
-00009d20: 6374 7572 6520 6f66 2074 6865 2076 616c  cture of the val
-00009d30: 6964 2076 616c 7565 730a 2020 2020 7072  id values.    pr
-00009d40: 6f70 5f20 3d20 6574 7265 652e 456c 656d  op_ = etree.Elem
-00009d50: 656e 7428 0a20 2020 2020 2020 2022 7b25  ent(.        "{%
-00009d60: 737d 696e 7465 6765 722d 7072 6f70 2220  s}integer-prop" 
-00009d70: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-00009d80: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-00009d90: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
-00009da0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-00009db0: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-00009dc0: 2020 2029 0a20 2020 2066 6f72 2076 616c     ).    for val
-00009dd0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-00009de0: 2020 2020 6b77 6172 6773 203d 207b 2270      kwargs = {"p
-00009df0: 6572 6d69 7373 696f 6e73 223a 2076 616c  ermissions": val
-00009e00: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
-00009e10: 2020 2020 2020 6966 2076 616c 2e63 6f6d        if val.com
-00009e20: 6d65 6e74 2061 6e64 2063 6865 636b 5f6e  ment and check_n
-00009e30: 6f74 6e61 2876 616c 2e63 6f6d 6d65 6e74  otna(val.comment
-00009e40: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
-00009e50: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
-00009e60: 203d 2076 616c 2e63 6f6d 6d65 6e74 0a20   = val.comment. 
-00009e70: 2020 2020 2020 2076 616c 7565 5f20 3d20         value_ = 
-00009e80: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-00009e90: 2020 2020 2020 2020 2020 2022 7b25 737d             "{%s}
-00009ea0: 696e 7465 6765 7222 2025 2078 6d6c 5f6e  integer" % xml_n
-00009eb0: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-00009ec0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00009ed0: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
-00009ee0: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
-00009ef0: 7065 5d0a 2020 2020 2020 2020 2020 2020  pe].            
-00009f00: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
-00009f10: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
-00009f20: 2029 0a20 2020 2020 2020 2076 616c 7565   ).        value
-00009f30: 5f2e 7465 7874 203d 2073 7472 2869 6e74  _.text = str(int
-00009f40: 2876 616c 2e76 616c 7565 2929 0a20 2020  (val.value)).   
-00009f50: 2020 2020 2070 726f 705f 2e61 7070 656e       prop_.appen
-00009f60: 6428 7661 6c75 655f 290a 0a20 2020 2072  d(value_)..    r
-00009f70: 6574 7572 6e20 7072 6f70 5f0a 0a0a 6465  eturn prop_...de
-00009f80: 6620 6d61 6b65 5f69 6e74 6572 7661 6c5f  f make_interval_
-00009f90: 7072 6f70 280a 2020 2020 6e61 6d65 3a20  prop(.    name: 
-00009fa0: 7374 722c 0a20 2020 2076 616c 7565 3a20  str,.    value: 
-00009fb0: 556e 696f 6e5b 5072 6f70 6572 7479 456c  Union[PropertyEl
-00009fc0: 656d 656e 742c 2073 7472 2c20 4974 6572  ement, str, Iter
-00009fd0: 6162 6c65 5b55 6e69 6f6e 5b50 726f 7065  able[Union[Prope
-00009fe0: 7274 7945 6c65 6d65 6e74 2c20 7374 725d  rtyElement, str]
-00009ff0: 5d5d 2c0a 2020 2020 6361 6c6c 696e 675f  ]],.    calling_
-0000a000: 7265 736f 7572 6365 3a20 7374 7220 3d20  resource: str = 
-0000a010: 2222 2c0a 2920 2d3e 2065 7472 6565 2e5f  "",.) -> etree._
-0000a020: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
-0000a030: 0a20 2020 204d 616b 6520 6120 3c69 6e74  .    Make a <int
-0000a040: 6572 7661 6c2d 7072 6f70 3e20 6672 6f6d  erval-prop> from
-0000a050: 206f 6e65 206f 7220 6d6f 7265 2044 5350   one or more DSP
-0000a060: 2069 6e74 6572 7661 6c73 2e20 5468 6520   intervals. The 
-0000a070: 696e 7465 7276 616c 2873 2920 6361 6e20  interval(s) can 
-0000a080: 6265 2070 726f 7669 6465 6420 6173 2073  be provided as s
-0000a090: 7472 696e 6720 6f72 2061 730a 2020 2020  tring or as.    
-0000a0a0: 5072 6f70 6572 7479 456c 656d 656e 7420  PropertyElement 
-0000a0b0: 7769 7468 2061 2073 7472 696e 6720 696e  with a string in
-0000a0c0: 7369 6465 2e20 4966 2070 726f 7669 6465  side. If provide
-0000a0d0: 6420 6173 2073 7472 696e 672c 2074 6865  d as string, the
-0000a0e0: 2070 6572 6d69 7373 696f 6e73 2064 6566   permissions def
-0000a0f0: 6175 6c74 2074 6f20 2270 726f 702d 6465  ault to "prop-de
-0000a100: 6661 756c 7422 2e0a 0a20 2020 2041 7267  fault"...    Arg
-0000a110: 733a 0a20 2020 2020 2020 206e 616d 653a  s:.        name:
-0000a120: 2074 6865 206e 616d 6520 6f66 2074 6869   the name of thi
-0000a130: 7320 7072 6f70 6572 7479 2061 7320 6465  s property as de
-0000a140: 6669 6e65 6420 696e 2074 6865 206f 6e74  fined in the ont
-0000a150: 6f0a 2020 2020 2020 2020 7661 6c75 653a  o.        value:
-0000a160: 206f 6e65 206f 7220 6d6f 7265 2044 5350   one or more DSP
-0000a170: 2069 6e74 6572 7661 6c73 2c20 6173 2073   intervals, as s
-0000a180: 7472 696e 672f 5072 6f70 6572 7479 456c  tring/PropertyEl
-0000a190: 656d 656e 742c 206f 7220 6173 2069 7465  ement, or as ite
-0000a1a0: 7261 626c 6520 6f66 2073 7472 696e 6773  rable of strings
-0000a1b0: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-0000a1c0: 730a 2020 2020 2020 2020 6361 6c6c 696e  s.        callin
-0000a1d0: 675f 7265 736f 7572 6365 3a20 7468 6520  g_resource: the 
-0000a1e0: 6e61 6d65 206f 6620 7468 6520 7061 7265  name of the pare
-0000a1f0: 6e74 2072 6573 6f75 7263 6520 2866 6f72  nt resource (for
-0000a200: 2062 6574 7465 7220 6572 726f 7220 6d65   better error me
-0000a210: 7373 6167 6573 290a 0a20 2020 2052 6169  ssages)..    Rai
-0000a220: 7365 733a 0a20 2020 2020 2020 2042 6173  ses:.        Bas
-0000a230: 6545 7272 6f72 3a20 4966 2074 6865 2076  eError: If the v
-0000a240: 616c 7565 2069 7320 6e6f 7420 6120 7661  alue is not a va
-0000a250: 6c69 6420 4453 5020 696e 7465 7276 616c  lid DSP interval
-0000a260: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000a270: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
-0000a280: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
-0000a290: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
-0000a2a0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-0000a2b0: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
-0000a2c0: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
-0000a2d0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
-0000a2e0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-0000a2f0: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000a300: 2e6d 616b 655f 696e 7465 7276 616c 5f70  .make_interval_p
-0000a310: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-0000a320: 7479 222c 2022 3631 3a33 3630 3022 290a  ty", "61:3600").
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a340: 3c69 6e74 6572 7661 6c2d 7072 6f70 206e  <interval-prop n
-0000a350: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-0000a360: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-0000a370: 2020 2020 2020 2020 203c 696e 7465 7276           <interv
-0000a380: 616c 2070 6572 6d69 7373 696f 6e73 3d22  al permissions="
-0000a390: 7072 6f70 2d64 6566 6175 6c74 223e 3631  prop-default">61
-0000a3a0: 3a33 3630 303c 2f69 6e74 6572 7661 6c3e  :3600</interval>
-0000a3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a3c0: 203c 2f69 6e74 6572 7661 6c2d 7072 6f70   </interval-prop
-0000a3d0: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
-0000a3e0: 6365 6c32 786d 6c2e 6d61 6b65 5f69 6e74  cel2xml.make_int
-0000a3f0: 6572 7661 6c5f 7072 6f70 2822 3a74 6573  erval_prop(":tes
-0000a400: 7470 726f 7065 7274 7922 2c20 6578 6365  tproperty", exce
-0000a410: 6c32 786d 6c2e 5072 6f70 6572 7479 456c  l2xml.PropertyEl
-0000a420: 656d 656e 7428 2236 313a 3336 3030 222c  ement("61:3600",
-0000a430: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000a440: 6f70 2d72 6573 7472 6963 7465 6422 2c20  op-restricted", 
-0000a450: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
-0000a460: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
-0000a470: 2020 2020 3c69 6e74 6572 7661 6c2d 7072      <interval-pr
-0000a480: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
-0000a490: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
-0000a4a0: 2020 2020 2020 2020 2020 2020 203c 696e               <in
-0000a4b0: 7465 7276 616c 2070 6572 6d69 7373 696f  terval permissio
-0000a4c0: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
-0000a4d0: 7465 6422 2063 6f6d 6d65 6e74 3d22 6578  ted" comment="ex
-0000a4e0: 616d 706c 6522 3e36 313a 3336 3030 3c2f  ample">61:3600</
-0000a4f0: 696e 7465 7276 616c 3e0a 2020 2020 2020  interval>.      
-0000a500: 2020 2020 2020 2020 2020 3c2f 696e 7465            </inte
-0000a510: 7276 616c 2d70 726f 703e 0a20 2020 2020  rval-prop>.     
-0000a520: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000a530: 2e6d 616b 655f 696e 7465 7276 616c 5f70  .make_interval_p
-0000a540: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-0000a550: 7479 222c 205b 2236 313a 3336 3030 222c  ty", ["61:3600",
-0000a560: 2022 3630 2e35 3a31 3230 2e35 225d 290a   "60.5:120.5"]).
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 3c69 6e74 6572 7661 6c2d 7072 6f70 206e  <interval-prop n
-0000a590: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-0000a5a0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-0000a5b0: 2020 2020 2020 2020 203c 696e 7465 7276           <interv
-0000a5c0: 616c 2070 6572 6d69 7373 696f 6e73 3d22  al permissions="
-0000a5d0: 7072 6f70 2d64 6566 6175 6c74 223e 3631  prop-default">61
-0000a5e0: 3a33 3630 303c 2f69 6e74 6572 7661 6c3e  :3600</interval>
-0000a5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a600: 2020 2020 203c 696e 7465 7276 616c 2070       <interval p
-0000a610: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-0000a620: 2d64 6566 6175 6c74 223e 3630 2e35 3a31  -default">60.5:1
-0000a630: 3230 2e35 3c2f 696e 7465 7276 616c 3e0a  20.5</interval>.
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a650: 3c2f 696e 7465 7276 616c 2d70 726f 703e  </interval-prop>
-0000a660: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-0000a670: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
-0000a680: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
-0000a690: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
-0000a6a0: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
-0000a6b0: 696e 7465 7276 616c 2d70 726f 700a 2020  interval-prop.  
-0000a6c0: 2020 2222 220a 0a20 2020 2023 2063 6865    """..    # che
-0000a6d0: 636b 2074 6865 2069 6e70 7574 3a20 7072  ck the input: pr
-0000a6e0: 6570 6172 6520 6120 6c69 7374 2077 6974  epare a list wit
-0000a6f0: 6820 7661 6c69 6420 7661 6c75 6573 0a20  h valid values. 
-0000a700: 2020 2076 616c 7565 7320 3d20 7072 6570     values = prep
-0000a710: 6172 655f 7661 6c75 6528 7661 6c75 6529  are_value(value)
-0000a720: 0a0a 2020 2020 2320 6368 6563 6b20 7661  ..    # check va
-0000a730: 6c75 6520 7479 7065 0a20 2020 2066 6f72  lue type.    for
-0000a740: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
-0000a750: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-0000a760: 6567 6578 2e6d 6174 6368 280a 2020 2020  egex.match(.    
-0000a770: 2020 2020 2020 2020 7222 285b 2b2d 5d3f          r"([+-]?
-0000a780: 285b 302d 395d 2b28 5b2e 5d5b 302d 395d  ([0-9]+([.][0-9]
-0000a790: 2a29 3f7c 5b2e 5d5b 302d 395d 2b29 293a  *)?|[.][0-9]+)):
-0000a7a0: 285b 2b2d 5d3f 285b 302d 395d 2b28 5b2e  ([+-]?([0-9]+([.
-0000a7b0: 5d5b 302d 395d 2a29 3f7c 5b2e 5d5b 302d  ][0-9]*)?|[.][0-
-0000a7c0: 395d 2b29 2922 2c0a 2020 2020 2020 2020  9]+))",.        
-0000a7d0: 2020 2020 7374 7228 7661 6c2e 7661 6c75      str(val.valu
-0000a7e0: 6529 2c0a 2020 2020 2020 2020 293a 0a20  e),.        ):. 
-0000a7f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000a800: 2042 6173 6545 7272 6f72 280a 2020 2020   BaseError(.    
-0000a810: 2020 2020 2020 2020 2020 2020 6622 4661              f"Fa
-0000a820: 696c 6564 2076 616c 6964 6174 696f 6e20  iled validation 
-0000a830: 696e 2072 6573 6f75 7263 6520 277b 6361  in resource '{ca
-0000a840: 6c6c 696e 675f 7265 736f 7572 6365 7d27  lling_resource}'
-0000a850: 2c20 7072 6f70 6572 7479 2027 7b6e 616d  , property '{nam
-0000a860: 657d 273a 2022 0a20 2020 2020 2020 2020  e}': ".         
-0000a870: 2020 2020 2020 2066 2227 7b76 616c 2e76         f"'{val.v
-0000a880: 616c 7565 7d27 2069 7320 6e6f 7420 6120  alue}' is not a 
-0000a890: 7661 6c69 6420 4453 5020 696e 7465 7276  valid DSP interv
-0000a8a0: 616c 2e22 0a20 2020 2020 2020 2020 2020  al.".           
-0000a8b0: 2029 0a0a 2020 2020 2320 6d61 6b65 2078   )..    # make x
-0000a8c0: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-0000a8d0: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
-0000a8e0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-0000a8f0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-0000a900: 2020 2020 227b 2573 7d69 6e74 6572 7661      "{%s}interva
-0000a910: 6c2d 7072 6f70 2220 2520 786d 6c5f 6e61  l-prop" % xml_na
-0000a920: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-0000a930: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
-0000a940: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
-0000a950: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
-0000a960: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
-0000a970: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
-0000a980: 6573 3a0a 2020 2020 2020 2020 6b77 6172  es:.        kwar
-0000a990: 6773 203d 207b 2270 6572 6d69 7373 696f  gs = {"permissio
-0000a9a0: 6e73 223a 2076 616c 2e70 6572 6d69 7373  ns": val.permiss
-0000a9b0: 696f 6e73 7d0a 2020 2020 2020 2020 6966  ions}.        if
-0000a9c0: 2076 616c 2e63 6f6d 6d65 6e74 2061 6e64   val.comment and
-0000a9d0: 2063 6865 636b 5f6e 6f74 6e61 2876 616c   check_notna(val
-0000a9e0: 2e63 6f6d 6d65 6e74 293a 0a20 2020 2020  .comment):.     
-0000a9f0: 2020 2020 2020 206b 7761 7267 735b 2263         kwargs["c
-0000aa00: 6f6d 6d65 6e74 225d 203d 2076 616c 2e63  omment"] = val.c
-0000aa10: 6f6d 6d65 6e74 0a20 2020 2020 2020 2076  omment.        v
-0000aa20: 616c 7565 5f20 3d20 6574 7265 652e 456c  alue_ = etree.El
-0000aa30: 656d 656e 7428 0a20 2020 2020 2020 2020  ement(.         
-0000aa40: 2020 2022 7b25 737d 696e 7465 7276 616c     "{%s}interval
-0000aa50: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000aa60: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000aa70: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-0000aa80: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000aa90: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-0000aaa0: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
-0000aab0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-0000aac0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000aad0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
-0000aae0: 3d20 7374 7228 7661 6c2e 7661 6c75 6529  = str(val.value)
-0000aaf0: 0a20 2020 2020 2020 2070 726f 705f 2e61  .        prop_.a
-0000ab00: 7070 656e 6428 7661 6c75 655f 290a 0a20  ppend(value_).. 
-0000ab10: 2020 2072 6574 7572 6e20 7072 6f70 5f0a     return prop_.
-0000ab20: 0a0a 6465 6620 6d61 6b65 5f6c 6973 745f  ..def make_list_
-0000ab30: 7072 6f70 280a 2020 2020 6c69 7374 5f6e  prop(.    list_n
-0000ab40: 616d 653a 2073 7472 2c0a 2020 2020 6e61  ame: str,.    na
-0000ab50: 6d65 3a20 7374 722c 0a20 2020 2076 616c  me: str,.    val
-0000ab60: 7565 3a20 556e 696f 6e5b 5072 6f70 6572  ue: Union[Proper
-0000ab70: 7479 456c 656d 656e 742c 2073 7472 2c20  tyElement, str, 
-0000ab80: 4974 6572 6162 6c65 5b55 6e69 6f6e 5b50  Iterable[Union[P
-0000ab90: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-0000aba0: 7374 725d 5d5d 2c0a 2020 2020 6361 6c6c  str]]],.    call
-0000abb0: 696e 675f 7265 736f 7572 6365 3a20 7374  ing_resource: st
-0000abc0: 7220 3d20 2222 2c0a 2920 2d3e 2065 7472  r = "",.) -> etr
-0000abd0: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-0000abe0: 2022 2222 0a20 2020 204d 616b 6520 6120   """.    Make a 
-0000abf0: 3c6c 6973 742d 7072 6f70 3e20 6672 6f6d  <list-prop> from
-0000ac00: 206f 6e65 206f 7220 6d6f 7265 206c 6973   one or more lis
-0000ac10: 7420 6e6f 6465 732e 2054 6865 206e 616d  t nodes. The nam
-0000ac20: 6528 7329 206f 6620 7468 6520 6c69 7374  e(s) of the list
-0000ac30: 206e 6f64 6528 7329 2063 616e 2062 6520   node(s) can be 
-0000ac40: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-0000ac50: 6e67 206f 7220 6173 0a20 2020 2050 726f  ng or as.    Pro
-0000ac60: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
-0000ac70: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
-0000ac80: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
-0000ac90: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
-0000aca0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
-0000acb0: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
-0000acc0: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
-0000acd0: 2020 2020 2020 2020 6c69 7374 5f6e 616d          list_nam
-0000ace0: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
-0000acf0: 6865 206c 6973 7420 6173 2064 6566 696e  he list as defin
-0000ad00: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
-0000ad10: 2020 2020 2020 206e 616d 653a 2074 6865         name: the
-0000ad20: 206e 616d 6520 6f66 2074 6869 7320 7072   name of this pr
-0000ad30: 6f70 6572 7479 2061 7320 6465 6669 6e65  operty as define
-0000ad40: 6420 696e 2074 6865 206f 6e74 6f0a 2020  d in the onto.  
-0000ad50: 2020 2020 2020 7661 6c75 653a 206f 6e65        value: one
-0000ad60: 206f 7220 6d6f 7265 206e 6f64 6520 6e61   or more node na
-0000ad70: 6d65 732c 2061 7320 7374 7269 6e67 2f50  mes, as string/P
-0000ad80: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-0000ad90: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
-0000ada0: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
-0000adb0: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
-0000adc0: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
-0000add0: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
-0000ade0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-0000adf0: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
-0000ae00: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
-0000ae10: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
-0000ae20: 2020 2020 2020 4261 7365 4572 726f 723a        BaseError:
-0000ae30: 2049 6620 7468 6520 6e61 6d65 206f 6620   If the name of 
-0000ae40: 6f6e 6520 6f66 2074 6865 206c 6973 7420  one of the list 
-0000ae50: 6e6f 6465 7320 6973 206e 6f74 2061 2076  nodes is not a v
-0000ae60: 616c 6964 2073 7472 696e 670a 0a20 2020  alid string..   
-0000ae70: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000ae80: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
-0000ae90: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
-0000aea0: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
-0000aeb0: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
-0000aec0: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
-0000aed0: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
-0000aee0: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
-0000aef0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
-0000af00: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
-0000af10: 5f6c 6973 745f 7072 6f70 2822 6d79 6c69  _list_prop("myli
-0000af20: 7374 222c 2022 3a74 6573 7470 726f 7065  st", ":testprope
-0000af30: 7274 7922 2c20 2266 6972 7374 5f6e 6f64  rty", "first_nod
-0000af40: 6522 290a 2020 2020 2020 2020 2020 2020  e").            
-0000af50: 2020 2020 3c6c 6973 742d 7072 6f70 206c      <list-prop l
-0000af60: 6973 743d 226d 796c 6973 7422 206e 616d  ist="mylist" nam
-0000af70: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
-0000af80: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-0000af90: 2020 2020 2020 203c 6c69 7374 2070 6572         <list per
-0000afa0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
-0000afb0: 6566 6175 6c74 223e 6669 7273 745f 6e6f  efault">first_no
-0000afc0: 6465 3c2f 6c69 7374 3e0a 2020 2020 2020  de</list>.      
-0000afd0: 2020 2020 2020 2020 2020 3c2f 6c69 7374            </list
-0000afe0: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
-0000aff0: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
-0000b000: 655f 6c69 7374 5f70 726f 7028 226d 796c  e_list_prop("myl
-0000b010: 6973 7422 2c20 223a 7465 7374 7072 6f70  ist", ":testprop
-0000b020: 6572 7479 222c 2065 7863 656c 3278 6d6c  erty", excel2xml
-0000b030: 2e50 726f 7065 7274 7945 6c65 6d65 6e74  .PropertyElement
-0000b040: 2822 6669 7273 745f 6e6f 6465 222c 2070  ("first_node", p
-0000b050: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-0000b060: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
-0000b070: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
-0000b080: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000b090: 2020 3c6c 6973 742d 7072 6f70 206c 6973    <list-prop lis
-0000b0a0: 743d 226d 796c 6973 7422 206e 616d 653d  t="mylist" name=
-0000b0b0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
-0000b0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b0d0: 2020 2020 203c 6c69 7374 2070 6572 6d69       <list permi
-0000b0e0: 7373 696f 6e73 3d22 7072 6f70 2d72 6573  ssions="prop-res
-0000b0f0: 7472 6963 7465 6422 2063 6f6d 6d65 6e74  tricted" comment
-0000b100: 3d22 6578 616d 706c 6522 3e66 6972 7374  ="example">first
-0000b110: 5f6e 6f64 653c 2f6c 6973 743e 0a20 2020  _node</list>.   
-0000b120: 2020 2020 2020 2020 2020 2020 203c 2f6c               </l
-0000b130: 6973 742d 7072 6f70 3e0a 2020 2020 2020  ist-prop>.      
-0000b140: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
-0000b150: 6d61 6b65 5f6c 6973 745f 7072 6f70 2822  make_list_prop("
-0000b160: 6d79 6c69 7374 222c 2022 3a74 6573 7470  mylist", ":testp
-0000b170: 726f 7065 7274 7922 2c20 5b22 6669 7273  roperty", ["firs
-0000b180: 745f 6e6f 6465 222c 2022 7365 636f 6e64  t_node", "second
-0000b190: 5f6e 6f64 6522 5d29 0a20 2020 2020 2020  _node"]).       
-0000b1a0: 2020 2020 2020 2020 203c 6c69 7374 2d70           <list-p
-0000b1b0: 726f 7020 6c69 7374 3d22 6d79 6c69 7374  rop list="mylist
-0000b1c0: 2220 6e61 6d65 3d22 3a74 6573 7470 726f  " name=":testpro
-0000b1d0: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
-0000b1e0: 2020 2020 2020 2020 2020 2020 3c6c 6973              <lis
-0000b1f0: 7420 7065 726d 6973 7369 6f6e 733d 2270  t permissions="p
-0000b200: 726f 702d 6465 6661 756c 7422 3e66 6972  rop-default">fir
-0000b210: 7374 5f6e 6f64 653c 2f6c 6973 743e 0a20  st_node</list>. 
-0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 203c 6c69 7374 2070 6572 6d69 7373     <list permiss
-0000b240: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-0000b250: 6c74 223e 7365 636f 6e64 5f6e 6f64 653c  lt">second_node<
-0000b260: 2f6c 6973 743e 0a20 2020 2020 2020 2020  /list>.         
-0000b270: 2020 2020 2020 203c 2f6c 6973 742d 7072         </list-pr
-0000b280: 6f70 3e0a 0a20 2020 2053 6565 2068 7474  op>..    See htt
-0000b290: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-0000b2a0: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
-0000b2b0: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
-0000b2c0: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
-0000b2d0: 652f 236c 6973 742d 7072 6f70 0a20 2020  e/#list-prop.   
-0000b2e0: 2022 2222 0a0a 2020 2020 2320 6368 6563   """..    # chec
-0000b2f0: 6b20 7468 6520 696e 7075 743a 2070 7265  k the input: pre
-0000b300: 7061 7265 2061 206c 6973 7420 7769 7468  pare a list with
-0000b310: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
-0000b320: 2020 7661 6c75 6573 203d 2070 7265 7061    values = prepa
-0000b330: 7265 5f76 616c 7565 2876 616c 7565 290a  re_value(value).
-0000b340: 0a20 2020 2023 2063 6865 636b 2076 616c  .    # check val
-0000b350: 7565 2074 7970 650a 2020 2020 666f 7220  ue type.    for 
-0000b360: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
-0000b370: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-0000b380: 696e 7374 616e 6365 2876 616c 2e76 616c  instance(val.val
-0000b390: 7565 2c20 7374 7229 206f 7220 6e6f 7420  ue, str) or not 
-0000b3a0: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
-0000b3b0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
-0000b3c0: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
-0000b3d0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000b3e0: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
-0000b3f0: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
-0000b400: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
-0000b410: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
-0000b420: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
-0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b440: 6622 277b 7661 6c2e 7661 6c75 657d 2720  f"'{val.value}' 
-0000b450: 6973 206e 6f74 2061 2076 616c 6964 206e  is not a valid n
-0000b460: 616d 6520 6f66 2061 206c 6973 7420 6e6f  ame of a list no
-0000b470: 6465 2e22 0a20 2020 2020 2020 2020 2020  de.".           
-0000b480: 2029 0a0a 2020 2020 2320 6d61 6b65 2078   )..    # make x
-0000b490: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-0000b4a0: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
-0000b4b0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-0000b4c0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-0000b4d0: 2020 2020 227b 2573 7d6c 6973 742d 7072      "{%s}list-pr
-0000b4e0: 6f70 2220 2520 786d 6c5f 6e61 6d65 7370  op" % xml_namesp
-0000b4f0: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-0000b500: 2020 2020 2020 206c 6973 743d 6c69 7374         list=list
-0000b510: 5f6e 616d 652c 0a20 2020 2020 2020 206e  _name,.        n
-0000b520: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
-0000b530: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
-0000b540: 7370 6163 655f 6d61 702c 0a20 2020 2029  space_map,.    )
-0000b550: 0a20 2020 2066 6f72 2076 616c 2069 6e20  .    for val in 
-0000b560: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
-0000b570: 6b77 6172 6773 203d 207b 2270 6572 6d69  kwargs = {"permi
-0000b580: 7373 696f 6e73 223a 2076 616c 2e70 6572  ssions": val.per
-0000b590: 6d69 7373 696f 6e73 7d0a 2020 2020 2020  missions}.      
-0000b5a0: 2020 6966 2076 616c 2e63 6f6d 6d65 6e74    if val.comment
-0000b5b0: 2061 6e64 2063 6865 636b 5f6e 6f74 6e61   and check_notna
-0000b5c0: 2876 616c 2e63 6f6d 6d65 6e74 293a 0a20  (val.comment):. 
-0000b5d0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-0000b5e0: 735b 2263 6f6d 6d65 6e74 225d 203d 2076  s["comment"] = v
-0000b5f0: 616c 2e63 6f6d 6d65 6e74 0a20 2020 2020  al.comment.     
-0000b600: 2020 2076 616c 7565 5f20 3d20 6574 7265     value_ = etre
-0000b610: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
-0000b620: 2020 2020 2020 2022 7b25 737d 6c69 7374         "{%s}list
-0000b630: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000b640: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000b650: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-0000b660: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000b670: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-0000b680: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
-0000b690: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-0000b6a0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000b6b0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
-0000b6c0: 3d20 7374 7228 7661 6c2e 7661 6c75 6529  = str(val.value)
-0000b6d0: 0a20 2020 2020 2020 2070 726f 705f 2e61  .        prop_.a
-0000b6e0: 7070 656e 6428 7661 6c75 655f 290a 0a20  ppend(value_).. 
-0000b6f0: 2020 2072 6574 7572 6e20 7072 6f70 5f0a     return prop_.
-0000b700: 0a0a 6465 6620 6d61 6b65 5f72 6573 7074  ..def make_respt
-0000b710: 725f 7072 6f70 280a 2020 2020 6e61 6d65  r_prop(.    name
-0000b720: 3a20 7374 722c 0a20 2020 2076 616c 7565  : str,.    value
-0000b730: 3a20 556e 696f 6e5b 5072 6f70 6572 7479  : Union[Property
-0000b740: 456c 656d 656e 742c 2073 7472 2c20 4974  Element, str, It
-0000b750: 6572 6162 6c65 5b55 6e69 6f6e 5b50 726f  erable[Union[Pro
-0000b760: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
-0000b770: 725d 5d5d 2c0a 2020 2020 6361 6c6c 696e  r]]],.    callin
-0000b780: 675f 7265 736f 7572 6365 3a20 7374 7220  g_resource: str 
-0000b790: 3d20 2222 2c0a 2920 2d3e 2065 7472 6565  = "",.) -> etree
-0000b7a0: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
-0000b7b0: 2222 0a20 2020 204d 616b 6520 6120 3c72  "".    Make a <r
-0000b7c0: 6573 7074 722d 7072 6f70 3e20 6672 6f6d  esptr-prop> from
-0000b7d0: 206f 6e65 206f 7220 6d6f 7265 2049 4473   one or more IDs
-0000b7e0: 206f 6620 6f74 6865 7220 7265 736f 7572   of other resour
-0000b7f0: 6365 732e 2054 6865 2049 4428 7329 2063  ces. The ID(s) c
-0000b800: 616e 2062 6520 7072 6f76 6964 6564 2061  an be provided a
-0000b810: 7320 7374 7269 6e67 206f 7220 6173 0a20  s string or as. 
-0000b820: 2020 2050 726f 7065 7274 7945 6c65 6d65     PropertyEleme
-0000b830: 6e74 2077 6974 6820 6120 7374 7269 6e67  nt with a string
-0000b840: 2069 6e73 6964 652e 2049 6620 7072 6f76   inside. If prov
-0000b850: 6964 6564 2061 7320 7374 7269 6e67 2c20  ided as string, 
-0000b860: 7468 6520 7065 726d 6973 7369 6f6e 7320  the permissions 
-0000b870: 6465 6661 756c 7420 746f 2022 7072 6f70  default to "prop
-0000b880: 2d64 6566 6175 6c74 222e 0a0a 2020 2020  -default"...    
-0000b890: 4172 6773 3a0a 2020 2020 2020 2020 6e61  Args:.        na
-0000b8a0: 6d65 3a20 7468 6520 6e61 6d65 206f 6620  me: the name of 
-0000b8b0: 7468 6973 2070 726f 7065 7274 7920 6173  this property as
-0000b8c0: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
-0000b8d0: 6f6e 746f 0a20 2020 2020 2020 2076 616c  onto.        val
-0000b8e0: 7565 3a20 6f6e 6520 6f72 206d 6f72 6520  ue: one or more 
-0000b8f0: 7265 736f 7572 6365 2069 6465 6e74 6966  resource identif
-0000b900: 6965 7273 2c20 6173 2073 7472 696e 672f  iers, as string/
-0000b910: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-0000b920: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
-0000b930: 6f66 2073 7472 696e 6773 2f50 726f 7065  of strings/Prope
-0000b940: 7274 7945 6c65 6d65 6e74 730a 2020 2020  rtyElements.    
-0000b950: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-0000b960: 7572 6365 3a20 7468 6520 6e61 6d65 206f  urce: the name o
-0000b970: 6620 7468 6520 7061 7265 6e74 2072 6573  f the parent res
-0000b980: 6f75 7263 6520 2866 6f72 2062 6574 7465  ource (for bette
-0000b990: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
-0000b9a0: 290a 0a20 2020 2052 6169 7365 733a 0a20  )..    Raises:. 
-0000b9b0: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
-0000b9c0: 3a20 4966 2074 6865 2049 4420 6f66 206f  : If the ID of o
-0000b9d0: 6e65 206f 6620 7468 6520 7461 7267 6574  ne of the target
-0000b9e0: 2072 6573 6f75 7263 6573 2069 7320 6e6f   resources is no
-0000b9f0: 7420 6120 7661 6c69 6420 7374 7269 6e67  t a valid string
-0000ba00: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000ba10: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
-0000ba20: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
-0000ba30: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
-0000ba40: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-0000ba50: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
-0000ba60: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
-0000ba70: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
-0000ba80: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-0000ba90: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000baa0: 2e6d 616b 655f 7265 7370 7472 5f70 726f  .make_resptr_pro
-0000bab0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-0000bac0: 222c 2022 7265 736f 7572 6365 5f31 2229  ", "resource_1")
-0000bad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bae0: 203c 7265 7370 7472 2d70 726f 7020 6e61   <resptr-prop na
-0000baf0: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-0000bb00: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-0000bb10: 2020 2020 2020 2020 3c72 6573 7074 7220          <resptr 
-0000bb20: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-0000bb30: 702d 6465 6661 756c 7422 3e72 6573 6f75  p-default">resou
-0000bb40: 7263 655f 313c 2f72 6573 7074 723e 0a20  rce_1</resptr>. 
-0000bb50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000bb60: 2f72 6573 7074 722d 7072 6f70 3e0a 2020  /resptr-prop>.  
-0000bb70: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-0000bb80: 786d 6c2e 6d61 6b65 5f72 6573 7074 725f  xml.make_resptr_
-0000bb90: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
-0000bba0: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
-0000bbb0: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
-0000bbc0: 2272 6573 6f75 7263 655f 3122 2c20 7065  "resource_1", pe
-0000bbd0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000bbe0: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
-0000bbf0: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
-0000bc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bc10: 203c 7265 7370 7472 2d70 726f 7020 6e61   <resptr-prop na
-0000bc20: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-0000bc30: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-0000bc40: 2020 2020 2020 2020 3c72 6573 7074 7220          <resptr 
-0000bc50: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-0000bc60: 702d 7265 7374 7269 6374 6564 2220 636f  p-restricted" co
-0000bc70: 6d6d 656e 743d 2265 7861 6d70 6c65 223e  mment="example">
-0000bc80: 7265 736f 7572 6365 5f31 3c2f 7265 7370  resource_1</resp
-0000bc90: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
-0000bca0: 2020 2020 3c2f 7265 7370 7472 2d70 726f      </resptr-pro
-0000bcb0: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-0000bcc0: 7863 656c 3278 6d6c 2e6d 616b 655f 7265  xcel2xml.make_re
-0000bcd0: 7370 7472 5f70 726f 7028 223a 7465 7374  sptr_prop(":test
-0000bce0: 7072 6f70 6572 7479 222c 205b 2272 6573  property", ["res
-0000bcf0: 6f75 7263 655f 3122 2c20 2272 6573 6f75  ource_1", "resou
-0000bd00: 7263 655f 3222 5d29 0a20 2020 2020 2020  rce_2"]).       
-0000bd10: 2020 2020 2020 2020 203c 7265 7370 7472           <resptr
-0000bd20: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
-0000bd30: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
-0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd50: 3c72 6573 7074 7220 7065 726d 6973 7369  <resptr permissi
-0000bd60: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000bd70: 7422 3e72 6573 6f75 7263 655f 313c 2f72  t">resource_1</r
-0000bd80: 6573 7074 723e 0a20 2020 2020 2020 2020  esptr>.         
-0000bd90: 2020 2020 2020 2020 2020 203c 7265 7370             <resp
-0000bda0: 7472 2070 6572 6d69 7373 696f 6e73 3d22  tr permissions="
-0000bdb0: 7072 6f70 2d64 6566 6175 6c74 223e 7265  prop-default">re
-0000bdc0: 736f 7572 6365 5f32 3c2f 7265 7370 7472  source_2</resptr
-0000bdd0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000bde0: 2020 3c2f 7265 7370 7472 2d70 726f 703e    </resptr-prop>
-0000bdf0: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-0000be00: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
-0000be10: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
-0000be20: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
-0000be30: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
-0000be40: 7265 7370 7472 2d70 726f 700a 2020 2020  resptr-prop.    
-0000be50: 2222 220a 0a20 2020 2023 2063 6865 636b  """..    # check
-0000be60: 2074 6865 2069 6e70 7574 3a20 7072 6570   the input: prep
-0000be70: 6172 6520 6120 6c69 7374 2077 6974 6820  are a list with 
-0000be80: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000be90: 2076 616c 7565 7320 3d20 7072 6570 6172   values = prepar
-0000bea0: 655f 7661 6c75 6528 7661 6c75 6529 0a0a  e_value(value)..
-0000beb0: 2020 2020 2320 6368 6563 6b20 7661 6c75      # check valu
-0000bec0: 6520 7479 7065 0a20 2020 2066 6f72 2076  e type.    for v
-0000bed0: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-0000bee0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000bef0: 6e73 7461 6e63 6528 7661 6c2e 7661 6c75  nstance(val.valu
-0000bf00: 652c 2073 7472 2920 6f72 206e 6f74 2063  e, str) or not c
-0000bf10: 6865 636b 5f6e 6f74 6e61 2876 616c 2e76  heck_notna(val.v
-0000bf20: 616c 7565 293a 0a20 2020 2020 2020 2020  alue):.         
-0000bf30: 2020 2072 6169 7365 2042 6173 6545 7272     raise BaseErr
-0000bf40: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000bf50: 2020 2020 6622 5661 6c69 6461 7469 6f6e      f"Validation
-0000bf60: 2045 7272 6f72 2069 6e20 7265 736f 7572   Error in resour
-0000bf70: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
-0000bf80: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
-0000bf90: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000bfb0: 5468 6520 666f 6c6c 6f77 696e 6720 646f  The following do
-0000bfc0: 6573 6e27 7420 7365 656d 2074 6f20 6265  esn't seem to be
-0000bfd0: 2061 2076 616c 6964 2049 4420 6f66 2061   a valid ID of a
-0000bfe0: 2074 6172 6765 7420 7265 736f 7572 6365   target resource
-0000bff0: 3a20 277b 7661 6c2e 7661 6c75 657d 2722  : '{val.value}'"
-0000c000: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0000c010: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
-0000c020: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
-0000c030: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000c040: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
-0000c050: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0000c060: 227b 2573 7d72 6573 7074 722d 7072 6f70  "{%s}resptr-prop
-0000c070: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000c080: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000c090: 2020 2020 206e 616d 653d 6e61 6d65 2c0a       name=name,.
-0000c0a0: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-0000c0b0: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-0000c0c0: 0a20 2020 2029 0a20 2020 2066 6f72 2076  .    ).    for v
-0000c0d0: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-0000c0e0: 2020 2020 2020 6b77 6172 6773 203d 207b        kwargs = {
-0000c0f0: 2270 6572 6d69 7373 696f 6e73 223a 2076  "permissions": v
-0000c100: 616c 2e70 6572 6d69 7373 696f 6e73 7d0a  al.permissions}.
-0000c110: 2020 2020 2020 2020 6966 2076 616c 2e63          if val.c
-0000c120: 6f6d 6d65 6e74 2061 6e64 2063 6865 636b  omment and check
-0000c130: 5f6e 6f74 6e61 2876 616c 2e63 6f6d 6d65  _notna(val.comme
-0000c140: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-0000c150: 206b 7761 7267 735b 2263 6f6d 6d65 6e74   kwargs["comment
-0000c160: 225d 203d 2076 616c 2e63 6f6d 6d65 6e74  "] = val.comment
-0000c170: 0a20 2020 2020 2020 2076 616c 7565 5f20  .        value_ 
-0000c180: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-0000c190: 0a20 2020 2020 2020 2020 2020 2022 7b25  .            "{%
-0000c1a0: 737d 7265 7370 7472 2220 2520 786d 6c5f  s}resptr" % xml_
-0000c1b0: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
-0000c1c0: 6e65 5d2c 0a20 2020 2020 2020 2020 2020  ne],.           
-0000c1d0: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
-0000c1e0: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
-0000c1f0: 7970 655d 0a20 2020 2020 2020 2020 2020  ype].           
-0000c200: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-0000c210: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
-0000c220: 2020 290a 2020 2020 2020 2020 7661 6c75    ).        valu
-0000c230: 655f 2e74 6578 7420 3d20 7374 7228 7661  e_.text = str(va
-0000c240: 6c2e 7661 6c75 6529 0a20 2020 2020 2020  l.value).       
-0000c250: 2070 726f 705f 2e61 7070 656e 6428 7661   prop_.append(va
-0000c260: 6c75 655f 290a 0a20 2020 2072 6574 7572  lue_)..    retur
-0000c270: 6e20 7072 6f70 5f0a 0a0a 6465 6620 6d61  n prop_...def ma
-0000c280: 6b65 5f74 6578 745f 7072 6f70 280a 2020  ke_text_prop(.  
-0000c290: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
-0000c2a0: 2076 616c 7565 3a20 556e 696f 6e5b 5072   value: Union[Pr
-0000c2b0: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-0000c2c0: 7472 2c20 4974 6572 6162 6c65 5b55 6e69  tr, Iterable[Uni
-0000c2d0: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
-0000c2e0: 6e74 2c20 7374 725d 5d5d 2c0a 2020 2020  nt, str]]],.    
-0000c2f0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-0000c300: 3a20 7374 7220 3d20 2222 2c0a 2920 2d3e  : str = "",.) ->
-0000c310: 2065 7472 6565 2e5f 456c 656d 656e 743a   etree._Element:
-0000c320: 0a20 2020 2022 2222 0a20 2020 204d 616b  .    """.    Mak
-0000c330: 6520 6120 3c74 6578 742d 7072 6f70 3e20  e a <text-prop> 
-0000c340: 6672 6f6d 206f 6e65 206f 7220 6d6f 7265  from one or more
-0000c350: 2073 7472 696e 6773 2e20 5468 6520 7374   strings. The st
-0000c360: 7269 6e67 2873 2920 6361 6e20 6265 2070  ring(s) can be p
-0000c370: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
-0000c380: 6720 6f72 2061 7320 5072 6f70 6572 7479  g or as Property
-0000c390: 456c 656d 656e 7420 7769 7468 2061 0a20  Element with a. 
-0000c3a0: 2020 2073 7472 696e 6720 696e 7369 6465     string inside
-0000c3b0: 2e20 4966 2070 726f 7669 6465 6420 6173  . If provided as
-0000c3c0: 2073 7472 696e 672c 2074 6865 2065 6e63   string, the enc
-0000c3d0: 6f64 696e 6720 6465 6661 756c 7473 2074  oding defaults t
-0000c3e0: 6f20 7574 6638 2c20 616e 6420 7468 6520  o utf8, and the 
-0000c3f0: 7065 726d 6973 7369 6f6e 7320 746f 2022  permissions to "
-0000c400: 7072 6f70 2d64 6566 6175 6c74 222e 0a0a  prop-default"...
-0000c410: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000c420: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
-0000c430: 206f 6620 7468 6973 2070 726f 7065 7274   of this propert
-0000c440: 7920 6173 2064 6566 696e 6564 2069 6e20  y as defined in 
-0000c450: 7468 6520 6f6e 746f 0a20 2020 2020 2020  the onto.       
-0000c460: 2076 616c 7565 3a20 6f6e 6520 6f72 206d   value: one or m
-0000c470: 6f72 6520 7374 7269 6e67 732c 2061 7320  ore strings, as 
-0000c480: 7374 7269 6e67 2f50 726f 7065 7274 7945  string/PropertyE
-0000c490: 6c65 6d65 6e74 2c20 6f72 2061 7320 6974  lement, or as it
-0000c4a0: 6572 6162 6c65 206f 6620 7374 7269 6e67  erable of string
-0000c4b0: 732f 5072 6f70 6572 7479 456c 656d 656e  s/PropertyElemen
-0000c4c0: 7473 0a20 2020 2020 2020 2063 616c 6c69  ts.        calli
-0000c4d0: 6e67 5f72 6573 6f75 7263 653a 2074 6865  ng_resource: the
-0000c4e0: 206e 616d 6520 6f66 2074 6865 2070 6172   name of the par
-0000c4f0: 656e 7420 7265 736f 7572 6365 2028 666f  ent resource (fo
-0000c500: 7220 6265 7474 6572 2065 7272 6f72 206d  r better error m
-0000c510: 6573 7361 6765 7329 0a0a 2020 2020 5261  essages)..    Ra
-0000c520: 6973 6573 3a0a 2020 2020 2020 2020 4261  ises:.        Ba
-0000c530: 7365 4572 726f 723a 2069 6620 6f6e 6520  seError: if one 
-0000c540: 6f66 2074 6865 2076 616c 7565 7320 6973  of the values is
-0000c550: 206e 6f74 2061 2076 616c 6964 2073 7472   not a valid str
-0000c560: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-0000c570: 206f 7220 6966 2074 6865 2058 4d4c 2074   or if the XML t
-0000c580: 6167 7320 696e 2061 2072 6963 6874 6578  ags in a richtex
-0000c590: 7420 7072 6f70 6572 7479 2028 656e 636f  t property (enco
-0000c5a0: 6469 6e67 3d78 6d6c 2920 6172 6520 6e6f  ding=xml) are no
-0000c5b0: 7420 7765 6c6c 2d66 6f72 6d65 640a 2020  t well-formed.  
-0000c5c0: 2020 2020 2020 5761 726e 696e 673a 2069        Warning: i
-0000c5d0: 6620 6f6e 6520 6f66 2074 6865 2076 616c  f one of the val
-0000c5e0: 7565 7320 646f 6573 6e27 7420 6c6f 6f6b  ues doesn't look
-0000c5f0: 206c 696b 6520 6120 7265 6173 6f6e 6162   like a reasonab
-0000c600: 6c65 2073 7472 696e 670a 2020 2020 2020  le string.      
-0000c610: 2020 2020 2020 2865 2e67 2e20 223c 4e41        (e.g. "<NA
-0000c620: 3e22 2069 7320 6120 7661 6c69 6420 7374  >" is a valid st
-0000c630: 7269 6e67 2c20 6275 7420 7072 6f62 6162  ring, but probab
-0000c640: 6c79 206e 6f74 2069 6e74 656e 6465 6429  ly not intended)
-0000c650: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000c660: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
-0000c670: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
-0000c680: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
-0000c690: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-0000c6a0: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
-0000c6b0: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
-0000c6c0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
-0000c6d0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-0000c6e0: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000c6f0: 2e6d 616b 655f 7465 7874 5f70 726f 7028  .make_text_prop(
-0000c700: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-0000c710: 2022 6669 7273 7420 7465 7874 2229 0a20   "first text"). 
-0000c720: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000c730: 7465 7874 2d70 726f 7020 6e61 6d65 3d22  text-prop name="
-0000c740: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c760: 2020 2020 3c74 6578 7420 656e 636f 6469      <text encodi
-0000c770: 6e67 3d22 7574 6638 2220 7065 726d 6973  ng="utf8" permis
-0000c780: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
-0000c790: 756c 7422 3e66 6972 7374 2074 6578 743c  ult">first text<
-0000c7a0: 2f74 6578 743e 0a20 2020 2020 2020 2020  /text>.         
-0000c7b0: 2020 2020 2020 203c 2f74 6578 742d 7072         </text-pr
-0000c7c0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
-0000c7d0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f74  excel2xml.make_t
-0000c7e0: 6578 745f 7072 6f70 2822 3a74 6573 7470  ext_prop(":testp
-0000c7f0: 726f 7065 7274 7922 2c20 6578 6365 6c32  roperty", excel2
-0000c800: 786d 6c2e 5072 6f70 6572 7479 456c 656d  xml.PropertyElem
-0000c810: 656e 7428 2266 6972 7374 2074 6578 7422  ent("first text"
-0000c820: 2c20 7065 726d 6973 7369 6f6e 733d 2270  , permissions="p
-0000c830: 726f 702d 7265 7374 7269 6374 6564 222c  rop-restricted",
-0000c840: 2065 6e63 6f64 696e 673d 2278 6d6c 2229   encoding="xml")
-0000c850: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c860: 2020 3c74 6578 742d 7072 6f70 206e 616d    <text-prop nam
-0000c870: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
-0000c880: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-0000c890: 2020 2020 2020 203c 7465 7874 2065 6e63         <text enc
-0000c8a0: 6f64 696e 673d 2278 6d6c 2220 7065 726d  oding="xml" perm
-0000c8b0: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-0000c8c0: 7374 7269 6374 6564 223e 6669 7273 7420  stricted">first 
-0000c8d0: 7465 7874 3c2f 7465 7874 3e0a 2020 2020  text</text>.    
-0000c8e0: 2020 2020 2020 2020 2020 2020 3c2f 7465              </te
-0000c8f0: 7874 2d70 726f 703e 0a20 2020 2020 2020  xt-prop>.       
-0000c900: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-0000c910: 616b 655f 7465 7874 5f70 726f 7028 223a  ake_text_prop(":
-0000c920: 7465 7374 7072 6f70 6572 7479 222c 205b  testproperty", [
-0000c930: 2266 6972 7374 2074 6578 7422 2c20 2273  "first text", "s
-0000c940: 6563 6f6e 6420 7465 7874 225d 290a 2020  econd text"]).  
-0000c950: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-0000c960: 6578 742d 7072 6f70 206e 616d 653d 223a  ext-prop name=":
-0000c970: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c990: 2020 203c 7465 7874 2065 6e63 6f64 696e     <text encodin
-0000c9a0: 673d 2275 7466 3822 2070 6572 6d69 7373  g="utf8" permiss
-0000c9b0: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-0000c9c0: 6c74 223e 6669 7273 7420 7465 7874 3c2f  lt">first text</
-0000c9d0: 7465 7874 3e0a 2020 2020 2020 2020 2020  text>.          
-0000c9e0: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
-0000c9f0: 656e 636f 6469 6e67 3d22 7574 6638 2220  encoding="utf8" 
-0000ca00: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-0000ca10: 702d 6465 6661 756c 7422 3e73 6563 6f6e  p-default">secon
-0000ca20: 6420 7465 7874 3c2f 7465 7874 3e0a 2020  d text</text>.  
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0000ca40: 7465 7874 2d70 726f 703e 0a0a 2020 2020  text-prop>..    
-0000ca50: 5365 6520 6874 7470 733a 2f2f 646f 6373  See https://docs
-0000ca60: 2e64 6173 6368 2e73 7769 7373 2f6c 6174  .dasch.swiss/lat
-0000ca70: 6573 742f 4453 502d 544f 4f4c 532f 6669  est/DSP-TOOLS/fi
-0000ca80: 6c65 2d66 6f72 6d61 7473 2f78 6d6c 2d64  le-formats/xml-d
-0000ca90: 6174 612d 6669 6c65 2f23 7465 7874 2d70  ata-file/#text-p
-0000caa0: 726f 700a 2020 2020 2222 220a 0a20 2020  rop.    """..   
-0000cab0: 2023 2063 6865 636b 2074 6865 2069 6e70   # check the inp
-0000cac0: 7574 3a20 7072 6570 6172 6520 6120 6c69  ut: prepare a li
-0000cad0: 7374 2077 6974 6820 7661 6c69 6420 7661  st with valid va
-0000cae0: 6c75 6573 0a20 2020 2076 616c 7565 7320  lues.    values 
-0000caf0: 3d20 7072 6570 6172 655f 7661 6c75 6528  = prepare_value(
-0000cb00: 7661 6c75 6529 0a0a 2020 2020 2320 6368  value)..    # ch
-0000cb10: 6563 6b20 7661 6c75 6520 7479 7065 0a20  eck value type. 
-0000cb20: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
-0000cb30: 6c75 6573 3a0a 2020 2020 2020 2020 6966  lues:.        if
-0000cb40: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0000cb50: 7661 6c2e 7661 6c75 652c 2073 7472 2920  val.value, str) 
-0000cb60: 6f72 206c 656e 2876 616c 2e76 616c 7565  or len(val.value
-0000cb70: 2920 3c20 313a 0a20 2020 2020 2020 2020  ) < 1:.         
-0000cb80: 2020 2072 6169 7365 2042 6173 6545 7272     raise BaseErr
-0000cb90: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000cba0: 2020 2020 6622 4661 696c 6564 2076 616c      f"Failed val
-0000cbb0: 6964 6174 696f 6e20 696e 2072 6573 6f75  idation in resou
-0000cbc0: 7263 6520 277b 6361 6c6c 696e 675f 7265  rce '{calling_re
-0000cbd0: 736f 7572 6365 7d27 2c20 7072 6f70 6572  source}', proper
-0000cbe0: 7479 2027 7b6e 616d 657d 273a 2022 0a20  ty '{name}': ". 
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000cc00: 2227 7b76 616c 2e76 616c 7565 7d27 2069  "'{val.value}' i
-0000cc10: 7320 6e6f 7420 6120 7661 6c69 6420 7374  s not a valid st
-0000cc20: 7269 6e67 2e22 0a20 2020 2020 2020 2020  ring.".         
-0000cc30: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-0000cc40: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
-0000cc50: 7661 6c2e 7661 6c75 6529 3a0a 2020 2020  val.value):.    
-0000cc60: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0000cc70: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-0000cc80: 2020 2020 2020 2066 2257 6172 6e69 6e67         f"Warning
-0000cc90: 2066 6f72 2072 6573 6f75 7263 6520 277b   for resource '{
-0000cca0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-0000ccb0: 7d27 2c20 7072 6f70 6572 7479 2027 7b6e  }', property '{n
-0000ccc0: 616d 657d 273a 2022 0a20 2020 2020 2020  ame}': ".       
-0000ccd0: 2020 2020 2020 2020 2066 2227 7b76 616c           f"'{val
-0000cce0: 2e76 616c 7565 7d27 2069 7320 7072 6f62  .value}' is prob
-0000ccf0: 6162 6c79 206e 6f74 2061 2075 7361 626c  ably not a usabl
-0000cd00: 6520 7374 7269 6e67 2e22 2c0a 2020 2020  e string.",.    
-0000cd10: 2020 2020 2020 2020 2020 2020 7374 6163              stac
-0000cd20: 6b6c 6576 656c 3d32 2c0a 2020 2020 2020  klevel=2,.      
-0000cd30: 2020 2020 2020 290a 0a20 2020 2023 206d        )..    # m
-0000cd40: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
-0000cd50: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
-0000cd60: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
-0000cd70: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-0000cd80: 0a20 2020 2020 2020 2022 7b25 737d 7465  .        "{%s}te
-0000cd90: 7874 2d70 726f 7022 2025 2078 6d6c 5f6e  xt-prop" % xml_n
-0000cda0: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-0000cdb0: 655d 2c0a 2020 2020 2020 2020 6e61 6d65  e],.        name
-0000cdc0: 3d6e 616d 652c 0a20 2020 2020 2020 206e  =name,.        n
-0000cdd0: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
-0000cde0: 6365 5f6d 6170 2c0a 2020 2020 290a 2020  ce_map,.    ).  
-0000cdf0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
-0000ce00: 7565 733a 0a20 2020 2020 2020 206b 7761  ues:.        kwa
-0000ce10: 7267 7320 3d20 7b22 7065 726d 6973 7369  rgs = {"permissi
-0000ce20: 6f6e 7322 3a20 7661 6c2e 7065 726d 6973  ons": val.permis
-0000ce30: 7369 6f6e 737d 0a20 2020 2020 2020 2069  sions}.        i
-0000ce40: 6620 6368 6563 6b5f 6e6f 746e 6128 7661  f check_notna(va
-0000ce50: 6c2e 636f 6d6d 656e 7429 3a0a 2020 2020  l.comment):.    
-0000ce60: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-0000ce70: 636f 6d6d 656e 7422 5d20 3d20 7661 6c2e  comment"] = val.
-0000ce80: 636f 6d6d 656e 740a 2020 2020 2020 2020  comment.        
-0000ce90: 6b77 6172 6773 5b22 656e 636f 6469 6e67  kwargs["encoding
-0000cea0: 225d 203d 2076 616c 2e65 6e63 6f64 696e  "] = val.encodin
-0000ceb0: 6720 6966 2063 6865 636b 5f6e 6f74 6e61  g if check_notna
-0000cec0: 2876 616c 2e65 6e63 6f64 696e 6729 2065  (val.encoding) e
-0000ced0: 6c73 6520 2275 7466 3822 0a20 2020 2020  lse "utf8".     
-0000cee0: 2020 2076 616c 7565 5f20 3d20 6574 7265     value_ = etre
-0000cef0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
-0000cf00: 2020 2020 2020 2022 7b25 737d 7465 7874         "{%s}text
-0000cf10: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000cf20: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000cf30: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-0000cf40: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-0000cf50: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-0000cf60: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
-0000cf70: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-0000cf80: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-0000cf90: 2020 2020 6966 206b 7761 7267 735b 2265      if kwargs["e
-0000cfa0: 6e63 6f64 696e 6722 5d20 3d3d 2022 7574  ncoding"] == "ut
-0000cfb0: 6638 223a 0a20 2020 2020 2020 2020 2020  f8":.           
-0000cfc0: 2023 2077 7269 7465 2074 6865 2074 6578   # write the tex
-0000cfd0: 7420 696e 746f 2074 6865 2074 6167 2c20  t into the tag, 
-0000cfe0: 7769 7468 6f75 7420 7661 6c69 6461 7469  without validati
-0000cff0: 6f6e 0a20 2020 2020 2020 2020 2020 2076  on.            v
-0000d000: 616c 7565 5f2e 7465 7874 203d 2073 7472  alue_.text = str
-0000d010: 2876 616c 2e76 616c 7565 290a 2020 2020  (val.value).    
-0000d020: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d030: 2020 2020 2020 6573 6361 7065 645f 7465        escaped_te
-0000d040: 7874 203d 205f 6573 6361 7065 5f72 6573  xt = _escape_res
-0000d050: 6572 7665 645f 6368 6172 7328 7374 7228  erved_chars(str(
-0000d060: 7661 6c2e 7661 6c75 6529 290a 2020 2020  val.value)).    
-0000d070: 2020 2020 2020 2020 2320 656e 666f 7263          # enforc
-0000d080: 6520 7468 6174 2074 6865 2074 6578 7420  e that the text 
-0000d090: 6973 2077 656c 6c2d 666f 726d 6564 2058  is well-formed X
-0000d0a0: 4d4c 3a20 7365 7269 616c 697a 6520 7461  ML: serialize ta
-0000d0b0: 6720 2e2e 2e0a 2020 2020 2020 2020 2020  g ....          
-0000d0c0: 2020 7365 7269 616c 697a 6564 203d 2065    serialized = e
-0000d0d0: 7472 6565 2e74 6f73 7472 696e 6728 7661  tree.tostring(va
-0000d0e0: 6c75 655f 2c20 656e 636f 6469 6e67 3d22  lue_, encoding="
-0000d0f0: 756e 6963 6f64 6522 290a 2020 2020 2020  unicode").      
-0000d100: 2020 2020 2020 2320 2e2e 2e20 696e 7365        # ... inse
-0000d110: 7274 2074 6578 7420 6174 2074 6865 2076  rt text at the v
-0000d120: 6572 7920 656e 6420 6f66 2074 6865 2073  ery end of the s
-0000d130: 7472 696e 672c 2061 6e64 2061 6464 2065  tring, and add e
-0000d140: 6e64 696e 6720 7461 6720 746f 2074 6865  nding tag to the
-0000d150: 2070 7265 7669 6f75 736c 7920 7369 6e67   previously sing
-0000d160: 6c65 203c 7465 7874 2f3e 2074 6167 202e  le <text/> tag .
-0000d170: 2e2e 0a20 2020 2020 2020 2020 2020 2073  ...            s
-0000d180: 6572 6961 6c69 7a65 6420 3d20 7265 6765  erialized = rege
-0000d190: 782e 7375 6228 7222 2f3e 2422 2c20 6622  x.sub(r"/>$", f"
-0000d1a0: 3e7b 6573 6361 7065 645f 7465 7874 7d3c  >{escaped_text}<
-0000d1b0: 2f74 6578 743e 222c 2073 6572 6961 6c69  /text>", seriali
-0000d1c0: 7a65 6429 0a20 2020 2020 2020 2020 2020  zed).           
-0000d1d0: 2023 202e 2e2e 2074 7279 2074 6f20 7061   # ... try to pa
-0000d1e0: 7273 6520 6974 2061 6761 696e 0a20 2020  rse it again.   
-0000d1f0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0000d200: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0000d210: 6c75 655f 203d 2065 7472 6565 2e66 726f  lue_ = etree.fro
-0000d220: 6d73 7472 696e 6728 7365 7269 616c 697a  mstring(serializ
-0000d230: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-0000d240: 6578 6365 7074 2065 7472 6565 2e58 4d4c  except etree.XML
-0000d250: 5379 6e74 6178 4572 726f 7220 6173 2065  SyntaxError as e
-0000d260: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
-0000d270: 2020 2020 6d73 6720 3d20 280a 2020 2020      msg = (.    
-0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d290: 2254 6865 2058 4d4c 2074 6167 7320 636f  "The XML tags co
-0000d2a0: 6e74 6169 6e65 6420 696e 2061 2072 6963  ntained in a ric
-0000d2b0: 6874 6578 7420 7072 6f70 6572 7479 2028  htext property (
-0000d2c0: 656e 636f 6469 6e67 3d78 6d6c 2920 6d75  encoding=xml) mu
-0000d2d0: 7374 2062 6520 7765 6c6c 2d66 6f72 6d65  st be well-forme
-0000d2e0: 642e 2022 0a20 2020 2020 2020 2020 2020  d. ".           
-0000d2f0: 2020 2020 2020 2020 2022 5468 6520 7370           "The sp
-0000d300: 6563 6961 6c20 6368 6172 6163 7465 7273  ecial characters
-0000d310: 203c 2c20 3e20 616e 6420 2620 6172 6520   <, > and & are 
-0000d320: 6f6e 6c79 2061 6c6c 6f77 6564 2074 6f20  only allowed to 
-0000d330: 636f 6e73 7472 7563 7420 6120 7461 672e  construct a tag.
-0000d340: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000d350: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d360: 2020 2020 2069 6620 6361 6c6c 696e 675f       if calling_
-0000d370: 7265 736f 7572 6365 3a0a 2020 2020 2020  resource:.      
-0000d380: 2020 2020 2020 2020 2020 2020 2020 6d73                ms
-0000d390: 6720 2b3d 2066 2254 6865 2065 7272 6f72  g += f"The error
-0000d3a0: 206f 6363 7572 7265 6420 696e 2072 6573   occurred in res
-0000d3b0: 6f75 7263 6520 7b63 616c 6c69 6e67 5f72  ource {calling_r
-0000d3c0: 6573 6f75 7263 657d 2c20 7072 6f70 6572  esource}, proper
-0000d3d0: 7479 207b 6e61 6d65 7d22 0a20 2020 2020  ty {name}".     
-0000d3e0: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
-0000d3f0: 3d20 6622 5c6e 4f72 6967 696e 616c 2065  = f"\nOriginal e
-0000d400: 7272 6f72 206d 6573 7361 6765 3a20 7b65  rror message: {e
-0000d410: 7272 2e6d 7367 7d22 0a20 2020 2020 2020  rr.msg}".       
-0000d420: 2020 2020 2020 2020 206d 7367 202b 3d20           msg += 
-0000d430: 6622 5c6e 4576 656e 7475 616c 206c 696e  f"\nEventual lin
-0000d440: 652f 636f 6c75 6d6e 206e 756d 6265 7273  e/column numbers
-0000d450: 2061 7265 2072 656c 6174 6976 6520 746f   are relative to
-0000d460: 2074 6869 7320 7365 7269 616c 697a 6564   this serialized
-0000d470: 2074 6578 743a 207b 7365 7269 616c 697a   text: {serializ
-0000d480: 6564 7d22 0a20 2020 2020 2020 2020 2020  ed}".           
-0000d490: 2020 2020 2072 6169 7365 2042 6173 6545       raise BaseE
-0000d4a0: 7272 6f72 286d 7367 2920 6672 6f6d 204e  rror(msg) from N
-0000d4b0: 6f6e 650a 2020 2020 2020 2020 7072 6f70  one.        prop
-0000d4c0: 5f2e 6170 7065 6e64 2876 616c 7565 5f29  _.append(value_)
-0000d4d0: 0a0a 2020 2020 7265 7475 726e 2070 726f  ..    return pro
-0000d4e0: 705f 0a0a 0a64 6566 205f 6573 6361 7065  p_...def _escape
-0000d4f0: 5f72 6573 6572 7665 645f 6368 6172 7328  _reserved_chars(
-0000d500: 7465 7874 3a20 7374 7229 202d 3e20 7374  text: str) -> st
-0000d510: 723a 0a20 2020 2022 2222 0a20 2020 2046  r:.    """.    F
-0000d520: 726f 6d20 7269 6368 7465 7874 2073 7472  rom richtext str
-0000d530: 696e 6773 2028 656e 636f 6469 6e67 3d22  ings (encoding="
-0000d540: 786d 6c22 292c 2065 7363 6170 6520 7468  xml"), escape th
-0000d550: 6520 7265 7365 7276 6564 2063 6861 7261  e reserved chara
-0000d560: 6374 6572 7320 3c2c 203e 2061 6e64 2026  cters <, > and &
-0000d570: 2c0a 2020 2020 6275 7420 6f6e 6c79 2069  ,.    but only i
-0000d580: 6620 7468 6579 2061 7265 206e 6f74 2070  f they are not p
-0000d590: 6172 7420 6f66 2061 2073 7461 6e64 6172  art of a standar
-0000d5a0: 6420 7374 616e 646f 6666 2074 6167 206f  d standoff tag o
-0000d5b0: 7220 6573 6361 7065 2073 6571 7565 6e63  r escape sequenc
-0000d5c0: 652e 0a20 2020 2054 6865 2073 7461 6e64  e..    The stand
-0000d5d0: 6172 6420 7374 616e 646f 6666 2074 6167  ard standoff tag
-0000d5e0: 7320 616c 6c6f 7765 6420 6279 2044 5350  s allowed by DSP
-0000d5f0: 2d41 5049 2061 7265 2064 6f63 756d 656e  -API are documen
-0000d600: 7465 6420 6865 7265 3a0a 2020 2020 6874  ted here:.    ht
-0000d610: 7470 733a 2f2f 646f 6373 2e64 6173 6368  tps://docs.dasch
-0000d620: 2e73 7769 7373 2f32 3032 332e 3132 2e30  .swiss/2023.12.0
-0000d630: 312f 4453 502d 4150 492f 3033 2d65 6e64  1/DSP-API/03-end
-0000d640: 706f 696e 7473 2f61 7069 2d76 322f 7465  points/api-v2/te
-0000d650: 7874 2f73 7461 6e64 6172 642d 7374 616e  xt/standard-stan
-0000d660: 646f 6666 2f0a 0a20 2020 2041 7267 733a  doff/..    Args:
-0000d670: 0a20 2020 2020 2020 2074 6578 743a 2074  .        text: t
-0000d680: 6865 2072 6963 6874 6578 7420 7374 7269  he richtext stri
-0000d690: 6e67 2074 6f20 6265 2065 7363 6170 6564  ng to be escaped
-0000d6a0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000d6b0: 2020 2020 2020 2074 6865 2065 7363 6170         the escap
-0000d6c0: 6564 2072 6963 6874 6578 7420 7374 7269  ed richtext stri
-0000d6d0: 6e67 0a20 2020 2022 2222 0a20 2020 2061  ng.    """.    a
-0000d6e0: 6c6c 6f77 6564 5f74 6167 7320 3d20 5b0a  llowed_tags = [.
-0000d6f0: 2020 2020 2020 2020 2261 2820 5b5e 3e5d          "a( [^>]
-0000d700: 2b29 3f22 2c20 2023 203c 613e 2069 7320  +)?",  # <a> is 
-0000d710: 7468 6520 6f6e 6c79 2074 6167 2074 6861  the only tag tha
-0000d720: 7420 6361 6e20 6861 7665 2061 7474 7269  t can have attri
-0000d730: 6275 7465 730a 2020 2020 2020 2020 2270  butes.        "p
-0000d740: 222c 0a20 2020 2020 2020 2022 656d 222c  ",.        "em",
-0000d750: 0a20 2020 2020 2020 2022 7374 726f 6e67  .        "strong
-0000d760: 222c 0a20 2020 2020 2020 2022 7522 2c0a  ",.        "u",.
-0000d770: 2020 2020 2020 2020 2273 7562 222c 0a20          "sub",. 
-0000d780: 2020 2020 2020 2022 7375 7022 2c0a 2020         "sup",.  
-0000d790: 2020 2020 2020 2273 7472 696b 6522 2c0a        "strike",.
-0000d7a0: 2020 2020 2020 2020 2268 3122 2c0a 2020          "h1",.  
-0000d7b0: 2020 2020 2020 226f 6c22 2c0a 2020 2020        "ol",.    
-0000d7c0: 2020 2020 2275 6c22 2c0a 2020 2020 2020      "ul",.      
-0000d7d0: 2020 226c 6922 2c0a 2020 2020 2020 2020    "li",.        
-0000d7e0: 2274 626f 6479 222c 0a20 2020 2020 2020  "tbody",.       
-0000d7f0: 2022 7461 626c 6522 2c0a 2020 2020 2020   "table",.      
-0000d800: 2020 2274 7222 2c0a 2020 2020 2020 2020    "tr",.        
-0000d810: 2274 6422 2c0a 2020 2020 2020 2020 2262  "td",.        "b
-0000d820: 7222 2c0a 2020 2020 2020 2020 2268 7222  r",.        "hr"
-0000d830: 2c0a 2020 2020 2020 2020 2270 7265 222c  ,.        "pre",
-0000d840: 0a20 2020 2020 2020 2022 6369 7465 222c  .        "cite",
-0000d850: 0a20 2020 2020 2020 2022 626c 6f63 6b71  .        "blockq
-0000d860: 756f 7465 222c 0a20 2020 2020 2020 2022  uote",.        "
-0000d870: 636f 6465 222c 0a20 2020 205d 0a20 2020  code",.    ].   
-0000d880: 2061 6c6c 6f77 6564 5f74 6167 735f 7265   allowed_tags_re
-0000d890: 6765 7820 3d20 227c 222e 6a6f 696e 2861  gex = "|".join(a
-0000d8a0: 6c6c 6f77 6564 5f74 6167 7329 0a20 2020  llowed_tags).   
-0000d8b0: 206c 6f6f 6b61 6865 6164 203d 2072 6622   lookahead = rf"
-0000d8c0: 283f 212f 3f28 7b61 6c6c 6f77 6564 5f74  (?!/?({allowed_t
-0000d8d0: 6167 735f 7265 6765 787d 292f 3f3e 2922  ags_regex})/?>)"
-0000d8e0: 0a20 2020 2069 6c6c 6567 616c 5f6c 7420  .    illegal_lt 
-0000d8f0: 3d20 7266 223c 7b6c 6f6f 6b61 6865 6164  = rf"<{lookahead
-0000d900: 7d22 0a20 2020 206c 6f6f 6b62 6568 696e  }".    lookbehin
-0000d910: 6420 3d20 7266 2228 3f3c 213c 2f3f 287b  d = rf"(?<!</?({
-0000d920: 616c 6c6f 7765 645f 7461 6773 5f72 6567  allowed_tags_reg
-0000d930: 6578 7d29 2f3f 2922 0a20 2020 2069 6c6c  ex})/?)".    ill
-0000d940: 6567 616c 5f67 7420 3d20 7266 227b 6c6f  egal_gt = rf"{lo
-0000d950: 6f6b 6265 6869 6e64 7d3e 220a 2020 2020  okbehind}>".    
-0000d960: 696c 6c65 6761 6c5f 616d 7020 3d20 7222  illegal_amp = r"
-0000d970: 2628 3f21 5b23 612d 7a41 2d5a 302d 395d  &(?![#a-zA-Z0-9]
-0000d980: 2b3b 2922 0a20 2020 2074 6578 7420 3d20  +;)".    text = 
-0000d990: 7265 6765 782e 7375 6228 696c 6c65 6761  regex.sub(illega
-0000d9a0: 6c5f 6c74 2c20 2226 6c74 3b22 2c20 7465  l_lt, "&lt;", te
-0000d9b0: 7874 290a 2020 2020 7465 7874 203d 2072  xt).    text = r
-0000d9c0: 6567 6578 2e73 7562 2869 6c6c 6567 616c  egex.sub(illegal
-0000d9d0: 5f67 742c 2022 2667 743b 222c 2074 6578  _gt, "&gt;", tex
-0000d9e0: 7429 0a20 2020 2074 6578 7420 3d20 7265  t).    text = re
-0000d9f0: 6765 782e 7375 6228 696c 6c65 6761 6c5f  gex.sub(illegal_
-0000da00: 616d 702c 2022 2661 6d70 3b22 2c20 7465  amp, "&amp;", te
-0000da10: 7874 290a 2020 2020 7265 7475 726e 2074  xt).    return t
-0000da20: 6578 740a 0a0a 6465 6620 6d61 6b65 5f74  ext...def make_t
-0000da30: 696d 655f 7072 6f70 280a 2020 2020 6e61  ime_prop(.    na
-0000da40: 6d65 3a20 7374 722c 0a20 2020 2076 616c  me: str,.    val
-0000da50: 7565 3a20 556e 696f 6e5b 5072 6f70 6572  ue: Union[Proper
-0000da60: 7479 456c 656d 656e 742c 2073 7472 2c20  tyElement, str, 
-0000da70: 4974 6572 6162 6c65 5b55 6e69 6f6e 5b50  Iterable[Union[P
-0000da80: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-0000da90: 7374 725d 5d5d 2c0a 2020 2020 6361 6c6c  str]]],.    call
-0000daa0: 696e 675f 7265 736f 7572 6365 3a20 7374  ing_resource: st
-0000dab0: 7220 3d20 2222 2c0a 2920 2d3e 2065 7472  r = "",.) -> etr
-0000dac0: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-0000dad0: 2022 2222 0a20 2020 204d 616b 6520 6120   """.    Make a 
-0000dae0: 3c74 696d 652d 7072 6f70 3e20 6672 6f6d  <time-prop> from
-0000daf0: 206f 6e65 206f 7220 6d6f 7265 2064 6174   one or more dat
-0000db00: 6574 696d 6520 7661 6c75 6573 206f 6620  etime values of 
-0000db10: 7468 6520 666f 726d 2022 3230 3039 2d31  the form "2009-1
-0000db20: 302d 3130 5431 323a 3030 3a30 302d 3035  0-10T12:00:00-05
-0000db30: 3a30 3022 2e20 5468 6520 7469 6d65 2873  :00". The time(s
-0000db40: 2920 6361 6e20 6265 0a20 2020 2070 726f  ) can be.    pro
-0000db50: 7669 6465 6420 6173 2073 7472 696e 6720  vided as string 
-0000db60: 6f72 2061 7320 5072 6f70 6572 7479 456c  or as PropertyEl
-0000db70: 656d 656e 7420 7769 7468 2061 2073 7472  ement with a str
-0000db80: 696e 6720 696e 7369 6465 2e20 4966 2070  ing inside. If p
-0000db90: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
-0000dba0: 672c 2074 6865 2070 6572 6d69 7373 696f  g, the permissio
-0000dbb0: 6e73 2064 6566 6175 6c74 2074 6f0a 2020  ns default to.  
-0000dbc0: 2020 2270 726f 702d 6465 6661 756c 7422    "prop-default"
-0000dbd0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000dbe0: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-0000dbf0: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-0000dc00: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
-0000dc10: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
-0000dc20: 2020 2020 7661 6c75 653a 206f 6e65 206f      value: one o
-0000dc30: 7220 6d6f 7265 2044 5350 2074 696d 6573  r more DSP times
-0000dc40: 2c20 6173 2073 7472 696e 672f 5072 6f70  , as string/Prop
-0000dc50: 6572 7479 456c 656d 656e 742c 206f 7220  ertyElement, or 
-0000dc60: 6173 2069 7465 7261 626c 6520 6f66 2073  as iterable of s
-0000dc70: 7472 696e 6773 2f50 726f 7065 7274 7945  trings/PropertyE
-0000dc80: 6c65 6d65 6e74 730a 2020 2020 2020 2020  lements.        
-0000dc90: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-0000dca0: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-0000dcb0: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-0000dcc0: 6520 2866 6f72 2062 6574 7465 7220 6572  e (for better er
-0000dcd0: 726f 7220 6d65 7373 6167 6573 290a 0a20  ror messages).. 
-0000dce0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-0000dcf0: 2020 2042 6173 6545 7272 6f72 3a20 4966     BaseError: If
-0000dd00: 206f 6e65 206f 6620 7468 6520 7661 6c75   one of the valu
-0000dd10: 6573 2069 7320 6e6f 7420 6120 7661 6c69  es is not a vali
-0000dd20: 6420 4453 5020 7469 6d65 2073 7472 696e  d DSP time strin
-0000dd30: 670a 0a20 2020 2052 6574 7572 6e73 3a0a  g..    Returns:.
-0000dd40: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
-0000dd50: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
-0000dd60: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
-0000dd70: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
-0000dd80: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
-0000dd90: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
-0000dda0: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
-0000ddb0: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
-0000ddc0: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
-0000ddd0: 6c2e 6d61 6b65 5f74 696d 655f 7072 6f70  l.make_time_prop
-0000dde0: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-0000ddf0: 2c20 2232 3030 392d 3130 2d31 3054 3132  , "2009-10-10T12
-0000de00: 3a30 303a 3030 2d30 353a 3030 2229 0a20  :00:00-05:00"). 
-0000de10: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000de20: 7469 6d65 2d70 726f 7020 6e61 6d65 3d22  time-prop name="
-0000de30: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-0000de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de50: 2020 2020 3c74 696d 6520 7065 726d 6973      <time permis
-0000de60: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
-0000de70: 756c 7422 3e0a 2020 2020 2020 2020 2020  ult">.          
-0000de80: 2020 2020 2020 2020 2020 2020 2020 3230                20
-0000de90: 3039 2d31 302d 3130 5431 323a 3030 3a30  09-10-10T12:00:0
-0000dea0: 302d 3035 3a30 300a 2020 2020 2020 2020  0-05:00.        
-0000deb0: 2020 2020 2020 2020 2020 2020 3c2f 7469              </ti
-0000dec0: 6d65 3e0a 2020 2020 2020 2020 2020 2020  me>.            
-0000ded0: 2020 2020 3c2f 7469 6d65 2d70 726f 703e      </time-prop>
-0000dee0: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
-0000def0: 656c 3278 6d6c 2e6d 616b 655f 7469 6d65  el2xml.make_time
-0000df00: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
-0000df10: 6572 7479 222c 2065 7863 656c 3278 6d6c  erty", excel2xml
-0000df20: 2e50 726f 7065 7274 7945 6c65 6d65 6e74  .PropertyElement
-0000df30: 2822 3230 3039 2d31 302d 3130 5431 323a  ("2009-10-10T12:
-0000df40: 3030 3a30 302d 3035 3a30 3022 2c20 7065  00:00-05:00", pe
-0000df50: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000df60: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
-0000df70: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
-0000df80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df90: 203c 7469 6d65 2d70 726f 7020 6e61 6d65   <time-prop name
-0000dfa0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-0000dfb0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000dfc0: 2020 2020 2020 3c74 696d 6520 7065 726d        <time perm
-0000dfd0: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-0000dfe0: 7374 7269 6374 6564 2220 636f 6d6d 656e  stricted" commen
-0000dff0: 743d 2265 7861 6d70 6c65 223e 0a20 2020  t="example">.   
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e010: 2020 2020 2032 3030 392d 3130 2d31 3054       2009-10-10T
-0000e020: 3132 3a30 303a 3030 2d30 353a 3030 0a20  12:00:00-05:00. 
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 2020 203c 2f74 696d 653e 0a20 2020 2020     </time>.     
-0000e050: 2020 2020 2020 2020 2020 203c 2f74 696d             </tim
-0000e060: 652d 7072 6f70 3e0a 2020 2020 2020 2020  e-prop>.        
-0000e070: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-0000e080: 6b65 5f74 696d 655f 7072 6f70 2822 3a74  ke_time_prop(":t
-0000e090: 6573 7470 726f 7065 7274 7922 2c20 5b22  estproperty", ["
-0000e0a0: 3230 3039 2d31 302d 3130 5431 323a 3030  2009-10-10T12:00
-0000e0b0: 3a30 302d 3035 3a30 3022 2c20 2231 3930  :00-05:00", "190
-0000e0c0: 312d 3031 2d30 3154 3031 3a30 303a 3030  1-01-01T01:00:00
-0000e0d0: 2d30 303a 3030 225d 290a 2020 2020 2020  -00:00"]).      
-0000e0e0: 2020 2020 2020 2020 2020 3c74 696d 652d            <time-
-0000e0f0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
-0000e100: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
-0000e110: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e120: 7469 6d65 2070 6572 6d69 7373 696f 6e73  time permissions
-0000e130: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-0000e140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e150: 2020 2020 2020 2020 2032 3030 392d 3130           2009-10
-0000e160: 2d31 3054 3132 3a30 303a 3030 2d30 353a  -10T12:00:00-05:
-0000e170: 3030 0a20 2020 2020 2020 2020 2020 2020  00.             
-0000e180: 2020 2020 2020 203c 2f74 696d 653e 0a20         </time>. 
-0000e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1a0: 2020 203c 7469 6d65 2070 6572 6d69 7373     <time permiss
-0000e1b0: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-0000e1c0: 6c74 223e 0a20 2020 2020 2020 2020 2020  lt">.           
-0000e1d0: 2020 2020 2020 2020 2020 2020 2031 3930               190
-0000e1e0: 312d 3031 2d30 3154 3031 3a30 303a 3030  1-01-01T01:00:00
-0000e1f0: 2d30 303a 3030 320a 2020 2020 2020 2020  -00:002.        
+00004b10: 6765 730a 2020 2020 2020 2020 6361 6c6c  ges.        call
+00004b20: 696e 675f 7265 736f 7572 6365 3a20 7265  ing_resource: re
+00004b30: 736f 7572 6365 206e 616d 652c 2066 6f72  source name, for
+00004b40: 2062 6574 7465 7220 6572 726f 7220 6d65   better error me
+00004b50: 7373 6167 6573 0a0a 2020 2020 5261 6973  ssages..    Rais
+00004b60: 6573 3a0a 2020 2020 2020 2020 4261 7365  es:.        Base
+00004b70: 4572 726f 723a 2069 6620 7468 6520 696e  Error: if the in
+00004b80: 7075 7420 6361 6e6e 6f74 2062 6520 7472  put cannot be tr
+00004b90: 616e 7366 6f72 6d65 6420 696e 746f 2022  ansformed into "
+00004ba0: 7472 7565 222f 2266 616c 7365 220a 0a20  true"/"false".. 
+00004bb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00004bc0: 2020 2020 2274 7275 6522 2069 6620 7468      "true" if th
+00004bd0: 6520 696e 7075 7420 6973 2069 6e20 2854  e input is in (T
+00004be0: 7275 652c 2022 7472 7565 222c 2022 3122  rue, "true", "1"
+00004bf0: 2c20 312c 2022 7965 7322 293b 2022 6661  , 1, "yes"); "fa
+00004c00: 6c73 6522 2069 6620 696e 7075 7420 6973  lse" if input is
+00004c10: 2069 6e20 2846 616c 7365 2c20 2266 616c   in (False, "fal
+00004c20: 7365 222c 2022 3022 2c20 302c 2022 6e6f  se", "0", 0, "no
+00004c30: 2229 0a20 2020 2022 2222 0a20 2020 2069  ").    """.    i
+00004c40: 6620 6973 696e 7374 616e 6365 2875 6e66  f isinstance(unf
+00004c50: 6f72 6d61 7474 6564 2c20 7374 7229 3a0a  ormatted, str):.
+00004c60: 2020 2020 2020 2020 756e 666f 726d 6174          unformat
+00004c70: 7465 6420 3d20 756e 666f 726d 6174 7465  ted = unformatte
+00004c80: 642e 6c6f 7765 7228 290a 2020 2020 6966  d.lower().    if
+00004c90: 2075 6e66 6f72 6d61 7474 6564 2069 6e20   unformatted in 
+00004ca0: 2846 616c 7365 2c20 2266 616c 7365 222c  (False, "false",
+00004cb0: 2022 3022 2c20 302c 2030 2e30 2c20 226e   "0", 0, 0.0, "n
+00004cc0: 6f22 293a 0a20 2020 2020 2020 2072 6574  o"):.        ret
+00004cd0: 7572 6e20 2266 616c 7365 220a 2020 2020  urn "false".    
+00004ce0: 656c 6966 2075 6e66 6f72 6d61 7474 6564  elif unformatted
+00004cf0: 2069 6e20 2854 7275 652c 2022 7472 7565   in (True, "true
+00004d00: 222c 2022 3122 2c20 312c 2031 2e30 2c20  ", "1", 1, 1.0, 
+00004d10: 2279 6573 2229 3a0a 2020 2020 2020 2020  "yes"):.        
+00004d20: 7265 7475 726e 2022 7472 7565 220a 2020  return "true".  
+00004d30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004d40: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
+00004d50: 0a20 2020 2020 2020 2020 2020 2066 2246  .            f"F
+00004d60: 6169 6c65 6420 7661 6c69 6461 7469 6f6e  ailed validation
+00004d70: 2069 6e20 7265 736f 7572 6365 2027 7b63   in resource '{c
+00004d80: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
+00004d90: 272c 2070 726f 7065 7274 7920 277b 6e61  ', property '{na
+00004da0: 6d65 7d27 3a20 220a 2020 2020 2020 2020  me}': ".        
+00004db0: 2020 2020 6622 277b 756e 666f 726d 6174      f"'{unformat
+00004dc0: 7465 647d 2720 6973 206e 6f74 2061 2076  ted}' is not a v
+00004dd0: 616c 6964 2062 6f6f 6c65 616e 2e22 0a20  alid boolean.". 
+00004de0: 2020 2020 2020 2029 0a0a 0a64 6566 206d         )...def m
+00004df0: 616b 655f 626f 6f6c 6561 6e5f 7072 6f70  ake_boolean_prop
+00004e00: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
+00004e10: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
+00004e20: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
+00004e30: 742c 2073 7472 2c20 696e 742c 2062 6f6f  t, str, int, boo
+00004e40: 6c5d 2c0a 2020 2020 6361 6c6c 696e 675f  l],.    calling_
+00004e50: 7265 736f 7572 6365 3a20 7374 7220 3d20  resource: str = 
+00004e60: 2222 2c0a 2920 2d3e 2065 7472 6565 2e5f  "",.) -> etree._
+00004e70: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
+00004e80: 0a20 2020 204d 616b 6520 6120 3c62 6f6f  .    Make a <boo
+00004e90: 6c65 616e 2d70 726f 703e 2066 726f 6d20  lean-prop> from 
+00004ea0: 6120 626f 6f6c 6561 6e20 7661 6c75 652e  a boolean value.
+00004eb0: 2054 6865 2076 616c 7565 2063 616e 2062   The value can b
+00004ec0: 6520 7072 6f76 6964 6564 2064 6972 6563  e provided direc
+00004ed0: 746c 7920 6f72 2069 6e73 6964 6520 6120  tly or inside a 
+00004ee0: 5072 6f70 6572 7479 456c 656d 656e 742e  PropertyElement.
+00004ef0: 2054 6865 0a20 2020 2066 6f6c 6c6f 7769   The.    followi
+00004f00: 6e67 2066 6f72 6d61 7473 2061 7265 2073  ng formats are s
+00004f10: 7570 706f 7274 6564 3a0a 2020 2020 202d  upported:.     -
+00004f20: 2074 7275 653a 2028 5472 7565 2c20 2274   true: (True, "t
+00004f30: 7275 6522 2c20 2254 7275 6522 2c20 2231  rue", "True", "1
+00004f40: 222c 2031 2c20 2279 6573 222c 2022 5965  ", 1, "yes", "Ye
+00004f50: 7322 290a 2020 2020 202d 2066 616c 7365  s").     - false
+00004f60: 3a20 2846 616c 7365 2c20 2266 616c 7365  : (False, "false
+00004f70: 222c 2022 4661 6c73 6522 2c20 2230 222c  ", "False", "0",
+00004f80: 2030 2c20 226e 6f22 2c20 224e 6f22 290a   0, "no", "No").
+00004f90: 0a20 2020 2055 6e6c 6573 7320 7072 6f76  .    Unless prov
+00004fa0: 6964 6564 2061 7320 5072 6f70 6572 7479  ided as Property
+00004fb0: 456c 656d 656e 742c 2074 6865 2070 6572  Element, the per
+00004fc0: 6d69 7373 696f 6e73 206f 6620 7468 6520  missions of the 
+00004fd0: 7661 6c75 6520 6465 6661 756c 7420 746f  value default to
+00004fe0: 2022 7072 6f70 2d64 6566 6175 6c74 222e   "prop-default".
+00004ff0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00005000: 2020 2020 6e61 6d65 3a20 7468 6520 6e61      name: the na
+00005010: 6d65 206f 6620 7468 6973 2070 726f 7065  me of this prope
+00005020: 7274 7920 6173 2064 6566 696e 6564 2069  rty as defined i
+00005030: 6e20 7468 6520 6f6e 746f 0a20 2020 2020  n the onto.     
+00005040: 2020 2076 616c 7565 3a20 6120 626f 6f6c     value: a bool
+00005050: 6561 6e20 7661 6c75 6520 6173 2073 7472  ean value as str
+00005060: 2f62 6f6f 6c2f 696e 742c 206f 7220 6173  /bool/int, or as
+00005070: 2073 7472 2f62 6f6f 6c2f 696e 7420 696e   str/bool/int in
+00005080: 7369 6465 2061 2050 726f 7065 7274 7945  side a PropertyE
+00005090: 6c65 6d65 6e74 0a20 2020 2020 2020 2063  lement.        c
+000050a0: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
+000050b0: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+000050c0: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
+000050d0: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
+000050e0: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
+000050f0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00005100: 2020 4261 7365 4572 726f 723a 2069 6620    BaseError: if 
+00005110: 7468 6520 7661 6c75 6520 6973 206e 6f74  the value is not
+00005120: 2061 2076 616c 6964 2062 6f6f 6c65 616e   a valid boolean
+00005130: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00005140: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
+00005150: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
+00005160: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
+00005170: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+00005180: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
+00005190: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
+000051a0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
+000051b0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+000051c0: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
+000051d0: 2e6d 616b 655f 626f 6f6c 6561 6e5f 7072  .make_boolean_pr
+000051e0: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
+000051f0: 7922 2c20 226e 6f22 290a 2020 2020 2020  y", "no").      
+00005200: 2020 2020 2020 2020 2020 3c62 6f6f 6c65            <boole
+00005210: 616e 2d70 726f 7020 6e61 6d65 3d22 3a74  an-prop name=":t
+00005220: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 3c62 6f6f 6c65 616e 2070 6572 6d69    <boolean permi
+00005250: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+00005260: 6175 6c74 223e 6661 6c73 653c 2f62 6f6f  ault">false</boo
+00005270: 6c65 616e 3e0a 2020 2020 2020 2020 2020  lean>.          
+00005280: 2020 2020 2020 3c2f 626f 6f6c 6561 6e2d        </boolean-
+00005290: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
+000052a0: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+000052b0: 5f62 6f6f 6c65 616e 5f70 726f 7028 223a  _boolean_prop(":
+000052c0: 7465 7374 7072 6f70 6572 7479 222c 2065  testproperty", e
+000052d0: 7863 656c 3278 6d6c 2e50 726f 7065 7274  xcel2xml.Propert
+000052e0: 7945 6c65 6d65 6e74 2822 3122 2c20 7065  yElement("1", pe
+000052f0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+00005300: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
+00005310: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
+00005320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005330: 203c 626f 6f6c 6561 6e2d 7072 6f70 206e   <boolean-prop n
+00005340: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+00005350: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+00005360: 2020 2020 2020 2020 203c 626f 6f6c 6561           <boolea
+00005370: 6e20 7065 726d 6973 7369 6f6e 733d 2270  n permissions="p
+00005380: 726f 702d 7265 7374 7269 6374 6564 2220  rop-restricted" 
+00005390: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
+000053a0: 223e 7472 7565 3c2f 626f 6f6c 6561 6e3e  ">true</boolean>
+000053b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053c0: 203c 2f62 6f6f 6c65 616e 2d70 726f 703e   </boolean-prop>
+000053d0: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
+000053e0: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
+000053f0: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
+00005400: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
+00005410: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
+00005420: 626f 6f6c 6561 6e2d 7072 6f70 0a20 2020  boolean-prop.   
+00005430: 2022 2222 0a0a 2020 2020 2320 7661 6c69   """..    # vali
+00005440: 6461 7465 2069 6e70 7574 0a20 2020 2069  date input.    i
+00005450: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+00005460: 7565 2c20 5072 6f70 6572 7479 456c 656d  ue, PropertyElem
+00005470: 656e 7429 3a0a 2020 2020 2020 2020 7661  ent):.        va
+00005480: 6c75 655f 6e65 7720 3d20 6461 7461 636c  lue_new = datacl
+00005490: 6173 7365 732e 7265 706c 6163 6528 7661  asses.replace(va
+000054a0: 6c75 652c 2076 616c 7565 3d5f 666f 726d  lue, value=_form
+000054b0: 6174 5f62 6f6f 6c28 7661 6c75 652e 7661  at_bool(value.va
+000054c0: 6c75 652c 206e 616d 652c 2063 616c 6c69  lue, name, calli
+000054d0: 6e67 5f72 6573 6f75 7263 6529 290a 2020  ng_resource)).  
+000054e0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000054f0: 6528 7661 6c75 652c 2028 7374 722c 2062  e(value, (str, b
+00005500: 6f6f 6c2c 2069 6e74 2929 3a0a 2020 2020  ool, int)):.    
+00005510: 2020 2020 7661 6c75 655f 6e65 7720 3d20      value_new = 
+00005520: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
+00005530: 5f66 6f72 6d61 745f 626f 6f6c 2876 616c  _format_bool(val
+00005540: 7565 2c20 6e61 6d65 2c20 6361 6c6c 696e  ue, name, callin
+00005550: 675f 7265 736f 7572 6365 2929 0a20 2020  g_resource)).   
+00005560: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+00005570: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
+00005580: 2020 2020 2020 2020 2020 2020 6622 4661              f"Fa
+00005590: 696c 6564 2076 616c 6964 6174 696f 6e20  iled validation 
+000055a0: 696e 2072 6573 6f75 7263 6520 277b 6361  in resource '{ca
+000055b0: 6c6c 696e 675f 7265 736f 7572 6365 7d27  lling_resource}'
+000055c0: 2c20 7072 6f70 6572 7479 2027 7b6e 616d  , property '{nam
+000055d0: 657d 273a 2027 7b76 616c 7565 7d27 2069  e}': '{value}' i
+000055e0: 7320 6e6f 7420 6120 7661 6c69 6420 626f  s not a valid bo
+000055f0: 6f6c 6561 6e2e 220a 2020 2020 2020 2020  olean.".        
+00005600: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+00005610: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+00005620: 6865 2076 616c 7565 0a20 2020 2070 726f  he value.    pro
+00005630: 705f 203d 2065 7472 6565 2e45 6c65 6d65  p_ = etree.Eleme
+00005640: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
+00005650: 7d62 6f6f 6c65 616e 2d70 726f 7022 2025  }boolean-prop" %
+00005660: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+00005670: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+00005680: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
+00005690: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
+000056a0: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
+000056b0: 2020 290a 2020 2020 6b77 6172 6773 203d    ).    kwargs =
+000056c0: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
+000056d0: 2076 616c 7565 5f6e 6577 2e70 6572 6d69   value_new.permi
+000056e0: 7373 696f 6e73 7d0a 2020 2020 6966 2076  ssions}.    if v
+000056f0: 616c 7565 5f6e 6577 2e63 6f6d 6d65 6e74  alue_new.comment
+00005700: 2061 6e64 2063 6865 636b 5f6e 6f74 6e61   and check_notna
+00005710: 2876 616c 7565 5f6e 6577 2e63 6f6d 6d65  (value_new.comme
+00005720: 6e74 293a 0a20 2020 2020 2020 206b 7761  nt):.        kwa
+00005730: 7267 735b 2263 6f6d 6d65 6e74 225d 203d  rgs["comment"] =
+00005740: 2076 616c 7565 5f6e 6577 2e63 6f6d 6d65   value_new.comme
+00005750: 6e74 0a20 2020 2076 616c 7565 5f20 3d20  nt.    value_ = 
+00005760: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
+00005770: 2020 2020 2020 2022 7b25 737d 626f 6f6c         "{%s}bool
+00005780: 6561 6e22 2025 2078 6d6c 5f6e 616d 6573  ean" % xml_names
+00005790: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
+000057a0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+000057b0: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
+000057c0: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
+000057d0: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
+000057e0: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
+000057f0: 2029 0a20 2020 2076 616c 7565 5f2e 7465   ).    value_.te
+00005800: 7874 203d 2073 7472 2876 616c 7565 5f6e  xt = str(value_n
+00005810: 6577 2e76 616c 7565 290a 2020 2020 7072  ew.value).    pr
+00005820: 6f70 5f2e 6170 7065 6e64 2876 616c 7565  op_.append(value
+00005830: 5f29 0a0a 2020 2020 7265 7475 726e 2070  _)..    return p
+00005840: 726f 705f 0a0a 0a64 6566 206d 616b 655f  rop_...def make_
+00005850: 636f 6c6f 725f 7072 6f70 280a 2020 2020  color_prop(.    
+00005860: 6e61 6d65 3a20 7374 722c 0a20 2020 2076  name: str,.    v
+00005870: 616c 7565 3a20 556e 696f 6e5b 5072 6f70  alue: Union[Prop
+00005880: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+00005890: 2c20 4974 6572 6162 6c65 5b55 6e69 6f6e  , Iterable[Union
+000058a0: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
+000058b0: 2c20 7374 725d 5d5d 2c0a 2020 2020 6361  , str]]],.    ca
+000058c0: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+000058d0: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
+000058e0: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
+000058f0: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
+00005900: 6120 3c63 6f6c 6f72 2d70 726f 703e 2066  a <color-prop> f
+00005910: 726f 6d20 6f6e 6520 6f72 206d 6f72 6520  rom one or more 
+00005920: 636f 6c6f 7273 2e20 5468 6520 636f 6c6f  colors. The colo
+00005930: 7228 7329 2063 616e 2062 6520 7072 6f76  r(s) can be prov
+00005940: 6964 6564 2061 7320 7374 7269 6e67 206f  ided as string o
+00005950: 7220 6173 2050 726f 7065 7274 7945 6c65  r as PropertyEle
+00005960: 6d65 6e74 2077 6974 6820 610a 2020 2020  ment with a.    
+00005970: 7374 7269 6e67 2069 6e73 6964 652e 2049  string inside. I
+00005980: 6620 7072 6f76 6964 6564 2061 7320 7374  f provided as st
+00005990: 7269 6e67 2c20 7468 6520 7065 726d 6973  ring, the permis
+000059a0: 7369 6f6e 7320 6465 6661 756c 7420 746f  sions default to
+000059b0: 2022 7072 6f70 2d64 6566 6175 6c74 222e   "prop-default".
+000059c0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000059d0: 2020 2020 6e61 6d65 3a20 7468 6520 6e61      name: the na
+000059e0: 6d65 206f 6620 7468 6973 2070 726f 7065  me of this prope
+000059f0: 7274 7920 6173 2064 6566 696e 6564 2069  rty as defined i
+00005a00: 6e20 7468 6520 6f6e 746f 0a20 2020 2020  n the onto.     
+00005a10: 2020 2076 616c 7565 3a20 6f6e 6520 6f72     value: one or
+00005a20: 206d 6f72 6520 4453 5020 636f 6c6f 7228   more DSP color(
+00005a30: 7329 2c20 6173 2073 7472 696e 672f 5072  s), as string/Pr
+00005a40: 6f70 6572 7479 456c 656d 656e 742c 206f  opertyElement, o
+00005a50: 7220 6173 2069 7465 7261 626c 6520 6f66  r as iterable of
+00005a60: 2073 7472 696e 6773 2f50 726f 7065 7274   strings/Propert
+00005a70: 7945 6c65 6d65 6e74 730a 2020 2020 2020  yElements.      
+00005a80: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+00005a90: 6365 3a20 7468 6520 6e61 6d65 206f 6620  ce: the name of 
+00005aa0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+00005ab0: 7263 6520 2866 6f72 2062 6574 7465 7220  rce (for better 
+00005ac0: 6572 726f 7220 6d65 7373 6167 6573 290a  error messages).
+00005ad0: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+00005ae0: 2020 2020 2042 6173 6545 7272 6f72 3a20       BaseError: 
+00005af0: 4966 2074 6865 2076 616c 7565 2069 7320  If the value is 
+00005b00: 6e6f 7420 6120 7661 6c69 6420 636f 6c6f  not a valid colo
+00005b10: 720a 0a20 2020 2052 6574 7572 6e73 3a0a  r..    Returns:.
+00005b20: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
+00005b30: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
+00005b40: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
+00005b50: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
+00005b60: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
+00005b70: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
+00005b80: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
+00005b90: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+00005ba0: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+00005bb0: 6c2e 6d61 6b65 5f63 6f6c 6f72 5f70 726f  l.make_color_pro
+00005bc0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+00005bd0: 222c 2022 2330 3066 6636 3622 290a 2020  ", "#00ff66").  
+00005be0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00005bf0: 6f6c 6f72 2d70 726f 7020 6e61 6d65 3d22  olor-prop name="
+00005c00: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c20: 2020 2020 3c63 6f6c 6f72 2070 6572 6d69      <color permi
+00005c30: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+00005c40: 6175 6c74 223e 2330 3066 6636 363c 2f63  ault">#00ff66</c
+00005c50: 6f6c 6f72 3e0a 2020 2020 2020 2020 2020  olor>.          
+00005c60: 2020 2020 2020 3c2f 636f 6c6f 722d 7072        </color-pr
+00005c70: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
+00005c80: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f63  excel2xml.make_c
+00005c90: 6f6c 6f72 5f70 726f 7028 223a 7465 7374  olor_prop(":test
+00005ca0: 7072 6f70 6572 7479 222c 2065 7863 656c  property", excel
+00005cb0: 3278 6d6c 2e50 726f 7065 7274 7945 6c65  2xml.PropertyEle
+00005cc0: 6d65 6e74 2822 2330 3066 6636 3622 2c20  ment("#00ff66", 
+00005cd0: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+00005ce0: 702d 7265 7374 7269 6374 6564 222c 2063  p-restricted", c
+00005cf0: 6f6d 6d65 6e74 3d22 6578 616d 706c 6522  omment="example"
+00005d00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00005d10: 2020 203c 636f 6c6f 722d 7072 6f70 206e     <color-prop n
+00005d20: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+00005d30: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+00005d40: 2020 2020 2020 2020 203c 636f 6c6f 7220           <color 
+00005d50: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+00005d60: 702d 7265 7374 7269 6374 6564 2220 636f  p-restricted" co
+00005d70: 6d6d 656e 743d 2265 7861 6d70 6c65 223e  mment="example">
+00005d80: 2330 3066 6636 363c 2f63 6f6c 6f72 3e0a  #00ff66</color>.
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 3c2f 636f 6c6f 722d 7072 6f70 3e0a 2020  </color-prop>.  
+00005db0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00005dc0: 786d 6c2e 6d61 6b65 5f63 6f6c 6f72 5f70  xml.make_color_p
+00005dd0: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+00005de0: 7479 222c 205b 2223 3030 6666 3636 222c  ty", ["#00ff66",
+00005df0: 2022 2330 3030 3030 3022 5d29 0a20 2020   "#000000"]).   
+00005e00: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00005e10: 6c6f 722d 7072 6f70 206e 616d 653d 223a  lor-prop name=":
+00005e20: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
+00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e40: 2020 203c 636f 6c6f 7220 7065 726d 6973     <color permis
+00005e50: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+00005e60: 756c 7422 3e23 3030 6666 3636 3c2f 636f  ult">#00ff66</co
+00005e70: 6c6f 723e 0a20 2020 2020 2020 2020 2020  lor>.           
+00005e80: 2020 2020 2020 2020 203c 636f 6c6f 7220           <color 
+00005e90: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+00005ea0: 702d 6465 6661 756c 7422 3e23 3030 3030  p-default">#0000
+00005eb0: 3030 3c2f 636f 6c6f 723e 0a20 2020 2020  00</color>.     
+00005ec0: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
+00005ed0: 6f72 2d70 726f 703e 0a0a 2020 2020 5365  or-prop>..    Se
+00005ee0: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
+00005ef0: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
+00005f00: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
+00005f10: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
+00005f20: 612d 6669 6c65 2f23 636f 6c6f 722d 7072  a-file/#color-pr
+00005f30: 6f70 0a20 2020 2022 2222 0a0a 2020 2020  op.    """..    
+00005f40: 2320 6368 6563 6b20 7468 6520 696e 7075  # check the inpu
+00005f50: 743a 2070 7265 7061 7265 2061 206c 6973  t: prepare a lis
+00005f60: 7420 7769 7468 2076 616c 6964 2076 616c  t with valid val
+00005f70: 7565 730a 2020 2020 7661 6c75 6573 203d  ues.    values =
+00005f80: 2070 7265 7061 7265 5f76 616c 7565 2876   prepare_value(v
+00005f90: 616c 7565 290a 0a20 2020 2023 2063 6865  alue)..    # che
+00005fa0: 636b 2076 616c 7565 2074 7970 650a 2020  ck value type.  
+00005fb0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
+00005fc0: 7565 733a 0a20 2020 2020 2020 2069 6620  ues:.        if 
+00005fd0: 6e6f 7420 7265 6765 782e 7365 6172 6368  not regex.search
+00005fe0: 2872 225e 235b 302d 3961 2d66 5d7b 367d  (r"^#[0-9a-f]{6}
+00005ff0: 2422 2c20 7374 7228 7661 6c2e 7661 6c75  $", str(val.valu
+00006000: 6529 2e73 7472 6970 2829 2c20 666c 6167  e).strip(), flag
+00006010: 733d 7265 6765 782e 4947 4e4f 5245 4341  s=regex.IGNORECA
+00006020: 5345 293a 0a20 2020 2020 2020 2020 2020  SE):.           
+00006030: 2072 6169 7365 2042 6173 6545 7272 6f72   raise BaseError
+00006040: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00006050: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
+00006060: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
+00006070: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
+00006080: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
+00006090: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
+000060a0: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
+000060b0: 7b76 616c 2e76 616c 7565 7d27 2069 7320  {val.value}' is 
+000060c0: 6e6f 7420 6120 7661 6c69 6420 636f 6c6f  not a valid colo
+000060d0: 722e 220a 2020 2020 2020 2020 2020 2020  r.".            
+000060e0: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+000060f0: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+00006100: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+00006110: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+00006120: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+00006130: 2020 2022 7b25 737d 636f 6c6f 722d 7072     "{%s}color-pr
+00006140: 6f70 2220 2520 786d 6c5f 6e61 6d65 7370  op" % xml_namesp
+00006150: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
+00006160: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
+00006170: 2c0a 2020 2020 2020 2020 6e73 6d61 703d  ,.        nsmap=
+00006180: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+00006190: 702c 0a20 2020 2029 0a20 2020 2066 6f72  p,.    ).    for
+000061a0: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
+000061b0: 2020 2020 2020 2020 6b77 6172 6773 203d          kwargs =
+000061c0: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
+000061d0: 2076 616c 2e70 6572 6d69 7373 696f 6e73   val.permissions
+000061e0: 7d0a 2020 2020 2020 2020 6966 2076 616c  }.        if val
+000061f0: 2e63 6f6d 6d65 6e74 2061 6e64 2063 6865  .comment and che
+00006200: 636b 5f6e 6f74 6e61 2876 616c 2e63 6f6d  ck_notna(val.com
+00006210: 6d65 6e74 293a 0a20 2020 2020 2020 2020  ment):.         
+00006220: 2020 206b 7761 7267 735b 2263 6f6d 6d65     kwargs["comme
+00006230: 6e74 225d 203d 2076 616c 2e63 6f6d 6d65  nt"] = val.comme
+00006240: 6e74 0a20 2020 2020 2020 2076 616c 7565  nt.        value
+00006250: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
+00006260: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
+00006270: 7b25 737d 636f 6c6f 7222 2025 2078 6d6c  {%s}color" % xml
+00006280: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+00006290: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
+000062a0: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
+000062b0: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
+000062c0: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
+000062d0: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
+000062e0: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
+000062f0: 2020 2029 0a20 2020 2020 2020 2076 616c     ).        val
+00006300: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
+00006310: 616c 2e76 616c 7565 292e 7374 7269 7028  al.value).strip(
+00006320: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
+00006330: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
+00006340: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
+00006350: 0a0a 0a64 6566 206d 616b 655f 6461 7465  ...def make_date
+00006360: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+00006370: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+00006380: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+00006390: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+000063a0: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+000063b0: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+000063c0: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+000063d0: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+000063e0: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+000063f0: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+00006400: 220a 2020 2020 4d61 6b65 2061 203c 6461  ".    Make a <da
+00006410: 7465 2d70 726f 703e 2066 726f 6d20 6f6e  te-prop> from on
+00006420: 6520 6f72 206d 6f72 6520 6461 7465 732f  e or more dates/
+00006430: 6461 7465 2072 616e 6765 732e 2054 6865  date ranges. The
+00006440: 2064 6174 6528 7329 2063 616e 2062 6520   date(s) can be 
+00006450: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+00006460: 6e67 206f 7220 6173 2050 726f 7065 7274  ng or as Propert
+00006470: 7945 6c65 6d65 6e74 0a20 2020 2077 6974  yElement.    wit
+00006480: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
+00006490: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
+000064a0: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
+000064b0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
+000064c0: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
+000064d0: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
+000064e0: 2020 2020 2020 2020 6e61 6d65 3a20 7468          name: th
+000064f0: 6520 6e61 6d65 206f 6620 7468 6973 2070  e name of this p
+00006500: 726f 7065 7274 7920 6173 2064 6566 696e  roperty as defin
+00006510: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
+00006520: 2020 2020 2020 2076 616c 7565 3a20 6f6e         value: on
+00006530: 6520 6f72 206d 6f72 6520 4453 5020 6461  e or more DSP da
+00006540: 7465 732c 2061 7320 7374 7269 6e67 2f50  tes, as string/P
+00006550: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+00006560: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
+00006570: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
+00006580: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
+00006590: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+000065a0: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
+000065b0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+000065c0: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
+000065d0: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
+000065e0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+000065f0: 2020 2020 2020 4261 7365 4572 726f 723a        BaseError:
+00006600: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00006610: 206e 6f74 2061 2076 616c 6964 2044 5350   not a valid DSP
+00006620: 2064 6174 650a 0a20 2020 2052 6574 7572   date..    Retur
+00006630: 6e73 3a0a 2020 2020 2020 2020 616e 2065  ns:.        an e
+00006640: 7472 6565 2e5f 456c 656d 656e 7420 7468  tree._Element th
+00006650: 6174 2063 616e 2062 6520 6170 7065 6e64  at can be append
+00006660: 6564 2074 6f20 7468 6520 7061 7265 6e74  ed to the parent
+00006670: 2072 6573 6f75 7263 6520 7769 7468 2072   resource with r
+00006680: 6573 6f75 7263 652e 6170 7065 6e64 286d  esource.append(m
+00006690: 616b 655f 2a5f 7072 6f70 282e 2e2e 2929  ake_*_prop(...))
+000066a0: 0a0a 2020 2020 4578 616d 706c 6573 3a0a  ..    Examples:.
+000066b0: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
+000066c0: 6c32 786d 6c2e 6d61 6b65 5f64 6174 655f  l2xml.make_date_
+000066d0: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
+000066e0: 7274 7922 2c20 2247 5245 474f 5249 414e  rty", "GREGORIAN
+000066f0: 3a43 453a 3230 3134 2d30 312d 3331 2229  :CE:2014-01-31")
+00006700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006710: 203c 6461 7465 2d70 726f 7020 6e61 6d65   <date-prop name
+00006720: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+00006730: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006740: 2020 2020 2020 3c64 6174 6520 7065 726d        <date perm
+00006750: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+00006760: 6661 756c 7422 3e47 5245 474f 5249 414e  fault">GREGORIAN
+00006770: 3a43 453a 3230 3134 2d30 312d 3331 3c2f  :CE:2014-01-31</
+00006780: 6461 7465 3e0a 2020 2020 2020 2020 2020  date>.          
+00006790: 2020 2020 2020 3c2f 6461 7465 2d70 726f        </date-pro
+000067a0: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
+000067b0: 7863 656c 3278 6d6c 2e6d 616b 655f 6461  xcel2xml.make_da
+000067c0: 7465 5f70 726f 7028 223a 7465 7374 7072  te_prop(":testpr
+000067d0: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
+000067e0: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
+000067f0: 6e74 2822 4752 4547 4f52 4941 4e3a 4345  nt("GREGORIAN:CE
+00006800: 3a32 3031 342d 3031 2d33 3122 2c20 7065  :2014-01-31", pe
+00006810: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+00006820: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
+00006830: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
+00006840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006850: 203c 6461 7465 2d70 726f 7020 6e61 6d65   <date-prop name
+00006860: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+00006870: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006880: 2020 2020 2020 3c64 6174 6520 7065 726d        <date perm
+00006890: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
+000068a0: 7374 7269 6374 6564 2220 636f 6d6d 656e  stricted" commen
+000068b0: 743d 2265 7861 6d70 6c65 223e 0a20 2020  t="example">.   
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2020 2047 5245 474f 5249 414e 3a43       GREGORIAN:C
+000068e0: 453a 3230 3134 2d30 312d 3331 0a20 2020  E:2014-01-31.   
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 203c 2f64 6174 653e 0a20 2020 2020 2020   </date>.       
+00006910: 2020 2020 2020 2020 203c 2f64 6174 652d           </date-
+00006920: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
+00006930: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+00006940: 5f64 6174 655f 7072 6f70 2822 3a74 6573  _date_prop(":tes
+00006950: 7470 726f 7065 7274 7922 2c20 5b22 4752  tproperty", ["GR
+00006960: 4547 4f52 4941 4e3a 4345 3a31 3933 302d  EGORIAN:CE:1930-
+00006970: 3039 2d30 323a 4345 3a31 3933 302d 3039  09-02:CE:1930-09
+00006980: 2d30 3322 2c20 2247 5245 474f 5249 414e  -03", "GREGORIAN
+00006990: 3a43 453a 3139 3330 2d30 392d 3032 3a43  :CE:1930-09-02:C
+000069a0: 453a 3139 3330 2d30 392d 3033 225d 290a  E:1930-09-03"]).
+000069b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069c0: 3c64 6174 652d 7072 6f70 206e 616d 653d  <date-prop name=
+000069d0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+000069e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069f0: 2020 2020 203c 6461 7465 2070 6572 6d69       <date permi
+00006a00: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+00006a10: 6175 6c74 223e 0a20 2020 2020 2020 2020  ault">.         
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2047                 G
+00006a30: 5245 474f 5249 414e 3a43 453a 3139 3330  REGORIAN:CE:1930
+00006a40: 2d30 392d 3032 3a43 453a 3139 3330 2d30  -09-02:CE:1930-0
+00006a50: 392d 3033 0a20 2020 2020 2020 2020 2020  9-03.           
+00006a60: 2020 2020 2020 2020 203c 2f64 6174 653e           </date>
+00006a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a80: 2020 2020 203c 6461 7465 2070 6572 6d69       <date permi
+00006a90: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+00006aa0: 6175 6c74 223e 0a20 2020 2020 2020 2020  ault">.         
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 2047                 G
+00006ac0: 5245 474f 5249 414e 3a43 453a 3139 3330  REGORIAN:CE:1930
+00006ad0: 2d30 392d 3032 3a43 453a 3139 3330 2d30  -09-02:CE:1930-0
+00006ae0: 392d 3033 0a20 2020 2020 2020 2020 2020  9-03.           
+00006af0: 2020 2020 2020 2020 203c 2f64 6174 653e           </date>
+00006b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006b10: 203c 2f64 6174 652d 7072 6f70 3e0a 0a20   </date-prop>.. 
+00006b20: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
+00006b30: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
+00006b40: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
+00006b50: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
+00006b60: 6c2d 6461 7461 2d66 696c 652f 2364 6174  l-data-file/#dat
+00006b70: 652d 7072 6f70 0a20 2020 2022 2222 0a0a  e-prop.    """..
+00006b80: 2020 2020 2320 6368 6563 6b20 7468 6520      # check the 
+00006b90: 696e 7075 743a 2070 7265 7061 7265 2061  input: prepare a
+00006ba0: 206c 6973 7420 7769 7468 2076 616c 6964   list with valid
+00006bb0: 2076 616c 7565 730a 2020 2020 7661 6c75   values.    valu
+00006bc0: 6573 203d 2070 7265 7061 7265 5f76 616c  es = prepare_val
+00006bd0: 7565 2876 616c 7565 290a 0a20 2020 2023  ue(value)..    #
+00006be0: 2063 6865 636b 2076 616c 7565 2074 7970   check value typ
+00006bf0: 650a 2020 2020 666f 7220 7661 6c20 696e  e.    for val in
+00006c00: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
+00006c10: 2069 6620 6e6f 7420 6973 5f66 756c 6c5f   if not is_full_
+00006c20: 6461 7465 2873 7472 2876 616c 2e76 616c  date(str(val.val
+00006c30: 7565 292e 7374 7269 7028 2929 3a0a 2020  ue).strip()):.  
+00006c40: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006c50: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
+00006c60: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
+00006c70: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
+00006c80: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
+00006c90: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
+00006ca0: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
+00006cb0: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
+00006cc0: 2020 2020 2020 6622 277b 7661 6c2e 7661        f"'{val.va
+00006cd0: 6c75 657d 2720 6973 206e 6f74 2061 2076  lue}' is not a v
+00006ce0: 616c 6964 2044 5350 2064 6174 652e 220a  alid DSP date.".
+00006cf0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00006d00: 2020 2023 206d 616b 6520 786d 6c20 7374     # make xml st
+00006d10: 7275 6374 7572 6520 6f66 2074 6865 2076  ructure of the v
+00006d20: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
+00006d30: 7072 6f70 5f20 3d20 6574 7265 652e 456c  prop_ = etree.El
+00006d40: 656d 656e 7428 0a20 2020 2020 2020 2022  ement(.        "
+00006d50: 7b25 737d 6461 7465 2d70 726f 7022 2025  {%s}date-prop" %
+00006d60: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+00006d70: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+00006d80: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
+00006d90: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
+00006da0: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
+00006db0: 2020 290a 2020 2020 666f 7220 7661 6c20    ).    for val 
+00006dc0: 696e 2076 616c 7565 733a 0a20 2020 2020  in values:.     
+00006dd0: 2020 206b 7761 7267 7320 3d20 7b22 7065     kwargs = {"pe
+00006de0: 726d 6973 7369 6f6e 7322 3a20 7661 6c2e  rmissions": val.
+00006df0: 7065 726d 6973 7369 6f6e 737d 0a20 2020  permissions}.   
+00006e00: 2020 2020 2069 6620 7661 6c2e 636f 6d6d       if val.comm
+00006e10: 656e 7420 616e 6420 6368 6563 6b5f 6e6f  ent and check_no
+00006e20: 746e 6128 7661 6c2e 636f 6d6d 656e 7429  tna(val.comment)
+00006e30: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+00006e40: 6172 6773 5b22 636f 6d6d 656e 7422 5d20  args["comment"] 
+00006e50: 3d20 7661 6c2e 636f 6d6d 656e 740a 2020  = val.comment.  
+00006e60: 2020 2020 2020 7661 6c75 655f 203d 2065        value_ = e
+00006e70: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
+00006e80: 2020 2020 2020 2020 2020 227b 2573 7d64            "{%s}d
+00006e90: 6174 6522 2025 2078 6d6c 5f6e 616d 6573  ate" % xml_names
+00006ea0: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
+00006eb0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+00006ec0: 6172 6773 2c20 2023 2074 7970 653a 2069  args,  # type: i
+00006ed0: 676e 6f72 655b 6172 672d 7479 7065 5d0a  gnore[arg-type].
+00006ee0: 2020 2020 2020 2020 2020 2020 6e73 6d61              nsma
+00006ef0: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
+00006f00: 6d61 702c 0a20 2020 2020 2020 2029 0a20  map,.        ). 
+00006f10: 2020 2020 2020 2076 616c 7565 5f2e 7465         value_.te
+00006f20: 7874 203d 2073 7472 2876 616c 2e76 616c  xt = str(val.val
+00006f30: 7565 292e 7374 7269 7028 290a 2020 2020  ue).strip().    
+00006f40: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
+00006f50: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
+00006f60: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
+00006f70: 206d 616b 655f 6465 6369 6d61 6c5f 7072   make_decimal_pr
+00006f80: 6f70 280a 2020 2020 6e61 6d65 3a20 7374  op(.    name: st
+00006f90: 722c 0a20 2020 2076 616c 7565 3a20 556e  r,.    value: Un
+00006fa0: 696f 6e5b 5072 6f70 6572 7479 456c 656d  ion[PropertyElem
+00006fb0: 656e 742c 2073 7472 2c20 4974 6572 6162  ent, str, Iterab
+00006fc0: 6c65 5b55 6e69 6f6e 5b50 726f 7065 7274  le[Union[Propert
+00006fd0: 7945 6c65 6d65 6e74 2c20 7374 725d 5d5d  yElement, str]]]
+00006fe0: 2c0a 2020 2020 6361 6c6c 696e 675f 7265  ,.    calling_re
+00006ff0: 736f 7572 6365 3a20 7374 7220 3d20 2222  source: str = ""
+00007000: 2c0a 2920 2d3e 2065 7472 6565 2e5f 456c  ,.) -> etree._El
+00007010: 656d 656e 743a 0a20 2020 2022 2222 0a20  ement:.    """. 
+00007020: 2020 204d 616b 6520 6120 3c64 6563 696d     Make a <decim
+00007030: 616c 2d70 726f 703e 2066 726f 6d20 6f6e  al-prop> from on
+00007040: 6520 6f72 206d 6f72 6520 6465 6369 6d61  e or more decima
+00007050: 6c20 6e75 6d62 6572 732e 2054 6865 2064  l numbers. The d
+00007060: 6563 696d 616c 2873 2920 6361 6e20 6265  ecimal(s) can be
+00007070: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
+00007080: 696e 672c 2066 6c6f 6174 2c20 6f72 2061  ing, float, or a
+00007090: 730a 2020 2020 5072 6f70 6572 7479 456c  s.    PropertyEl
+000070a0: 656d 656e 7420 7769 7468 2061 2073 7472  ement with a str
+000070b0: 696e 672f 666c 6f61 7420 696e 7369 6465  ing/float inside
+000070c0: 2e20 4966 2070 726f 7669 6465 6420 6173  . If provided as
+000070d0: 2073 7472 696e 672f 666c 6f61 742c 2074   string/float, t
+000070e0: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
+000070f0: 6566 6175 6c74 2074 6f0a 2020 2020 2270  efault to.    "p
+00007100: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
+00007110: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00007120: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
+00007130: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
+00007140: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
+00007150: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
+00007160: 7661 6c75 653a 206f 6e65 206f 7220 6d6f  value: one or mo
+00007170: 7265 2064 6563 696d 616c 206e 756d 6265  re decimal numbe
+00007180: 7273 2c20 6173 2073 7472 696e 672f 666c  rs, as string/fl
+00007190: 6f61 742f 5072 6f70 6572 7479 456c 656d  oat/PropertyElem
+000071a0: 656e 742c 206f 7220 6173 2069 7465 7261  ent, or as itera
+000071b0: 626c 6520 6f66 2073 7472 696e 6773 2f50  ble of strings/P
+000071c0: 726f 7065 7274 7945 6c65 6d65 6e74 730a  ropertyElements.
+000071d0: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
+000071e0: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
+000071f0: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
+00007200: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
+00007210: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
+00007220: 6167 6573 290a 0a20 2020 2052 6169 7365  ages)..    Raise
+00007230: 733a 0a20 2020 2020 2020 2042 6173 6545  s:.        BaseE
+00007240: 7272 6f72 3a20 4966 2074 6865 2076 616c  rror: If the val
+00007250: 7565 2069 7320 6e6f 7420 6120 7661 6c69  ue is not a vali
+00007260: 6420 6465 6369 6d61 6c20 6e75 6d62 6572  d decimal number
+00007270: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+00007280: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
+00007290: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
+000072a0: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
+000072b0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+000072c0: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
+000072d0: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
+000072e0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
+000072f0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+00007300: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
+00007310: 2e6d 616b 655f 6465 6369 6d61 6c5f 7072  .make_decimal_pr
+00007320: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
+00007330: 7922 2c20 2233 2e31 3431 3539 2229 0a20  y", "3.14159"). 
+00007340: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007350: 6465 6369 6d61 6c2d 7072 6f70 206e 616d  decimal-prop nam
+00007360: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+00007370: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00007380: 2020 2020 2020 203c 6465 6369 6d61 6c20         <decimal 
+00007390: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+000073a0: 702d 6465 6661 756c 7422 3e33 2e31 3431  p-default">3.141
+000073b0: 3539 3c2f 6465 6369 6d61 6c3e 0a20 2020  59</decimal>.   
+000073c0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+000073d0: 6563 696d 616c 2d70 726f 703e 0a20 2020  ecimal-prop>.   
+000073e0: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+000073f0: 6d6c 2e6d 616b 655f 6465 6369 6d61 6c5f  ml.make_decimal_
+00007400: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
+00007410: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
+00007420: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
+00007430: 2233 2e31 3431 3539 222c 2070 6572 6d69  "3.14159", permi
+00007440: 7373 696f 6e73 3d22 7072 6f70 2d72 6573  ssions="prop-res
+00007450: 7472 6963 7465 6422 2c20 636f 6d6d 656e  tricted", commen
+00007460: 743d 2265 7861 6d70 6c65 2229 290a 2020  t="example")).  
+00007470: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00007480: 6563 696d 616c 2d70 726f 7020 6e61 6d65  ecimal-prop name
+00007490: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+000074a0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000074b0: 2020 2020 2020 3c64 6563 696d 616c 2070        <decimal p
+000074c0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+000074d0: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
+000074e0: 6d65 6e74 3d22 6578 616d 706c 6522 3e33  ment="example">3
+000074f0: 2e31 3431 3539 3c2f 6465 6369 6d61 6c3e  .14159</decimal>
+00007500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007510: 203c 2f64 6563 696d 616c 2d70 726f 703e   </decimal-prop>
+00007520: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
+00007530: 656c 3278 6d6c 2e6d 616b 655f 6465 6369  el2xml.make_deci
+00007540: 6d61 6c5f 7072 6f70 2822 3a74 6573 7470  mal_prop(":testp
+00007550: 726f 7065 7274 7922 2c20 5b22 332e 3134  roperty", ["3.14
+00007560: 3135 3922 2c20 2232 2e37 3138 225d 290a  159", "2.718"]).
+00007570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007580: 3c64 6563 696d 616c 2d70 726f 7020 6e61  <decimal-prop na
+00007590: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
+000075a0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
+000075b0: 2020 2020 2020 2020 3c64 6563 696d 616c          <decimal
+000075c0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+000075d0: 6f70 2d64 6566 6175 6c74 223e 332e 3134  op-default">3.14
+000075e0: 3135 393c 2f64 6563 696d 616c 3e0a 2020  159</decimal>.  
+000075f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007600: 2020 3c64 6563 696d 616c 2070 6572 6d69    <decimal permi
+00007610: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+00007620: 6175 6c74 223e 322e 3731 383c 2f64 6563  ault">2.718</dec
+00007630: 696d 616c 3e0a 2020 2020 2020 2020 2020  imal>.          
+00007640: 2020 2020 2020 3c2f 6465 6369 6d61 6c2d        </decimal-
+00007650: 7072 6f70 3e0a 0a20 2020 2053 6565 2068  prop>..    See h
+00007660: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
+00007670: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
+00007680: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
+00007690: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
+000076a0: 696c 652f 2364 6563 696d 616c 2d70 726f  ile/#decimal-pro
+000076b0: 700a 2020 2020 2222 220a 0a20 2020 2023  p.    """..    #
+000076c0: 2063 6865 636b 2074 6865 2069 6e70 7574   check the input
+000076d0: 3a20 7072 6570 6172 6520 6120 6c69 7374  : prepare a list
+000076e0: 2077 6974 6820 7661 6c69 6420 7661 6c75   with valid valu
+000076f0: 6573 0a20 2020 2076 616c 7565 7320 3d20  es.    values = 
+00007700: 7072 6570 6172 655f 7661 6c75 6528 7661  prepare_value(va
+00007710: 6c75 6529 0a0a 2020 2020 2320 6368 6563  lue)..    # chec
+00007720: 6b20 7661 6c75 6520 7479 7065 0a20 2020  k value type.   
+00007730: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
+00007740: 6573 3a0a 2020 2020 2020 2020 7472 793a  es:.        try:
+00007750: 0a20 2020 2020 2020 2020 2020 2066 6c6f  .            flo
+00007760: 6174 2876 616c 2e76 616c 7565 290a 2020  at(val.value).  
+00007770: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+00007780: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
+00007790: 2020 2020 2072 6169 7365 2042 6173 6545       raise BaseE
+000077a0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+000077b0: 2020 2020 2020 6622 4661 696c 6564 2076        f"Failed v
+000077c0: 616c 6964 6174 696f 6e20 696e 2072 6573  alidation in res
+000077d0: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
+000077e0: 7265 736f 7572 6365 7d27 2c20 7072 6f70  resource}', prop
+000077f0: 6572 7479 2027 7b6e 616d 657d 273a 2022  erty '{name}': "
+00007800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007810: 2066 2227 7b76 616c 2e76 616c 7565 7d27   f"'{val.value}'
+00007820: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
+00007830: 6465 6369 6d61 6c20 6e75 6d62 6572 2e22  decimal number."
+00007840: 0a20 2020 2020 2020 2020 2020 2029 2066  .            ) f
+00007850: 726f 6d20 4e6f 6e65 0a0a 2020 2020 2320  rom None..    # 
+00007860: 6d61 6b65 2078 6d6c 2073 7472 7563 7475  make xml structu
+00007870: 7265 206f 6620 7468 6520 7661 6c69 6420  re of the valid 
+00007880: 7661 6c75 6573 0a20 2020 2070 726f 705f  values.    prop_
+00007890: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+000078a0: 280a 2020 2020 2020 2020 227b 2573 7d64  (.        "{%s}d
+000078b0: 6563 696d 616c 2d70 726f 7022 2025 2078  ecimal-prop" % x
+000078c0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+000078d0: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+000078e0: 6e61 6d65 3d6e 616d 652c 0a20 2020 2020  name=name,.     
+000078f0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+00007900: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+00007910: 290a 2020 2020 666f 7220 7661 6c20 696e  ).    for val in
+00007920: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
+00007930: 206b 7761 7267 7320 3d20 7b22 7065 726d   kwargs = {"perm
+00007940: 6973 7369 6f6e 7322 3a20 7661 6c2e 7065  issions": val.pe
+00007950: 726d 6973 7369 6f6e 737d 0a20 2020 2020  rmissions}.     
+00007960: 2020 2069 6620 7661 6c2e 636f 6d6d 656e     if val.commen
+00007970: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
+00007980: 6128 7661 6c2e 636f 6d6d 656e 7429 3a0a  a(val.comment):.
+00007990: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+000079a0: 6773 5b22 636f 6d6d 656e 7422 5d20 3d20  gs["comment"] = 
+000079b0: 7661 6c2e 636f 6d6d 656e 740a 2020 2020  val.comment.    
+000079c0: 2020 2020 7661 6c75 655f 203d 2065 7472      value_ = etr
+000079d0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+000079e0: 2020 2020 2020 2020 227b 2573 7d64 6563          "{%s}dec
+000079f0: 696d 616c 2220 2520 786d 6c5f 6e61 6d65  imal" % xml_name
+00007a00: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
+00007a10: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00007a20: 7761 7267 732c 2020 2320 7479 7065 3a20  wargs,  # type: 
+00007a30: 6967 6e6f 7265 5b61 7267 2d74 7970 655d  ignore[arg-type]
+00007a40: 0a20 2020 2020 2020 2020 2020 206e 736d  .            nsm
+00007a50: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
+00007a60: 5f6d 6170 2c0a 2020 2020 2020 2020 290a  _map,.        ).
+00007a70: 2020 2020 2020 2020 7661 6c75 655f 2e74          value_.t
+00007a80: 6578 7420 3d20 7374 7228 666c 6f61 7428  ext = str(float(
+00007a90: 7661 6c2e 7661 6c75 6529 290a 2020 2020  val.value)).    
+00007aa0: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
+00007ab0: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
+00007ac0: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
+00007ad0: 206d 616b 655f 6765 6f6d 6574 7279 5f70   make_geometry_p
+00007ae0: 726f 7028 0a20 2020 206e 616d 653a 2073  rop(.    name: s
+00007af0: 7472 2c0a 2020 2020 7661 6c75 653a 2055  tr,.    value: U
+00007b00: 6e69 6f6e 5b50 726f 7065 7274 7945 6c65  nion[PropertyEle
+00007b10: 6d65 6e74 2c20 7374 722c 2049 7465 7261  ment, str, Itera
+00007b20: 626c 655b 556e 696f 6e5b 5072 6f70 6572  ble[Union[Proper
+00007b30: 7479 456c 656d 656e 742c 2073 7472 5d5d  tyElement, str]]
+00007b40: 5d2c 0a20 2020 2063 616c 6c69 6e67 5f72  ],.    calling_r
+00007b50: 6573 6f75 7263 653a 2073 7472 203d 2022  esource: str = "
+00007b60: 222c 0a29 202d 3e20 6574 7265 652e 5f45  ",.) -> etree._E
+00007b70: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
+00007b80: 2020 2020 4d61 6b65 2061 203c 6765 6f6d      Make a <geom
+00007b90: 6574 7279 2d70 726f 703e 2066 726f 6d20  etry-prop> from 
+00007ba0: 6f6e 6520 6f72 206d 6f72 6520 6172 6561  one or more area
+00007bb0: 7320 6f66 2061 6e20 696d 6167 652e 2054  s of an image. T
+00007bc0: 6865 2061 7265 6128 7329 2063 616e 2062  he area(s) can b
+00007bd0: 6520 7072 6f76 6964 6564 2061 7320 4a53  e provided as JS
+00007be0: 4f4e 2d73 7472 696e 6720 6f72 2061 730a  ON-string or as.
+00007bf0: 2020 2020 5072 6f70 6572 7479 456c 656d      PropertyElem
+00007c00: 656e 7420 7769 7468 2074 6865 204a 534f  ent with the JSO
+00007c10: 4e2d 7374 7269 6e67 2069 6e73 6964 652e  N-string inside.
+00007c20: 2049 6620 7072 6f76 6964 6564 2061 7320   If provided as 
+00007c30: 7374 7269 6e67 2c20 7468 6520 7065 726d  string, the perm
+00007c40: 6973 7369 6f6e 7320 6465 6661 756c 7420  issions default 
+00007c50: 746f 2022 7072 6f70 2d64 6566 6175 6c74  to "prop-default
+00007c60: 222e 0a0a 2020 2020 4172 6773 3a0a 2020  "...    Args:.  
+00007c70: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
+00007c80: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
+00007c90: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
+00007ca0: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
+00007cb0: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
+00007cc0: 6f72 206d 6f72 6520 4a53 4f4e 2067 656f  or more JSON geo
+00007cd0: 6d65 7472 7920 6f62 6a65 6374 732c 2061  metry objects, a
+00007ce0: 7320 7374 7269 6e67 2f50 726f 7065 7274  s string/Propert
+00007cf0: 7945 6c65 6d65 6e74 2c20 6f72 2061 7320  yElement, or as 
+00007d00: 6974 6572 6162 6c65 206f 6620 7374 7269  iterable of stri
+00007d10: 6e67 732f 5072 6f70 6572 7479 456c 656d  ngs/PropertyElem
+00007d20: 656e 7473 0a20 2020 2020 2020 2063 616c  ents.        cal
+00007d30: 6c69 6e67 5f72 6573 6f75 7263 653a 2074  ling_resource: t
+00007d40: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+00007d50: 6172 656e 7420 7265 736f 7572 6365 2028  arent resource (
+00007d60: 666f 7220 6265 7474 6572 2065 7272 6f72  for better error
+00007d70: 206d 6573 7361 6765 7329 0a0a 2020 2020   messages)..    
+00007d80: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00007d90: 4261 7365 4572 726f 723a 2049 6620 7468  BaseError: If th
+00007da0: 6520 7661 6c75 6520 6973 206e 6f74 2061  e value is not a
+00007db0: 2076 616c 6964 204a 534f 4e20 6765 6f6d   valid JSON geom
+00007dc0: 6574 7279 206f 626a 6563 740a 0a20 2020  etry object..   
+00007dd0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00007de0: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
+00007df0: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
+00007e00: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
+00007e10: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+00007e20: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
+00007e30: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
+00007e40: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
+00007e50: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+00007e60: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+00007e70: 5f67 656f 6d65 7472 795f 7072 6f70 2822  _geometry_prop("
+00007e80: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
+00007e90: 6a73 6f6e 5f73 7472 696e 6729 0a20 2020  json_string).   
+00007ea0: 2020 2020 2020 2020 2020 2020 203c 6765               <ge
+00007eb0: 6f6d 6574 7279 2d70 726f 7020 6e61 6d65  ometry-prop name
+00007ec0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+00007ed0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00007ee0: 2020 2020 2020 3c67 656f 6d65 7472 7920        <geometry 
+00007ef0: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+00007f00: 702d 6465 6661 756c 7422 3e7b 4a53 4f4e  p-default">{JSON
+00007f10: 7d3c 2f67 656f 6d65 7472 793e 0a20 2020  }</geometry>.   
+00007f20: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
+00007f30: 656f 6d65 7472 792d 7072 6f70 3e0a 2020  eometry-prop>.  
+00007f40: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00007f50: 786d 6c2e 6d61 6b65 5f67 656f 6d65 7472  xml.make_geometr
+00007f60: 795f 7072 6f70 2822 3a74 6573 7470 726f  y_prop(":testpro
+00007f70: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
+00007f80: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
+00007f90: 7428 6a73 6f6e 5f73 7472 696e 672c 2070  t(json_string, p
+00007fa0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+00007fb0: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
+00007fc0: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
+00007fd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007fe0: 2020 3c67 656f 6d65 7472 792d 7072 6f70    <geometry-prop
+00007ff0: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+00008000: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+00008010: 2020 2020 2020 2020 2020 203c 6765 6f6d             <geom
+00008020: 6574 7279 2070 6572 6d69 7373 696f 6e73  etry permissions
+00008030: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
+00008040: 6422 2063 6f6d 6d65 6e74 3d22 6578 616d  d" comment="exam
+00008050: 706c 6522 3e7b 4a53 4f4e 7d3c 2f67 656f  ple">{JSON}</geo
+00008060: 6d65 7472 793e 0a20 2020 2020 2020 2020  metry>.         
+00008070: 2020 2020 2020 203c 2f67 656f 6d65 7472         </geometr
+00008080: 792d 7072 6f70 3e0a 2020 2020 2020 2020  y-prop>.        
+00008090: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+000080a0: 6b65 5f67 656f 6d65 7472 795f 7072 6f70  ke_geometry_prop
+000080b0: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+000080c0: 2c20 5b6a 736f 6e5f 7374 7269 6e67 312c  , [json_string1,
+000080d0: 206a 736f 6e5f 7374 7269 6e67 325d 290a   json_string2]).
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 3c67 656f 6d65 7472 792d 7072 6f70 206e  <geometry-prop n
+00008100: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+00008110: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+00008120: 2020 2020 2020 2020 203c 6765 6f6d 6574           <geomet
+00008130: 7279 2070 6572 6d69 7373 696f 6e73 3d22  ry permissions="
+00008140: 7072 6f70 2d64 6566 6175 6c74 223e 7b4a  prop-default">{J
+00008150: 534f 4e7d 3c2f 6765 6f6d 6574 7279 3e0a  SON}</geometry>.
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 3c67 656f 6d65 7472 7920 7065      <geometry pe
+00008180: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+00008190: 6465 6661 756c 7422 3e7b 4a53 4f4e 7d3c  default">{JSON}<
+000081a0: 2f67 656f 6d65 7472 793e 0a20 2020 2020  /geometry>.     
+000081b0: 2020 2020 2020 2020 2020 203c 2f67 656f             </geo
+000081c0: 6d65 7472 792d 7072 6f70 3e0a 0a20 2020  metry-prop>..   
+000081d0: 2053 6565 2068 7474 7073 3a2f 2f64 6f63   See https://doc
+000081e0: 732e 6461 7363 682e 7377 6973 732f 6c61  s.dasch.swiss/la
+000081f0: 7465 7374 2f44 5350 2d54 4f4f 4c53 2f66  test/DSP-TOOLS/f
+00008200: 696c 652d 666f 726d 6174 732f 786d 6c2d  ile-formats/xml-
+00008210: 6461 7461 2d66 696c 652f 2367 656f 6d65  data-file/#geome
+00008220: 7472 792d 7072 6f70 0a20 2020 2022 2222  try-prop.    """
+00008230: 0a0a 2020 2020 2320 6368 6563 6b20 7468  ..    # check th
+00008240: 6520 696e 7075 743a 2070 7265 7061 7265  e input: prepare
+00008250: 2061 206c 6973 7420 7769 7468 2076 616c   a list with val
+00008260: 6964 2076 616c 7565 730a 2020 2020 7661  id values.    va
+00008270: 6c75 6573 203d 2070 7265 7061 7265 5f76  lues = prepare_v
+00008280: 616c 7565 2876 616c 7565 290a 0a20 2020  alue(value)..   
+00008290: 2023 2063 6865 636b 2076 616c 7565 2074   # check value t
+000082a0: 7970 650a 2020 2020 666f 7220 7661 6c20  ype.    for val 
+000082b0: 696e 2076 616c 7565 733a 0a20 2020 2020  in values:.     
+000082c0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000082d0: 2020 2020 7661 6c75 655f 6173 5f64 6963      value_as_dic
+000082e0: 7420 3d20 6a73 6f6e 2e6c 6f61 6473 2873  t = json.loads(s
+000082f0: 7472 2876 616c 2e76 616c 7565 2929 0a20  tr(val.value)). 
+00008300: 2020 2020 2020 2020 2020 2069 6620 7661             if va
+00008310: 6c75 655f 6173 5f64 6963 745b 2274 7970  lue_as_dict["typ
+00008320: 6522 5d20 6e6f 7420 696e 205b 2272 6563  e"] not in ["rec
+00008330: 7461 6e67 6c65 222c 2022 6369 7263 6c65  tangle", "circle
+00008340: 222c 2022 706f 6c79 676f 6e22 5d3a 0a20  ", "polygon"]:. 
+00008350: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00008360: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
+00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008380: 2020 2020 6622 4661 696c 6564 2076 616c      f"Failed val
+00008390: 6964 6174 696f 6e20 696e 2072 6573 6f75  idation in resou
+000083a0: 7263 6520 277b 6361 6c6c 696e 675f 7265  rce '{calling_re
+000083b0: 736f 7572 6365 7d27 2c20 7072 6f70 6572  source}', proper
+000083c0: 7479 2027 7b6e 616d 657d 273a 2022 0a20  ty '{name}': ". 
+000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083e0: 2020 2066 2254 6865 2027 7479 7065 2720     f"The 'type' 
+000083f0: 6f66 2074 6865 204a 534f 4e20 6765 6f6d  of the JSON geom
+00008400: 6574 7279 206f 626a 6563 7420 6d75 7374  etry object must
+00008410: 2062 6520 2772 6563 7461 6e67 6c65 272c   be 'rectangle',
+00008420: 2027 6369 7263 6c65 272c 206f 7220 2770   'circle', or 'p
+00008430: 6f6c 7967 6f6e 272e 220a 2020 2020 2020  olygon'.".      
+00008440: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008450: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00008460: 7369 6e73 7461 6e63 6528 7661 6c75 655f  sinstance(value_
+00008470: 6173 5f64 6963 745b 2270 6f69 6e74 7322  as_dict["points"
+00008480: 5d2c 206c 6973 7429 3a0a 2020 2020 2020  ], list):.      
+00008490: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000084a0: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000084c0: 2246 6169 6c65 6420 7661 6c69 6461 7469  "Failed validati
+000084d0: 6f6e 2069 6e20 7265 736f 7572 6365 2027  on in resource '
+000084e0: 7b63 616c 6c69 6e67 5f72 6573 6f75 7263  {calling_resourc
+000084f0: 657d 272c 2070 726f 7065 7274 7920 277b  e}', property '{
+00008500: 6e61 6d65 7d27 3a20 220a 2020 2020 2020  name}': ".      
+00008510: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00008520: 5468 6520 2770 6f69 6e74 7327 6f66 2074  The 'points'of t
+00008530: 6865 204a 534f 4e20 6765 6f6d 6574 7279  he JSON geometry
+00008540: 206f 626a 6563 7420 6d75 7374 2062 6520   object must be 
+00008550: 6120 6c69 7374 206f 6620 706f 696e 7473  a list of points
+00008560: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00008570: 2020 2029 0a20 2020 2020 2020 2065 7863     ).        exc
+00008580: 6570 7420 286a 736f 6e2e 4a53 4f4e 4465  ept (json.JSONDe
+00008590: 636f 6465 4572 726f 722c 2054 7970 6545  codeError, TypeE
+000085a0: 7272 6f72 2c20 496e 6465 7845 7272 6f72  rror, IndexError
+000085b0: 2c20 4b65 7945 7272 6f72 2c20 4173 7365  , KeyError, Asse
+000085c0: 7274 696f 6e45 7272 6f72 293a 0a20 2020  rtionError):.   
+000085d0: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
+000085e0: 6173 6545 7272 6f72 280a 2020 2020 2020  aseError(.      
+000085f0: 2020 2020 2020 2020 2020 6622 4661 696c            f"Fail
+00008600: 6564 2076 616c 6964 6174 696f 6e20 696e  ed validation in
+00008610: 2072 6573 6f75 7263 6520 277b 6361 6c6c   resource '{call
+00008620: 696e 675f 7265 736f 7572 6365 7d27 2c20  ing_resource}', 
+00008630: 7072 6f70 6572 7479 2027 7b6e 616d 657d  property '{name}
+00008640: 273a 2022 0a20 2020 2020 2020 2020 2020  ': ".           
+00008650: 2020 2020 2066 2227 7b76 616c 2e76 616c       f"'{val.val
+00008660: 7565 7d27 2069 7320 6e6f 7420 6120 7661  ue}' is not a va
+00008670: 6c69 6420 4a53 4f4e 2067 656f 6d65 7472  lid JSON geometr
+00008680: 7920 6f62 6a65 6374 2e22 0a20 2020 2020  y object.".     
+00008690: 2020 2020 2020 2029 2066 726f 6d20 4e6f         ) from No
+000086a0: 6e65 0a0a 2020 2020 2320 6d61 6b65 2078  ne..    # make x
+000086b0: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
+000086c0: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
+000086d0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
+000086e0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+000086f0: 2020 2020 227b 2573 7d67 656f 6d65 7472      "{%s}geometr
+00008700: 792d 7072 6f70 2220 2520 786d 6c5f 6e61  y-prop" % xml_na
+00008710: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
+00008720: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
+00008730: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
+00008740: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
+00008750: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
+00008760: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
+00008770: 6573 3a0a 2020 2020 2020 2020 6b77 6172  es:.        kwar
+00008780: 6773 203d 207b 2270 6572 6d69 7373 696f  gs = {"permissio
+00008790: 6e73 223a 2076 616c 2e70 6572 6d69 7373  ns": val.permiss
+000087a0: 696f 6e73 7d0a 2020 2020 2020 2020 6966  ions}.        if
+000087b0: 2076 616c 2e63 6f6d 6d65 6e74 2061 6e64   val.comment and
+000087c0: 2063 6865 636b 5f6e 6f74 6e61 2876 616c   check_notna(val
+000087d0: 2e63 6f6d 6d65 6e74 293a 0a20 2020 2020  .comment):.     
+000087e0: 2020 2020 2020 206b 7761 7267 735b 2263         kwargs["c
+000087f0: 6f6d 6d65 6e74 225d 203d 2076 616c 2e63  omment"] = val.c
+00008800: 6f6d 6d65 6e74 0a20 2020 2020 2020 2076  omment.        v
+00008810: 616c 7565 5f20 3d20 6574 7265 652e 456c  alue_ = etree.El
+00008820: 656d 656e 7428 0a20 2020 2020 2020 2020  ement(.         
+00008830: 2020 2022 7b25 737d 6765 6f6d 6574 7279     "{%s}geometry
+00008840: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
+00008850: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
+00008860: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+00008870: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
+00008880: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
+00008890: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
+000088a0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+000088b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000088c0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
+000088d0: 3d20 7374 7228 7661 6c2e 7661 6c75 6529  = str(val.value)
+000088e0: 0a20 2020 2020 2020 2070 726f 705f 2e61  .        prop_.a
+000088f0: 7070 656e 6428 7661 6c75 655f 290a 2020  ppend(value_).  
+00008900: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+00008910: 0a64 6566 206d 616b 655f 6765 6f6e 616d  .def make_geonam
+00008920: 655f 7072 6f70 280a 2020 2020 6e61 6d65  e_prop(.    name
+00008930: 3a20 7374 722c 0a20 2020 2076 616c 7565  : str,.    value
+00008940: 3a20 556e 696f 6e5b 5072 6f70 6572 7479  : Union[Property
+00008950: 456c 656d 656e 742c 2073 7472 2c20 696e  Element, str, in
+00008960: 742c 2049 7465 7261 626c 655b 556e 696f  t, Iterable[Unio
+00008970: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
+00008980: 742c 2073 7472 2c20 696e 745d 5d5d 2c0a  t, str, int]]],.
+00008990: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+000089a0: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
+000089b0: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
+000089c0: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
+000089d0: 204d 616b 6520 6120 3c67 656f 6e61 6d65   Make a <geoname
+000089e0: 2d70 726f 703e 2066 726f 6d20 6f6e 6520  -prop> from one 
+000089f0: 6f72 206d 6f72 6520 6765 6f6e 616d 6573  or more geonames
+00008a00: 2e6f 7267 2049 4473 2e20 5468 6520 4944  .org IDs. The ID
+00008a10: 2873 2920 6361 6e20 6265 2070 726f 7669  (s) can be provi
+00008a20: 6465 6420 6173 2073 7472 696e 672c 2069  ded as string, i
+00008a30: 6e74 6567 6572 2c20 6f72 2061 730a 2020  nteger, or as.  
+00008a40: 2020 5072 6f70 6572 7479 456c 656d 656e    PropertyElemen
+00008a50: 7420 7769 7468 2061 2073 7472 696e 672f  t with a string/
+00008a60: 696e 7465 6765 7220 696e 7369 6465 2e20  integer inside. 
+00008a70: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
+00008a80: 7472 696e 672f 696e 7465 6765 722c 2074  tring/integer, t
+00008a90: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
+00008aa0: 6566 6175 6c74 2074 6f0a 2020 2020 2270  efault to.    "p
+00008ab0: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
+00008ac0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00008ad0: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
+00008ae0: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
+00008af0: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
+00008b00: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
+00008b10: 7661 6c75 653a 206f 6e65 206f 7220 6d6f  value: one or mo
+00008b20: 7265 2067 656f 6e61 6d65 732e 6f72 6720  re geonames.org 
+00008b30: 4944 732c 2061 7320 7374 722f 696e 742f  IDs, as str/int/
+00008b40: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
+00008b50: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
+00008b60: 6f66 2073 7472 2f69 6e74 2f50 726f 7065  of str/int/Prope
+00008b70: 7274 7945 6c65 6d65 6e74 0a20 2020 2020  rtyElement.     
+00008b80: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+00008b90: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
+00008ba0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+00008bb0: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
+00008bc0: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
+00008bd0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+00008be0: 2020 2020 2020 4261 7365 4572 726f 723a        BaseError:
+00008bf0: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00008c00: 206e 6f74 2061 2076 616c 6964 2067 656f   not a valid geo
+00008c10: 6e61 6d65 732e 6f72 6720 6964 656e 7469  names.org identi
+00008c20: 6669 6572 0a0a 2020 2020 5265 7475 726e  fier..    Return
+00008c30: 733a 0a20 2020 2020 2020 2061 6e20 6574  s:.        an et
+00008c40: 7265 652e 5f45 6c65 6d65 6e74 2074 6861  ree._Element tha
+00008c50: 7420 6361 6e20 6265 2061 7070 656e 6465  t can be appende
+00008c60: 6420 746f 2074 6865 2070 6172 656e 7420  d to the parent 
+00008c70: 7265 736f 7572 6365 2077 6974 6820 7265  resource with re
+00008c80: 736f 7572 6365 2e61 7070 656e 6428 6d61  source.append(ma
+00008c90: 6b65 5f2a 5f70 726f 7028 2e2e 2e29 290a  ke_*_prop(...)).
+00008ca0: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
+00008cb0: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
+00008cc0: 3278 6d6c 2e6d 616b 655f 6765 6f6e 616d  2xml.make_geonam
+00008cd0: 655f 7072 6f70 2822 3a74 6573 7470 726f  e_prop(":testpro
+00008ce0: 7065 7274 7922 2c20 2232 3736 3133 3639  perty", "2761369
+00008cf0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00008d00: 2020 203c 6765 6f6e 616d 652d 7072 6f70     <geoname-prop
+00008d10: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+00008d20: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+00008d30: 2020 2020 2020 2020 2020 203c 6765 6f6e             <geon
+00008d40: 616d 6520 7065 726d 6973 7369 6f6e 733d  ame permissions=
+00008d50: 2270 726f 702d 6465 6661 756c 7422 3e32  "prop-default">2
+00008d60: 3736 3133 3639 3c2f 6765 6f6e 616d 653e  761369</geoname>
+00008d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d80: 203c 2f67 656f 6e61 6d65 2d70 726f 703e   </geoname-prop>
+00008d90: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
+00008da0: 656c 3278 6d6c 2e6d 616b 655f 6765 6f6e  el2xml.make_geon
+00008db0: 616d 655f 7072 6f70 2822 3a74 6573 7470  ame_prop(":testp
+00008dc0: 726f 7065 7274 7922 2c20 6578 6365 6c32  roperty", excel2
+00008dd0: 786d 6c2e 5072 6f70 6572 7479 456c 656d  xml.PropertyElem
+00008de0: 656e 7428 2232 3736 3133 3639 222c 2070  ent("2761369", p
+00008df0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+00008e00: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
+00008e10: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
+00008e20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00008e30: 2020 3c67 656f 6e61 6d65 2d70 726f 7020    <geoname-prop 
+00008e40: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
+00008e50: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
+00008e60: 2020 2020 2020 2020 2020 3c67 656f 6e61            <geona
+00008e70: 6d65 2070 6572 6d69 7373 696f 6e73 3d22  me permissions="
+00008e80: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+00008e90: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
+00008ea0: 6522 3e32 3736 3133 3639 3c2f 6765 6f6e  e">2761369</geon
+00008eb0: 616d 653e 0a20 2020 2020 2020 2020 2020  ame>.           
+00008ec0: 2020 2020 203c 2f67 656f 6e61 6d65 2d70       </geoname-p
+00008ed0: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
+00008ee0: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+00008ef0: 6765 6f6e 616d 655f 7072 6f70 2822 3a74  geoname_prop(":t
+00008f00: 6573 7470 726f 7065 7274 7922 2c20 5b22  estproperty", ["
+00008f10: 3237 3631 3336 3922 2c20 2231 3031 3031  2761369", "10101
+00008f20: 3031 225d 290a 2020 2020 2020 2020 2020  01"]).          
+00008f30: 2020 2020 2020 3c67 656f 6e61 6d65 2d70        <geoname-p
+00008f40: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
+00008f50: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
+00008f60: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
+00008f70: 656f 6e61 6d65 2070 6572 6d69 7373 696f  eoname permissio
+00008f80: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
+00008f90: 223e 3237 3631 3336 393c 2f67 656f 6e61  ">2761369</geona
+00008fa0: 6d65 3e0a 2020 2020 2020 2020 2020 2020  me>.            
+00008fb0: 2020 2020 2020 2020 3c67 656f 6e61 6d65          <geoname
+00008fc0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+00008fd0: 6f70 2d64 6566 6175 6c74 223e 3130 3130  op-default">1010
+00008fe0: 3130 313c 2f67 656f 6e61 6d65 3e0a 2020  101</geoname>.  
+00008ff0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00009000: 6765 6f6e 616d 652d 7072 6f70 3e0a 0a20  geoname-prop>.. 
+00009010: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
+00009020: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
+00009030: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
+00009040: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
+00009050: 6c2d 6461 7461 2d66 696c 652f 2367 656f  l-data-file/#geo
+00009060: 6e61 6d65 2d70 726f 700a 2020 2020 2222  name-prop.    ""
+00009070: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
+00009080: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
+00009090: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
+000090a0: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
+000090b0: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
+000090c0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
+000090d0: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
+000090e0: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
+000090f0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+00009100: 2020 2020 6966 206e 6f74 2072 6567 6578      if not regex
+00009110: 2e73 6561 7263 6828 7222 5e5b 302d 395d  .search(r"^[0-9]
+00009120: 2b24 222c 2073 7472 2876 616c 2e76 616c  +$", str(val.val
+00009130: 7565 2929 3a0a 2020 2020 2020 2020 2020  ue)):.          
+00009140: 2020 7261 6973 6520 4261 7365 4572 726f    raise BaseErro
+00009150: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00009160: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
+00009170: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
+00009180: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
+00009190: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
+000091a0: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
+000091b0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000091c0: 277b 7661 6c2e 7661 6c75 657d 2720 6973  '{val.value}' is
+000091d0: 206e 6f74 2061 2067 656f 6e61 6d65 732e   not a geonames.
+000091e0: 6f72 6720 6964 656e 7469 6669 6572 2e22  org identifier."
+000091f0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00009200: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
+00009210: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+00009220: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+00009230: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
+00009240: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+00009250: 227b 2573 7d67 656f 6e61 6d65 2d70 726f  "{%s}geoname-pro
+00009260: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+00009270: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+00009280: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+00009290: 0a20 2020 2020 2020 206e 736d 6170 3d78  .        nsmap=x
+000092a0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+000092b0: 2c0a 2020 2020 290a 2020 2020 666f 7220  ,.    ).    for 
+000092c0: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+000092d0: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+000092e0: 7b22 7065 726d 6973 7369 6f6e 7322 3a20  {"permissions": 
+000092f0: 7661 6c2e 7065 726d 6973 7369 6f6e 737d  val.permissions}
+00009300: 0a20 2020 2020 2020 2069 6620 7661 6c2e  .        if val.
+00009310: 636f 6d6d 656e 7420 616e 6420 6368 6563  comment and chec
+00009320: 6b5f 6e6f 746e 6128 7661 6c2e 636f 6d6d  k_notna(val.comm
+00009330: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
+00009340: 2020 6b77 6172 6773 5b22 636f 6d6d 656e    kwargs["commen
+00009350: 7422 5d20 3d20 7661 6c2e 636f 6d6d 656e  t"] = val.commen
+00009360: 740a 2020 2020 2020 2020 7661 6c75 655f  t.        value_
+00009370: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+00009380: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+00009390: 2573 7d67 656f 6e61 6d65 2220 2520 786d  %s}geoname" % xm
+000093a0: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
+000093b0: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
+000093c0: 2020 202a 2a6b 7761 7267 732c 2020 2320     **kwargs,  # 
+000093d0: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
+000093e0: 2d74 7970 655d 0a20 2020 2020 2020 2020  -type].         
+000093f0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+00009400: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+00009410: 2020 2020 290a 2020 2020 2020 2020 7661      ).        va
+00009420: 6c75 655f 2e74 6578 7420 3d20 7374 7228  lue_.text = str(
+00009430: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
+00009440: 2020 2070 726f 705f 2e61 7070 656e 6428     prop_.append(
+00009450: 7661 6c75 655f 290a 0a20 2020 2072 6574  value_)..    ret
+00009460: 7572 6e20 7072 6f70 5f0a 0a0a 6465 6620  urn prop_...def 
+00009470: 6d61 6b65 5f69 6e74 6567 6572 5f70 726f  make_integer_pro
+00009480: 7028 0a20 2020 206e 616d 653a 2073 7472  p(.    name: str
+00009490: 2c0a 2020 2020 7661 6c75 653a 2055 6e69  ,.    value: Uni
+000094a0: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
+000094b0: 6e74 2c20 7374 722c 2069 6e74 2c20 4974  nt, str, int, It
+000094c0: 6572 6162 6c65 5b55 6e69 6f6e 5b50 726f  erable[Union[Pro
+000094d0: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
+000094e0: 722c 2069 6e74 5d5d 5d2c 0a20 2020 2063  r, int]]],.    c
+000094f0: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
+00009500: 2073 7472 203d 2022 222c 0a29 202d 3e20   str = "",.) -> 
+00009510: 6574 7265 652e 5f45 6c65 6d65 6e74 3a0a  etree._Element:.
+00009520: 2020 2020 2222 220a 2020 2020 4d61 6b65      """.    Make
+00009530: 2061 203c 696e 7465 6765 722d 7072 6f70   a <integer-prop
+00009540: 3e20 6672 6f6d 206f 6e65 206f 7220 6d6f  > from one or mo
+00009550: 7265 2069 6e74 6567 6572 732e 2054 6865  re integers. The
+00009560: 2069 6e74 6567 6572 7320 6361 6e20 6265   integers can be
+00009570: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
+00009580: 696e 672c 2069 6e74 6567 6572 2c20 6f72  ing, integer, or
+00009590: 2061 730a 2020 2020 5072 6f70 6572 7479   as.    Property
+000095a0: 456c 656d 656e 7420 7769 7468 2061 2073  Element with a s
+000095b0: 7472 696e 672f 696e 7465 6765 7220 696e  tring/integer in
+000095c0: 7369 6465 2e20 4966 2070 726f 7669 6465  side. If provide
+000095d0: 6420 6173 2073 7472 696e 672f 696e 7465  d as string/inte
+000095e0: 6765 722c 2074 6865 2070 6572 6d69 7373  ger, the permiss
+000095f0: 696f 6e73 2064 6566 6175 6c74 2074 6f0a  ions default to.
+00009600: 2020 2020 2270 726f 702d 6465 6661 756c      "prop-defaul
+00009610: 7422 2e0a 0a20 2020 2041 7267 733a 0a20  t"...    Args:. 
+00009620: 2020 2020 2020 206e 616d 653a 2074 6865         name: the
+00009630: 206e 616d 6520 6f66 2074 6869 7320 7072   name of this pr
+00009640: 6f70 6572 7479 2061 7320 6465 6669 6e65  operty as define
+00009650: 6420 696e 2074 6865 206f 6e74 6f0a 2020  d in the onto.  
+00009660: 2020 2020 2020 7661 6c75 653a 206f 6e65        value: one
+00009670: 206f 7220 6d6f 7265 2069 6e74 6567 6572   or more integer
+00009680: 732c 2061 7320 7374 7269 6e67 2f69 6e74  s, as string/int
+00009690: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
+000096a0: 2c20 6f72 2061 7320 6974 6572 6162 6c65  , or as iterable
+000096b0: 206f 6620 7374 7269 6e67 732f 696e 7473   of strings/ints
+000096c0: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
+000096d0: 730a 2020 2020 2020 2020 6361 6c6c 696e  s.        callin
+000096e0: 675f 7265 736f 7572 6365 3a20 7468 6520  g_resource: the 
+000096f0: 6e61 6d65 206f 6620 7468 6520 7061 7265  name of the pare
+00009700: 6e74 2072 6573 6f75 7263 6520 2866 6f72  nt resource (for
+00009710: 2062 6574 7465 7220 6572 726f 7220 6d65   better error me
+00009720: 7373 6167 6573 290a 0a20 2020 2052 6169  ssages)..    Rai
+00009730: 7365 733a 0a20 2020 2020 2020 2042 6173  ses:.        Bas
+00009740: 6545 7272 6f72 3a20 4966 2074 6865 2076  eError: If the v
+00009750: 616c 7565 2069 7320 6e6f 7420 6120 7661  alue is not a va
+00009760: 6c69 6420 696e 7465 6765 720a 0a20 2020  lid integer..   
+00009770: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00009780: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
+00009790: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
+000097a0: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
+000097b0: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+000097c0: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
+000097d0: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
+000097e0: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
+000097f0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+00009800: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+00009810: 5f69 6e74 6567 6572 5f70 726f 7028 223a  _integer_prop(":
+00009820: 7465 7374 7072 6f70 6572 7479 222c 2022  testproperty", "
+00009830: 3237 3631 3336 3922 290a 2020 2020 2020  2761369").      
+00009840: 2020 2020 2020 2020 2020 3c69 6e74 6567            <integ
+00009850: 6572 2d70 726f 7020 6e61 6d65 3d22 3a74  er-prop name=":t
+00009860: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 2020 3c69 6e74 6567 6572 2070 6572 6d69    <integer permi
+00009890: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+000098a0: 6175 6c74 223e 3237 3631 3336 393c 2f69  ault">2761369</i
+000098b0: 6e74 6567 6572 3e0a 2020 2020 2020 2020  nteger>.        
+000098c0: 2020 2020 2020 2020 3c2f 696e 7465 6765          </intege
+000098d0: 722d 7072 6f70 3e0a 2020 2020 2020 2020  r-prop>.        
+000098e0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+000098f0: 6b65 5f69 6e74 6567 6572 5f70 726f 7028  ke_integer_prop(
+00009900: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
+00009910: 2065 7863 656c 3278 6d6c 2e50 726f 7065   excel2xml.Prope
+00009920: 7274 7945 6c65 6d65 6e74 2822 3237 3631  rtyElement("2761
+00009930: 3336 3922 2c20 7065 726d 6973 7369 6f6e  369", permission
+00009940: 733d 2270 726f 702d 7265 7374 7269 6374  s="prop-restrict
+00009950: 6564 222c 2063 6f6d 6d65 6e74 3d22 6578  ed", comment="ex
+00009960: 616d 706c 6522 2929 0a20 2020 2020 2020  ample")).       
+00009970: 2020 2020 2020 2020 203c 696e 7465 6765           <intege
+00009980: 722d 7072 6f70 206e 616d 653d 223a 7465  r-prop name=":te
+00009990: 7374 7072 6f70 6572 7479 223e 0a20 2020  stproperty">.   
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 203c 696e 7465 6765 7220 7065 726d 6973   <integer permis
+000099c0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+000099d0: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
+000099e0: 2265 7861 6d70 6c65 223e 3237 3631 3336  "example">276136
+000099f0: 393c 2f69 6e74 6567 6572 3e0a 2020 2020  9</integer>.    
+00009a00: 2020 2020 2020 2020 2020 2020 3c2f 696e              </in
+00009a10: 7465 6765 722d 7072 6f70 3e0a 2020 2020  teger-prop>.    
+00009a20: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+00009a30: 6c2e 6d61 6b65 5f69 6e74 6567 6572 5f70  l.make_integer_p
+00009a40: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+00009a50: 7479 222c 205b 2232 3736 3133 3639 222c  ty", ["2761369",
+00009a60: 2022 3130 3130 3130 3122 5d29 0a20 2020   "1010101"]).   
+00009a70: 2020 2020 2020 2020 2020 2020 203c 696e               <in
+00009a80: 7465 6765 722d 7072 6f70 206e 616d 653d  teger-prop name=
+00009a90: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+00009aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009ab0: 2020 2020 203c 696e 7465 6765 7220 7065       <integer pe
+00009ac0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+00009ad0: 6465 6661 756c 7422 3e32 3736 3133 3639  default">2761369
+00009ae0: 3c2f 696e 7465 6765 723e 0a20 2020 2020  </integer>.     
+00009af0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00009b00: 696e 7465 6765 7220 7065 726d 6973 7369  integer permissi
+00009b10: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
+00009b20: 7422 3e31 3031 3031 3031 3c2f 696e 7465  t">1010101</inte
+00009b30: 6765 723e 0a20 2020 2020 2020 2020 2020  ger>.           
+00009b40: 2020 2020 203c 2f69 6e74 6567 6572 2d70       </integer-p
+00009b50: 726f 703e 0a0a 2020 2020 5365 6520 6874  rop>..    See ht
+00009b60: 7470 733a 2f2f 646f 6373 2e64 6173 6368  tps://docs.dasch
+00009b70: 2e73 7769 7373 2f6c 6174 6573 742f 4453  .swiss/latest/DS
+00009b80: 502d 544f 4f4c 532f 6669 6c65 2d66 6f72  P-TOOLS/file-for
+00009b90: 6d61 7473 2f78 6d6c 2d64 6174 612d 6669  mats/xml-data-fi
+00009ba0: 6c65 2f23 696e 7465 6765 722d 7072 6f70  le/#integer-prop
+00009bb0: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+00009bc0: 6368 6563 6b20 7468 6520 696e 7075 743a  check the input:
+00009bd0: 2070 7265 7061 7265 2061 206c 6973 7420   prepare a list 
+00009be0: 7769 7468 2076 616c 6964 2076 616c 7565  with valid value
+00009bf0: 730a 2020 2020 7661 6c75 6573 203d 2070  s.    values = p
+00009c00: 7265 7061 7265 5f76 616c 7565 2876 616c  repare_value(val
+00009c10: 7565 290a 0a20 2020 2023 2063 6865 636b  ue)..    # check
+00009c20: 2076 616c 7565 2074 7970 650a 2020 2020   value type.    
+00009c30: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
+00009c40: 733a 0a20 2020 2020 2020 2074 7279 3a0a  s:.        try:.
+00009c50: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+00009c60: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
+00009c70: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+00009c80: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+00009c90: 2020 7261 6973 6520 4261 7365 4572 726f    raise BaseErro
+00009ca0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00009cb0: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
+00009cc0: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
+00009cd0: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
+00009ce0: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
+00009cf0: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
+00009d00: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00009d10: 277b 7661 6c2e 7661 6c75 657d 2720 6973  '{val.value}' is
+00009d20: 206e 6f74 2061 2076 616c 6964 2069 6e74   not a valid int
+00009d30: 6567 6572 2e22 0a20 2020 2020 2020 2020  eger.".         
+00009d40: 2020 2029 2066 726f 6d20 4e6f 6e65 0a0a     ) from None..
+00009d50: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
+00009d60: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+00009d70: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+00009d80: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
+00009d90: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+00009da0: 227b 2573 7d69 6e74 6567 6572 2d70 726f  "{%s}integer-pro
+00009db0: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+00009dc0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+00009dd0: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+00009de0: 0a20 2020 2020 2020 206e 736d 6170 3d78  .        nsmap=x
+00009df0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+00009e00: 2c0a 2020 2020 290a 2020 2020 666f 7220  ,.    ).    for 
+00009e10: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+00009e20: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+00009e30: 7b22 7065 726d 6973 7369 6f6e 7322 3a20  {"permissions": 
+00009e40: 7661 6c2e 7065 726d 6973 7369 6f6e 737d  val.permissions}
+00009e50: 0a20 2020 2020 2020 2069 6620 7661 6c2e  .        if val.
+00009e60: 636f 6d6d 656e 7420 616e 6420 6368 6563  comment and chec
+00009e70: 6b5f 6e6f 746e 6128 7661 6c2e 636f 6d6d  k_notna(val.comm
+00009e80: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
+00009e90: 2020 6b77 6172 6773 5b22 636f 6d6d 656e    kwargs["commen
+00009ea0: 7422 5d20 3d20 7661 6c2e 636f 6d6d 656e  t"] = val.commen
+00009eb0: 740a 2020 2020 2020 2020 7661 6c75 655f  t.        value_
+00009ec0: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+00009ed0: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+00009ee0: 2573 7d69 6e74 6567 6572 2220 2520 786d  %s}integer" % xm
+00009ef0: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
+00009f00: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
+00009f10: 2020 202a 2a6b 7761 7267 732c 2020 2320     **kwargs,  # 
+00009f20: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
+00009f30: 2d74 7970 655d 0a20 2020 2020 2020 2020  -type].         
+00009f40: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+00009f50: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+00009f60: 2020 2020 290a 2020 2020 2020 2020 7661      ).        va
+00009f70: 6c75 655f 2e74 6578 7420 3d20 7374 7228  lue_.text = str(
+00009f80: 696e 7428 7661 6c2e 7661 6c75 6529 290a  int(val.value)).
+00009f90: 2020 2020 2020 2020 7072 6f70 5f2e 6170          prop_.ap
+00009fa0: 7065 6e64 2876 616c 7565 5f29 0a0a 2020  pend(value_)..  
+00009fb0: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+00009fc0: 0a64 6566 206d 616b 655f 696e 7465 7276  .def make_interv
+00009fd0: 616c 5f70 726f 7028 0a20 2020 206e 616d  al_prop(.    nam
+00009fe0: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
+00009ff0: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
+0000a000: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
+0000a010: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
+0000a020: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
+0000a030: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
+0000a040: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
+0000a050: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
+0000a060: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
+0000a070: 2222 220a 2020 2020 4d61 6b65 2061 203c  """.    Make a <
+0000a080: 696e 7465 7276 616c 2d70 726f 703e 2066  interval-prop> f
+0000a090: 726f 6d20 6f6e 6520 6f72 206d 6f72 6520  rom one or more 
+0000a0a0: 4453 5020 696e 7465 7276 616c 732e 2054  DSP intervals. T
+0000a0b0: 6865 2069 6e74 6572 7661 6c28 7329 2063  he interval(s) c
+0000a0c0: 616e 2062 6520 7072 6f76 6964 6564 2061  an be provided a
+0000a0d0: 7320 7374 7269 6e67 206f 7220 6173 0a20  s string or as. 
+0000a0e0: 2020 2050 726f 7065 7274 7945 6c65 6d65     PropertyEleme
+0000a0f0: 6e74 2077 6974 6820 6120 7374 7269 6e67  nt with a string
+0000a100: 2069 6e73 6964 652e 2049 6620 7072 6f76   inside. If prov
+0000a110: 6964 6564 2061 7320 7374 7269 6e67 2c20  ided as string, 
+0000a120: 7468 6520 7065 726d 6973 7369 6f6e 7320  the permissions 
+0000a130: 6465 6661 756c 7420 746f 2022 7072 6f70  default to "prop
+0000a140: 2d64 6566 6175 6c74 222e 0a0a 2020 2020  -default"...    
+0000a150: 4172 6773 3a0a 2020 2020 2020 2020 6e61  Args:.        na
+0000a160: 6d65 3a20 7468 6520 6e61 6d65 206f 6620  me: the name of 
+0000a170: 7468 6973 2070 726f 7065 7274 7920 6173  this property as
+0000a180: 2064 6566 696e 6564 2069 6e20 7468 6520   defined in the 
+0000a190: 6f6e 746f 0a20 2020 2020 2020 2076 616c  onto.        val
+0000a1a0: 7565 3a20 6f6e 6520 6f72 206d 6f72 6520  ue: one or more 
+0000a1b0: 4453 5020 696e 7465 7276 616c 732c 2061  DSP intervals, a
+0000a1c0: 7320 7374 7269 6e67 2f50 726f 7065 7274  s string/Propert
+0000a1d0: 7945 6c65 6d65 6e74 2c20 6f72 2061 7320  yElement, or as 
+0000a1e0: 6974 6572 6162 6c65 206f 6620 7374 7269  iterable of stri
+0000a1f0: 6e67 732f 5072 6f70 6572 7479 456c 656d  ngs/PropertyElem
+0000a200: 656e 7473 0a20 2020 2020 2020 2063 616c  ents.        cal
+0000a210: 6c69 6e67 5f72 6573 6f75 7263 653a 2074  ling_resource: t
+0000a220: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+0000a230: 6172 656e 7420 7265 736f 7572 6365 2028  arent resource (
+0000a240: 666f 7220 6265 7474 6572 2065 7272 6f72  for better error
+0000a250: 206d 6573 7361 6765 7329 0a0a 2020 2020   messages)..    
+0000a260: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0000a270: 4261 7365 4572 726f 723a 2049 6620 7468  BaseError: If th
+0000a280: 6520 7661 6c75 6520 6973 206e 6f74 2061  e value is not a
+0000a290: 2076 616c 6964 2044 5350 2069 6e74 6572   valid DSP inter
+0000a2a0: 7661 6c0a 0a20 2020 2052 6574 7572 6e73  val..    Returns
+0000a2b0: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
+0000a2c0: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
+0000a2d0: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
+0000a2e0: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
+0000a2f0: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
+0000a300: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
+0000a310: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
+0000a320: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
+0000a330: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000a340: 786d 6c2e 6d61 6b65 5f69 6e74 6572 7661  xml.make_interva
+0000a350: 6c5f 7072 6f70 2822 3a74 6573 7470 726f  l_prop(":testpro
+0000a360: 7065 7274 7922 2c20 2236 313a 3336 3030  perty", "61:3600
+0000a370: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000a380: 2020 203c 696e 7465 7276 616c 2d70 726f     <interval-pro
+0000a390: 7020 6e61 6d65 3d22 3a74 6573 7470 726f  p name=":testpro
+0000a3a0: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
+0000a3b0: 2020 2020 2020 2020 2020 2020 3c69 6e74              <int
+0000a3c0: 6572 7661 6c20 7065 726d 6973 7369 6f6e  erval permission
+0000a3d0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000a3e0: 3e36 313a 3336 3030 3c2f 696e 7465 7276  >61:3600</interv
+0000a3f0: 616c 3e0a 2020 2020 2020 2020 2020 2020  al>.            
+0000a400: 2020 2020 3c2f 696e 7465 7276 616c 2d70      </interval-p
+0000a410: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
+0000a420: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+0000a430: 696e 7465 7276 616c 5f70 726f 7028 223a  interval_prop(":
+0000a440: 7465 7374 7072 6f70 6572 7479 222c 2065  testproperty", e
+0000a450: 7863 656c 3278 6d6c 2e50 726f 7065 7274  xcel2xml.Propert
+0000a460: 7945 6c65 6d65 6e74 2822 3631 3a33 3630  yElement("61:360
+0000a470: 3022 2c20 7065 726d 6973 7369 6f6e 733d  0", permissions=
+0000a480: 2270 726f 702d 7265 7374 7269 6374 6564  "prop-restricted
+0000a490: 222c 2063 6f6d 6d65 6e74 3d22 6578 616d  ", comment="exam
+0000a4a0: 706c 6522 2929 0a20 2020 2020 2020 2020  ple")).         
+0000a4b0: 2020 2020 2020 203c 696e 7465 7276 616c         <interval
+0000a4c0: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
+0000a4d0: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+0000a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4f0: 3c69 6e74 6572 7661 6c20 7065 726d 6973  <interval permis
+0000a500: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+0000a510: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
+0000a520: 2265 7861 6d70 6c65 223e 3631 3a33 3630  "example">61:360
+0000a530: 303c 2f69 6e74 6572 7661 6c3e 0a20 2020  0</interval>.   
+0000a540: 2020 2020 2020 2020 2020 2020 203c 2f69               </i
+0000a550: 6e74 6572 7661 6c2d 7072 6f70 3e0a 2020  nterval-prop>.  
+0000a560: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000a570: 786d 6c2e 6d61 6b65 5f69 6e74 6572 7661  xml.make_interva
+0000a580: 6c5f 7072 6f70 2822 3a74 6573 7470 726f  l_prop(":testpro
+0000a590: 7065 7274 7922 2c20 5b22 3631 3a33 3630  perty", ["61:360
+0000a5a0: 3022 2c20 2236 302e 353a 3132 302e 3522  0", "60.5:120.5"
+0000a5b0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000a5c0: 2020 203c 696e 7465 7276 616c 2d70 726f     <interval-pro
+0000a5d0: 7020 6e61 6d65 3d22 3a74 6573 7470 726f  p name=":testpro
+0000a5e0: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
+0000a5f0: 2020 2020 2020 2020 2020 2020 3c69 6e74              <int
+0000a600: 6572 7661 6c20 7065 726d 6973 7369 6f6e  erval permission
+0000a610: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000a620: 3e36 313a 3336 3030 3c2f 696e 7465 7276  >61:3600</interv
+0000a630: 616c 3e0a 2020 2020 2020 2020 2020 2020  al>.            
+0000a640: 2020 2020 2020 2020 3c69 6e74 6572 7661          <interva
+0000a650: 6c20 7065 726d 6973 7369 6f6e 733d 2270  l permissions="p
+0000a660: 726f 702d 6465 6661 756c 7422 3e36 302e  rop-default">60.
+0000a670: 353a 3132 302e 353c 2f69 6e74 6572 7661  5:120.5</interva
+0000a680: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+0000a690: 2020 203c 2f69 6e74 6572 7661 6c2d 7072     </interval-pr
+0000a6a0: 6f70 3e0a 0a20 2020 2053 6565 2068 7474  op>..    See htt
+0000a6b0: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
+0000a6c0: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
+0000a6d0: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
+0000a6e0: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
+0000a6f0: 652f 2369 6e74 6572 7661 6c2d 7072 6f70  e/#interval-prop
+0000a700: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
+0000a710: 206e 616d 6520 3d3d 2022 6861 7353 6571   name == "hasSeq
+0000a720: 7565 6e63 6542 6f75 6e64 7322 3a0a 2020  uenceBounds":.  
+0000a730: 2020 2020 2020 6d73 6720 3d20 2244 6570        msg = "Dep
+0000a740: 7265 6361 7469 6f6e 2057 6172 6e69 6e67  recation Warning
+0000a750: 3a20 5375 7070 6f72 7420 666f 7220 7468  : Support for th
+0000a760: 6520 6861 7353 6571 7565 6e63 6542 6f75  e hasSequenceBou
+0000a770: 6e64 7320 7072 6f70 6572 7479 2077 696c  nds property wil
+0000a780: 6c20 6265 2072 656d 6f76 6564 2073 6f6f  l be removed soo
+0000a790: 6e22 0a20 2020 2020 2020 2077 6172 6e69  n".        warni
+0000a7a0: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
+0000a7b0: 7346 7574 7572 6557 6172 6e69 6e67 286d  sFutureWarning(m
+0000a7c0: 7367 2929 0a0a 2020 2020 2320 6368 6563  sg))..    # chec
+0000a7d0: 6b20 7468 6520 696e 7075 743a 2070 7265  k the input: pre
+0000a7e0: 7061 7265 2061 206c 6973 7420 7769 7468  pare a list with
+0000a7f0: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
+0000a800: 2020 7661 6c75 6573 203d 2070 7265 7061    values = prepa
+0000a810: 7265 5f76 616c 7565 2876 616c 7565 290a  re_value(value).
+0000a820: 0a20 2020 2023 2063 6865 636b 2076 616c  .    # check val
+0000a830: 7565 2074 7970 650a 2020 2020 666f 7220  ue type.    for 
+0000a840: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+0000a850: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
+0000a860: 6765 782e 6d61 7463 6828 0a20 2020 2020  gex.match(.     
+0000a870: 2020 2020 2020 2072 2228 5b2b 2d5d 3f28         r"([+-]?(
+0000a880: 5b30 2d39 5d2b 285b 2e5d 5b30 2d39 5d2a  [0-9]+([.][0-9]*
+0000a890: 293f 7c5b 2e5d 5b30 2d39 5d2b 2929 3a28  )?|[.][0-9]+)):(
+0000a8a0: 5b2b 2d5d 3f28 5b30 2d39 5d2b 285b 2e5d  [+-]?([0-9]+([.]
+0000a8b0: 5b30 2d39 5d2a 293f 7c5b 2e5d 5b30 2d39  [0-9]*)?|[.][0-9
+0000a8c0: 5d2b 2929 222c 0a20 2020 2020 2020 2020  ]+))",.         
+0000a8d0: 2020 2073 7472 2876 616c 2e76 616c 7565     str(val.value
+0000a8e0: 292c 0a20 2020 2020 2020 2029 3a0a 2020  ),.        ):.  
+0000a8f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000a900: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
+0000a910: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
+0000a920: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
+0000a930: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
+0000a940: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
+0000a950: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
+0000a960: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
+0000a970: 2020 2020 2020 6622 277b 7661 6c2e 7661        f"'{val.va
+0000a980: 6c75 657d 2720 6973 206e 6f74 2061 2076  lue}' is not a v
+0000a990: 616c 6964 2044 5350 2069 6e74 6572 7661  alid DSP interva
+0000a9a0: 6c2e 220a 2020 2020 2020 2020 2020 2020  l.".            
+0000a9b0: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+0000a9c0: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+0000a9d0: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+0000a9e0: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+0000a9f0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+0000aa00: 2020 2022 7b25 737d 696e 7465 7276 616c     "{%s}interval
+0000aa10: 2d70 726f 7022 2025 2078 6d6c 5f6e 616d  -prop" % xml_nam
+0000aa20: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+0000aa30: 2c0a 2020 2020 2020 2020 6e61 6d65 3d6e  ,.        name=n
+0000aa40: 616d 652c 0a20 2020 2020 2020 206e 736d  ame,.        nsm
+0000aa50: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
+0000aa60: 5f6d 6170 2c0a 2020 2020 290a 2020 2020  _map,.    ).    
+0000aa70: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
+0000aa80: 733a 0a20 2020 2020 2020 206b 7761 7267  s:.        kwarg
+0000aa90: 7320 3d20 7b22 7065 726d 6973 7369 6f6e  s = {"permission
+0000aaa0: 7322 3a20 7661 6c2e 7065 726d 6973 7369  s": val.permissi
+0000aab0: 6f6e 737d 0a20 2020 2020 2020 2069 6620  ons}.        if 
+0000aac0: 7661 6c2e 636f 6d6d 656e 7420 616e 6420  val.comment and 
+0000aad0: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
+0000aae0: 636f 6d6d 656e 7429 3a0a 2020 2020 2020  comment):.      
+0000aaf0: 2020 2020 2020 6b77 6172 6773 5b22 636f        kwargs["co
+0000ab00: 6d6d 656e 7422 5d20 3d20 7661 6c2e 636f  mment"] = val.co
+0000ab10: 6d6d 656e 740a 2020 2020 2020 2020 7661  mment.        va
+0000ab20: 6c75 655f 203d 2065 7472 6565 2e45 6c65  lue_ = etree.Ele
+0000ab30: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
+0000ab40: 2020 227b 2573 7d69 6e74 6572 7661 6c22    "{%s}interval"
+0000ab50: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
+0000ab60: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
+0000ab70: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000ab80: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
+0000ab90: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
+0000aba0: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
+0000abb0: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
+0000abc0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000abd0: 2020 2076 616c 7565 5f2e 7465 7874 203d     value_.text =
+0000abe0: 2073 7472 2876 616c 2e76 616c 7565 290a   str(val.value).
+0000abf0: 2020 2020 2020 2020 7072 6f70 5f2e 6170          prop_.ap
+0000ac00: 7065 6e64 2876 616c 7565 5f29 0a0a 2020  pend(value_)..  
+0000ac10: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+0000ac20: 0a64 6566 206d 616b 655f 6c69 7374 5f70  .def make_list_p
+0000ac30: 726f 7028 0a20 2020 206c 6973 745f 6e61  rop(.    list_na
+0000ac40: 6d65 3a20 7374 722c 0a20 2020 206e 616d  me: str,.    nam
+0000ac50: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
+0000ac60: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
+0000ac70: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
+0000ac80: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
+0000ac90: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
+0000aca0: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
+0000acb0: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
+0000acc0: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
+0000acd0: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
+0000ace0: 2222 220a 2020 2020 4d61 6b65 2061 203c  """.    Make a <
+0000acf0: 6c69 7374 2d70 726f 703e 2066 726f 6d20  list-prop> from 
+0000ad00: 6f6e 6520 6f72 206d 6f72 6520 6c69 7374  one or more list
+0000ad10: 206e 6f64 6573 2e20 5468 6520 6e61 6d65   nodes. The name
+0000ad20: 2873 2920 6f66 2074 6865 206c 6973 7420  (s) of the list 
+0000ad30: 6e6f 6465 2873 2920 6361 6e20 6265 2070  node(s) can be p
+0000ad40: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
+0000ad50: 6720 6f72 2061 730a 2020 2020 5072 6f70  g or as.    Prop
+0000ad60: 6572 7479 456c 656d 656e 7420 7769 7468  ertyElement with
+0000ad70: 2061 2073 7472 696e 6720 696e 7369 6465   a string inside
+0000ad80: 2e20 4966 2070 726f 7669 6465 6420 6173  . If provided as
+0000ad90: 2073 7472 696e 672c 2074 6865 2070 6572   string, the per
+0000ada0: 6d69 7373 696f 6e73 2064 6566 6175 6c74  missions default
+0000adb0: 2074 6f20 2270 726f 702d 6465 6661 756c   to "prop-defaul
+0000adc0: 7422 2e0a 0a20 2020 2041 7267 733a 0a20  t"...    Args:. 
+0000add0: 2020 2020 2020 206c 6973 745f 6e61 6d65         list_name
+0000ade0: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
+0000adf0: 6520 6c69 7374 2061 7320 6465 6669 6e65  e list as define
+0000ae00: 6420 696e 2074 6865 206f 6e74 6f0a 2020  d in the onto.  
+0000ae10: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
+0000ae20: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
+0000ae30: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
+0000ae40: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
+0000ae50: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
+0000ae60: 6f72 206d 6f72 6520 6e6f 6465 206e 616d  or more node nam
+0000ae70: 6573 2c20 6173 2073 7472 696e 672f 5072  es, as string/Pr
+0000ae80: 6f70 6572 7479 456c 656d 656e 742c 206f  opertyElement, o
+0000ae90: 7220 6173 2069 7465 7261 626c 6520 6f66  r as iterable of
+0000aea0: 2073 7472 696e 6773 2f50 726f 7065 7274   strings/Propert
+0000aeb0: 7945 6c65 6d65 6e74 730a 2020 2020 2020  yElements.      
+0000aec0: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+0000aed0: 6365 3a20 7468 6520 6e61 6d65 206f 6620  ce: the name of 
+0000aee0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+0000aef0: 7263 6520 2866 6f72 2062 6574 7465 7220  rce (for better 
+0000af00: 6572 726f 7220 6d65 7373 6167 6573 290a  error messages).
+0000af10: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+0000af20: 2020 2020 2042 6173 6545 7272 6f72 3a20       BaseError: 
+0000af30: 4966 2074 6865 206e 616d 6520 6f66 206f  If the name of o
+0000af40: 6e65 206f 6620 7468 6520 6c69 7374 206e  ne of the list n
+0000af50: 6f64 6573 2069 7320 6e6f 7420 6120 7661  odes is not a va
+0000af60: 6c69 6420 7374 7269 6e67 0a0a 2020 2020  lid string..    
+0000af70: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000af80: 2061 6e20 6574 7265 652e 5f45 6c65 6d65   an etree._Eleme
+0000af90: 6e74 2074 6861 7420 6361 6e20 6265 2061  nt that can be a
+0000afa0: 7070 656e 6465 6420 746f 2074 6865 2070  ppended to the p
+0000afb0: 6172 656e 7420 7265 736f 7572 6365 2077  arent resource w
+0000afc0: 6974 6820 7265 736f 7572 6365 2e61 7070  ith resource.app
+0000afd0: 656e 6428 6d61 6b65 5f2a 5f70 726f 7028  end(make_*_prop(
+0000afe0: 2e2e 2e29 290a 0a20 2020 2045 7861 6d70  ...))..    Examp
+0000aff0: 6c65 733a 0a20 2020 2020 2020 203e 3e3e  les:.        >>>
+0000b000: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+0000b010: 6c69 7374 5f70 726f 7028 226d 796c 6973  list_prop("mylis
+0000b020: 7422 2c20 223a 7465 7374 7072 6f70 6572  t", ":testproper
+0000b030: 7479 222c 2022 6669 7273 745f 6e6f 6465  ty", "first_node
+0000b040: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000b050: 2020 203c 6c69 7374 2d70 726f 7020 6c69     <list-prop li
+0000b060: 7374 3d22 6d79 6c69 7374 2220 6e61 6d65  st="mylist" name
+0000b070: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000b080: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000b090: 2020 2020 2020 3c6c 6973 7420 7065 726d        <list perm
+0000b0a0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+0000b0b0: 6661 756c 7422 3e66 6972 7374 5f6e 6f64  fault">first_nod
+0000b0c0: 653c 2f6c 6973 743e 0a20 2020 2020 2020  e</list>.       
+0000b0d0: 2020 2020 2020 2020 203c 2f6c 6973 742d           </list-
+0000b0e0: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
+0000b0f0: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+0000b100: 5f6c 6973 745f 7072 6f70 2822 6d79 6c69  _list_prop("myli
+0000b110: 7374 222c 2022 3a74 6573 7470 726f 7065  st", ":testprope
+0000b120: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
+0000b130: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
+0000b140: 2266 6972 7374 5f6e 6f64 6522 2c20 7065  "first_node", pe
+0000b150: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000b160: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
+0000b170: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
+0000b180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b190: 203c 6c69 7374 2d70 726f 7020 6c69 7374   <list-prop list
+0000b1a0: 3d22 6d79 6c69 7374 2220 6e61 6d65 3d22  ="mylist" name="
+0000b1b0: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1d0: 2020 2020 3c6c 6973 7420 7065 726d 6973      <list permis
+0000b1e0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+0000b1f0: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
+0000b200: 2265 7861 6d70 6c65 223e 6669 7273 745f  "example">first_
+0000b210: 6e6f 6465 3c2f 6c69 7374 3e0a 2020 2020  node</list>.    
+0000b220: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
+0000b230: 7374 2d70 726f 703e 0a20 2020 2020 2020  st-prop>.       
+0000b240: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000b250: 616b 655f 6c69 7374 5f70 726f 7028 226d  ake_list_prop("m
+0000b260: 796c 6973 7422 2c20 223a 7465 7374 7072  ylist", ":testpr
+0000b270: 6f70 6572 7479 222c 205b 2266 6972 7374  operty", ["first
+0000b280: 5f6e 6f64 6522 2c20 2273 6563 6f6e 645f  _node", "second_
+0000b290: 6e6f 6465 225d 290a 2020 2020 2020 2020  node"]).        
+0000b2a0: 2020 2020 2020 2020 3c6c 6973 742d 7072          <list-pr
+0000b2b0: 6f70 206c 6973 743d 226d 796c 6973 7422  op list="mylist"
+0000b2c0: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000b2d0: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000b2e0: 2020 2020 2020 2020 2020 203c 6c69 7374             <list
+0000b2f0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000b300: 6f70 2d64 6566 6175 6c74 223e 6669 7273  op-default">firs
+0000b310: 745f 6e6f 6465 3c2f 6c69 7374 3e0a 2020  t_node</list>.  
+0000b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b330: 2020 3c6c 6973 7420 7065 726d 6973 7369    <list permissi
+0000b340: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
+0000b350: 7422 3e73 6563 6f6e 645f 6e6f 6465 3c2f  t">second_node</
+0000b360: 6c69 7374 3e0a 2020 2020 2020 2020 2020  list>.          
+0000b370: 2020 2020 2020 3c2f 6c69 7374 2d70 726f        </list-pro
+0000b380: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
+0000b390: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+0000b3a0: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+0000b3b0: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+0000b3c0: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+0000b3d0: 2f23 6c69 7374 2d70 726f 700a 2020 2020  /#list-prop.    
+0000b3e0: 2222 220a 0a20 2020 2023 2063 6865 636b  """..    # check
+0000b3f0: 2074 6865 2069 6e70 7574 3a20 7072 6570   the input: prep
+0000b400: 6172 6520 6120 6c69 7374 2077 6974 6820  are a list with 
+0000b410: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+0000b420: 2076 616c 7565 7320 3d20 7072 6570 6172   values = prepar
+0000b430: 655f 7661 6c75 6528 7661 6c75 6529 0a0a  e_value(value)..
+0000b440: 2020 2020 2320 6368 6563 6b20 7661 6c75      # check valu
+0000b450: 6520 7479 7065 0a20 2020 2066 6f72 2076  e type.    for v
+0000b460: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
+0000b470: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0000b480: 6e73 7461 6e63 6528 7661 6c2e 7661 6c75  nstance(val.valu
+0000b490: 652c 2073 7472 2920 6f72 206e 6f74 2063  e, str) or not c
+0000b4a0: 6865 636b 5f6e 6f74 6e61 2876 616c 2e76  heck_notna(val.v
+0000b4b0: 616c 7565 293a 0a20 2020 2020 2020 2020  alue):.         
+0000b4c0: 2020 2072 6169 7365 2042 6173 6545 7272     raise BaseErr
+0000b4d0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000b4e0: 2020 2020 6622 4661 696c 6564 2076 616c      f"Failed val
+0000b4f0: 6964 6174 696f 6e20 696e 2072 6573 6f75  idation in resou
+0000b500: 7263 6520 277b 6361 6c6c 696e 675f 7265  rce '{calling_re
+0000b510: 736f 7572 6365 7d27 2c20 7072 6f70 6572  source}', proper
+0000b520: 7479 2027 7b6e 616d 657d 273a 2022 0a20  ty '{name}': ". 
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b540: 2227 7b76 616c 2e76 616c 7565 7d27 2069  "'{val.value}' i
+0000b550: 7320 6e6f 7420 6120 7661 6c69 6420 6e61  s not a valid na
+0000b560: 6d65 206f 6620 6120 6c69 7374 206e 6f64  me of a list nod
+0000b570: 652e 220a 2020 2020 2020 2020 2020 2020  e.".            
+0000b580: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+0000b590: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+0000b5a0: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+0000b5b0: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+0000b5c0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+0000b5d0: 2020 2022 7b25 737d 6c69 7374 2d70 726f     "{%s}list-pro
+0000b5e0: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+0000b5f0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000b600: 2020 2020 2020 6c69 7374 3d6c 6973 745f        list=list_
+0000b610: 6e61 6d65 2c0a 2020 2020 2020 2020 6e61  name,.        na
+0000b620: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
+0000b630: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+0000b640: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
+0000b650: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
+0000b660: 616c 7565 733a 0a20 2020 2020 2020 206b  alues:.        k
+0000b670: 7761 7267 7320 3d20 7b22 7065 726d 6973  wargs = {"permis
+0000b680: 7369 6f6e 7322 3a20 7661 6c2e 7065 726d  sions": val.perm
+0000b690: 6973 7369 6f6e 737d 0a20 2020 2020 2020  issions}.       
+0000b6a0: 2069 6620 7661 6c2e 636f 6d6d 656e 7420   if val.comment 
+0000b6b0: 616e 6420 6368 6563 6b5f 6e6f 746e 6128  and check_notna(
+0000b6c0: 7661 6c2e 636f 6d6d 656e 7429 3a0a 2020  val.comment):.  
+0000b6d0: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+0000b6e0: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
+0000b6f0: 6c2e 636f 6d6d 656e 740a 2020 2020 2020  l.comment.      
+0000b700: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
+0000b710: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
+0000b720: 2020 2020 2020 227b 2573 7d6c 6973 7422        "{%s}list"
+0000b730: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
+0000b740: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
+0000b750: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000b760: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
+0000b770: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
+0000b780: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
+0000b790: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
+0000b7a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000b7b0: 2020 2076 616c 7565 5f2e 7465 7874 203d     value_.text =
+0000b7c0: 2073 7472 2876 616c 2e76 616c 7565 290a   str(val.value).
+0000b7d0: 2020 2020 2020 2020 7072 6f70 5f2e 6170          prop_.ap
+0000b7e0: 7065 6e64 2876 616c 7565 5f29 0a0a 2020  pend(value_)..  
+0000b7f0: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+0000b800: 0a64 6566 206d 616b 655f 7265 7370 7472  .def make_resptr
+0000b810: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+0000b820: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+0000b830: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+0000b840: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+0000b850: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+0000b860: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+0000b870: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+0000b880: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+0000b890: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+0000b8a0: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+0000b8b0: 220a 2020 2020 4d61 6b65 2061 203c 7265  ".    Make a <re
+0000b8c0: 7370 7472 2d70 726f 703e 2066 726f 6d20  sptr-prop> from 
+0000b8d0: 6f6e 6520 6f72 206d 6f72 6520 4944 7320  one or more IDs 
+0000b8e0: 6f66 206f 7468 6572 2072 6573 6f75 7263  of other resourc
+0000b8f0: 6573 2e20 5468 6520 4944 2873 2920 6361  es. The ID(s) ca
+0000b900: 6e20 6265 2070 726f 7669 6465 6420 6173  n be provided as
+0000b910: 2073 7472 696e 6720 6f72 2061 730a 2020   string or as.  
+0000b920: 2020 5072 6f70 6572 7479 456c 656d 656e    PropertyElemen
+0000b930: 7420 7769 7468 2061 2073 7472 696e 6720  t with a string 
+0000b940: 696e 7369 6465 2e20 4966 2070 726f 7669  inside. If provi
+0000b950: 6465 6420 6173 2073 7472 696e 672c 2074  ded as string, t
+0000b960: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
+0000b970: 6566 6175 6c74 2074 6f20 2270 726f 702d  efault to "prop-
+0000b980: 6465 6661 756c 7422 2e0a 0a20 2020 2041  default"...    A
+0000b990: 7267 733a 0a20 2020 2020 2020 206e 616d  rgs:.        nam
+0000b9a0: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+0000b9b0: 6869 7320 7072 6f70 6572 7479 2061 7320  his property as 
+0000b9c0: 6465 6669 6e65 6420 696e 2074 6865 206f  defined in the o
+0000b9d0: 6e74 6f0a 2020 2020 2020 2020 7661 6c75  nto.        valu
+0000b9e0: 653a 206f 6e65 206f 7220 6d6f 7265 2072  e: one or more r
+0000b9f0: 6573 6f75 7263 6520 6964 656e 7469 6669  esource identifi
+0000ba00: 6572 732c 2061 7320 7374 7269 6e67 2f50  ers, as string/P
+0000ba10: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+0000ba20: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
+0000ba30: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
+0000ba40: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
+0000ba50: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+0000ba60: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
+0000ba70: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+0000ba80: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
+0000ba90: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
+0000baa0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+0000bab0: 2020 2020 2020 4261 7365 4572 726f 723a        BaseError:
+0000bac0: 2049 6620 7468 6520 4944 206f 6620 6f6e   If the ID of on
+0000bad0: 6520 6f66 2074 6865 2074 6172 6765 7420  e of the target 
+0000bae0: 7265 736f 7572 6365 7320 6973 206e 6f74  resources is not
+0000baf0: 2061 2076 616c 6964 2073 7472 696e 670a   a valid string.
+0000bb00: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000bb10: 2020 2020 2020 616e 2065 7472 6565 2e5f        an etree._
+0000bb20: 456c 656d 656e 7420 7468 6174 2063 616e  Element that can
+0000bb30: 2062 6520 6170 7065 6e64 6564 2074 6f20   be appended to 
+0000bb40: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+0000bb50: 7263 6520 7769 7468 2072 6573 6f75 7263  rce with resourc
+0000bb60: 652e 6170 7065 6e64 286d 616b 655f 2a5f  e.append(make_*_
+0000bb70: 7072 6f70 282e 2e2e 2929 0a0a 2020 2020  prop(...))..    
+0000bb80: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+0000bb90: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
+0000bba0: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+0000bbb0: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+0000bbc0: 2c20 2272 6573 6f75 7263 655f 3122 290a  , "resource_1").
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 3c72 6573 7074 722d 7072 6f70 206e 616d  <resptr-prop nam
+0000bbf0: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+0000bc00: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000bc10: 2020 2020 2020 203c 7265 7370 7472 2070         <resptr p
+0000bc20: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000bc30: 2d64 6566 6175 6c74 223e 7265 736f 7572  -default">resour
+0000bc40: 6365 5f31 3c2f 7265 7370 7472 3e0a 2020  ce_1</resptr>.  
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000bc60: 7265 7370 7472 2d70 726f 703e 0a20 2020  resptr-prop>.   
+0000bc70: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+0000bc80: 6d6c 2e6d 616b 655f 7265 7370 7472 5f70  ml.make_resptr_p
+0000bc90: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+0000bca0: 7479 222c 2065 7863 656c 3278 6d6c 2e50  ty", excel2xml.P
+0000bcb0: 726f 7065 7274 7945 6c65 6d65 6e74 2822  ropertyElement("
+0000bcc0: 7265 736f 7572 6365 5f31 222c 2070 6572  resource_1", per
+0000bcd0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
+0000bce0: 6573 7472 6963 7465 6422 2c20 636f 6d6d  estricted", comm
+0000bcf0: 656e 743d 2265 7861 6d70 6c65 2229 290a  ent="example")).
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 3c72 6573 7074 722d 7072 6f70 206e 616d  <resptr-prop nam
+0000bd20: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+0000bd30: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000bd40: 2020 2020 2020 203c 7265 7370 7472 2070         <resptr p
+0000bd50: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000bd60: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
+0000bd70: 6d65 6e74 3d22 6578 616d 706c 6522 3e72  ment="example">r
+0000bd80: 6573 6f75 7263 655f 313c 2f72 6573 7074  esource_1</respt
+0000bd90: 723e 0a20 2020 2020 2020 2020 2020 2020  r>.             
+0000bda0: 2020 203c 2f72 6573 7074 722d 7072 6f70     </resptr-prop
+0000bdb0: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
+0000bdc0: 6365 6c32 786d 6c2e 6d61 6b65 5f72 6573  cel2xml.make_res
+0000bdd0: 7074 725f 7072 6f70 2822 3a74 6573 7470  ptr_prop(":testp
+0000bde0: 726f 7065 7274 7922 2c20 5b22 7265 736f  roperty", ["reso
+0000bdf0: 7572 6365 5f31 222c 2022 7265 736f 7572  urce_1", "resour
+0000be00: 6365 5f32 225d 290a 2020 2020 2020 2020  ce_2"]).        
+0000be10: 2020 2020 2020 2020 3c72 6573 7074 722d          <resptr-
+0000be20: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+0000be30: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+0000be40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000be50: 7265 7370 7472 2070 6572 6d69 7373 696f  resptr permissio
+0000be60: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
+0000be70: 223e 7265 736f 7572 6365 5f31 3c2f 7265  ">resource_1</re
+0000be80: 7370 7472 3e0a 2020 2020 2020 2020 2020  sptr>.          
+0000be90: 2020 2020 2020 2020 2020 3c72 6573 7074            <respt
+0000bea0: 7220 7065 726d 6973 7369 6f6e 733d 2270  r permissions="p
+0000beb0: 726f 702d 6465 6661 756c 7422 3e72 6573  rop-default">res
+0000bec0: 6f75 7263 655f 323c 2f72 6573 7074 723e  ource_2</resptr>
+0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bee0: 203c 2f72 6573 7074 722d 7072 6f70 3e0a   </resptr-prop>.
+0000bef0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+0000bf00: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
+0000bf10: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
+0000bf20: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
+0000bf30: 786d 6c2d 6461 7461 2d66 696c 652f 2372  xml-data-file/#r
+0000bf40: 6573 7074 722d 7072 6f70 0a20 2020 2022  esptr-prop.    "
+0000bf50: 2222 0a0a 2020 2020 6966 206e 616d 6520  ""..    if name 
+0000bf60: 3d3d 2022 6973 5365 7175 656e 6365 4f66  == "isSequenceOf
+0000bf70: 223a 0a20 2020 2020 2020 206d 7367 203d  ":.        msg =
+0000bf80: 2022 4465 7072 6563 6174 696f 6e20 5761   "Deprecation Wa
+0000bf90: 726e 696e 673a 2053 7570 706f 7274 2066  rning: Support f
+0000bfa0: 6f72 2074 6865 2069 7353 6571 7565 6e63  or the isSequenc
+0000bfb0: 654f 6620 7072 6f70 6572 7479 2077 696c  eOf property wil
+0000bfc0: 6c20 6265 2072 656d 6f76 6564 2073 6f6f  l be removed soo
+0000bfd0: 6e22 0a20 2020 2020 2020 2077 6172 6e69  n".        warni
+0000bfe0: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
+0000bff0: 7346 7574 7572 6557 6172 6e69 6e67 286d  sFutureWarning(m
+0000c000: 7367 2929 0a0a 2020 2020 2320 6368 6563  sg))..    # chec
+0000c010: 6b20 7468 6520 696e 7075 743a 2070 7265  k the input: pre
+0000c020: 7061 7265 2061 206c 6973 7420 7769 7468  pare a list with
+0000c030: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
+0000c040: 2020 7661 6c75 6573 203d 2070 7265 7061    values = prepa
+0000c050: 7265 5f76 616c 7565 2876 616c 7565 290a  re_value(value).
+0000c060: 0a20 2020 2023 2063 6865 636b 2076 616c  .    # check val
+0000c070: 7565 2074 7970 650a 2020 2020 666f 7220  ue type.    for 
+0000c080: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+0000c090: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000c0a0: 696e 7374 616e 6365 2876 616c 2e76 616c  instance(val.val
+0000c0b0: 7565 2c20 7374 7229 206f 7220 6e6f 7420  ue, str) or not 
+0000c0c0: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
+0000c0d0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0000c0e0: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
+0000c0f0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000c100: 2020 2020 2066 2256 616c 6964 6174 696f       f"Validatio
+0000c110: 6e20 4572 726f 7220 696e 2072 6573 6f75  n Error in resou
+0000c120: 7263 6520 277b 6361 6c6c 696e 675f 7265  rce '{calling_re
+0000c130: 736f 7572 6365 7d27 2c20 7072 6f70 6572  source}', proper
+0000c140: 7479 2027 7b6e 616d 657d 273a 2022 0a20  ty '{name}': ". 
+0000c150: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000c160: 2254 6865 2066 6f6c 6c6f 7769 6e67 2064  "The following d
+0000c170: 6f65 736e 2774 2073 6565 6d20 746f 2062  oesn't seem to b
+0000c180: 6520 6120 7661 6c69 6420 4944 206f 6620  e a valid ID of 
+0000c190: 6120 7461 7267 6574 2072 6573 6f75 7263  a target resourc
+0000c1a0: 653a 2027 7b76 616c 2e76 616c 7565 7d27  e: '{val.value}'
+0000c1b0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000c1c0: 0a20 2020 2023 206d 616b 6520 786d 6c20  .    # make xml 
+0000c1d0: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
+0000c1e0: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
+0000c1f0: 2020 7072 6f70 5f20 3d20 6574 7265 652e    prop_ = etree.
+0000c200: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+0000c210: 2022 7b25 737d 7265 7370 7472 2d70 726f   "{%s}resptr-pro
+0000c220: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+0000c230: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000c240: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+0000c250: 0a20 2020 2020 2020 206e 736d 6170 3d78  .        nsmap=x
+0000c260: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+0000c270: 2c0a 2020 2020 290a 2020 2020 666f 7220  ,.    ).    for 
+0000c280: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+0000c290: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+0000c2a0: 7b22 7065 726d 6973 7369 6f6e 7322 3a20  {"permissions": 
+0000c2b0: 7661 6c2e 7065 726d 6973 7369 6f6e 737d  val.permissions}
+0000c2c0: 0a20 2020 2020 2020 2069 6620 7661 6c2e  .        if val.
+0000c2d0: 636f 6d6d 656e 7420 616e 6420 6368 6563  comment and chec
+0000c2e0: 6b5f 6e6f 746e 6128 7661 6c2e 636f 6d6d  k_notna(val.comm
+0000c2f0: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
+0000c300: 2020 6b77 6172 6773 5b22 636f 6d6d 656e    kwargs["commen
+0000c310: 7422 5d20 3d20 7661 6c2e 636f 6d6d 656e  t"] = val.commen
+0000c320: 740a 2020 2020 2020 2020 7661 6c75 655f  t.        value_
+0000c330: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+0000c340: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+0000c350: 2573 7d72 6573 7074 7222 2025 2078 6d6c  %s}resptr" % xml
+0000c360: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+0000c370: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
+0000c380: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
+0000c390: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
+0000c3a0: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
+0000c3b0: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
+0000c3c0: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
+0000c3d0: 2020 2029 0a20 2020 2020 2020 2076 616c     ).        val
+0000c3e0: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
+0000c3f0: 616c 2e76 616c 7565 290a 2020 2020 2020  al.value).      
+0000c400: 2020 7072 6f70 5f2e 6170 7065 6e64 2876    prop_.append(v
+0000c410: 616c 7565 5f29 0a0a 2020 2020 7265 7475  alue_)..    retu
+0000c420: 726e 2070 726f 705f 0a0a 0a64 6566 206d  rn prop_...def m
+0000c430: 616b 655f 7465 7874 5f70 726f 7028 0a20  ake_text_prop(. 
+0000c440: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
+0000c450: 2020 7661 6c75 653a 2055 6e69 6f6e 5b50    value: Union[P
+0000c460: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+0000c470: 7374 722c 2049 7465 7261 626c 655b 556e  str, Iterable[Un
+0000c480: 696f 6e5b 5072 6f70 6572 7479 456c 656d  ion[PropertyElem
+0000c490: 656e 742c 2073 7472 5d5d 5d2c 0a20 2020  ent, str]]],.   
+0000c4a0: 2063 616c 6c69 6e67 5f72 6573 6f75 7263   calling_resourc
+0000c4b0: 653a 2073 7472 203d 2022 222c 0a29 202d  e: str = "",.) -
+0000c4c0: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
+0000c4d0: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
+0000c4e0: 6b65 2061 203c 7465 7874 2d70 726f 703e  ke a <text-prop>
+0000c4f0: 2066 726f 6d20 6f6e 6520 6f72 206d 6f72   from one or mor
+0000c500: 6520 7374 7269 6e67 732e 2054 6865 2073  e strings. The s
+0000c510: 7472 696e 6728 7329 2063 616e 2062 6520  tring(s) can be 
+0000c520: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+0000c530: 6e67 206f 7220 6173 2050 726f 7065 7274  ng or as Propert
+0000c540: 7945 6c65 6d65 6e74 2077 6974 6820 610a  yElement with a.
+0000c550: 2020 2020 7374 7269 6e67 2069 6e73 6964      string insid
+0000c560: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
+0000c570: 7320 7374 7269 6e67 2c20 7468 6520 656e  s string, the en
+0000c580: 636f 6469 6e67 2064 6566 6175 6c74 7320  coding defaults 
+0000c590: 746f 2075 7466 382c 2061 6e64 2074 6865  to utf8, and the
+0000c5a0: 2070 6572 6d69 7373 696f 6e73 2074 6f20   permissions to 
+0000c5b0: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
+0000c5c0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000c5d0: 2020 206e 616d 653a 2074 6865 206e 616d     name: the nam
+0000c5e0: 6520 6f66 2074 6869 7320 7072 6f70 6572  e of this proper
+0000c5f0: 7479 2061 7320 6465 6669 6e65 6420 696e  ty as defined in
+0000c600: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
+0000c610: 2020 7661 6c75 653a 206f 6e65 206f 7220    value: one or 
+0000c620: 6d6f 7265 2073 7472 696e 6773 2c20 6173  more strings, as
+0000c630: 2073 7472 696e 672f 5072 6f70 6572 7479   string/Property
+0000c640: 456c 656d 656e 742c 206f 7220 6173 2069  Element, or as i
+0000c650: 7465 7261 626c 6520 6f66 2073 7472 696e  terable of strin
+0000c660: 6773 2f50 726f 7065 7274 7945 6c65 6d65  gs/PropertyEleme
+0000c670: 6e74 730a 2020 2020 2020 2020 6361 6c6c  nts.        call
+0000c680: 696e 675f 7265 736f 7572 6365 3a20 7468  ing_resource: th
+0000c690: 6520 6e61 6d65 206f 6620 7468 6520 7061  e name of the pa
+0000c6a0: 7265 6e74 2072 6573 6f75 7263 6520 2866  rent resource (f
+0000c6b0: 6f72 2062 6574 7465 7220 6572 726f 7220  or better error 
+0000c6c0: 6d65 7373 6167 6573 290a 0a20 2020 2052  messages)..    R
+0000c6d0: 6169 7365 733a 0a20 2020 2020 2020 2042  aises:.        B
+0000c6e0: 6173 6545 7272 6f72 3a20 6966 206f 6e65  aseError: if one
+0000c6f0: 206f 6620 7468 6520 7661 6c75 6573 2069   of the values i
+0000c700: 7320 6e6f 7420 6120 7661 6c69 6420 7374  s not a valid st
+0000c710: 7269 6e67 2c0a 2020 2020 2020 2020 2020  ring,.          
+0000c720: 2020 6f72 2069 6620 7468 6520 584d 4c20    or if the XML 
+0000c730: 7461 6773 2069 6e20 6120 7269 6368 7465  tags in a richte
+0000c740: 7874 2070 726f 7065 7274 7920 2865 6e63  xt property (enc
+0000c750: 6f64 696e 673d 786d 6c29 2061 7265 206e  oding=xml) are n
+0000c760: 6f74 2077 656c 6c2d 666f 726d 6564 0a20  ot well-formed. 
+0000c770: 2020 2020 2020 2057 6172 6e69 6e67 3a20         Warning: 
+0000c780: 6966 206f 6e65 206f 6620 7468 6520 7661  if one of the va
+0000c790: 6c75 6573 2064 6f65 736e 2774 206c 6f6f  lues doesn't loo
+0000c7a0: 6b20 6c69 6b65 2061 2072 6561 736f 6e61  k like a reasona
+0000c7b0: 626c 6520 7374 7269 6e67 0a20 2020 2020  ble string.     
+0000c7c0: 2020 2020 2020 2028 652e 672e 2022 3c4e         (e.g. "<N
+0000c7d0: 413e 2220 6973 2061 2076 616c 6964 2073  A>" is a valid s
+0000c7e0: 7472 696e 672c 2062 7574 2070 726f 6261  tring, but proba
+0000c7f0: 626c 7920 6e6f 7420 696e 7465 6e64 6564  bly not intended
+0000c800: 290a 0a20 2020 2052 6574 7572 6e73 3a0a  )..    Returns:.
+0000c810: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
+0000c820: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
+0000c830: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
+0000c840: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
+0000c850: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
+0000c860: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
+0000c870: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
+0000c880: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+0000c890: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+0000c8a0: 6c2e 6d61 6b65 5f74 6578 745f 7072 6f70  l.make_text_prop
+0000c8b0: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+0000c8c0: 2c20 2266 6972 7374 2074 6578 7422 290a  , "first text").
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 3c74 6578 742d 7072 6f70 206e 616d 653d  <text-prop name=
+0000c8f0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+0000c900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c910: 2020 2020 203c 7465 7874 2065 6e63 6f64       <text encod
+0000c920: 696e 673d 2275 7466 3822 2070 6572 6d69  ing="utf8" permi
+0000c930: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+0000c940: 6175 6c74 223e 6669 7273 7420 7465 7874  ault">first text
+0000c950: 3c2f 7465 7874 3e0a 2020 2020 2020 2020  </text>.        
+0000c960: 2020 2020 2020 2020 3c2f 7465 7874 2d70          </text-p
+0000c970: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
+0000c980: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+0000c990: 7465 7874 5f70 726f 7028 223a 7465 7374  text_prop(":test
+0000c9a0: 7072 6f70 6572 7479 222c 2065 7863 656c  property", excel
+0000c9b0: 3278 6d6c 2e50 726f 7065 7274 7945 6c65  2xml.PropertyEle
+0000c9c0: 6d65 6e74 2822 6669 7273 7420 7465 7874  ment("first text
+0000c9d0: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
+0000c9e0: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+0000c9f0: 2c20 656e 636f 6469 6e67 3d22 786d 6c22  , encoding="xml"
+0000ca00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0000ca10: 2020 203c 7465 7874 2d70 726f 7020 6e61     <text-prop na
+0000ca20: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
+0000ca30: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
+0000ca40: 2020 2020 2020 2020 3c74 6578 7420 656e          <text en
+0000ca50: 636f 6469 6e67 3d22 786d 6c22 2070 6572  coding="xml" per
+0000ca60: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
+0000ca70: 6573 7472 6963 7465 6422 3e66 6972 7374  estricted">first
+0000ca80: 2074 6578 743c 2f74 6578 743e 0a20 2020   text</text>.   
+0000ca90: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+0000caa0: 6578 742d 7072 6f70 3e0a 2020 2020 2020  ext-prop>.      
+0000cab0: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
+0000cac0: 6d61 6b65 5f74 6578 745f 7072 6f70 2822  make_text_prop("
+0000cad0: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
+0000cae0: 5b22 6669 7273 7420 7465 7874 222c 2022  ["first text", "
+0000caf0: 7365 636f 6e64 2074 6578 7422 5d29 0a20  second text"]). 
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cb10: 7465 7874 2d70 726f 7020 6e61 6d65 3d22  text-prop name="
+0000cb20: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb40: 2020 2020 3c74 6578 7420 656e 636f 6469      <text encodi
+0000cb50: 6e67 3d22 7574 6638 2220 7065 726d 6973  ng="utf8" permis
+0000cb60: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+0000cb70: 756c 7422 3e66 6972 7374 2074 6578 743c  ult">first text<
+0000cb80: 2f74 6578 743e 0a20 2020 2020 2020 2020  /text>.         
+0000cb90: 2020 2020 2020 2020 2020 203c 7465 7874             <text
+0000cba0: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
+0000cbb0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000cbc0: 6f70 2d64 6566 6175 6c74 223e 7365 636f  op-default">seco
+0000cbd0: 6e64 2074 6578 743c 2f74 6578 743e 0a20  nd text</text>. 
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cbf0: 2f74 6578 742d 7072 6f70 3e0a 0a20 2020  /text-prop>..   
+0000cc00: 2053 6565 2068 7474 7073 3a2f 2f64 6f63   See https://doc
+0000cc10: 732e 6461 7363 682e 7377 6973 732f 6c61  s.dasch.swiss/la
+0000cc20: 7465 7374 2f44 5350 2d54 4f4f 4c53 2f66  test/DSP-TOOLS/f
+0000cc30: 696c 652d 666f 726d 6174 732f 786d 6c2d  ile-formats/xml-
+0000cc40: 6461 7461 2d66 696c 652f 2374 6578 742d  data-file/#text-
+0000cc50: 7072 6f70 0a20 2020 2022 2222 0a0a 2020  prop.    """..  
+0000cc60: 2020 2320 6368 6563 6b20 7468 6520 696e    # check the in
+0000cc70: 7075 743a 2070 7265 7061 7265 2061 206c  put: prepare a l
+0000cc80: 6973 7420 7769 7468 2076 616c 6964 2076  ist with valid v
+0000cc90: 616c 7565 730a 2020 2020 7661 6c75 6573  alues.    values
+0000cca0: 203d 2070 7265 7061 7265 5f76 616c 7565   = prepare_value
+0000ccb0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
+0000ccc0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
+0000ccd0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
+0000cce0: 616c 7565 733a 0a20 2020 2020 2020 2069  alues:.        i
+0000ccf0: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+0000cd00: 2876 616c 2e76 616c 7565 2c20 7374 7229  (val.value, str)
+0000cd10: 206f 7220 6c65 6e28 7661 6c2e 7661 6c75   or len(val.valu
+0000cd20: 6529 203c 2031 3a0a 2020 2020 2020 2020  e) < 1:.        
+0000cd30: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
+0000cd40: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000cd50: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
+0000cd60: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
+0000cd70: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
+0000cd80: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
+0000cd90: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 6622 277b 7661 6c2e 7661 6c75 657d 2720  f"'{val.value}' 
+0000cdc0: 6973 206e 6f74 2061 2076 616c 6964 2073  is not a valid s
+0000cdd0: 7472 696e 672e 220a 2020 2020 2020 2020  tring.".        
+0000cde0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+0000cdf0: 206e 6f74 2063 6865 636b 5f6e 6f74 6e61   not check_notna
+0000ce00: 2876 616c 2e76 616c 7565 293a 0a20 2020  (val.value):.   
+0000ce10: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+0000ce20: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+0000ce30: 2020 2020 2020 2020 6622 5761 726e 696e          f"Warnin
+0000ce40: 6720 666f 7220 7265 736f 7572 6365 2027  g for resource '
+0000ce50: 7b63 616c 6c69 6e67 5f72 6573 6f75 7263  {calling_resourc
+0000ce60: 657d 272c 2070 726f 7065 7274 7920 277b  e}', property '{
+0000ce70: 6e61 6d65 7d27 3a20 220a 2020 2020 2020  name}': ".      
+0000ce80: 2020 2020 2020 2020 2020 6622 277b 7661            f"'{va
+0000ce90: 6c2e 7661 6c75 657d 2720 6973 2070 726f  l.value}' is pro
+0000cea0: 6261 626c 7920 6e6f 7420 6120 7573 6162  bably not a usab
+0000ceb0: 6c65 2073 7472 696e 672e 222c 0a20 2020  le string.",.   
+0000cec0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000ced0: 636b 6c65 7665 6c3d 322c 0a20 2020 2020  cklevel=2,.     
+0000cee0: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+0000cef0: 6d61 6b65 2078 6d6c 2073 7472 7563 7475  make xml structu
+0000cf00: 7265 206f 6620 7468 6520 7661 6c69 6420  re of the valid 
+0000cf10: 7661 6c75 6573 0a20 2020 2070 726f 705f  values.    prop_
+0000cf20: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+0000cf30: 280a 2020 2020 2020 2020 227b 2573 7d74  (.        "{%s}t
+0000cf40: 6578 742d 7072 6f70 2220 2520 786d 6c5f  ext-prop" % xml_
+0000cf50: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
+0000cf60: 6e65 5d2c 0a20 2020 2020 2020 206e 616d  ne],.        nam
+0000cf70: 653d 6e61 6d65 2c0a 2020 2020 2020 2020  e=name,.        
+0000cf80: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
+0000cf90: 6163 655f 6d61 702c 0a20 2020 2029 0a20  ace_map,.    ). 
+0000cfa0: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
+0000cfb0: 6c75 6573 3a0a 2020 2020 2020 2020 6b77  lues:.        kw
+0000cfc0: 6172 6773 203d 207b 2270 6572 6d69 7373  args = {"permiss
+0000cfd0: 696f 6e73 223a 2076 616c 2e70 6572 6d69  ions": val.permi
+0000cfe0: 7373 696f 6e73 7d0a 2020 2020 2020 2020  ssions}.        
+0000cff0: 6966 2063 6865 636b 5f6e 6f74 6e61 2876  if check_notna(v
+0000d000: 616c 2e63 6f6d 6d65 6e74 293a 0a20 2020  al.comment):.   
+0000d010: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+0000d020: 2263 6f6d 6d65 6e74 225d 203d 2076 616c  "comment"] = val
+0000d030: 2e63 6f6d 6d65 6e74 0a20 2020 2020 2020  .comment.       
+0000d040: 206b 7761 7267 735b 2265 6e63 6f64 696e   kwargs["encodin
+0000d050: 6722 5d20 3d20 7661 6c2e 656e 636f 6469  g"] = val.encodi
+0000d060: 6e67 2069 6620 6368 6563 6b5f 6e6f 746e  ng if check_notn
+0000d070: 6128 7661 6c2e 656e 636f 6469 6e67 2920  a(val.encoding) 
+0000d080: 656c 7365 2022 7574 6638 220a 2020 2020  else "utf8".    
+0000d090: 2020 2020 7661 6c75 655f 203d 2065 7472      value_ = etr
+0000d0a0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+0000d0b0: 2020 2020 2020 2020 227b 2573 7d74 6578          "{%s}tex
+0000d0c0: 7422 2025 2078 6d6c 5f6e 616d 6573 7061  t" % xml_namespa
+0000d0d0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000d0e0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+0000d0f0: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
+0000d100: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
+0000d110: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
+0000d120: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000d130: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
+0000d140: 2020 2020 2069 6620 6b77 6172 6773 5b22       if kwargs["
+0000d150: 656e 636f 6469 6e67 225d 203d 3d20 2275  encoding"] == "u
+0000d160: 7466 3822 3a0a 2020 2020 2020 2020 2020  tf8":.          
+0000d170: 2020 2320 7772 6974 6520 7468 6520 7465    # write the te
+0000d180: 7874 2069 6e74 6f20 7468 6520 7461 672c  xt into the tag,
+0000d190: 2077 6974 686f 7574 2076 616c 6964 6174   without validat
+0000d1a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+0000d1b0: 7661 6c75 655f 2e74 6578 7420 3d20 7374  value_.text = st
+0000d1c0: 7228 7661 6c2e 7661 6c75 6529 0a20 2020  r(val.value).   
+0000d1d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d1e0: 2020 2020 2020 2065 7363 6170 6564 5f74         escaped_t
+0000d1f0: 6578 7420 3d20 5f65 7363 6170 655f 7265  ext = _escape_re
+0000d200: 7365 7276 6564 5f63 6861 7273 2873 7472  served_chars(str
+0000d210: 2876 616c 2e76 616c 7565 2929 0a20 2020  (val.value)).   
+0000d220: 2020 2020 2020 2020 2023 2065 6e66 6f72           # enfor
+0000d230: 6365 2074 6861 7420 7468 6520 7465 7874  ce that the text
+0000d240: 2069 7320 7765 6c6c 2d66 6f72 6d65 6420   is well-formed 
+0000d250: 584d 4c3a 2073 6572 6961 6c69 7a65 2074  XML: serialize t
+0000d260: 6167 202e 2e2e 0a20 2020 2020 2020 2020  ag ....         
+0000d270: 2020 2073 6572 6961 6c69 7a65 6420 3d20     serialized = 
+0000d280: 6574 7265 652e 746f 7374 7269 6e67 2876  etree.tostring(v
+0000d290: 616c 7565 5f2c 2065 6e63 6f64 696e 673d  alue_, encoding=
+0000d2a0: 2275 6e69 636f 6465 2229 0a20 2020 2020  "unicode").     
+0000d2b0: 2020 2020 2020 2023 202e 2e2e 2069 6e73         # ... ins
+0000d2c0: 6572 7420 7465 7874 2061 7420 7468 6520  ert text at the 
+0000d2d0: 7665 7279 2065 6e64 206f 6620 7468 6520  very end of the 
+0000d2e0: 7374 7269 6e67 2c20 616e 6420 6164 6420  string, and add 
+0000d2f0: 656e 6469 6e67 2074 6167 2074 6f20 7468  ending tag to th
+0000d300: 6520 7072 6576 696f 7573 6c79 2073 696e  e previously sin
+0000d310: 676c 6520 3c74 6578 742f 3e20 7461 6720  gle <text/> tag 
+0000d320: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+0000d330: 7365 7269 616c 697a 6564 203d 2072 6567  serialized = reg
+0000d340: 6578 2e73 7562 2872 222f 3e24 222c 2066  ex.sub(r"/>$", f
+0000d350: 223e 7b65 7363 6170 6564 5f74 6578 747d  ">{escaped_text}
+0000d360: 3c2f 7465 7874 3e22 2c20 7365 7269 616c  </text>", serial
+0000d370: 697a 6564 290a 2020 2020 2020 2020 2020  ized).          
+0000d380: 2020 2320 2e2e 2e20 7472 7920 746f 2070    # ... try to p
+0000d390: 6172 7365 2069 7420 6167 6169 6e0a 2020  arse it again.  
+0000d3a0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000d3c0: 616c 7565 5f20 3d20 6574 7265 652e 6672  alue_ = etree.fr
+0000d3d0: 6f6d 7374 7269 6e67 2873 6572 6961 6c69  omstring(seriali
+0000d3e0: 7a65 6429 0a20 2020 2020 2020 2020 2020  zed).           
+0000d3f0: 2065 7863 6570 7420 6574 7265 652e 584d   except etree.XM
+0000d400: 4c53 796e 7461 7845 7272 6f72 2061 7320  LSyntaxError as 
+0000d410: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+0000d420: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d440: 2022 5468 6520 584d 4c20 7461 6773 2063   "The XML tags c
+0000d450: 6f6e 7461 696e 6564 2069 6e20 6120 7269  ontained in a ri
+0000d460: 6368 7465 7874 2070 726f 7065 7274 7920  chtext property 
+0000d470: 2865 6e63 6f64 696e 673d 786d 6c29 206d  (encoding=xml) m
+0000d480: 7573 7420 6265 2077 656c 6c2d 666f 726d  ust be well-form
+0000d490: 6564 2e20 220a 2020 2020 2020 2020 2020  ed. ".          
+0000d4a0: 2020 2020 2020 2020 2020 2254 6865 2073            "The s
+0000d4b0: 7065 6369 616c 2063 6861 7261 6374 6572  pecial character
+0000d4c0: 7320 3c2c 203e 2061 6e64 2026 2061 7265  s <, > and & are
+0000d4d0: 206f 6e6c 7920 616c 6c6f 7765 6420 746f   only allowed to
+0000d4e0: 2063 6f6e 7374 7275 6374 2061 2074 6167   construct a tag
+0000d4f0: 2e20 220a 2020 2020 2020 2020 2020 2020  . ".            
+0000d500: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000d510: 2020 2020 2020 6966 2063 616c 6c69 6e67        if calling
+0000d520: 5f72 6573 6f75 7263 653a 0a20 2020 2020  _resource:.     
+0000d530: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000d540: 7367 202b 3d20 6622 5468 6520 6572 726f  sg += f"The erro
+0000d550: 7220 6f63 6375 7272 6564 2069 6e20 7265  r occurred in re
+0000d560: 736f 7572 6365 207b 6361 6c6c 696e 675f  source {calling_
+0000d570: 7265 736f 7572 6365 7d2c 2070 726f 7065  resource}, prope
+0000d580: 7274 7920 7b6e 616d 657d 220a 2020 2020  rty {name}".    
+0000d590: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+0000d5a0: 2b3d 2066 225c 6e4f 7269 6769 6e61 6c20  += f"\nOriginal 
+0000d5b0: 6572 726f 7220 6d65 7373 6167 653a 207b  error message: {
+0000d5c0: 6572 722e 6d73 677d 220a 2020 2020 2020  err.msg}".      
+0000d5d0: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
+0000d5e0: 2066 225c 6e45 7665 6e74 7561 6c20 6c69   f"\nEventual li
+0000d5f0: 6e65 2f63 6f6c 756d 6e20 6e75 6d62 6572  ne/column number
+0000d600: 7320 6172 6520 7265 6c61 7469 7665 2074  s are relative t
+0000d610: 6f20 7468 6973 2073 6572 6961 6c69 7a65  o this serialize
+0000d620: 6420 7465 7874 3a20 7b73 6572 6961 6c69  d text: {seriali
+0000d630: 7a65 647d 220a 2020 2020 2020 2020 2020  zed}".          
+0000d640: 2020 2020 2020 7261 6973 6520 4261 7365        raise Base
+0000d650: 4572 726f 7228 6d73 6729 2066 726f 6d20  Error(msg) from 
+0000d660: 4e6f 6e65 0a20 2020 2020 2020 2070 726f  None.        pro
+0000d670: 705f 2e61 7070 656e 6428 7661 6c75 655f  p_.append(value_
+0000d680: 290a 0a20 2020 2072 6574 7572 6e20 7072  )..    return pr
+0000d690: 6f70 5f0a 0a0a 6465 6620 5f65 7363 6170  op_...def _escap
+0000d6a0: 655f 7265 7365 7276 6564 5f63 6861 7273  e_reserved_chars
+0000d6b0: 2874 6578 743a 2073 7472 2920 2d3e 2073  (text: str) -> s
+0000d6c0: 7472 3a0a 2020 2020 2222 220a 2020 2020  tr:.    """.    
+0000d6d0: 4672 6f6d 2072 6963 6874 6578 7420 7374  From richtext st
+0000d6e0: 7269 6e67 7320 2865 6e63 6f64 696e 673d  rings (encoding=
+0000d6f0: 2278 6d6c 2229 2c20 6573 6361 7065 2074  "xml"), escape t
+0000d700: 6865 2072 6573 6572 7665 6420 6368 6172  he reserved char
+0000d710: 6163 7465 7273 203c 2c20 3e20 616e 6420  acters <, > and 
+0000d720: 262c 0a20 2020 2062 7574 206f 6e6c 7920  &,.    but only 
+0000d730: 6966 2074 6865 7920 6172 6520 6e6f 7420  if they are not 
+0000d740: 7061 7274 206f 6620 6120 7374 616e 6461  part of a standa
+0000d750: 7264 2073 7461 6e64 6f66 6620 7461 6720  rd standoff tag 
+0000d760: 6f72 2065 7363 6170 6520 7365 7175 656e  or escape sequen
+0000d770: 6365 2e0a 2020 2020 5468 6520 7374 616e  ce..    The stan
+0000d780: 6461 7264 2073 7461 6e64 6f66 6620 7461  dard standoff ta
+0000d790: 6773 2061 6c6c 6f77 6564 2062 7920 4453  gs allowed by DS
+0000d7a0: 502d 4150 4920 6172 6520 646f 6375 6d65  P-API are docume
+0000d7b0: 6e74 6564 2068 6572 653a 0a20 2020 2068  nted here:.    h
+0000d7c0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
+0000d7d0: 682e 7377 6973 732f 3230 3233 2e31 322e  h.swiss/2023.12.
+0000d7e0: 3031 2f44 5350 2d41 5049 2f30 332d 656e  01/DSP-API/03-en
+0000d7f0: 6470 6f69 6e74 732f 6170 692d 7632 2f74  dpoints/api-v2/t
+0000d800: 6578 742f 7374 616e 6461 7264 2d73 7461  ext/standard-sta
+0000d810: 6e64 6f66 662f 0a0a 2020 2020 4172 6773  ndoff/..    Args
+0000d820: 3a0a 2020 2020 2020 2020 7465 7874 3a20  :.        text: 
+0000d830: 7468 6520 7269 6368 7465 7874 2073 7472  the richtext str
+0000d840: 696e 6720 746f 2062 6520 6573 6361 7065  ing to be escape
+0000d850: 640a 0a20 2020 2052 6574 7572 6e73 3a0a  d..    Returns:.
+0000d860: 2020 2020 2020 2020 7468 6520 6573 6361          the esca
+0000d870: 7065 6420 7269 6368 7465 7874 2073 7472  ped richtext str
+0000d880: 696e 670a 2020 2020 2222 220a 2020 2020  ing.    """.    
+0000d890: 616c 6c6f 7765 645f 7461 6773 203d 205b  allowed_tags = [
+0000d8a0: 0a20 2020 2020 2020 2022 6128 205b 5e3e  .        "a( [^>
+0000d8b0: 5d2b 293f 222c 2020 2320 3c61 3e20 6973  ]+)?",  # <a> is
+0000d8c0: 2074 6865 206f 6e6c 7920 7461 6720 7468   the only tag th
+0000d8d0: 6174 2063 616e 2068 6176 6520 6174 7472  at can have attr
+0000d8e0: 6962 7574 6573 0a20 2020 2020 2020 2022  ibutes.        "
+0000d8f0: 7022 2c0a 2020 2020 2020 2020 2265 6d22  p",.        "em"
+0000d900: 2c0a 2020 2020 2020 2020 2273 7472 6f6e  ,.        "stron
+0000d910: 6722 2c0a 2020 2020 2020 2020 2275 222c  g",.        "u",
+0000d920: 0a20 2020 2020 2020 2022 7375 6222 2c0a  .        "sub",.
+0000d930: 2020 2020 2020 2020 2273 7570 222c 0a20          "sup",. 
+0000d940: 2020 2020 2020 2022 7374 7269 6b65 222c         "strike",
+0000d950: 0a20 2020 2020 2020 2022 6831 222c 0a20  .        "h1",. 
+0000d960: 2020 2020 2020 2022 6f6c 222c 0a20 2020         "ol",.   
+0000d970: 2020 2020 2022 756c 222c 0a20 2020 2020       "ul",.     
+0000d980: 2020 2022 6c69 222c 0a20 2020 2020 2020     "li",.       
+0000d990: 2022 7462 6f64 7922 2c0a 2020 2020 2020   "tbody",.      
+0000d9a0: 2020 2274 6162 6c65 222c 0a20 2020 2020    "table",.     
+0000d9b0: 2020 2022 7472 222c 0a20 2020 2020 2020     "tr",.       
+0000d9c0: 2022 7464 222c 0a20 2020 2020 2020 2022   "td",.        "
+0000d9d0: 6272 222c 0a20 2020 2020 2020 2022 6872  br",.        "hr
+0000d9e0: 222c 0a20 2020 2020 2020 2022 7072 6522  ",.        "pre"
+0000d9f0: 2c0a 2020 2020 2020 2020 2263 6974 6522  ,.        "cite"
+0000da00: 2c0a 2020 2020 2020 2020 2262 6c6f 636b  ,.        "block
+0000da10: 7175 6f74 6522 2c0a 2020 2020 2020 2020  quote",.        
+0000da20: 2263 6f64 6522 2c0a 2020 2020 5d0a 2020  "code",.    ].  
+0000da30: 2020 616c 6c6f 7765 645f 7461 6773 5f72    allowed_tags_r
+0000da40: 6567 6578 203d 2022 7c22 2e6a 6f69 6e28  egex = "|".join(
+0000da50: 616c 6c6f 7765 645f 7461 6773 290a 2020  allowed_tags).  
+0000da60: 2020 6c6f 6f6b 6168 6561 6420 3d20 7266    lookahead = rf
+0000da70: 2228 3f21 2f3f 287b 616c 6c6f 7765 645f  "(?!/?({allowed_
+0000da80: 7461 6773 5f72 6567 6578 7d29 2f3f 3e29  tags_regex})/?>)
+0000da90: 220a 2020 2020 696c 6c65 6761 6c5f 6c74  ".    illegal_lt
+0000daa0: 203d 2072 6622 3c7b 6c6f 6f6b 6168 6561   = rf"<{lookahea
+0000dab0: 647d 220a 2020 2020 6c6f 6f6b 6265 6869  d}".    lookbehi
+0000dac0: 6e64 203d 2072 6622 283f 3c21 3c2f 3f28  nd = rf"(?<!</?(
+0000dad0: 7b61 6c6c 6f77 6564 5f74 6167 735f 7265  {allowed_tags_re
+0000dae0: 6765 787d 292f 3f29 220a 2020 2020 696c  gex})/?)".    il
+0000daf0: 6c65 6761 6c5f 6774 203d 2072 6622 7b6c  legal_gt = rf"{l
+0000db00: 6f6f 6b62 6568 696e 647d 3e22 0a20 2020  ookbehind}>".   
+0000db10: 2069 6c6c 6567 616c 5f61 6d70 203d 2072   illegal_amp = r
+0000db20: 2226 283f 215b 2361 2d7a 412d 5a30 2d39  "&(?![#a-zA-Z0-9
+0000db30: 5d2b 3b29 220a 2020 2020 7465 7874 203d  ]+;)".    text =
+0000db40: 2072 6567 6578 2e73 7562 2869 6c6c 6567   regex.sub(illeg
+0000db50: 616c 5f6c 742c 2022 266c 743b 222c 2074  al_lt, "&lt;", t
+0000db60: 6578 7429 0a20 2020 2074 6578 7420 3d20  ext).    text = 
+0000db70: 7265 6765 782e 7375 6228 696c 6c65 6761  regex.sub(illega
+0000db80: 6c5f 6774 2c20 2226 6774 3b22 2c20 7465  l_gt, "&gt;", te
+0000db90: 7874 290a 2020 2020 7465 7874 203d 2072  xt).    text = r
+0000dba0: 6567 6578 2e73 7562 2869 6c6c 6567 616c  egex.sub(illegal
+0000dbb0: 5f61 6d70 2c20 2226 616d 703b 222c 2074  _amp, "&amp;", t
+0000dbc0: 6578 7429 0a20 2020 2072 6574 7572 6e20  ext).    return 
+0000dbd0: 7465 7874 0a0a 0a64 6566 206d 616b 655f  text...def make_
+0000dbe0: 7469 6d65 5f70 726f 7028 0a20 2020 206e  time_prop(.    n
+0000dbf0: 616d 653a 2073 7472 2c0a 2020 2020 7661  ame: str,.    va
+0000dc00: 6c75 653a 2055 6e69 6f6e 5b50 726f 7065  lue: Union[Prope
+0000dc10: 7274 7945 6c65 6d65 6e74 2c20 7374 722c  rtyElement, str,
+0000dc20: 2049 7465 7261 626c 655b 556e 696f 6e5b   Iterable[Union[
+0000dc30: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
+0000dc40: 2073 7472 5d5d 5d2c 0a20 2020 2063 616c   str]]],.    cal
+0000dc50: 6c69 6e67 5f72 6573 6f75 7263 653a 2073  ling_resource: s
+0000dc60: 7472 203d 2022 222c 0a29 202d 3e20 6574  tr = "",.) -> et
+0000dc70: 7265 652e 5f45 6c65 6d65 6e74 3a0a 2020  ree._Element:.  
+0000dc80: 2020 2222 220a 2020 2020 4d61 6b65 2061    """.    Make a
+0000dc90: 203c 7469 6d65 2d70 726f 703e 2066 726f   <time-prop> fro
+0000dca0: 6d20 6f6e 6520 6f72 206d 6f72 6520 6461  m one or more da
+0000dcb0: 7465 7469 6d65 2076 616c 7565 7320 6f66  tetime values of
+0000dcc0: 2074 6865 2066 6f72 6d20 2232 3030 392d   the form "2009-
+0000dcd0: 3130 2d31 3054 3132 3a30 303a 3030 2d30  10-10T12:00:00-0
+0000dce0: 353a 3030 222e 2054 6865 2074 696d 6528  5:00". The time(
+0000dcf0: 7329 2063 616e 2062 650a 2020 2020 7072  s) can be.    pr
+0000dd00: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
+0000dd10: 206f 7220 6173 2050 726f 7065 7274 7945   or as PropertyE
+0000dd20: 6c65 6d65 6e74 2077 6974 6820 6120 7374  lement with a st
+0000dd30: 7269 6e67 2069 6e73 6964 652e 2049 6620  ring inside. If 
+0000dd40: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+0000dd50: 6e67 2c20 7468 6520 7065 726d 6973 7369  ng, the permissi
+0000dd60: 6f6e 7320 6465 6661 756c 7420 746f 0a20  ons default to. 
+0000dd70: 2020 2022 7072 6f70 2d64 6566 6175 6c74     "prop-default
+0000dd80: 222e 0a0a 2020 2020 4172 6773 3a0a 2020  "...    Args:.  
+0000dd90: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
+0000dda0: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
+0000ddb0: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
+0000ddc0: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
+0000ddd0: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
+0000dde0: 6f72 206d 6f72 6520 4453 5020 7469 6d65  or more DSP time
+0000ddf0: 732c 2061 7320 7374 7269 6e67 2f50 726f  s, as string/Pro
+0000de00: 7065 7274 7945 6c65 6d65 6e74 2c20 6f72  pertyElement, or
+0000de10: 2061 7320 6974 6572 6162 6c65 206f 6620   as iterable of 
+0000de20: 7374 7269 6e67 732f 5072 6f70 6572 7479  strings/Property
+0000de30: 456c 656d 656e 7473 0a20 2020 2020 2020  Elements.       
+0000de40: 2063 616c 6c69 6e67 5f72 6573 6f75 7263   calling_resourc
+0000de50: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+0000de60: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
+0000de70: 6365 2028 666f 7220 6265 7474 6572 2065  ce (for better e
+0000de80: 7272 6f72 206d 6573 7361 6765 7329 0a0a  rror messages)..
+0000de90: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000dea0: 2020 2020 4261 7365 4572 726f 723a 2049      BaseError: I
+0000deb0: 6620 6f6e 6520 6f66 2074 6865 2076 616c  f one of the val
+0000dec0: 7565 7320 6973 206e 6f74 2061 2076 616c  ues is not a val
+0000ded0: 6964 2044 5350 2074 696d 6520 7374 7269  id DSP time stri
+0000dee0: 6e67 0a0a 2020 2020 5265 7475 726e 733a  ng..    Returns:
+0000def0: 0a20 2020 2020 2020 2061 6e20 6574 7265  .        an etre
+0000df00: 652e 5f45 6c65 6d65 6e74 2074 6861 7420  e._Element that 
+0000df10: 6361 6e20 6265 2061 7070 656e 6465 6420  can be appended 
+0000df20: 746f 2074 6865 2070 6172 656e 7420 7265  to the parent re
+0000df30: 736f 7572 6365 2077 6974 6820 7265 736f  source with reso
+0000df40: 7572 6365 2e61 7070 656e 6428 6d61 6b65  urce.append(make
+0000df50: 5f2a 5f70 726f 7028 2e2e 2e29 290a 0a20  _*_prop(...)).. 
+0000df60: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+0000df70: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+0000df80: 6d6c 2e6d 616b 655f 7469 6d65 5f70 726f  ml.make_time_pro
+0000df90: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+0000dfa0: 222c 2022 3230 3039 2d31 302d 3130 5431  ", "2009-10-10T1
+0000dfb0: 323a 3030 3a30 302d 3035 3a30 3022 290a  2:00:00-05:00").
+0000dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfd0: 3c74 696d 652d 7072 6f70 206e 616d 653d  <time-prop name=
+0000dfe0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+0000dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e000: 2020 2020 203c 7469 6d65 2070 6572 6d69       <time permi
+0000e010: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+0000e020: 6175 6c74 223e 0a20 2020 2020 2020 2020  ault">.         
+0000e030: 2020 2020 2020 2020 2020 2020 2020 2032                 2
+0000e040: 3030 392d 3130 2d31 3054 3132 3a30 303a  009-10-10T12:00:
+0000e050: 3030 2d30 353a 3030 0a20 2020 2020 2020  00-05:00.       
+0000e060: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+0000e070: 696d 653e 0a20 2020 2020 2020 2020 2020  ime>.           
+0000e080: 2020 2020 203c 2f74 696d 652d 7072 6f70       </time-prop
+0000e090: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
+0000e0a0: 6365 6c32 786d 6c2e 6d61 6b65 5f74 696d  cel2xml.make_tim
+0000e0b0: 655f 7072 6f70 2822 3a74 6573 7470 726f  e_prop(":testpro
+0000e0c0: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
+0000e0d0: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
+0000e0e0: 7428 2232 3030 392d 3130 2d31 3054 3132  t("2009-10-10T12
+0000e0f0: 3a30 303a 3030 2d30 353a 3030 222c 2070  :00:00-05:00", p
+0000e100: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000e110: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
+0000e120: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
+0000e130: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e140: 2020 3c74 696d 652d 7072 6f70 206e 616d    <time-prop nam
+0000e150: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+0000e160: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000e170: 2020 2020 2020 203c 7469 6d65 2070 6572         <time per
+0000e180: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
+0000e190: 6573 7472 6963 7465 6422 2063 6f6d 6d65  estricted" comme
+0000e1a0: 6e74 3d22 6578 616d 706c 6522 3e0a 2020  nt="example">.  
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 2020 2020 2020 3230 3039 2d31 302d 3130        2009-10-10
+0000e1d0: 5431 323a 3030 3a30 302d 3035 3a30 300a  T12:00:00-05:00.
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 3c2f 7469 6d65 3e0a 2020 2020      </time>.    
 0000e200: 2020 2020 2020 2020 2020 2020 3c2f 7469              </ti
-0000e210: 6d65 3e0a 2020 2020 2020 2020 2020 2020  me>.            
-0000e220: 2020 2020 3c2f 7469 6d65 2d70 726f 703e      </time-prop>
-0000e230: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-0000e240: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
-0000e250: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
-0000e260: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
-0000e270: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
-0000e280: 7469 6d65 2d70 726f 700a 2020 2020 2222  time-prop.    ""
-0000e290: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
-0000e2a0: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
-0000e2b0: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
-0000e2c0: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
-0000e2d0: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
-0000e2e0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
-0000e2f0: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
-0000e300: 7479 7065 0a20 2020 2076 616c 6964 6174  type.    validat
-0000e310: 696f 6e5f 7265 6765 7820 3d20 7222 5e5c  ion_regex = r"^\
-0000e320: 647b 347d 2d5b 302d 315d 5c64 2d5b 302d  d{4}-[0-1]\d-[0-
-0000e330: 335d 5c64 545b 302d 325d 5c64 3a5b 302d  3]\dT[0-2]\d:[0-
-0000e340: 355d 5c64 3a5b 302d 355d 5c64 282e 5c64  5]\d:[0-5]\d(.\d
-0000e350: 7b31 2c31 327d 293f 285a 7c5b 2b2d 5d5b  {1,12})?(Z|[+-][
-0000e360: 302d 315d 5c64 3a5b 302d 355d 5c64 2924  0-1]\d:[0-5]\d)$
-0000e370: 220a 2020 2020 666f 7220 7661 6c20 696e  ".    for val in
-0000e380: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
-0000e390: 2069 6620 6e6f 7420 7265 6765 782e 7365   if not regex.se
-0000e3a0: 6172 6368 2876 616c 6964 6174 696f 6e5f  arch(validation_
-0000e3b0: 7265 6765 782c 2073 7472 2876 616c 2e76  regex, str(val.v
-0000e3c0: 616c 7565 2929 3a0a 2020 2020 2020 2020  alue)):.        
-0000e3d0: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
-0000e3e0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000e3f0: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
-0000e400: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
-0000e410: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
-0000e420: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
-0000e430: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
-0000e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e450: 6622 277b 7661 6c2e 7661 6c75 657d 2720  f"'{val.value}' 
-0000e460: 6973 206e 6f74 2061 2076 616c 6964 2044  is not a valid D
-0000e470: 5350 2074 696d 652e 220a 2020 2020 2020  SP time.".      
-0000e480: 2020 2020 2020 290a 0a20 2020 2023 206d        )..    # m
-0000e490: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
-0000e4a0: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
-0000e4b0: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
-0000e4c0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-0000e4d0: 0a20 2020 2020 2020 2022 7b25 737d 7469  .        "{%s}ti
-0000e4e0: 6d65 2d70 726f 7022 2025 2078 6d6c 5f6e  me-prop" % xml_n
-0000e4f0: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-0000e500: 655d 2c0a 2020 2020 2020 2020 6e61 6d65  e],.        name
-0000e510: 3d6e 616d 652c 0a20 2020 2020 2020 206e  =name,.        n
-0000e520: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
-0000e530: 6365 5f6d 6170 2c0a 2020 2020 290a 2020  ce_map,.    ).  
-0000e540: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
-0000e550: 7565 733a 0a20 2020 2020 2020 206b 7761  ues:.        kwa
-0000e560: 7267 7320 3d20 7b22 7065 726d 6973 7369  rgs = {"permissi
-0000e570: 6f6e 7322 3a20 7661 6c2e 7065 726d 6973  ons": val.permis
-0000e580: 7369 6f6e 737d 0a20 2020 2020 2020 2069  sions}.        i
-0000e590: 6620 7661 6c2e 636f 6d6d 656e 7420 616e  f val.comment an
-0000e5a0: 6420 6368 6563 6b5f 6e6f 746e 6128 7661  d check_notna(va
-0000e5b0: 6c2e 636f 6d6d 656e 7429 3a0a 2020 2020  l.comment):.    
-0000e5c0: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-0000e5d0: 636f 6d6d 656e 7422 5d20 3d20 7661 6c2e  comment"] = val.
-0000e5e0: 636f 6d6d 656e 740a 2020 2020 2020 2020  comment.        
-0000e5f0: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
-0000e600: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0000e610: 2020 2020 227b 2573 7d74 696d 6522 2025      "{%s}time" %
-0000e620: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-0000e630: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
-0000e640: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
-0000e650: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
-0000e660: 6172 672d 7479 7065 5d0a 2020 2020 2020  arg-type].      
-0000e670: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-0000e680: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-0000e690: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000e6a0: 2076 616c 7565 5f2e 7465 7874 203d 2073   value_.text = s
-0000e6b0: 7472 2876 616c 2e76 616c 7565 290a 2020  tr(val.value).  
-0000e6c0: 2020 2020 2020 7072 6f70 5f2e 6170 7065        prop_.appe
-0000e6d0: 6e64 2876 616c 7565 5f29 0a0a 2020 2020  nd(value_)..    
-0000e6e0: 7265 7475 726e 2070 726f 705f 0a0a 0a64  return prop_...d
-0000e6f0: 6566 206d 616b 655f 7572 695f 7072 6f70  ef make_uri_prop
-0000e700: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-0000e710: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-0000e720: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-0000e730: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
-0000e740: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
-0000e750: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
-0000e760: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-0000e770: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-0000e780: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-0000e790: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-0000e7a0: 204d 616b 6520 616e 203c 7572 692d 7072   Make an <uri-pr
-0000e7b0: 6f70 3e20 6672 6f6d 206f 6e65 206f 7220  op> from one or 
-0000e7c0: 6d6f 7265 2055 5249 732e 2054 6865 2055  more URIs. The U
-0000e7d0: 5249 2873 2920 6361 6e20 6265 2070 726f  RI(s) can be pro
-0000e7e0: 7669 6465 6420 6173 2073 7472 696e 6720  vided as string 
-0000e7f0: 6f72 2061 7320 5072 6f70 6572 7479 456c  or as PropertyEl
-0000e800: 656d 656e 7420 7769 7468 2061 2073 7472  ement with a str
-0000e810: 696e 670a 2020 2020 696e 7369 6465 2e20  ing.    inside. 
-0000e820: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
-0000e830: 7472 696e 672c 2074 6865 2070 6572 6d69  tring, the permi
-0000e840: 7373 696f 6e73 2064 6566 6175 6c74 2074  ssions default t
-0000e850: 6f20 2270 726f 702d 6465 6661 756c 7422  o "prop-default"
-0000e860: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000e870: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-0000e880: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-0000e890: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
-0000e8a0: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
-0000e8b0: 2020 2020 7661 6c75 653a 206f 6e65 206f      value: one o
-0000e8c0: 7220 6d6f 7265 2055 5249 732c 2061 7320  r more URIs, as 
-0000e8d0: 7374 7269 6e67 2f50 726f 7065 7274 7945  string/PropertyE
-0000e8e0: 6c65 6d65 6e74 2c20 6f72 2061 7320 6974  lement, or as it
-0000e8f0: 6572 6162 6c65 206f 6620 7374 7269 6e67  erable of string
-0000e900: 732f 5072 6f70 6572 7479 456c 656d 656e  s/PropertyElemen
-0000e910: 7473 0a20 2020 2020 2020 2063 616c 6c69  ts.        calli
-0000e920: 6e67 5f72 6573 6f75 7263 653a 2074 6865  ng_resource: the
-0000e930: 206e 616d 6520 6f66 2074 6865 2070 6172   name of the par
-0000e940: 656e 7420 7265 736f 7572 6365 2028 666f  ent resource (fo
-0000e950: 7220 6265 7474 6572 2065 7272 6f72 206d  r better error m
-0000e960: 6573 7361 6765 7329 0a0a 2020 2020 5261  essages)..    Ra
-0000e970: 6973 6573 3a0a 2020 2020 2020 2020 4261  ises:.        Ba
-0000e980: 7365 4572 726f 723a 2049 6620 6f6e 6520  seError: If one 
-0000e990: 6f66 2074 6865 2076 616c 7565 7320 6973  of the values is
-0000e9a0: 206e 6f74 2061 2076 616c 6964 2055 5249   not a valid URI
-0000e9b0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-0000e9c0: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
-0000e9d0: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
-0000e9e0: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
-0000e9f0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-0000ea00: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
-0000ea10: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
-0000ea20: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
-0000ea30: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-0000ea40: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-0000ea50: 2e6d 616b 655f 7572 695f 7072 6f70 2822  .make_uri_prop("
-0000ea60: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-0000ea70: 2277 7777 2e74 6573 742e 636f 6d22 290a  "www.test.com").
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea90: 3c75 7269 2d70 726f 7020 6e61 6d65 3d22  <uri-prop name="
-0000eaa0: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 2020 3c75 7269 2070 6572 6d69 7373      <uri permiss
-0000ead0: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
-0000eae0: 6c74 223e 7777 772e 7465 7374 2e63 6f6d  lt">www.test.com
-0000eaf0: 3c2f 7572 693e 0a20 2020 2020 2020 2020  </uri>.         
-0000eb00: 2020 2020 2020 203c 2f75 7269 2d70 726f         </uri-pro
-0000eb10: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-0000eb20: 7863 656c 3278 6d6c 2e6d 616b 655f 7572  xcel2xml.make_ur
-0000eb30: 695f 7072 6f70 2822 3a74 6573 7470 726f  i_prop(":testpro
-0000eb40: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
-0000eb50: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
-0000eb60: 7428 2277 7777 2e74 6573 742e 636f 6d22  t("www.test.com"
-0000eb70: 2c20 7065 726d 6973 7369 6f6e 733d 2270  , permissions="p
-0000eb80: 726f 702d 7265 7374 7269 6374 6564 222c  rop-restricted",
-0000eb90: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
-0000eba0: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
-0000ebb0: 2020 2020 203c 7572 692d 7072 6f70 206e       <uri-prop n
-0000ebc0: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-0000ebd0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-0000ebe0: 2020 2020 2020 2020 203c 7572 6920 7065           <uri pe
-0000ebf0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000ec00: 7265 7374 7269 6374 6564 2220 636f 6d6d  restricted" comm
-0000ec10: 656e 743d 2265 7861 6d70 6c65 223e 7777  ent="example">ww
-0000ec20: 772e 7465 7374 2e63 6f6d 3c2f 7572 693e  w.test.com</uri>
+0000e210: 6d65 2d70 726f 703e 0a20 2020 2020 2020  me-prop>.       
+0000e220: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000e230: 616b 655f 7469 6d65 5f70 726f 7028 223a  ake_time_prop(":
+0000e240: 7465 7374 7072 6f70 6572 7479 222c 205b  testproperty", [
+0000e250: 2232 3030 392d 3130 2d31 3054 3132 3a30  "2009-10-10T12:0
+0000e260: 303a 3030 2d30 353a 3030 222c 2022 3139  0:00-05:00", "19
+0000e270: 3031 2d30 312d 3031 5430 313a 3030 3a30  01-01-01T01:00:0
+0000e280: 302d 3030 3a30 3022 5d29 0a20 2020 2020  0-00:00"]).     
+0000e290: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
+0000e2a0: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
+0000e2b0: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2d0: 3c74 696d 6520 7065 726d 6973 7369 6f6e  <time permission
+0000e2e0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000e2f0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000e300: 2020 2020 2020 2020 2020 3230 3039 2d31            2009-1
+0000e310: 302d 3130 5431 323a 3030 3a30 302d 3035  0-10T12:00:00-05
+0000e320: 3a30 300a 2020 2020 2020 2020 2020 2020  :00.            
+0000e330: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e350: 2020 2020 3c74 696d 6520 7065 726d 6973      <time permis
+0000e360: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+0000e370: 756c 7422 3e0a 2020 2020 2020 2020 2020  ult">.          
+0000e380: 2020 2020 2020 2020 2020 2020 2020 3139                19
+0000e390: 3031 2d30 312d 3031 5430 313a 3030 3a30  01-01-01T01:00:0
+0000e3a0: 302d 3030 3a30 3032 0a20 2020 2020 2020  0-00:002.       
+0000e3b0: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+0000e3c0: 696d 653e 0a20 2020 2020 2020 2020 2020  ime>.           
+0000e3d0: 2020 2020 203c 2f74 696d 652d 7072 6f70       </time-prop
+0000e3e0: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
+0000e3f0: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+0000e400: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+0000e410: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+0000e420: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+0000e430: 2374 696d 652d 7072 6f70 0a20 2020 2022  #time-prop.    "
+0000e440: 2222 0a0a 2020 2020 2320 6368 6563 6b20  ""..    # check 
+0000e450: 7468 6520 696e 7075 743a 2070 7265 7061  the input: prepa
+0000e460: 7265 2061 206c 6973 7420 7769 7468 2076  re a list with v
+0000e470: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
+0000e480: 7661 6c75 6573 203d 2070 7265 7061 7265  values = prepare
+0000e490: 5f76 616c 7565 2876 616c 7565 290a 0a20  _value(value).. 
+0000e4a0: 2020 2023 2063 6865 636b 2076 616c 7565     # check value
+0000e4b0: 2074 7970 650a 2020 2020 7661 6c69 6461   type.    valida
+0000e4c0: 7469 6f6e 5f72 6567 6578 203d 2072 225e  tion_regex = r"^
+0000e4d0: 5c64 7b34 7d2d 5b30 2d31 5d5c 642d 5b30  \d{4}-[0-1]\d-[0
+0000e4e0: 2d33 5d5c 6454 5b30 2d32 5d5c 643a 5b30  -3]\dT[0-2]\d:[0
+0000e4f0: 2d35 5d5c 643a 5b30 2d35 5d5c 6428 2e5c  -5]\d:[0-5]\d(.\
+0000e500: 647b 312c 3132 7d29 3f28 5a7c 5b2b 2d5d  d{1,12})?(Z|[+-]
+0000e510: 5b30 2d31 5d5c 643a 5b30 2d35 5d5c 6429  [0-1]\d:[0-5]\d)
+0000e520: 2422 0a20 2020 2066 6f72 2076 616c 2069  $".    for val i
+0000e530: 6e20 7661 6c75 6573 3a0a 2020 2020 2020  n values:.      
+0000e540: 2020 6966 206e 6f74 2072 6567 6578 2e73    if not regex.s
+0000e550: 6561 7263 6828 7661 6c69 6461 7469 6f6e  earch(validation
+0000e560: 5f72 6567 6578 2c20 7374 7228 7661 6c2e  _regex, str(val.
+0000e570: 7661 6c75 6529 293a 0a20 2020 2020 2020  value)):.       
+0000e580: 2020 2020 2072 6169 7365 2042 6173 6545       raise BaseE
+0000e590: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000e5a0: 2020 2020 2020 6622 4661 696c 6564 2076        f"Failed v
+0000e5b0: 616c 6964 6174 696f 6e20 696e 2072 6573  alidation in res
+0000e5c0: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
+0000e5d0: 7265 736f 7572 6365 7d27 2c20 7072 6f70  resource}', prop
+0000e5e0: 6572 7479 2027 7b6e 616d 657d 273a 2022  erty '{name}': "
+0000e5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e600: 2066 2227 7b76 616c 2e76 616c 7565 7d27   f"'{val.value}'
+0000e610: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
+0000e620: 4453 5020 7469 6d65 2e22 0a20 2020 2020  DSP time.".     
+0000e630: 2020 2020 2020 2029 0a0a 2020 2020 2320         )..    # 
+0000e640: 6d61 6b65 2078 6d6c 2073 7472 7563 7475  make xml structu
+0000e650: 7265 206f 6620 7468 6520 7661 6c69 6420  re of the valid 
+0000e660: 7661 6c75 6573 0a20 2020 2070 726f 705f  values.    prop_
+0000e670: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+0000e680: 280a 2020 2020 2020 2020 227b 2573 7d74  (.        "{%s}t
+0000e690: 696d 652d 7072 6f70 2220 2520 786d 6c5f  ime-prop" % xml_
+0000e6a0: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
+0000e6b0: 6e65 5d2c 0a20 2020 2020 2020 206e 616d  ne],.        nam
+0000e6c0: 653d 6e61 6d65 2c0a 2020 2020 2020 2020  e=name,.        
+0000e6d0: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
+0000e6e0: 6163 655f 6d61 702c 0a20 2020 2029 0a20  ace_map,.    ). 
+0000e6f0: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
+0000e700: 6c75 6573 3a0a 2020 2020 2020 2020 6b77  lues:.        kw
+0000e710: 6172 6773 203d 207b 2270 6572 6d69 7373  args = {"permiss
+0000e720: 696f 6e73 223a 2076 616c 2e70 6572 6d69  ions": val.permi
+0000e730: 7373 696f 6e73 7d0a 2020 2020 2020 2020  ssions}.        
+0000e740: 6966 2076 616c 2e63 6f6d 6d65 6e74 2061  if val.comment a
+0000e750: 6e64 2063 6865 636b 5f6e 6f74 6e61 2876  nd check_notna(v
+0000e760: 616c 2e63 6f6d 6d65 6e74 293a 0a20 2020  al.comment):.   
+0000e770: 2020 2020 2020 2020 206b 7761 7267 735b           kwargs[
+0000e780: 2263 6f6d 6d65 6e74 225d 203d 2076 616c  "comment"] = val
+0000e790: 2e63 6f6d 6d65 6e74 0a20 2020 2020 2020  .comment.       
+0000e7a0: 2076 616c 7565 5f20 3d20 6574 7265 652e   value_ = etree.
+0000e7b0: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+0000e7c0: 2020 2020 2022 7b25 737d 7469 6d65 2220       "{%s}time" 
+0000e7d0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+0000e7e0: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+0000e7f0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+0000e800: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+0000e810: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
+0000e820: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
+0000e830: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
+0000e840: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e850: 2020 7661 6c75 655f 2e74 6578 7420 3d20    value_.text = 
+0000e860: 7374 7228 7661 6c2e 7661 6c75 6529 0a20  str(val.value). 
+0000e870: 2020 2020 2020 2070 726f 705f 2e61 7070         prop_.app
+0000e880: 656e 6428 7661 6c75 655f 290a 0a20 2020  end(value_)..   
+0000e890: 2072 6574 7572 6e20 7072 6f70 5f0a 0a0a   return prop_...
+0000e8a0: 6465 6620 6d61 6b65 5f75 7269 5f70 726f  def make_uri_pro
+0000e8b0: 7028 0a20 2020 206e 616d 653a 2073 7472  p(.    name: str
+0000e8c0: 2c0a 2020 2020 7661 6c75 653a 2055 6e69  ,.    value: Uni
+0000e8d0: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
+0000e8e0: 6e74 2c20 7374 722c 2049 7465 7261 626c  nt, str, Iterabl
+0000e8f0: 655b 556e 696f 6e5b 5072 6f70 6572 7479  e[Union[Property
+0000e900: 456c 656d 656e 742c 2073 7472 5d5d 5d2c  Element, str]]],
+0000e910: 0a20 2020 2063 616c 6c69 6e67 5f72 6573  .    calling_res
+0000e920: 6f75 7263 653a 2073 7472 203d 2022 222c  ource: str = "",
+0000e930: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
+0000e940: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
+0000e950: 2020 4d61 6b65 2061 6e20 3c75 7269 2d70    Make an <uri-p
+0000e960: 726f 703e 2066 726f 6d20 6f6e 6520 6f72  rop> from one or
+0000e970: 206d 6f72 6520 5552 4973 2e20 5468 6520   more URIs. The 
+0000e980: 5552 4928 7329 2063 616e 2062 6520 7072  URI(s) can be pr
+0000e990: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
+0000e9a0: 206f 7220 6173 2050 726f 7065 7274 7945   or as PropertyE
+0000e9b0: 6c65 6d65 6e74 2077 6974 6820 6120 7374  lement with a st
+0000e9c0: 7269 6e67 0a20 2020 2069 6e73 6964 652e  ring.    inside.
+0000e9d0: 2049 6620 7072 6f76 6964 6564 2061 7320   If provided as 
+0000e9e0: 7374 7269 6e67 2c20 7468 6520 7065 726d  string, the perm
+0000e9f0: 6973 7369 6f6e 7320 6465 6661 756c 7420  issions default 
+0000ea00: 746f 2022 7072 6f70 2d64 6566 6175 6c74  to "prop-default
+0000ea10: 222e 0a0a 2020 2020 4172 6773 3a0a 2020  "...    Args:.  
+0000ea20: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
+0000ea30: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
+0000ea40: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
+0000ea50: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
+0000ea60: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
+0000ea70: 6f72 206d 6f72 6520 5552 4973 2c20 6173  or more URIs, as
+0000ea80: 2073 7472 696e 672f 5072 6f70 6572 7479   string/Property
+0000ea90: 456c 656d 656e 742c 206f 7220 6173 2069  Element, or as i
+0000eaa0: 7465 7261 626c 6520 6f66 2073 7472 696e  terable of strin
+0000eab0: 6773 2f50 726f 7065 7274 7945 6c65 6d65  gs/PropertyEleme
+0000eac0: 6e74 730a 2020 2020 2020 2020 6361 6c6c  nts.        call
+0000ead0: 696e 675f 7265 736f 7572 6365 3a20 7468  ing_resource: th
+0000eae0: 6520 6e61 6d65 206f 6620 7468 6520 7061  e name of the pa
+0000eaf0: 7265 6e74 2072 6573 6f75 7263 6520 2866  rent resource (f
+0000eb00: 6f72 2062 6574 7465 7220 6572 726f 7220  or better error 
+0000eb10: 6d65 7373 6167 6573 290a 0a20 2020 2052  messages)..    R
+0000eb20: 6169 7365 733a 0a20 2020 2020 2020 2042  aises:.        B
+0000eb30: 6173 6545 7272 6f72 3a20 4966 206f 6e65  aseError: If one
+0000eb40: 206f 6620 7468 6520 7661 6c75 6573 2069   of the values i
+0000eb50: 7320 6e6f 7420 6120 7661 6c69 6420 5552  s not a valid UR
+0000eb60: 490a 0a20 2020 2052 6574 7572 6e73 3a0a  I..    Returns:.
+0000eb70: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
+0000eb80: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
+0000eb90: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
+0000eba0: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
+0000ebb0: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
+0000ebc0: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
+0000ebd0: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
+0000ebe0: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+0000ebf0: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+0000ec00: 6c2e 6d61 6b65 5f75 7269 5f70 726f 7028  l.make_uri_prop(
+0000ec10: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
+0000ec20: 2022 7777 772e 7465 7374 2e63 6f6d 2229   "www.test.com")
 0000ec30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec40: 203c 2f75 7269 2d70 726f 703e 0a20 2020   </uri-prop>.   
-0000ec50: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-0000ec60: 6d6c 2e6d 616b 655f 7572 695f 7072 6f70  ml.make_uri_prop
-0000ec70: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-0000ec80: 2c20 5b22 7777 772e 312e 636f 6d22 2c20  , ["www.1.com", 
-0000ec90: 2277 7777 2e32 2e63 6f6d 225d 290a 2020  "www.2.com"]).  
-0000eca0: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
-0000ecb0: 7269 2d70 726f 7020 6e61 6d65 3d22 3a74  ri-prop name=":t
-0000ecc0: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2020 3c75 7269 2070 6572 6d69 7373 696f    <uri permissio
-0000ecf0: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
-0000ed00: 223e 7777 772e 312e 636f 6d3c 2f75 7269  ">www.1.com</uri
-0000ed10: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000ed20: 2020 2020 2020 3c75 7269 2070 6572 6d69        <uri permi
-0000ed30: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-0000ed40: 6175 6c74 223e 7777 772e 322e 636f 6d3c  ault">www.2.com<
-0000ed50: 2f75 7269 3e0a 2020 2020 2020 2020 2020  /uri>.          
-0000ed60: 2020 2020 2020 3c2f 7572 692d 7072 6f70        </uri-prop
-0000ed70: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-0000ed80: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-0000ed90: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-0000eda0: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-0000edb0: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-0000edc0: 2375 7269 2d70 726f 700a 2020 2020 2222  #uri-prop.    ""
-0000edd0: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
-0000ede0: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
-0000edf0: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
-0000ee00: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
-0000ee10: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
-0000ee20: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
-0000ee30: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
-0000ee40: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
-0000ee50: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-0000ee60: 2020 2020 6966 206e 6f74 2069 735f 7572      if not is_ur
-0000ee70: 6928 7374 7228 7661 6c2e 7661 6c75 6529  i(str(val.value)
-0000ee80: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000ee90: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-0000eec0: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
-0000eed0: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
-0000eee0: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
-0000eef0: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
-0000ef00: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
-0000ef10: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
-0000ef20: 7420 6120 7661 6c69 6420 5552 492e 220a  t a valid URI.".
-0000ef30: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000ef40: 2020 2023 206d 616b 6520 786d 6c20 7374     # make xml st
-0000ef50: 7275 6374 7572 6520 6f66 2074 6865 2076  ructure of the v
-0000ef60: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
-0000ef70: 7072 6f70 5f20 3d20 6574 7265 652e 456c  prop_ = etree.El
-0000ef80: 656d 656e 7428 0a20 2020 2020 2020 2022  ement(.        "
-0000ef90: 7b25 737d 7572 692d 7072 6f70 2220 2520  {%s}uri-prop" % 
-0000efa0: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000efb0: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
-0000efc0: 206e 616d 653d 6e61 6d65 2c0a 2020 2020   name=name,.    
-0000efd0: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
-0000efe0: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
-0000eff0: 2029 0a20 2020 2066 6f72 2076 616c 2069   ).    for val i
-0000f000: 6e20 7661 6c75 6573 3a0a 2020 2020 2020  n values:.      
-0000f010: 2020 6b77 6172 6773 203d 207b 2270 6572    kwargs = {"per
-0000f020: 6d69 7373 696f 6e73 223a 2076 616c 2e70  missions": val.p
-0000f030: 6572 6d69 7373 696f 6e73 7d0a 2020 2020  ermissions}.    
-0000f040: 2020 2020 6966 2076 616c 2e63 6f6d 6d65      if val.comme
-0000f050: 6e74 2061 6e64 2063 6865 636b 5f6e 6f74  nt and check_not
-0000f060: 6e61 2876 616c 2e63 6f6d 6d65 6e74 293a  na(val.comment):
-0000f070: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-0000f080: 7267 735b 2263 6f6d 6d65 6e74 225d 203d  rgs["comment"] =
-0000f090: 2076 616c 2e63 6f6d 6d65 6e74 0a20 2020   val.comment.   
-0000f0a0: 2020 2020 2076 616c 7565 5f20 3d20 6574       value_ = et
-0000f0b0: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-0000f0c0: 2020 2020 2020 2020 2022 7b25 737d 7572           "{%s}ur
-0000f0d0: 6922 2025 2078 6d6c 5f6e 616d 6573 7061  i" % xml_namespa
-0000f0e0: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
-0000f0f0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000f100: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
-0000f110: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
-0000f120: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
-0000f130: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000f140: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
-0000f150: 2020 2020 2076 616c 7565 5f2e 7465 7874       value_.text
-0000f160: 203d 2073 7472 2876 616c 2e76 616c 7565   = str(val.value
-0000f170: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
-0000f180: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
-0000f190: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
-0000f1a0: 0a0a 0a64 6566 206d 616b 655f 7265 6769  ...def make_regi
-0000f1b0: 6f6e 2820 2023 206e 6f71 613a 2044 3431  on(  # noqa: D41
-0000f1c0: 3720 2875 6e64 6f63 756d 656e 7465 642d  7 (undocumented-
-0000f1d0: 7061 7261 6d29 0a20 2020 206c 6162 656c  param).    label
-0000f1e0: 3a20 7374 722c 0a20 2020 2069 643a 2073  : str,.    id: s
-0000f1f0: 7472 2c0a 2020 2020 7065 726d 6973 7369  tr,.    permissi
-0000f200: 6f6e 733a 2073 7472 203d 2022 7265 732d  ons: str = "res-
-0000f210: 6465 6661 756c 7422 2c0a 2020 2020 6172  default",.    ar
-0000f220: 6b3a 204f 7074 696f 6e61 6c5b 7374 725d  k: Optional[str]
-0000f230: 203d 204e 6f6e 652c 0a20 2020 2069 7269   = None,.    iri
-0000f240: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-0000f250: 3d20 4e6f 6e65 2c0a 2020 2020 6372 6561  = None,.    crea
-0000f260: 7469 6f6e 5f64 6174 653a 204f 7074 696f  tion_date: Optio
-0000f270: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-0000f280: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-0000f290: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-0000f2a0: 2020 4372 6561 7465 7320 616e 2065 6d70    Creates an emp
-0000f2b0: 7479 2072 6567 696f 6e20 656c 656d 656e  ty region elemen
-0000f2c0: 742c 2077 6974 6820 7468 6520 6174 7472  t, with the attr
-0000f2d0: 6962 7574 6573 2061 7320 7370 6563 6966  ibutes as specif
-0000f2e0: 6965 6420 6279 2074 6865 2061 7267 756d  ied by the argum
-0000f2f0: 656e 7473 0a0a 2020 2020 4172 6773 3a0a  ents..    Args:.
-0000f300: 2020 2020 2020 2020 5468 6520 6172 6775          The argu
-0000f310: 6d65 6e74 7320 636f 7272 6573 706f 6e64  ments correspond
-0000f320: 2031 3a31 2074 6f20 7468 6520 6174 7472   1:1 to the attr
-0000f330: 6962 7574 6573 206f 6620 7468 6520 3c72  ibutes of the <r
-0000f340: 6567 696f 6e3e 2065 6c65 6d65 6e74 2e0a  egion> element..
-0000f350: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
-0000f360: 2020 2020 2057 6172 6e69 6e67 3a20 6966       Warning: if
-0000f370: 2062 6f74 6820 616e 2041 524b 2061 6e64   both an ARK and
-0000f380: 2061 6e20 4952 4920 6172 6520 7072 6f76   an IRI are prov
-0000f390: 6964 6564 0a20 2020 2020 2020 2042 6173  ided.        Bas
-0000f3a0: 6545 7272 6f72 3a20 6966 2074 6865 2063  eError: if the c
-0000f3b0: 7265 6174 696f 6e20 6461 7465 2069 7320  reation date is 
-0000f3c0: 696e 7661 6c69 640a 0a20 2020 2052 6574  invalid..    Ret
-0000f3d0: 7572 6e73 3a0a 2020 2020 2020 2020 5468  urns:.        Th
-0000f3e0: 6520 7265 6769 6f6e 2065 6c65 6d65 6e74  e region element
-0000f3f0: 2c20 7769 7468 6f75 7420 616e 7920 6368  , without any ch
-0000f400: 696c 6472 656e 2c20 6275 7420 7769 7468  ildren, but with
-0000f410: 2074 6865 2061 7474 7269 6275 7465 733a   the attributes:
-0000f420: 0a20 2020 2020 2020 203c 7265 6769 6f6e  .        <region
-0000f430: 206c 6162 656c 3d6c 6162 656c 2069 643d   label=label id=
-0000f440: 6964 2070 6572 6d69 7373 696f 6e73 3d70  id permissions=p
-0000f450: 6572 6d69 7373 696f 6e73 2061 726b 3d61  ermissions ark=a
-0000f460: 726b 2069 7269 3d69 7269 3e3c 2f72 6567  rk iri=iri></reg
-0000f470: 696f 6e3e 0a0a 2020 2020 4578 616d 706c  ion>..    Exampl
-0000f480: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
-0000f490: 7265 6769 6f6e 203d 2065 7863 656c 3278  region = excel2x
-0000f4a0: 6d6c 2e6d 616b 655f 7265 6769 6f6e 2822  ml.make_region("
-0000f4b0: 6c61 6265 6c22 2c20 2269 6422 290a 2020  label", "id").  
-0000f4c0: 2020 2020 2020 3e3e 3e20 7265 6769 6f6e        >>> region
-0000f4d0: 2e61 7070 656e 6428 6578 6365 6c32 786d  .append(excel2xm
-0000f4e0: 6c2e 6d61 6b65 5f74 6578 745f 7072 6f70  l.make_text_prop
-0000f4f0: 2822 6861 7343 6f6d 6d65 6e74 222c 2022  ("hasComment", "
-0000f500: 5468 6973 2069 7320 6120 636f 6d6d 656e  This is a commen
-0000f510: 7422 2929 0a20 2020 2020 2020 203e 3e3e  t")).        >>>
-0000f520: 2072 6567 696f 6e2e 6170 7065 6e64 2865   region.append(e
-0000f530: 7863 656c 3278 6d6c 2e6d 616b 655f 636f  xcel2xml.make_co
-0000f540: 6c6f 725f 7072 6f70 2822 6861 7343 6f6c  lor_prop("hasCol
-0000f550: 6f72 222c 2022 2335 6431 6631 6522 2929  or", "#5d1f1e"))
-0000f560: 0a20 2020 2020 2020 203e 3e3e 2072 6567  .        >>> reg
-0000f570: 696f 6e2e 6170 7065 6e64 2865 7863 656c  ion.append(excel
-0000f580: 3278 6d6c 2e6d 616b 655f 7265 7370 7472  2xml.make_resptr
-0000f590: 5f70 726f 7028 2269 7352 6567 696f 6e4f  _prop("isRegionO
-0000f5a0: 6622 2c20 2269 6d61 6765 5f30 2229 290a  f", "image_0")).
-0000f5b0: 2020 2020 2020 2020 3e3e 3e20 7265 6769          >>> regi
-0000f5c0: 6f6e 2e61 7070 656e 6428 6578 6365 6c32  on.append(excel2
-0000f5d0: 786d 6c2e 6d61 6b65 5f67 656f 6d65 7472  xml.make_geometr
-0000f5e0: 795f 7072 6f70 2822 6861 7347 656f 6d65  y_prop("hasGeome
-0000f5f0: 7472 7922 2c20 227b 2e2e 2e7d 2229 290a  try", "{...}")).
-0000f600: 2020 2020 2020 2020 3e3e 3e20 726f 6f74          >>> root
-0000f610: 2e61 7070 656e 6428 7265 6769 6f6e 290a  .append(region).
-0000f620: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-0000f630: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
-0000f640: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
-0000f650: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
-0000f660: 786d 6c2d 6461 7461 2d66 696c 652f 2372  xml-data-file/#r
-0000f670: 6567 696f 6e0a 2020 2020 2222 220a 0a20  egion.    """.. 
-0000f680: 2020 206b 7761 7267 7320 3d20 7b22 6c61     kwargs = {"la
-0000f690: 6265 6c22 3a20 6c61 6265 6c2c 2022 6964  bel": label, "id
-0000f6a0: 223a 2069 642c 2022 7065 726d 6973 7369  ": id, "permissi
-0000f6b0: 6f6e 7322 3a20 7065 726d 6973 7369 6f6e  ons": permission
-0000f6c0: 732c 2022 6e73 6d61 7022 3a20 786d 6c5f  s, "nsmap": xml_
-0000f6d0: 6e61 6d65 7370 6163 655f 6d61 707d 0a20  namespace_map}. 
-0000f6e0: 2020 2069 6620 6172 6b3a 0a20 2020 2020     if ark:.     
-0000f6f0: 2020 206b 7761 7267 735b 2261 726b 225d     kwargs["ark"]
-0000f700: 203d 2061 726b 0a20 2020 2069 6620 6972   = ark.    if ir
-0000f710: 693a 0a20 2020 2020 2020 206b 7761 7267  i:.        kwarg
-0000f720: 735b 2269 7269 225d 203d 2069 7269 0a20  s["iri"] = iri. 
-0000f730: 2020 2069 6620 6172 6b20 616e 6420 6972     if ark and ir
-0000f740: 693a 0a20 2020 2020 2020 2077 6172 6e69  i:.        warni
-0000f750: 6e67 732e 7761 726e 280a 2020 2020 2020  ngs.warn(.      
-0000f760: 2020 2020 2020 6622 426f 7468 2041 524b        f"Both ARK
-0000f770: 2061 6e64 2049 5249 2077 6572 6520 7072   and IRI were pr
-0000f780: 6f76 6964 6564 2066 6f72 2072 6573 6f75  ovided for resou
-0000f790: 7263 6520 277b 6c61 6265 6c7d 2720 287b  rce '{label}' ({
-0000f7a0: 6964 7d29 2e20 5468 6520 4152 4b20 7769  id}). The ARK wi
-0000f7b0: 6c6c 206f 7665 7272 6964 6520 7468 6520  ll override the 
-0000f7c0: 4952 492e 222c 0a20 2020 2020 2020 2020  IRI.",.         
-0000f7d0: 2020 2073 7461 636b 6c65 7665 6c3d 322c     stacklevel=2,
-0000f7e0: 0a20 2020 2020 2020 2029 0a20 2020 2069  .        ).    i
-0000f7f0: 6620 6372 6561 7469 6f6e 5f64 6174 653a  f creation_date:
-0000f800: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000f810: 2020 2020 2020 2020 2020 4461 7465 5469            DateTi
-0000f820: 6d65 5374 616d 7028 6372 6561 7469 6f6e  meStamp(creation
-0000f830: 5f64 6174 6529 0a20 2020 2020 2020 2065  _date).        e
-0000f840: 7863 6570 7420 4261 7365 4572 726f 723a  xcept BaseError:
-0000f850: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000f860: 7365 2042 6173 6545 7272 6f72 280a 2020  se BaseError(.  
-0000f870: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000f880: 5468 6520 7265 6769 6f6e 2027 7b6c 6162  The region '{lab
-0000f890: 656c 7d27 2028 4944 3a20 7b69 647d 2920  el}' (ID: {id}) 
-0000f8a0: 6861 7320 616e 2069 6e76 616c 6964 2063  has an invalid c
-0000f8b0: 7265 6174 696f 6e20 6461 7465 2027 7b63  reation date '{c
-0000f8c0: 7265 6174 696f 6e5f 6461 7465 7d27 2e20  reation_date}'. 
-0000f8d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000f8e0: 2020 6622 4469 6420 796f 7520 7065 7268    f"Did you perh
-0000f8f0: 6170 7320 666f 7267 6574 2074 6865 2074  aps forget the t
-0000f900: 696d 657a 6f6e 653f 220a 2020 2020 2020  imezone?".      
-0000f910: 2020 2020 2020 2920 6672 6f6d 204e 6f6e        ) from Non
-0000f920: 650a 2020 2020 2020 2020 6b77 6172 6773  e.        kwargs
-0000f930: 5b22 6372 6561 7469 6f6e 5f64 6174 6522  ["creation_date"
-0000f940: 5d20 3d20 6372 6561 7469 6f6e 5f64 6174  ] = creation_dat
-0000f950: 650a 0a20 2020 2072 6574 7572 6e20 6574  e..    return et
-0000f960: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-0000f970: 2020 2020 2022 7b25 737d 7265 6769 6f6e       "{%s}region
-0000f980: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-0000f990: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-0000f9a0: 2020 2020 202a 2a6b 7761 7267 732c 2020       **kwargs,  
-0000f9b0: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
-0000f9c0: 7267 2d74 7970 655d 0a20 2020 2029 0a0a  rg-type].    )..
-0000f9d0: 0a64 6566 206d 616b 655f 616e 6e6f 7461  .def make_annota
-0000f9e0: 7469 6f6e 2820 2023 206e 6f71 613a 2044  tion(  # noqa: D
-0000f9f0: 3431 3720 2875 6e64 6f63 756d 656e 7465  417 (undocumente
-0000fa00: 642d 7061 7261 6d29 0a20 2020 206c 6162  d-param).    lab
-0000fa10: 656c 3a20 7374 722c 0a20 2020 2069 643a  el: str,.    id:
-0000fa20: 2073 7472 2c0a 2020 2020 7065 726d 6973   str,.    permis
-0000fa30: 7369 6f6e 733a 2073 7472 203d 2022 7265  sions: str = "re
-0000fa40: 732d 6465 6661 756c 7422 2c0a 2020 2020  s-default",.    
-0000fa50: 6172 6b3a 204f 7074 696f 6e61 6c5b 7374  ark: Optional[st
-0000fa60: 725d 203d 204e 6f6e 652c 0a20 2020 2069  r] = None,.    i
-0000fa70: 7269 3a20 4f70 7469 6f6e 616c 5b73 7472  ri: Optional[str
-0000fa80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6372  ] = None,.    cr
-0000fa90: 6561 7469 6f6e 5f64 6174 653a 204f 7074  eation_date: Opt
-0000faa0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000fab0: 652c 0a29 202d 3e20 6574 7265 652e 5f45  e,.) -> etree._E
-0000fac0: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
-0000fad0: 2020 2020 4372 6561 7465 7320 616e 2065      Creates an e
-0000fae0: 6d70 7479 2061 6e6e 6f74 6174 696f 6e20  mpty annotation 
-0000faf0: 656c 656d 656e 742c 2077 6974 6820 7468  element, with th
-0000fb00: 6520 6174 7472 6962 7574 6573 2061 7320  e attributes as 
-0000fb10: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
-0000fb20: 2061 7267 756d 656e 7473 0a0a 2020 2020   arguments..    
-0000fb30: 4172 6773 3a0a 2020 2020 2020 2020 5468  Args:.        Th
-0000fb40: 6520 6172 6775 6d65 6e74 7320 636f 7272  e arguments corr
-0000fb50: 6573 706f 6e64 2031 3a31 2074 6f20 7468  espond 1:1 to th
-0000fb60: 6520 6174 7472 6962 7574 6573 206f 6620  e attributes of 
-0000fb70: 7468 6520 3c61 6e6e 6f74 6174 696f 6e3e  the <annotation>
-0000fb80: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2052   element...    R
-0000fb90: 6169 7365 733a 0a20 2020 2020 2020 2057  aises:.        W
-0000fba0: 6172 6e69 6e67 3a20 6966 2062 6f74 6820  arning: if both 
-0000fbb0: 616e 2041 524b 2061 6e64 2061 6e20 4952  an ARK and an IR
-0000fbc0: 4920 6172 6520 7072 6f76 6964 6564 0a20  I are provided. 
-0000fbd0: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
-0000fbe0: 3a20 6966 2074 6865 2063 7265 6174 696f  : if the creatio
-0000fbf0: 6e20 6461 7465 2069 7320 696e 7661 6c69  n date is invali
-0000fc00: 640a 0a20 2020 2052 6574 7572 6e73 3a0a  d..    Returns:.
-0000fc10: 2020 2020 2020 2020 5468 6520 616e 6e6f          The anno
-0000fc20: 7461 7469 6f6e 2065 6c65 6d65 6e74 2c20  tation element, 
-0000fc30: 7769 7468 6f75 7420 616e 7920 6368 696c  without any chil
-0000fc40: 6472 656e 2c20 6275 7420 7769 7468 2074  dren, but with t
-0000fc50: 6865 2061 7474 7269 6275 7465 733a 0a20  he attributes:. 
-0000fc60: 2020 2020 2020 203c 616e 6e6f 7461 7469         <annotati
-0000fc70: 6f6e 206c 6162 656c 3d6c 6162 656c 2069  on label=label i
-0000fc80: 643d 6964 2070 6572 6d69 7373 696f 6e73  d=id permissions
-0000fc90: 3d70 6572 6d69 7373 696f 6e73 2061 726b  =permissions ark
-0000fca0: 3d61 726b 2069 7269 3d69 7269 3e3c 2f61  =ark iri=iri></a
-0000fcb0: 6e6e 6f74 6174 696f 6e3e 0a0a 2020 2020  nnotation>..    
-0000fcc0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-0000fcd0: 2020 3e3e 3e20 616e 6e6f 7461 7469 6f6e    >>> annotation
-0000fce0: 203d 2065 7863 656c 3278 6d6c 2e6d 616b   = excel2xml.mak
-0000fcf0: 655f 616e 6e6f 7461 7469 6f6e 2822 6c61  e_annotation("la
-0000fd00: 6265 6c22 2c20 2269 6422 290a 2020 2020  bel", "id").    
-0000fd10: 2020 2020 3e3e 3e20 616e 6e6f 7461 7469      >>> annotati
-0000fd20: 6f6e 2e61 7070 656e 6428 6578 6365 6c32  on.append(excel2
-0000fd30: 786d 6c2e 6d61 6b65 5f74 6578 745f 7072  xml.make_text_pr
-0000fd40: 6f70 2822 6861 7343 6f6d 6d65 6e74 222c  op("hasComment",
-0000fd50: 2022 5468 6973 2069 7320 6120 636f 6d6d   "This is a comm
-0000fd60: 656e 7422 2929 0a20 2020 2020 2020 203e  ent")).        >
-0000fd70: 3e3e 2061 6e6e 6f74 6174 696f 6e2e 6170  >> annotation.ap
-0000fd80: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
-0000fd90: 616b 655f 7265 7370 7472 5f70 726f 7028  ake_resptr_prop(
-0000fda0: 2269 7341 6e6e 6f74 6174 696f 6e4f 6622  "isAnnotationOf"
-0000fdb0: 2c20 2272 6573 6f75 7263 655f 3022 2929  , "resource_0"))
-0000fdc0: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
-0000fdd0: 742e 6170 7065 6e64 2861 6e6e 6f74 6174  t.append(annotat
-0000fde0: 696f 6e29 0a0a 2020 2020 5365 6520 6874  ion)..    See ht
-0000fdf0: 7470 733a 2f2f 646f 6373 2e64 6173 6368  tps://docs.dasch
-0000fe00: 2e73 7769 7373 2f6c 6174 6573 742f 4453  .swiss/latest/DS
-0000fe10: 502d 544f 4f4c 532f 6669 6c65 2d66 6f72  P-TOOLS/file-for
-0000fe20: 6d61 7473 2f78 6d6c 2d64 6174 612d 6669  mats/xml-data-fi
-0000fe30: 6c65 2f23 616e 6e6f 7461 7469 6f6e 0a20  le/#annotation. 
-0000fe40: 2020 2022 2222 0a0a 2020 2020 6b77 6172     """..    kwar
-0000fe50: 6773 203d 207b 226c 6162 656c 223a 206c  gs = {"label": l
-0000fe60: 6162 656c 2c20 2269 6422 3a20 6964 2c20  abel, "id": id, 
-0000fe70: 2270 6572 6d69 7373 696f 6e73 223a 2070  "permissions": p
-0000fe80: 6572 6d69 7373 696f 6e73 2c20 226e 736d  ermissions, "nsm
-0000fe90: 6170 223a 2078 6d6c 5f6e 616d 6573 7061  ap": xml_namespa
-0000fea0: 6365 5f6d 6170 7d0a 2020 2020 6966 2061  ce_map}.    if a
-0000feb0: 726b 3a0a 2020 2020 2020 2020 6b77 6172  rk:.        kwar
-0000fec0: 6773 5b22 6172 6b22 5d20 3d20 6172 6b0a  gs["ark"] = ark.
-0000fed0: 2020 2020 6966 2069 7269 3a0a 2020 2020      if iri:.    
-0000fee0: 2020 2020 6b77 6172 6773 5b22 6972 6922      kwargs["iri"
-0000fef0: 5d20 3d20 6972 690a 2020 2020 6966 2061  ] = iri.    if a
-0000ff00: 726b 2061 6e64 2069 7269 3a0a 2020 2020  rk and iri:.    
-0000ff10: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-0000ff20: 6e28 0a20 2020 2020 2020 2020 2020 2066  n(.            f
-0000ff30: 2242 6f74 6820 4152 4b20 616e 6420 4952  "Both ARK and IR
-0000ff40: 4920 7765 7265 2070 726f 7669 6465 6420  I were provided 
-0000ff50: 666f 7220 7265 736f 7572 6365 2027 7b6c  for resource '{l
-0000ff60: 6162 656c 7d27 2028 7b69 647d 292e 2054  abel}' ({id}). T
-0000ff70: 6865 2041 524b 2077 696c 6c20 6f76 6572  he ARK will over
-0000ff80: 7269 6465 2074 6865 2049 5249 2e22 2c0a  ride the IRI.",.
-0000ff90: 2020 2020 2020 2020 2020 2020 7374 6163              stac
-0000ffa0: 6b6c 6576 656c 3d32 2c0a 2020 2020 2020  klevel=2,.      
-0000ffb0: 2020 290a 2020 2020 6966 2063 7265 6174    ).    if creat
-0000ffc0: 696f 6e5f 6461 7465 3a0a 2020 2020 2020  ion_date:.      
-0000ffd0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000ffe0: 2020 2044 6174 6554 696d 6553 7461 6d70     DateTimeStamp
-0000fff0: 2863 7265 6174 696f 6e5f 6461 7465 290a  (creation_date).
-00010000: 2020 2020 2020 2020 6578 6365 7074 2042          except B
-00010010: 6173 6545 7272 6f72 3a0a 2020 2020 2020  aseError:.      
-00010020: 2020 2020 2020 7261 6973 6520 4261 7365        raise Base
-00010030: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00010040: 2020 2020 2020 2066 2254 6865 2061 6e6e         f"The ann
-00010050: 6f74 6174 696f 6e20 277b 6c61 6265 6c7d  otation '{label}
-00010060: 2720 2849 443a 207b 6964 7d29 2068 6173  ' (ID: {id}) has
-00010070: 2061 6e20 696e 7661 6c69 6420 6372 6561   an invalid crea
-00010080: 7469 6f6e 2064 6174 6520 277b 6372 6561  tion date '{crea
-00010090: 7469 6f6e 5f64 6174 657d 272e 2022 0a20  tion_date}'. ". 
-000100a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000100b0: 2244 6964 2079 6f75 2070 6572 6861 7073  "Did you perhaps
-000100c0: 2066 6f72 6765 7420 7468 6520 7469 6d65   forget the time
-000100d0: 7a6f 6e65 3f22 0a20 2020 2020 2020 2020  zone?".         
-000100e0: 2020 2029 2066 726f 6d20 4e6f 6e65 0a20     ) from None. 
-000100f0: 2020 2020 2020 206b 7761 7267 735b 2263         kwargs["c
-00010100: 7265 6174 696f 6e5f 6461 7465 225d 203d  reation_date"] =
-00010110: 2063 7265 6174 696f 6e5f 6461 7465 0a0a   creation_date..
-00010120: 2020 2020 7265 7475 726e 2065 7472 6565      return etree
-00010130: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
-00010140: 2020 227b 2573 7d61 6e6e 6f74 6174 696f    "{%s}annotatio
-00010150: 6e22 2025 2078 6d6c 5f6e 616d 6573 7061  n" % xml_namespa
-00010160: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
-00010170: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
-00010180: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
-00010190: 6172 672d 7479 7065 5d0a 2020 2020 290a  arg-type].    ).
-000101a0: 0a0a 6465 6620 6d61 6b65 5f6c 696e 6b28  ..def make_link(
-000101b0: 2020 2320 6e6f 7161 3a20 4434 3137 2028    # noqa: D417 (
-000101c0: 756e 646f 6375 6d65 6e74 6564 2d70 6172  undocumented-par
-000101d0: 616d 290a 2020 2020 6c61 6265 6c3a 2073  am).    label: s
-000101e0: 7472 2c0a 2020 2020 6964 3a20 7374 722c  tr,.    id: str,
-000101f0: 0a20 2020 2070 6572 6d69 7373 696f 6e73  .    permissions
-00010200: 3a20 7374 7220 3d20 2272 6573 2d64 6566  : str = "res-def
-00010210: 6175 6c74 222c 0a20 2020 2061 726b 3a20  ault",.    ark: 
-00010220: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-00010230: 4e6f 6e65 2c0a 2020 2020 6972 693a 204f  None,.    iri: O
-00010240: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00010250: 6f6e 652c 0a20 2020 2063 7265 6174 696f  one,.    creatio
-00010260: 6e5f 6461 7465 3a20 4f70 7469 6f6e 616c  n_date: Optional
-00010270: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2920  [str] = None,.) 
-00010280: 2d3e 2065 7472 6565 2e5f 456c 656d 656e  -> etree._Elemen
-00010290: 743a 0a20 2020 2022 2222 0a20 2020 2043  t:.    """.    C
-000102a0: 7265 6174 6573 2061 6e20 656d 7074 7920  reates an empty 
-000102b0: 6c69 6e6b 2065 6c65 6d65 6e74 2c20 7769  link element, wi
-000102c0: 7468 2074 6865 2061 7474 7269 6275 7465  th the attribute
-000102d0: 7320 6173 2073 7065 6369 6669 6564 2062  s as specified b
-000102e0: 7920 7468 6520 6172 6775 6d65 6e74 730a  y the arguments.
-000102f0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00010300: 2020 2054 6865 2061 7267 756d 656e 7473     The arguments
-00010310: 2063 6f72 7265 7370 6f6e 6420 313a 3120   correspond 1:1 
-00010320: 746f 2074 6865 2061 7474 7269 6275 7465  to the attribute
-00010330: 7320 6f66 2074 6865 203c 6c69 6e6b 3e20  s of the <link> 
-00010340: 656c 656d 656e 742e 0a0a 2020 2020 5261  element...    Ra
-00010350: 6973 6573 3a0a 2020 2020 2020 2020 5761  ises:.        Wa
-00010360: 726e 696e 673a 2069 6620 626f 7468 2061  rning: if both a
-00010370: 6e20 4152 4b20 616e 6420 616e 2049 5249  n ARK and an IRI
-00010380: 2061 7265 2070 726f 7669 6465 640a 2020   are provided.  
-00010390: 2020 2020 2020 4261 7365 4572 726f 723a        BaseError:
-000103a0: 2069 6620 7468 6520 6372 6561 7469 6f6e   if the creation
-000103b0: 2064 6174 6520 6973 2069 6e76 616c 6964   date is invalid
-000103c0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000103d0: 2020 2020 2020 2054 6865 206c 696e 6b20         The link 
-000103e0: 656c 656d 656e 742c 2077 6974 686f 7574  element, without
-000103f0: 2061 6e79 2063 6869 6c64 7265 6e2c 2062   any children, b
-00010400: 7574 2077 6974 6820 7468 6520 6174 7472  ut with the attr
-00010410: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00010420: 3c6c 696e 6b20 6c61 6265 6c3d 6c61 6265  <link label=labe
-00010430: 6c20 6964 3d69 6420 7065 726d 6973 7369  l id=id permissi
-00010440: 6f6e 733d 7065 726d 6973 7369 6f6e 7320  ons=permissions 
-00010450: 6172 6b3d 6172 6b20 6972 693d 6972 693e  ark=ark iri=iri>
-00010460: 3c2f 6c69 6e6b 3e0a 0a20 2020 2045 7861  </link>..    Exa
-00010470: 6d70 6c65 733a 0a20 2020 2020 2020 203e  mples:.        >
-00010480: 3e3e 206c 696e 6b20 3d20 6578 6365 6c32  >> link = excel2
-00010490: 786d 6c2e 6d61 6b65 5f6c 696e 6b28 226c  xml.make_link("l
-000104a0: 6162 656c 222c 2022 6964 2229 0a20 2020  abel", "id").   
-000104b0: 2020 2020 203e 3e3e 206c 696e 6b2e 6170       >>> link.ap
-000104c0: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
-000104d0: 616b 655f 7465 7874 5f70 726f 7028 2268  ake_text_prop("h
-000104e0: 6173 436f 6d6d 656e 7422 2c20 2254 6869  asComment", "Thi
-000104f0: 7320 6973 2061 2063 6f6d 6d65 6e74 2229  s is a comment")
-00010500: 290a 2020 2020 2020 2020 3e3e 3e20 6c69  ).        >>> li
-00010510: 6e6b 2e61 7070 656e 6428 6578 6365 6c32  nk.append(excel2
-00010520: 786d 6c2e 6d61 6b65 5f72 6573 7074 725f  xml.make_resptr_
-00010530: 7072 6f70 2822 6861 734c 696e 6b54 6f22  prop("hasLinkTo"
-00010540: 2c20 5b22 7265 736f 7572 6365 5f30 222c  , ["resource_0",
-00010550: 2022 7265 736f 7572 6365 5f31 225d 2929   "resource_1"]))
-00010560: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
-00010570: 742e 6170 7065 6e64 286c 696e 6b29 0a0a  t.append(link)..
-00010580: 2020 2020 5365 6520 6874 7470 733a 2f2f      See https://
-00010590: 646f 6373 2e64 6173 6368 2e73 7769 7373  docs.dasch.swiss
-000105a0: 2f6c 6174 6573 742f 4453 502d 544f 4f4c  /latest/DSP-TOOL
-000105b0: 532f 6669 6c65 2d66 6f72 6d61 7473 2f78  S/file-formats/x
-000105c0: 6d6c 2d64 6174 612d 6669 6c65 2f23 6c69  ml-data-file/#li
-000105d0: 6e6b 0a20 2020 2022 2222 0a0a 2020 2020  nk.    """..    
-000105e0: 6b77 6172 6773 203d 207b 226c 6162 656c  kwargs = {"label
-000105f0: 223a 206c 6162 656c 2c20 2269 6422 3a20  ": label, "id": 
-00010600: 6964 2c20 2270 6572 6d69 7373 696f 6e73  id, "permissions
-00010610: 223a 2070 6572 6d69 7373 696f 6e73 2c20  ": permissions, 
-00010620: 226e 736d 6170 223a 2078 6d6c 5f6e 616d  "nsmap": xml_nam
-00010630: 6573 7061 6365 5f6d 6170 7d0a 2020 2020  espace_map}.    
-00010640: 6966 2061 726b 3a0a 2020 2020 2020 2020  if ark:.        
-00010650: 6b77 6172 6773 5b22 6172 6b22 5d20 3d20  kwargs["ark"] = 
-00010660: 6172 6b0a 2020 2020 6966 2069 7269 3a0a  ark.    if iri:.
-00010670: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-00010680: 6972 6922 5d20 3d20 6972 690a 2020 2020  iri"] = iri.    
-00010690: 6966 2061 726b 2061 6e64 2069 7269 3a0a  if ark and iri:.
-000106a0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-000106b0: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-000106c0: 2020 2066 2242 6f74 6820 4152 4b20 616e     f"Both ARK an
-000106d0: 6420 4952 4920 7765 7265 2070 726f 7669  d IRI were provi
-000106e0: 6465 6420 666f 7220 7265 736f 7572 6365  ded for resource
-000106f0: 2027 7b6c 6162 656c 7d27 2028 7b69 647d   '{label}' ({id}
-00010700: 292e 2054 6865 2041 524b 2077 696c 6c20  ). The ARK will 
-00010710: 6f76 6572 7269 6465 2074 6865 2049 5249  override the IRI
-00010720: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00010730: 7374 6163 6b6c 6576 656c 3d32 2c0a 2020  stacklevel=2,.  
-00010740: 2020 2020 2020 290a 2020 2020 6966 2063        ).    if c
-00010750: 7265 6174 696f 6e5f 6461 7465 3a0a 2020  reation_date:.  
-00010760: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00010770: 2020 2020 2020 2044 6174 6554 696d 6553         DateTimeS
-00010780: 7461 6d70 2863 7265 6174 696f 6e5f 6461  tamp(creation_da
-00010790: 7465 290a 2020 2020 2020 2020 6578 6365  te).        exce
-000107a0: 7074 2042 6173 6545 7272 6f72 3a0a 2020  pt BaseError:.  
-000107b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000107c0: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
-000107d0: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
-000107e0: 206c 696e 6b20 277b 6c61 6265 6c7d 2720   link '{label}' 
-000107f0: 2849 443a 207b 6964 7d29 2068 6173 2061  (ID: {id}) has a
-00010800: 6e20 696e 7661 6c69 6420 6372 6561 7469  n invalid creati
-00010810: 6f6e 2064 6174 6520 277b 6372 6561 7469  on date '{creati
-00010820: 6f6e 5f64 6174 657d 272e 2022 0a20 2020  on_date}'. ".   
-00010830: 2020 2020 2020 2020 2020 2020 2066 2244               f"D
-00010840: 6964 2079 6f75 2070 6572 6861 7073 2066  id you perhaps f
-00010850: 6f72 6765 7420 7468 6520 7469 6d65 7a6f  orget the timezo
-00010860: 6e65 3f22 0a20 2020 2020 2020 2020 2020  ne?".           
-00010870: 2029 2066 726f 6d20 4e6f 6e65 0a20 2020   ) from None.   
-00010880: 2020 2020 206b 7761 7267 735b 2263 7265       kwargs["cre
-00010890: 6174 696f 6e5f 6461 7465 225d 203d 2063  ation_date"] = c
-000108a0: 7265 6174 696f 6e5f 6461 7465 0a0a 2020  reation_date..  
-000108b0: 2020 7265 7475 726e 2065 7472 6565 2e45    return etree.E
-000108c0: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-000108d0: 227b 2573 7d6c 696e 6b22 2025 2078 6d6c  "{%s}link" % xml
-000108e0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-000108f0: 6f6e 655d 2c0a 2020 2020 2020 2020 2a2a  one],.        **
-00010900: 6b77 6172 6773 2c20 2023 2074 7970 653a  kwargs,  # type:
-00010910: 2069 676e 6f72 655b 6172 672d 7479 7065   ignore[arg-type
-00010920: 5d0a 2020 2020 290a 0a0a 6465 6620 6372  ].    )...def cr
-00010930: 6561 7465 5f6a 736f 6e5f 6578 6365 6c5f  eate_json_excel_
-00010940: 6c69 7374 5f6d 6170 7069 6e67 280a 2020  list_mapping(.  
-00010950: 2020 7061 7468 5f74 6f5f 6a73 6f6e 3a20    path_to_json: 
-00010960: 7374 722c 0a20 2020 206c 6973 745f 6e61  str,.    list_na
-00010970: 6d65 3a20 7374 722c 0a20 2020 2065 7863  me: str,.    exc
-00010980: 656c 5f76 616c 7565 733a 2049 7465 7261  el_values: Itera
-00010990: 626c 655b 7374 725d 2c0a 2020 2020 7365  ble[str],.    se
-000109a0: 703a 2073 7472 203d 2027 2b22 2ac3 a725  p: str = '+"*..%
-000109b0: 262f 2829 3d27 2c0a 2020 2020 636f 7272  &/()=',.    corr
-000109c0: 6563 7469 6f6e 733a 204f 7074 696f 6e61  ections: Optiona
-000109d0: 6c5b 6469 6374 5b73 7472 2c20 7374 725d  l[dict[str, str]
-000109e0: 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e 2064  ] = None,.) -> d
-000109f0: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
-00010a00: 2020 2022 2222 0a20 2020 204f 6674 656e     """.    Often
-00010a10: 2c20 6461 7461 2073 6f75 7263 6573 2063  , data sources c
-00010a20: 6f6e 7461 696e 206c 6973 7420 7661 6c75  ontain list valu
-00010a30: 6573 2074 6861 7420 6172 656e 2774 2069  es that aren't i
-00010a40: 6465 6e74 6963 616c 2074 6f20 7468 6520  dentical to the 
-00010a50: 6e61 6d65 206f 6620 7468 6520 6e6f 6465  name of the node
-00010a60: 2069 6e20 7468 6520 6c69 7374 206f 6620   in the list of 
-00010a70: 7468 6520 4a53 4f4e 0a20 2020 2070 726f  the JSON.    pro
-00010a80: 6a65 6374 2066 696c 6520 2863 6f6c 6c6f  ject file (collo
-00010a90: 7175 6961 6c6c 793a 206f 6e74 6f6c 6f67  quially: ontolog
-00010aa0: 7929 2e20 496e 206f 7264 6572 2074 6f20  y). In order to 
-00010ab0: 6372 6561 7465 2061 2063 6f72 7265 6374  create a correct
-00010ac0: 2058 4d4c 2066 6f72 2074 6865 2060 6473   XML for the `ds
-00010ad0: 702d 746f 6f6c 7320 786d 6c75 706c 6f61  p-tools xmluploa
-00010ae0: 6460 2c20 6120 6d61 7070 696e 6720 6973  d`, a mapping is
-00010af0: 0a20 2020 206e 6563 6573 7361 7279 2e20  .    necessary. 
-00010b00: 5468 6973 2066 756e 6374 696f 6e20 7461  This function ta
-00010b10: 6b65 7320 6120 4a53 4f4e 206c 6973 7420  kes a JSON list 
-00010b20: 616e 6420 616e 2045 7863 656c 2063 6f6c  and an Excel col
-00010b30: 756d 6e20 636f 6e74 6169 6e69 6e67 206c  umn containing l
-00010b40: 6973 742d 7661 6c75 6573 2c20 616e 6420  ist-values, and 
-00010b50: 7472 6965 7320 746f 206d 6174 6368 2074  tries to match t
-00010b60: 6865 6d0a 2020 2020 6175 746f 6d61 7469  hem.    automati
-00010b70: 6361 6c6c 7920 6261 7365 6420 6f6e 2073  cally based on s
-00010b80: 696d 696c 6172 6974 792e 2054 6865 2072  imilarity. The r
-00010b90: 6573 756c 7420 6973 2061 2064 6963 7420  esult is a dict 
-00010ba0: 6f66 2074 6865 2066 6f72 6d20 7b65 7863  of the form {exc
-00010bb0: 656c 5f76 616c 7565 3a20 6c69 7374 5f6e  el_value: list_n
-00010bc0: 6f64 655f 6e61 6d65 7d2e 0a0a 2020 2020  ode_name}...    
-00010bd0: 416c 7465 726e 6174 6976 656c 792c 2063  Alternatively, c
-00010be0: 6f6e 7369 6465 7220 7573 696e 6720 7468  onsider using th
-00010bf0: 6520 6675 6e63 7469 6f6e 2063 7265 6174  e function creat
-00010c00: 655f 6a73 6f6e 5f6c 6973 745f 6d61 7070  e_json_list_mapp
-00010c10: 696e 6728 292c 2077 6869 6368 2061 6c73  ing(), which als
-00010c20: 6f20 6275 696c 6473 2061 2064 6963 7469  o builds a dicti
-00010c30: 6f6e 6172 792c 0a20 2020 2062 7574 2066  onary,.    but f
-00010c40: 726f 6d20 7468 6520 6e61 6d65 7320 616e  rom the names an
-00010c50: 6420 6c61 6265 6c73 2069 6e20 7468 6520  d labels in the 
-00010c60: 4a53 4f4e 206c 6973 742c 2077 6869 6368  JSON list, which
-00010c70: 2069 7320 6c65 7373 2065 7272 6f72 2d70   is less error-p
-00010c80: 726f 6e65 2074 6861 6e20 7468 6973 2066  rone than this f
-00010c90: 756e 6374 696f 6e27 7320 6170 7072 6f61  unction's approa
-00010ca0: 6368 2e20 486f 7765 7665 722c 0a20 2020  ch. However,.   
-00010cb0: 2074 6869 7320 6675 6e63 7469 6f6e 2068   this function h
-00010cc0: 6173 2074 6865 2061 6476 616e 7461 6765  as the advantage
-00010cd0: 2074 6861 7420 6974 2065 7665 6e20 776f   that it even wo
-00010ce0: 726b 7320 7768 656e 2079 6f75 7220 6461  rks when your da
-00010cf0: 7461 2073 6f75 7263 6520 646f 6573 6e27  ta source doesn'
-00010d00: 7420 7573 6520 7468 6520 6c69 7374 206c  t use the list l
-00010d10: 6162 656c 7320 636f 7272 6563 746c 792e  abels correctly.
-00010d20: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00010d30: 2020 2020 7061 7468 5f74 6f5f 6a73 6f6e      path_to_json
-00010d40: 3a20 7061 7468 2074 6f20 7468 6520 4a53  : path to the JS
-00010d50: 4f4e 2070 726f 6a65 6374 2066 696c 650a  ON project file.
-00010d60: 2020 2020 2020 2020 6c69 7374 5f6e 616d          list_nam
-00010d70: 653a 206e 616d 6520 6f66 2074 6865 206c  e: name of the l
-00010d80: 6973 7420 696e 2074 6865 204a 534f 4e20  ist in the JSON 
-00010d90: 7072 6f6a 6563 7420 6669 6c65 2028 6361  project file (ca
-00010da0: 6e20 616c 736f 2062 6520 6120 6e65 7374  n also be a nest
-00010db0: 6564 206c 6973 7429 0a20 2020 2020 2020  ed list).       
-00010dc0: 2065 7863 656c 5f76 616c 7565 733a 2074   excel_values: t
-00010dd0: 6865 2045 7863 656c 2063 6f6c 756d 6e20  he Excel column 
-00010de0: 2865 2e67 2e20 6173 206c 6973 7429 2077  (e.g. as list) w
-00010df0: 6974 6820 7468 6520 6c69 7374 2076 616c  ith the list val
-00010e00: 7565 7320 696e 2069 740a 2020 2020 2020  ues in it.      
-00010e10: 2020 7365 703a 2073 6570 6172 6174 6f72    sep: separator
-00010e20: 2073 7472 696e 672c 2069 6620 7468 6520   string, if the 
-00010e30: 6365 6c6c 7320 696e 2074 6865 2045 7863  cells in the Exc
-00010e40: 656c 2063 6f6e 7461 696e 206d 6f72 6520  el contain more 
-00010e50: 7468 616e 206f 6e65 206c 6973 7420 656e  than one list en
-00010e60: 7472 790a 2020 2020 2020 2020 636f 7272  try.        corr
-00010e70: 6563 7469 6f6e 733a 2064 6963 7420 7769  ections: dict wi
-00010e80: 7468 2077 726f 6e67 2065 6e74 7269 6573  th wrong entries
-00010e90: 2c20 6561 6368 2070 6f69 6e74 696e 6720  , each pointing 
-00010ea0: 746f 2069 7473 2063 6f72 7265 6374 2063  to its correct c
-00010eb0: 6f75 6e74 6572 7061 7274 0a0a 2020 2020  ounterpart..    
-00010ec0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-00010ed0: 5761 726e 696e 673a 2069 6620 7468 6572  Warning: if ther
-00010ee0: 6520 6973 2061 6e20 4578 6365 6c20 7661  e is an Excel va
-00010ef0: 6c75 6520 7468 6174 2063 6f75 6c64 6e27  lue that couldn'
-00010f00: 7420 6265 206d 6174 6368 6564 0a20 2020  t be matched.   
-00010f10: 2020 2020 2045 7863 6570 7469 6f6e 3a20       Exception: 
-00010f20: 6966 2074 6865 2070 6174 6820 646f 6573  if the path does
-00010f30: 6e27 7420 706f 696e 7420 746f 2061 204a  n't point to a J
-00010f40: 534f 4e20 7072 6f6a 6563 7420 6669 6c65  SON project file
-00010f50: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00010f60: 2020 2020 2020 2064 6963 7420 6f66 2074         dict of t
-00010f70: 6865 2066 6f72 6d20 6060 7b65 7863 656c  he form ``{excel
-00010f80: 5f76 616c 7565 3a20 6c69 7374 5f6e 6f64  _value: list_nod
-00010f90: 655f 6e61 6d65 7d60 602e 0a20 2020 2020  e_name}``..     
-00010fa0: 2020 2020 2020 2045 7665 7279 2065 7863         Every exc
-00010fb0: 656c 5f76 616c 7565 2069 7320 7374 7269  el_value is stri
-00010fc0: 7070 6564 2c20 616e 6420 616c 736f 2070  pped, and also p
-00010fd0: 7265 7365 6e74 2069 6e20 6120 6c6f 7765  resent in a lowe
-00010fe0: 7263 6173 6520 666f 726d 2e0a 0a20 2020  rcase form...   
-00010ff0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-00011000: 2020 203e 3e3e 206a 736f 6e5f 6c69 7374     >>> json_list
-00011010: 5f6e 6f64 6573 203d 205b 0a20 2020 2020  _nodes = [.     
-00011020: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00011030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011040: 2022 6e61 6d65 223a 2022 6769 7261 6666   "name": "giraff
-00011050: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00011060: 2020 2020 2020 2020 226c 6162 656c 7322          "labels"
-00011070: 3a20 7b22 656e 223a 2022 6769 7261 6666  : {"en": "giraff
-00011080: 6522 7d0a 2020 2020 2020 2020 2020 2020  e"}.            
-00011090: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000110a0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000110b0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
-000110c0: 6d65 223a 2022 616e 7465 6c6f 7065 222c  me": "antelope",
-000110d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000110e0: 2020 2020 2022 6c61 6265 6c73 223a 207b       "labels": {
-000110f0: 2265 6e22 3a20 2261 6e74 656c 6f70 6522  "en": "antelope"
-00011100: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00011110: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00011120: 5d0a 2020 2020 2020 2020 3e3e 3e20 6578  ].        >>> ex
-00011130: 6365 6c5f 726f 775f 3120 3d20 5b22 4769  cel_row_1 = ["Gi
-00011140: 7261 6666 6565 6820 222c 2022 2041 6e74  raffeeh ", " Ant
-00011150: 696c 6f75 7065 222c 2022 4769 7272 6166  iloupe", "Girraf
-00011160: 6665 202c 2041 6e74 696c 6f75 7065 2022  fe , Antiloupe "
-00011170: 5d0a 2020 2020 2020 2020 3e3e 3e20 6a73  ].        >>> js
-00011180: 6f6e 5f65 7863 656c 5f6c 6973 745f 6d61  on_excel_list_ma
-00011190: 7070 696e 6720 3d20 7b0a 2020 2020 2020  pping = {.      
-000111a0: 2020 2020 2020 2020 2020 2247 6972 6166            "Giraf
-000111b0: 6665 6568 223a 2022 6769 7261 6666 6522  feeh": "giraffe"
-000111c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000111d0: 2020 2267 6972 6166 6665 6568 223a 2022    "giraffeeh": "
-000111e0: 6769 7261 6666 6522 2c0a 2020 2020 2020  giraffe",.      
-000111f0: 2020 2020 2020 2020 2020 2247 6972 7261            "Girra
-00011200: 6666 6522 3a20 2267 6972 6166 6665 222c  ffe": "giraffe",
-00011210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011220: 2022 6769 7272 6166 6665 223a 2022 6769   "girraffe": "gi
-00011230: 7261 6666 6522 2c0a 2020 2020 2020 2020  raffe",.        
-00011240: 2020 2020 2020 2020 2241 6e74 696c 6f75          "Antilou
-00011250: 7065 223a 2022 616e 7465 6c6f 7065 222c  pe": "antelope",
-00011260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011270: 2022 616e 7469 6c6f 7570 6522 3a20 2261   "antiloupe": "a
-00011280: 6e74 656c 6f70 6522 0a20 2020 2020 2020  ntelope".       
-00011290: 2020 2020 207d 0a20 2020 2022 2222 0a0a       }.    """..
-000112a0: 2020 2020 2320 6176 6f69 6420 6d75 7461      # avoid muta
-000112b0: 626c 6520 6465 6661 756c 7420 6172 6775  ble default argu
-000112c0: 6d65 6e74 0a20 2020 2063 6f72 7265 6374  ment.    correct
-000112d0: 696f 6e73 203d 2063 6f72 7265 6374 696f  ions = correctio
-000112e0: 6e73 206f 7220 7b7d 0a0a 2020 2020 2320  ns or {}..    # 
-000112f0: 7370 6c69 7420 7468 6520 7661 6c75 6573  split the values
-00011300: 2c20 6966 206e 6563 6573 7361 7279 0a20  , if necessary. 
-00011310: 2020 2065 7863 656c 5f76 616c 7565 735f     excel_values_
-00011320: 6e65 7720 3d20 5b5d 0a20 2020 2066 6f72  new = [].    for
-00011330: 2076 616c 2069 6e20 6578 6365 6c5f 7661   val in excel_va
-00011340: 6c75 6573 3a0a 2020 2020 2020 2020 6966  lues:.        if
-00011350: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
-00011360: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00011370: 2020 2065 7863 656c 5f76 616c 7565 735f     excel_values_
-00011380: 6e65 772e 6578 7465 6e64 285b 782e 7374  new.extend([x.st
-00011390: 7269 7028 2920 666f 7220 7820 696e 2076  rip() for x in v
-000113a0: 616c 2e73 706c 6974 2873 6570 2920 6966  al.split(sep) if
-000113b0: 2078 5d29 0a0a 2020 2020 2320 7265 6164   x])..    # read
-000113c0: 2074 6865 206c 6973 7420 6f66 2074 6865   the list of the
-000113d0: 204a 534f 4e20 7072 6f6a 6563 7420 2877   JSON project (w
-000113e0: 6f72 6b73 2061 6c73 6f20 666f 7220 6e65  orks also for ne
-000113f0: 7374 6564 206c 6973 7473 290a 2020 2020  sted lists).    
-00011400: 7769 7468 206f 7065 6e28 7061 7468 5f74  with open(path_t
-00011410: 6f5f 6a73 6f6e 2c20 656e 636f 6469 6e67  o_json, encoding
-00011420: 3d22 7574 662d 3822 2920 6173 2066 3a0a  ="utf-8") as f:.
-00011430: 2020 2020 2020 2020 6a73 6f6e 5f66 696c          json_fil
-00011440: 6520 3d20 6a73 6f6e 2e6c 6f61 6428 6629  e = json.load(f)
-00011450: 0a20 2020 206a 736f 6e5f 7375 6273 6574  .    json_subset
-00011460: 203d 205b 5d0a 2020 2020 666f 7220 656c   = [].    for el
-00011470: 656d 2069 6e20 6a73 6f6e 5f66 696c 655b  em in json_file[
-00011480: 2270 726f 6a65 6374 225d 5b22 6c69 7374  "project"]["list
-00011490: 7322 5d3a 0a20 2020 2020 2020 2069 6620  s"]:.        if 
-000114a0: 656c 656d 5b22 6e61 6d65 225d 203d 3d20  elem["name"] == 
-000114b0: 6c69 7374 5f6e 616d 653a 0a20 2020 2020  list_name:.     
-000114c0: 2020 2020 2020 206a 736f 6e5f 7375 6273         json_subs
-000114d0: 6574 203d 2065 6c65 6d5b 226e 6f64 6573  et = elem["nodes
-000114e0: 225d 0a20 2020 206a 736f 6e5f 7661 6c75  "].    json_valu
-000114f0: 6573 203d 2073 6574 285f 6e65 7374 6564  es = set(_nested
-00011500: 5f64 6963 745f 7661 6c75 6573 5f69 7465  _dict_values_ite
-00011510: 7261 746f 7228 6a73 6f6e 5f73 7562 7365  rator(json_subse
-00011520: 7429 290a 0a20 2020 2023 2062 7569 6c64  t))..    # build
-00011530: 2064 6963 7469 6f6e 6172 7920 7769 7468   dictionary with
-00011540: 2074 6865 206d 6170 7069 6e67 2c20 6261   the mapping, ba
-00011550: 7365 6420 6f6e 2073 7472 696e 6720 7369  sed on string si
-00011560: 6d69 6c61 7269 7479 0a20 2020 2072 6573  milarity.    res
-00011570: 203d 207b 7d0a 2020 2020 666f 7220 6578   = {}.    for ex
-00011580: 6365 6c5f 7661 6c75 6520 696e 2065 7863  cel_value in exc
-00011590: 656c 5f76 616c 7565 735f 6e65 773a 0a20  el_values_new:. 
-000115a0: 2020 2020 2020 2065 7863 656c 5f76 616c         excel_val
-000115b0: 7565 5f63 6f72 7265 6374 6564 203d 2063  ue_corrected = c
-000115c0: 6f72 7265 6374 696f 6e73 2e67 6574 2865  orrections.get(e
-000115d0: 7863 656c 5f76 616c 7565 2c20 6578 6365  xcel_value, exce
-000115e0: 6c5f 7661 6c75 6529 0a20 2020 2020 2020  l_value).       
-000115f0: 2065 7863 656c 5f76 616c 7565 5f73 696d   excel_value_sim
-00011600: 706c 203d 2073 696d 706c 6966 795f 6e61  pl = simplify_na
-00011610: 6d65 2865 7863 656c 5f76 616c 7565 5f63  me(excel_value_c
-00011620: 6f72 7265 6374 6564 2920 2023 2069 6e63  orrected)  # inc
-00011630: 7265 6173 6520 6d61 7463 6820 7072 6f62  rease match prob
-00011640: 6162 696c 6974 7920 6279 2072 656d 6f76  ability by remov
-00011650: 696e 6720 696c 6c65 6761 6c20 6368 6172  ing illegal char
-00011660: 730a 2020 2020 2020 2020 6966 206d 6174  s.        if mat
-00011670: 6368 6573 203a 3d20 6469 6666 6c69 622e  ches := difflib.
-00011680: 6765 745f 636c 6f73 655f 6d61 7463 6865  get_close_matche
-00011690: 7328 0a20 2020 2020 2020 2020 2020 2077  s(.            w
-000116a0: 6f72 643d 6578 6365 6c5f 7661 6c75 655f  ord=excel_value_
-000116b0: 7369 6d70 6c2c 0a20 2020 2020 2020 2020  simpl,.         
-000116c0: 2020 2070 6f73 7369 6269 6c69 7469 6573     possibilities
-000116d0: 3d6a 736f 6e5f 7661 6c75 6573 2c0a 2020  =json_values,.  
-000116e0: 2020 2020 2020 2020 2020 6e3d 312c 0a20            n=1,. 
-000116f0: 2020 2020 2020 2020 2020 2063 7574 6f66             cutof
-00011700: 663d 302e 362c 0a20 2020 2020 2020 2029  f=0.6,.        )
-00011710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00011720: 735b 6578 6365 6c5f 7661 6c75 655d 203d  s[excel_value] =
-00011730: 206d 6174 6368 6573 5b30 5d0a 2020 2020   matches[0].    
-00011740: 2020 2020 2020 2020 7265 735b 6578 6365          res[exce
-00011750: 6c5f 7661 6c75 652e 6c6f 7765 7228 295d  l_value.lower()]
-00011760: 203d 206d 6174 6368 6573 5b30 5d0a 2020   = matches[0].  
-00011770: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00011780: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00011790: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
-000117a0: 2020 2020 2020 2066 2244 6964 206e 6f74         f"Did not
-000117b0: 2066 696e 6420 6120 636c 6f73 6520 6d61   find a close ma
-000117c0: 7463 6820 746f 2074 6865 2065 7863 656c  tch to the excel
-000117d0: 206c 6973 7420 656e 7472 7920 277b 6578   list entry '{ex
-000117e0: 6365 6c5f 7661 6c75 657d 2720 220a 2020  cel_value}' ".  
-000117f0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00011800: 616d 6f6e 6720 7468 6520 7661 6c75 6573  among the values
-00011810: 2069 6e20 7468 6520 4a53 4f4e 2070 726f   in the JSON pro
-00011820: 6a65 6374 206c 6973 7420 277b 6c69 7374  ject list '{list
-00011830: 5f6e 616d 657d 2722 2c0a 2020 2020 2020  _name}'",.      
-00011840: 2020 2020 2020 2020 2020 7374 6163 6b6c            stackl
-00011850: 6576 656c 3d32 2c0a 2020 2020 2020 2020  evel=2,.        
-00011860: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-00011870: 6e20 7265 730a 0a0a 6465 6620 5f6e 6573  n res...def _nes
-00011880: 7465 645f 6469 6374 5f76 616c 7565 735f  ted_dict_values_
-00011890: 6974 6572 6174 6f72 2864 6963 7473 3a20  iterator(dicts: 
-000118a0: 6c69 7374 5b64 6963 745b 7374 722c 2041  list[dict[str, A
-000118b0: 6e79 5d5d 2920 2d3e 2049 7465 7261 626c  ny]]) -> Iterabl
-000118c0: 655b 7374 725d 3a0a 2020 2020 2222 220a  e[str]:.    """.
-000118d0: 2020 2020 5969 656c 6420 616c 6c20 7661      Yield all va
-000118e0: 6c75 6573 206f 6620 6120 6e65 7374 6564  lues of a nested
-000118f0: 2064 6963 7469 6f6e 6172 792e 0a0a 2020   dictionary...  
-00011900: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00011910: 6469 6374 733a 206c 6973 7420 6f66 206e  dicts: list of n
-00011920: 6573 7465 6420 6469 6374 696f 6e61 7269  ested dictionari
-00011930: 6573 0a0a 2020 2020 5969 656c 6473 3a0a  es..    Yields:.
-00011940: 2020 2020 2020 2020 7661 6c75 6573 206f          values o
-00011950: 6620 7468 6520 6e65 7374 6564 2064 6963  f the nested dic
-00011960: 7469 6f6e 6172 6965 730a 2020 2020 2222  tionaries.    ""
-00011970: 220a 2020 2020 2320 4372 6564 6974 733a  ".    # Credits:
-00011980: 2068 7474 7073 3a2f 2f74 6869 7370 6f69   https://thispoi
-00011990: 6e74 6572 2e63 6f6d 2f70 7974 686f 6e2d  nter.com/python-
-000119a0: 6974 6572 6174 652d 6c6f 6f70 2d6f 7665  iterate-loop-ove
-000119b0: 722d 616c 6c2d 6e65 7374 6564 2d64 6963  r-all-nested-dic
-000119c0: 7469 6f6e 6172 792d 7661 6c75 6573 2f0a  tionary-values/.
-000119d0: 2020 2020 666f 7220 5f64 6963 7420 696e      for _dict in
-000119e0: 2064 6963 7473 3a0a 2020 2020 2020 2020   dicts:.        
-000119f0: 6966 2022 6e6f 6465 7322 2069 6e20 5f64  if "nodes" in _d
-00011a00: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
-00011a10: 2079 6965 6c64 2066 726f 6d20 5f6e 6573   yield from _nes
-00011a20: 7465 645f 6469 6374 5f76 616c 7565 735f  ted_dict_values_
-00011a30: 6974 6572 6174 6f72 285f 6469 6374 5b22  iterator(_dict["
-00011a40: 6e6f 6465 7322 5d29 0a20 2020 2020 2020  nodes"]).       
-00011a50: 2069 6620 226e 616d 6522 2069 6e20 5f64   if "name" in _d
-00011a60: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
-00011a70: 2079 6965 6c64 205f 6469 6374 5b22 6e61   yield _dict["na
-00011a80: 6d65 225d 0a0a 0a64 6566 2063 7265 6174  me"]...def creat
-00011a90: 655f 6a73 6f6e 5f6c 6973 745f 6d61 7070  e_json_list_mapp
-00011aa0: 696e 6728 0a20 2020 2070 6174 685f 746f  ing(.    path_to
-00011ab0: 5f6a 736f 6e3a 2073 7472 2c0a 2020 2020  _json: str,.    
-00011ac0: 6c69 7374 5f6e 616d 653a 2073 7472 2c0a  list_name: str,.
-00011ad0: 2020 2020 6c61 6e67 7561 6765 5f6c 6162      language_lab
-00011ae0: 656c 3a20 7374 722c 0a29 202d 3e20 6469  el: str,.) -> di
-00011af0: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
-00011b00: 2020 2222 220a 2020 2020 4f66 7465 6e2c    """.    Often,
-00011b10: 2064 6174 6120 736f 7572 6365 7320 636f   data sources co
-00011b20: 6e74 6169 6e20 6c69 7374 2076 616c 7565  ntain list value
-00011b30: 7320 6e61 6d65 6420 6166 7465 7220 7468  s named after th
-00011b40: 6520 226c 6162 656c 2220 6f66 2074 6865  e "label" of the
-00011b50: 204a 534f 4e20 7072 6f6a 6563 7420 6c69   JSON project li
-00011b60: 7374 206e 6f64 652c 2069 6e73 7465 6164  st node, instead
-00011b70: 206f 6620 7468 6520 226e 616d 6522 0a20   of the "name". 
-00011b80: 2020 2077 6869 6368 2069 7320 6e65 6564     which is need
-00011b90: 6564 2066 6f72 2074 6865 2060 6473 702d  ed for the `dsp-
-00011ba0: 746f 6f6c 7320 786d 6c75 706c 6f61 6460  tools xmlupload`
-00011bb0: 2e20 496e 206f 7264 6572 2074 6f20 6372  . In order to cr
-00011bc0: 6561 7465 2061 2063 6f72 7265 6374 2058  eate a correct X
-00011bd0: 4d4c 2c20 796f 7520 6e65 6564 2061 2064  ML, you need a d
-00011be0: 6963 7469 6f6e 6172 7920 7468 6174 206d  ictionary that m
-00011bf0: 6170 7320 7468 650a 2020 2020 226c 6162  aps the.    "lab
-00011c00: 656c 7322 2074 6f20 7468 6569 7220 636f  els" to their co
-00011c10: 7272 6563 7420 226e 616d 6573 222e 0a0a  rrect "names"...
-00011c20: 2020 2020 416c 7465 726e 6174 6976 656c      Alternativel
-00011c30: 792c 2063 6f6e 7369 6465 7220 7573 696e  y, consider usin
-00011c40: 6720 7468 6520 6d65 7468 6f64 2063 7265  g the method cre
-00011c50: 6174 655f 6a73 6f6e 5f65 7863 656c 5f6c  ate_json_excel_l
-00011c60: 6973 745f 6d61 7070 696e 6728 292c 2077  ist_mapping(), w
-00011c70: 6869 6368 2061 6c73 6f20 6372 6561 7465  hich also create
-00011c80: 7320 6120 6469 6374 696f 6e61 7279 2c20  s a dictionary, 
-00011c90: 6275 7420 6d61 7073 0a20 2020 2076 616c  but maps.    val
-00011ca0: 7565 7320 6672 6f6d 2079 6f75 7220 6461  ues from your da
-00011cb0: 7461 2073 6f75 7263 6520 746f 206c 6973  ta source to lis
-00011cc0: 7420 6e6f 6465 206e 616d 6573 2066 726f  t node names fro
-00011cd0: 6d20 7468 6520 4a53 4f4e 2070 726f 6a65  m the JSON proje
-00011ce0: 6374 2066 696c 652c 2062 6173 6564 206f  ct file, based o
-00011cf0: 6e20 7369 6d69 6c61 7269 7479 2e0a 0a20  n similarity... 
-00011d00: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00011d10: 2070 6174 685f 746f 5f6a 736f 6e3a 2070   path_to_json: p
-00011d20: 6174 6820 746f 2061 204a 534f 4e20 7072  ath to a JSON pr
-00011d30: 6f6a 6563 7420 6669 6c65 2028 612e 6b2e  oject file (a.k.
-00011d40: 612e 206f 6e74 6f6c 6f67 7929 0a20 2020  a. ontology).   
-00011d50: 2020 2020 206c 6973 745f 6e61 6d65 3a20       list_name: 
-00011d60: 6e61 6d65 206f 6620 6120 6c69 7374 2069  name of a list i
-00011d70: 6e20 7468 6520 4a53 4f4e 2070 726f 6a65  n the JSON proje
-00011d80: 6374 2028 776f 726b 7320 616c 736f 2066  ct (works also f
-00011d90: 6f72 206e 6573 7465 6420 6c69 7374 7329  or nested lists)
-00011da0: 0a20 2020 2020 2020 206c 616e 6775 6167  .        languag
-00011db0: 655f 6c61 6265 6c3a 2077 6869 6368 206c  e_label: which l
-00011dc0: 616e 6775 6167 6520 6f66 2074 6865 206c  anguage of the l
-00011dd0: 6162 656c 2074 6f20 6368 6f6f 7365 0a0a  abel to choose..
-00011de0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00011df0: 2020 2020 2061 2064 6963 7469 6f6e 6172       a dictionar
-00011e00: 7920 6f66 2074 6865 2066 6f72 6d20 7b6c  y of the form {l
-00011e10: 6162 656c 3a20 6e61 6d65 7d0a 2020 2020  abel: name}.    
-00011e20: 2222 220a 2020 2020 7769 7468 206f 7065  """.    with ope
-00011e30: 6e28 7061 7468 5f74 6f5f 6a73 6f6e 2c20  n(path_to_json, 
-00011e40: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00011e50: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00011e60: 6a73 6f6e 5f66 696c 6520 3d20 6a73 6f6e  json_file = json
-00011e70: 2e6c 6f61 6428 6629 0a20 2020 206a 736f  .load(f).    jso
-00011e80: 6e5f 7375 6273 6574 203d 205b 7820 666f  n_subset = [x fo
-00011e90: 7220 7820 696e 206a 736f 6e5f 6669 6c65  r x in json_file
-00011ea0: 5b22 7072 6f6a 6563 7422 5d5b 226c 6973  ["project"]["lis
-00011eb0: 7473 225d 2069 6620 785b 226e 616d 6522  ts"] if x["name"
-00011ec0: 5d20 3d3d 206c 6973 745f 6e61 6d65 5d0a  ] == list_name].
-00011ed0: 2020 2020 2320 6a73 6f6e 5f73 7562 7365      # json_subse
-00011ee0: 7420 6973 2061 206c 6973 7420 636f 6e74  t is a list cont
-00011ef0: 6169 6e69 6e67 206f 6e65 2069 7465 6d2c  aining one item,
-00011f00: 206e 616d 656c 7920 7468 6520 6a73 6f6e   namely the json
-00011f10: 206f 626a 6563 7420 636f 6e74 6169 6e69   object containi
-00011f20: 6e67 2074 6865 2065 6e74 6972 6520 6a73  ng the entire js
-00011f30: 6f6e 2d6c 6973 740a 0a20 2020 2072 6573  on-list..    res
-00011f40: 203d 207b 7d0a 2020 2020 666f 7220 6c61   = {}.    for la
-00011f50: 6265 6c2c 206e 616d 6520 696e 205f 6e61  bel, name in _na
-00011f60: 6d65 5f6c 6162 656c 5f6d 6170 7065 725f  me_label_mapper_
-00011f70: 6974 6572 6174 6f72 286a 736f 6e5f 7375  iterator(json_su
-00011f80: 6273 6574 2c20 6c61 6e67 7561 6765 5f6c  bset, language_l
-00011f90: 6162 656c 293a 0a20 2020 2020 2020 2069  abel):.        i
-00011fa0: 6620 6e61 6d65 2021 3d20 6c69 7374 5f6e  f name != list_n
-00011fb0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-00011fc0: 2072 6573 5b6c 6162 656c 5d20 3d20 6e61   res[label] = na
-00011fd0: 6d65 0a20 2020 2020 2020 2020 2020 2072  me.            r
-00011fe0: 6573 5b6c 6162 656c 2e73 7472 6970 2829  es[label.strip()
-00011ff0: 2e6c 6f77 6572 2829 5d20 3d20 6e61 6d65  .lower()] = name
-00012000: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-00012010: 0a0a 0a64 6566 205f 6e61 6d65 5f6c 6162  ...def _name_lab
-00012020: 656c 5f6d 6170 7065 725f 6974 6572 6174  el_mapper_iterat
-00012030: 6f72 280a 2020 2020 6a73 6f6e 5f73 7562  or(.    json_sub
-00012040: 7365 743a 206c 6973 745b 6469 6374 5b73  set: list[dict[s
-00012050: 7472 2c20 416e 795d 5d2c 0a20 2020 206c  tr, Any]],.    l
-00012060: 616e 6775 6167 655f 6c61 6265 6c3a 2073  anguage_label: s
-00012070: 7472 2c0a 2920 2d3e 2049 7465 7261 626c  tr,.) -> Iterabl
-00012080: 655b 7475 706c 655b 7374 722c 2073 7472  e[tuple[str, str
-00012090: 5d5d 3a0a 2020 2020 2222 220a 2020 2020  ]]:.    """.    
-000120a0: 476f 2074 6872 6f75 6768 206c 6973 7420  Go through list 
-000120b0: 6e6f 6465 7320 6f66 2061 204a 534f 4e20  nodes of a JSON 
-000120c0: 7072 6f6a 6563 7420 616e 6420 7969 656c  project and yiel
-000120d0: 6420 286c 6162 656c 2c20 6e61 6d65 2920  d (label, name) 
-000120e0: 7061 6972 732e 0a0a 2020 2020 4172 6773  pairs...    Args
-000120f0: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f73  :.        json_s
-00012100: 7562 7365 743a 206c 6973 7420 6f66 2044  ubset: list of D
-00012110: 5350 206c 6973 7473 2028 6120 4453 5020  SP lists (a DSP 
-00012120: 6c69 7374 2062 6569 6e67 2061 2064 6963  list being a dic
-00012130: 7469 6f6e 6172 7920 7769 7468 2074 6865  tionary with the
-00012140: 206b 6579 7320 226e 616d 6522 2c20 226c   keys "name", "l
-00012150: 6162 656c 7322 2061 6e64 2022 6e6f 6465  abels" and "node
-00012160: 7322 290a 2020 2020 2020 2020 6c61 6e67  s").        lang
-00012170: 7561 6765 5f6c 6162 656c 3a20 7768 6963  uage_label: whic
-00012180: 6820 6c61 6e67 7561 6765 206f 6620 7468  h language of th
-00012190: 6520 6c61 6265 6c20 746f 2063 686f 6f73  e label to choos
-000121a0: 650a 0a20 2020 2059 6965 6c64 733a 0a20  e..    Yields:. 
-000121b0: 2020 2020 2020 2028 6c61 6265 6c2c 206e         (label, n
-000121c0: 616d 6529 2070 6169 7273 0a20 2020 2022  ame) pairs.    "
-000121d0: 2222 0a20 2020 2066 6f72 206e 6f64 6520  "".    for node 
-000121e0: 696e 206a 736f 6e5f 7375 6273 6574 3a0a  in json_subset:.
-000121f0: 2020 2020 2020 2020 2320 6e6f 6465 2069          # node i
-00012200: 7320 7468 6520 6a73 6f6e 206f 626a 6563  s the json objec
-00012210: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
-00012220: 2065 6e74 6972 6520 6a73 6f6e 2d6c 6973   entire json-lis
-00012230: 740a 2020 2020 2020 2020 6966 2022 6e6f  t.        if "no
-00012240: 6465 7322 2069 6e20 6e6f 6465 3a0a 2020  des" in node:.  
-00012250: 2020 2020 2020 2020 2020 2320 226e 6f64            # "nod
-00012260: 6573 2220 6973 2074 6865 206a 736f 6e20  es" is the json 
-00012270: 7375 622d 6f62 6a65 6374 2063 6f6e 7461  sub-object conta
-00012280: 696e 696e 6720 7468 6520 656e 7472 6965  ining the entrie
-00012290: 7320 6f66 2074 6865 206a 736f 6e2d 6c69  s of the json-li
-000122a0: 7374 0a20 2020 2020 2020 2020 2020 2079  st.            y
-000122b0: 6965 6c64 2066 726f 6d20 5f6e 616d 655f  ield from _name_
-000122c0: 6c61 6265 6c5f 6d61 7070 6572 5f69 7465  label_mapper_ite
-000122d0: 7261 746f 7228 6e6f 6465 5b22 6e6f 6465  rator(node["node
-000122e0: 7322 5d2c 206c 616e 6775 6167 655f 6c61  s"], language_la
-000122f0: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
-00012300: 2023 2065 6163 6820 7969 656c 6465 6420   # each yielded 
-00012310: 7661 6c75 6520 6973 2061 2028 6c61 6265  value is a (labe
-00012320: 6c2c 206e 616d 6529 2070 6169 7220 6f66  l, name) pair of
-00012330: 2061 2073 696e 676c 6520 6c69 7374 2065   a single list e
-00012340: 6e74 7279 0a20 2020 2020 2020 2069 6620  ntry.        if 
-00012350: 226e 616d 6522 2069 6e20 6e6f 6465 3a0a  "name" in node:.
-00012360: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00012370: 6420 286e 6f64 655b 226c 6162 656c 7322  d (node["labels"
-00012380: 5d5b 6c61 6e67 7561 6765 5f6c 6162 656c  ][language_label
-00012390: 5d2c 206e 6f64 655b 226e 616d 6522 5d29  ], node["name"])
-000123a0: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-000123b0: 6865 2061 6374 7561 6c20 7661 6c75 6573  he actual values
-000123c0: 206f 6620 7468 6520 6e61 6d65 2061 6e64   of the name and
-000123d0: 2074 6865 206c 6162 656c 0a0a 0a64 6566   the label...def
-000123e0: 2077 7269 7465 5f78 6d6c 280a 2020 2020   write_xml(.    
-000123f0: 726f 6f74 3a20 6574 7265 652e 5f45 6c65  root: etree._Ele
-00012400: 6d65 6e74 2c0a 2020 2020 6669 6c65 7061  ment,.    filepa
-00012410: 7468 3a20 7374 7220 7c20 5061 7468 2c0a  th: str | Path,.
-00012420: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
-00012430: 2222 0a20 2020 2057 7269 7465 2074 6865  "".    Write the
-00012440: 2066 696e 6973 6865 6420 584d 4c20 746f   finished XML to
-00012450: 2061 2066 696c 652e 0a0a 2020 2020 4172   a file...    Ar
-00012460: 6773 3a0a 2020 2020 2020 2020 726f 6f74  gs:.        root
-00012470: 3a20 6574 7265 6520 456c 656d 656e 7420  : etree Element 
-00012480: 7769 7468 2074 6865 2065 6e74 6972 6520  with the entire 
-00012490: 584d 4c20 646f 6375 6d65 6e74 0a20 2020  XML document.   
-000124a0: 2020 2020 2066 696c 6570 6174 683a 2077       filepath: w
-000124b0: 6865 7265 2074 6f20 7361 7665 2074 6865  here to save the
-000124c0: 2066 696c 650a 0a20 2020 2057 6172 6e69   file..    Warni
-000124d0: 6e67 3a0a 2020 2020 2020 2020 6966 2074  ng:.        if t
-000124e0: 6865 2058 4d4c 2069 7320 6e6f 7420 7661  he XML is not va
-000124f0: 6c69 6420 6163 636f 7264 696e 6720 746f  lid according to
-00012500: 2074 6865 2073 6368 656d 610a 2020 2020   the schema.    
-00012510: 2222 220a 2020 2020 6574 7265 652e 696e  """.    etree.in
-00012520: 6465 6e74 2872 6f6f 742c 2073 7061 6365  dent(root, space
-00012530: 3d22 2020 2020 2229 0a20 2020 2078 6d6c  ="    ").    xml
-00012540: 5f73 7472 696e 6720 3d20 6574 7265 652e  _string = etree.
-00012550: 746f 7374 7269 6e67 280a 2020 2020 2020  tostring(.      
-00012560: 2020 726f 6f74 2c0a 2020 2020 2020 2020    root,.        
-00012570: 656e 636f 6469 6e67 3d22 756e 6963 6f64  encoding="unicod
-00012580: 6522 2c0a 2020 2020 2020 2020 7072 6574  e",.        pret
-00012590: 7479 5f70 7269 6e74 3d54 7275 652c 0a20  ty_print=True,. 
-000125a0: 2020 2020 2020 2064 6f63 7479 7065 3d27         doctype='
-000125b0: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
-000125c0: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-000125d0: 462d 3822 3f3e 272c 0a20 2020 2029 0a20  F-8"?>',.    ). 
-000125e0: 2020 2078 6d6c 5f73 7472 696e 6720 3d20     xml_string = 
-000125f0: 786d 6c5f 7374 7269 6e67 2e72 6570 6c61  xml_string.repla
-00012600: 6365 2872 225c 2722 2c20 2227 2229 0a20  ce(r"\'", "'"). 
-00012610: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
-00012620: 6570 6174 682c 2022 7722 2c20 656e 636f  epath, "w", enco
-00012630: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00012640: 2066 3a0a 2020 2020 2020 2020 662e 7772   f:.        f.wr
-00012650: 6974 6528 786d 6c5f 7374 7269 6e67 290a  ite(xml_string).
-00012660: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00012670: 2076 616c 6964 6174 655f 786d 6c28 696e   validate_xml(in
-00012680: 7075 745f 6669 6c65 3d66 696c 6570 6174  put_file=filepat
-00012690: 6829 0a20 2020 2020 2020 2070 7269 6e74  h).        print
-000126a0: 2866 2254 6865 2058 4d4c 2066 696c 6520  (f"The XML file 
-000126b0: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
-000126c0: 2073 6176 6564 2074 6f20 7b66 696c 6570   saved to {filep
-000126d0: 6174 687d 2229 0a20 2020 2065 7863 6570  ath}").    excep
-000126e0: 7420 4261 7365 4572 726f 7220 6173 2065  t BaseError as e
-000126f0: 7272 3a0a 2020 2020 2020 2020 7761 726e  rr:.        warn
-00012700: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
-00012710: 2020 2020 2020 2066 2254 6865 2058 4d4c         f"The XML
-00012720: 2066 696c 6520 7761 7320 7375 6363 6573   file was succes
-00012730: 7366 756c 6c79 2073 6176 6564 2074 6f20  sfully saved to 
-00012740: 7b66 696c 6570 6174 687d 2c20 220a 2020  {filepath}, ".  
-00012750: 2020 2020 2020 2020 2020 6622 6275 7420            f"but 
-00012760: 7468 6520 666f 6c6c 6f77 696e 6720 5363  the following Sc
-00012770: 6865 6d61 2076 616c 6964 6174 696f 6e20  hema validation 
-00012780: 6572 726f 7228 7329 206f 6363 7572 7265  error(s) occurre
-00012790: 643a 207b 6572 722e 6d65 7373 6167 657d  d: {err.message}
-000127a0: 220a 2020 2020 2020 2020 290a            ".        ).
+0000ec40: 203c 7572 692d 7072 6f70 206e 616d 653d   <uri-prop name=
+0000ec50: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+0000ec60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ec70: 2020 2020 203c 7572 6920 7065 726d 6973       <uri permis
+0000ec80: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+0000ec90: 756c 7422 3e77 7777 2e74 6573 742e 636f  ult">www.test.co
+0000eca0: 6d3c 2f75 7269 3e0a 2020 2020 2020 2020  m</uri>.        
+0000ecb0: 2020 2020 2020 2020 3c2f 7572 692d 7072          </uri-pr
+0000ecc0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
+0000ecd0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f75  excel2xml.make_u
+0000ece0: 7269 5f70 726f 7028 223a 7465 7374 7072  ri_prop(":testpr
+0000ecf0: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
+0000ed00: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
+0000ed10: 6e74 2822 7777 772e 7465 7374 2e63 6f6d  nt("www.test.com
+0000ed20: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
+0000ed30: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+0000ed40: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
+0000ed50: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
+0000ed60: 2020 2020 2020 3c75 7269 2d70 726f 7020        <uri-prop 
+0000ed70: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
+0000ed80: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
+0000ed90: 2020 2020 2020 2020 2020 3c75 7269 2070            <uri p
+0000eda0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000edb0: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
+0000edc0: 6d65 6e74 3d22 6578 616d 706c 6522 3e77  ment="example">w
+0000edd0: 7777 2e74 6573 742e 636f 6d3c 2f75 7269  ww.test.com</uri
+0000ede0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000edf0: 2020 3c2f 7572 692d 7072 6f70 3e0a 2020    </uri-prop>.  
+0000ee00: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000ee10: 786d 6c2e 6d61 6b65 5f75 7269 5f70 726f  xml.make_uri_pro
+0000ee20: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+0000ee30: 222c 205b 2277 7777 2e31 2e63 6f6d 222c  ", ["www.1.com",
+0000ee40: 2022 7777 772e 322e 636f 6d22 5d29 0a20   "www.2.com"]). 
+0000ee50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000ee60: 7572 692d 7072 6f70 206e 616d 653d 223a  uri-prop name=":
+0000ee70: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
+0000ee80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee90: 2020 203c 7572 6920 7065 726d 6973 7369     <uri permissi
+0000eea0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
+0000eeb0: 7422 3e77 7777 2e31 2e63 6f6d 3c2f 7572  t">www.1.com</ur
+0000eec0: 693e 0a20 2020 2020 2020 2020 2020 2020  i>.             
+0000eed0: 2020 2020 2020 203c 7572 6920 7065 726d         <uri perm
+0000eee0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+0000eef0: 6661 756c 7422 3e77 7777 2e32 2e63 6f6d  fault">www.2.com
+0000ef00: 3c2f 7572 693e 0a20 2020 2020 2020 2020  </uri>.         
+0000ef10: 2020 2020 2020 203c 2f75 7269 2d70 726f         </uri-pro
+0000ef20: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
+0000ef30: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+0000ef40: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+0000ef50: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+0000ef60: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+0000ef70: 2f23 7572 692d 7072 6f70 0a20 2020 2022  /#uri-prop.    "
+0000ef80: 2222 0a0a 2020 2020 2320 6368 6563 6b20  ""..    # check 
+0000ef90: 7468 6520 696e 7075 743a 2070 7265 7061  the input: prepa
+0000efa0: 7265 2061 206c 6973 7420 7769 7468 2076  re a list with v
+0000efb0: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
+0000efc0: 7661 6c75 6573 203d 2070 7265 7061 7265  values = prepare
+0000efd0: 5f76 616c 7565 2876 616c 7565 290a 0a20  _value(value).. 
+0000efe0: 2020 2023 2063 6865 636b 2076 616c 7565     # check value
+0000eff0: 2074 7970 650a 2020 2020 666f 7220 7661   type.    for va
+0000f000: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
+0000f010: 2020 2020 2069 6620 6e6f 7420 6973 5f75       if not is_u
+0000f020: 7269 2873 7472 2876 616c 2e76 616c 7565  ri(str(val.value
+0000f030: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000f040: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
+0000f050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f060: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
+0000f070: 7469 6f6e 2069 6e20 7265 736f 7572 6365  tion in resource
+0000f080: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
+0000f090: 7263 657d 272c 2070 726f 7065 7274 7920  rce}', property 
+0000f0a0: 277b 6e61 6d65 7d27 3a20 220a 2020 2020  '{name}': ".    
+0000f0b0: 2020 2020 2020 2020 2020 2020 6622 277b              f"'{
+0000f0c0: 7661 6c2e 7661 6c75 657d 2720 6973 206e  val.value}' is n
+0000f0d0: 6f74 2061 2076 616c 6964 2055 5249 2e22  ot a valid URI."
+0000f0e0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+0000f0f0: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
+0000f100: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
+0000f110: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
+0000f120: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
+0000f130: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0000f140: 227b 2573 7d75 7269 2d70 726f 7022 2025  "{%s}uri-prop" %
+0000f150: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+0000f160: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+0000f170: 2020 6e61 6d65 3d6e 616d 652c 0a20 2020    name=name,.   
+0000f180: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
+0000f190: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
+0000f1a0: 2020 290a 2020 2020 666f 7220 7661 6c20    ).    for val 
+0000f1b0: 696e 2076 616c 7565 733a 0a20 2020 2020  in values:.     
+0000f1c0: 2020 206b 7761 7267 7320 3d20 7b22 7065     kwargs = {"pe
+0000f1d0: 726d 6973 7369 6f6e 7322 3a20 7661 6c2e  rmissions": val.
+0000f1e0: 7065 726d 6973 7369 6f6e 737d 0a20 2020  permissions}.   
+0000f1f0: 2020 2020 2069 6620 7661 6c2e 636f 6d6d       if val.comm
+0000f200: 656e 7420 616e 6420 6368 6563 6b5f 6e6f  ent and check_no
+0000f210: 746e 6128 7661 6c2e 636f 6d6d 656e 7429  tna(val.comment)
+0000f220: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
+0000f230: 6172 6773 5b22 636f 6d6d 656e 7422 5d20  args["comment"] 
+0000f240: 3d20 7661 6c2e 636f 6d6d 656e 740a 2020  = val.comment.  
+0000f250: 2020 2020 2020 7661 6c75 655f 203d 2065        value_ = e
+0000f260: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
+0000f270: 2020 2020 2020 2020 2020 227b 2573 7d75            "{%s}u
+0000f280: 7269 2220 2520 786d 6c5f 6e61 6d65 7370  ri" % xml_namesp
+0000f290: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
+0000f2a0: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+0000f2b0: 7267 732c 2020 2320 7479 7065 3a20 6967  rgs,  # type: ig
+0000f2c0: 6e6f 7265 5b61 7267 2d74 7970 655d 0a20  nore[arg-type]. 
+0000f2d0: 2020 2020 2020 2020 2020 206e 736d 6170             nsmap
+0000f2e0: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
+0000f2f0: 6170 2c0a 2020 2020 2020 2020 290a 2020  ap,.        ).  
+0000f300: 2020 2020 2020 7661 6c75 655f 2e74 6578        value_.tex
+0000f310: 7420 3d20 7374 7228 7661 6c2e 7661 6c75  t = str(val.valu
+0000f320: 6529 0a20 2020 2020 2020 2070 726f 705f  e).        prop_
+0000f330: 2e61 7070 656e 6428 7661 6c75 655f 290a  .append(value_).
+0000f340: 0a20 2020 2072 6574 7572 6e20 7072 6f70  .    return prop
+0000f350: 5f0a 0a0a 6465 6620 6d61 6b65 5f72 6567  _...def make_reg
+0000f360: 696f 6e28 2020 2320 6e6f 7161 3a20 4434  ion(  # noqa: D4
+0000f370: 3137 2028 756e 646f 6375 6d65 6e74 6564  17 (undocumented
+0000f380: 2d70 6172 616d 290a 2020 2020 6c61 6265  -param).    labe
+0000f390: 6c3a 2073 7472 2c0a 2020 2020 6964 3a20  l: str,.    id: 
+0000f3a0: 7374 722c 0a20 2020 2070 6572 6d69 7373  str,.    permiss
+0000f3b0: 696f 6e73 3a20 7374 7220 3d20 2272 6573  ions: str = "res
+0000f3c0: 2d64 6566 6175 6c74 222c 0a20 2020 2061  -default",.    a
+0000f3d0: 726b 3a20 4f70 7469 6f6e 616c 5b73 7472  rk: Optional[str
+0000f3e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6972  ] = None,.    ir
+0000f3f0: 693a 204f 7074 696f 6e61 6c5b 7374 725d  i: Optional[str]
+0000f400: 203d 204e 6f6e 652c 0a20 2020 2063 7265   = None,.    cre
+0000f410: 6174 696f 6e5f 6461 7465 3a20 4f70 7469  ation_date: Opti
+0000f420: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000f430: 2c0a 2920 2d3e 2065 7472 6565 2e5f 456c  ,.) -> etree._El
+0000f440: 656d 656e 743a 0a20 2020 2022 2222 0a20  ement:.    """. 
+0000f450: 2020 2043 7265 6174 6573 2061 6e20 656d     Creates an em
+0000f460: 7074 7920 7265 6769 6f6e 2065 6c65 6d65  pty region eleme
+0000f470: 6e74 2c20 7769 7468 2074 6865 2061 7474  nt, with the att
+0000f480: 7269 6275 7465 7320 6173 2073 7065 6369  ributes as speci
+0000f490: 6669 6564 2062 7920 7468 6520 6172 6775  fied by the argu
+0000f4a0: 6d65 6e74 730a 0a20 2020 2041 7267 733a  ments..    Args:
+0000f4b0: 0a20 2020 2020 2020 2054 6865 2061 7267  .        The arg
+0000f4c0: 756d 656e 7473 2063 6f72 7265 7370 6f6e  uments correspon
+0000f4d0: 6420 313a 3120 746f 2074 6865 2061 7474  d 1:1 to the att
+0000f4e0: 7269 6275 7465 7320 6f66 2074 6865 203c  ributes of the <
+0000f4f0: 7265 6769 6f6e 3e20 656c 656d 656e 742e  region> element.
+0000f500: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
+0000f510: 2020 2020 2020 5761 726e 696e 673a 2069        Warning: i
+0000f520: 6620 626f 7468 2061 6e20 4152 4b20 616e  f both an ARK an
+0000f530: 6420 616e 2049 5249 2061 7265 2070 726f  d an IRI are pro
+0000f540: 7669 6465 640a 2020 2020 2020 2020 4261  vided.        Ba
+0000f550: 7365 4572 726f 723a 2069 6620 7468 6520  seError: if the 
+0000f560: 6372 6561 7469 6f6e 2064 6174 6520 6973  creation date is
+0000f570: 2069 6e76 616c 6964 0a0a 2020 2020 5265   invalid..    Re
+0000f580: 7475 726e 733a 0a20 2020 2020 2020 2054  turns:.        T
+0000f590: 6865 2072 6567 696f 6e20 656c 656d 656e  he region elemen
+0000f5a0: 742c 2077 6974 686f 7574 2061 6e79 2063  t, without any c
+0000f5b0: 6869 6c64 7265 6e2c 2062 7574 2077 6974  hildren, but wit
+0000f5c0: 6820 7468 6520 6174 7472 6962 7574 6573  h the attributes
+0000f5d0: 3a0a 2020 2020 2020 2020 3c72 6567 696f  :.        <regio
+0000f5e0: 6e20 6c61 6265 6c3d 6c61 6265 6c20 6964  n label=label id
+0000f5f0: 3d69 6420 7065 726d 6973 7369 6f6e 733d  =id permissions=
+0000f600: 7065 726d 6973 7369 6f6e 7320 6172 6b3d  permissions ark=
+0000f610: 6172 6b20 6972 693d 6972 693e 3c2f 7265  ark iri=iri></re
+0000f620: 6769 6f6e 3e0a 0a20 2020 2045 7861 6d70  gion>..    Examp
+0000f630: 6c65 733a 0a20 2020 2020 2020 203e 3e3e  les:.        >>>
+0000f640: 2072 6567 696f 6e20 3d20 6578 6365 6c32   region = excel2
+0000f650: 786d 6c2e 6d61 6b65 5f72 6567 696f 6e28  xml.make_region(
+0000f660: 226c 6162 656c 222c 2022 6964 2229 0a20  "label", "id"). 
+0000f670: 2020 2020 2020 203e 3e3e 2072 6567 696f         >>> regio
+0000f680: 6e2e 6170 7065 6e64 2865 7863 656c 3278  n.append(excel2x
+0000f690: 6d6c 2e6d 616b 655f 7465 7874 5f70 726f  ml.make_text_pro
+0000f6a0: 7028 2268 6173 436f 6d6d 656e 7422 2c20  p("hasComment", 
+0000f6b0: 2254 6869 7320 6973 2061 2063 6f6d 6d65  "This is a comme
+0000f6c0: 6e74 2229 290a 2020 2020 2020 2020 3e3e  nt")).        >>
+0000f6d0: 3e20 7265 6769 6f6e 2e61 7070 656e 6428  > region.append(
+0000f6e0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f63  excel2xml.make_c
+0000f6f0: 6f6c 6f72 5f70 726f 7028 2268 6173 436f  olor_prop("hasCo
+0000f700: 6c6f 7222 2c20 2223 3564 3166 3165 2229  lor", "#5d1f1e")
+0000f710: 290a 2020 2020 2020 2020 3e3e 3e20 7265  ).        >>> re
+0000f720: 6769 6f6e 2e61 7070 656e 6428 6578 6365  gion.append(exce
+0000f730: 6c32 786d 6c2e 6d61 6b65 5f72 6573 7074  l2xml.make_respt
+0000f740: 725f 7072 6f70 2822 6973 5265 6769 6f6e  r_prop("isRegion
+0000f750: 4f66 222c 2022 696d 6167 655f 3022 2929  Of", "image_0"))
+0000f760: 0a20 2020 2020 2020 203e 3e3e 2072 6567  .        >>> reg
+0000f770: 696f 6e2e 6170 7065 6e64 2865 7863 656c  ion.append(excel
+0000f780: 3278 6d6c 2e6d 616b 655f 6765 6f6d 6574  2xml.make_geomet
+0000f790: 7279 5f70 726f 7028 2268 6173 4765 6f6d  ry_prop("hasGeom
+0000f7a0: 6574 7279 222c 2022 7b2e 2e2e 7d22 2929  etry", "{...}"))
+0000f7b0: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
+0000f7c0: 742e 6170 7065 6e64 2872 6567 696f 6e29  t.append(region)
+0000f7d0: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
+0000f7e0: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
+0000f7f0: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
+0000f800: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
+0000f810: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
+0000f820: 7265 6769 6f6e 0a20 2020 2022 2222 0a0a  region.    """..
+0000f830: 2020 2020 6b77 6172 6773 203d 207b 226c      kwargs = {"l
+0000f840: 6162 656c 223a 206c 6162 656c 2c20 2269  abel": label, "i
+0000f850: 6422 3a20 6964 2c20 2270 6572 6d69 7373  d": id, "permiss
+0000f860: 696f 6e73 223a 2070 6572 6d69 7373 696f  ions": permissio
+0000f870: 6e73 2c20 226e 736d 6170 223a 2078 6d6c  ns, "nsmap": xml
+0000f880: 5f6e 616d 6573 7061 6365 5f6d 6170 7d0a  _namespace_map}.
+0000f890: 2020 2020 6966 2061 726b 3a0a 2020 2020      if ark:.    
+0000f8a0: 2020 2020 6b77 6172 6773 5b22 6172 6b22      kwargs["ark"
+0000f8b0: 5d20 3d20 6172 6b0a 2020 2020 6966 2069  ] = ark.    if i
+0000f8c0: 7269 3a0a 2020 2020 2020 2020 6b77 6172  ri:.        kwar
+0000f8d0: 6773 5b22 6972 6922 5d20 3d20 6972 690a  gs["iri"] = iri.
+0000f8e0: 2020 2020 6966 2061 726b 2061 6e64 2069      if ark and i
+0000f8f0: 7269 3a0a 2020 2020 2020 2020 7761 726e  ri:.        warn
+0000f900: 696e 6773 2e77 6172 6e28 0a20 2020 2020  ings.warn(.     
+0000f910: 2020 2020 2020 2066 2242 6f74 6820 4152         f"Both AR
+0000f920: 4b20 616e 6420 4952 4920 7765 7265 2070  K and IRI were p
+0000f930: 726f 7669 6465 6420 666f 7220 7265 736f  rovided for reso
+0000f940: 7572 6365 2027 7b6c 6162 656c 7d27 2028  urce '{label}' (
+0000f950: 7b69 647d 292e 2054 6865 2041 524b 2077  {id}). The ARK w
+0000f960: 696c 6c20 6f76 6572 7269 6465 2074 6865  ill override the
+0000f970: 2049 5249 2e22 2c0a 2020 2020 2020 2020   IRI.",.        
+0000f980: 2020 2020 7374 6163 6b6c 6576 656c 3d32      stacklevel=2
+0000f990: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0000f9a0: 6966 2063 7265 6174 696f 6e5f 6461 7465  if creation_date
+0000f9b0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+0000f9c0: 2020 2020 2020 2020 2020 2044 6174 6554             DateT
+0000f9d0: 696d 6553 7461 6d70 2863 7265 6174 696f  imeStamp(creatio
+0000f9e0: 6e5f 6461 7465 290a 2020 2020 2020 2020  n_date).        
+0000f9f0: 6578 6365 7074 2042 6173 6545 7272 6f72  except BaseError
+0000fa00: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000fa10: 6973 6520 4261 7365 4572 726f 7228 0a20  ise BaseError(. 
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000fa30: 2254 6865 2072 6567 696f 6e20 277b 6c61  "The region '{la
+0000fa40: 6265 6c7d 2720 2849 443a 207b 6964 7d29  bel}' (ID: {id})
+0000fa50: 2068 6173 2061 6e20 696e 7661 6c69 6420   has an invalid 
+0000fa60: 6372 6561 7469 6f6e 2064 6174 6520 277b  creation date '{
+0000fa70: 6372 6561 7469 6f6e 5f64 6174 657d 272e  creation_date}'.
+0000fa80: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000fa90: 2020 2066 2244 6964 2079 6f75 2070 6572     f"Did you per
+0000faa0: 6861 7073 2066 6f72 6765 7420 7468 6520  haps forget the 
+0000fab0: 7469 6d65 7a6f 6e65 3f22 0a20 2020 2020  timezone?".     
+0000fac0: 2020 2020 2020 2029 2066 726f 6d20 4e6f         ) from No
+0000fad0: 6e65 0a20 2020 2020 2020 206b 7761 7267  ne.        kwarg
+0000fae0: 735b 2263 7265 6174 696f 6e5f 6461 7465  s["creation_date
+0000faf0: 225d 203d 2063 7265 6174 696f 6e5f 6461  "] = creation_da
+0000fb00: 7465 0a0a 2020 2020 7265 7475 726e 2065  te..    return e
+0000fb10: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
+0000fb20: 2020 2020 2020 227b 2573 7d72 6567 696f        "{%s}regio
+0000fb30: 6e22 2025 2078 6d6c 5f6e 616d 6573 7061  n" % xml_namespa
+0000fb40: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000fb50: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
+0000fb60: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+0000fb70: 6172 672d 7479 7065 5d0a 2020 2020 290a  arg-type].    ).
+0000fb80: 0a0a 6465 6620 6d61 6b65 5f61 6e6e 6f74  ..def make_annot
+0000fb90: 6174 696f 6e28 2020 2320 6e6f 7161 3a20  ation(  # noqa: 
+0000fba0: 4434 3137 2028 756e 646f 6375 6d65 6e74  D417 (undocument
+0000fbb0: 6564 2d70 6172 616d 290a 2020 2020 6c61  ed-param).    la
+0000fbc0: 6265 6c3a 2073 7472 2c0a 2020 2020 6964  bel: str,.    id
+0000fbd0: 3a20 7374 722c 0a20 2020 2070 6572 6d69  : str,.    permi
+0000fbe0: 7373 696f 6e73 3a20 7374 7220 3d20 2272  ssions: str = "r
+0000fbf0: 6573 2d64 6566 6175 6c74 222c 0a20 2020  es-default",.   
+0000fc00: 2061 726b 3a20 4f70 7469 6f6e 616c 5b73   ark: Optional[s
+0000fc10: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000fc20: 6972 693a 204f 7074 696f 6e61 6c5b 7374  iri: Optional[st
+0000fc30: 725d 203d 204e 6f6e 652c 0a20 2020 2063  r] = None,.    c
+0000fc40: 7265 6174 696f 6e5f 6461 7465 3a20 4f70  reation_date: Op
+0000fc50: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000fc60: 6e65 2c0a 2920 2d3e 2065 7472 6565 2e5f  ne,.) -> etree._
+0000fc70: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
+0000fc80: 0a20 2020 2043 7265 6174 6573 2061 6e20  .    Creates an 
+0000fc90: 656d 7074 7920 616e 6e6f 7461 7469 6f6e  empty annotation
+0000fca0: 2065 6c65 6d65 6e74 2c20 7769 7468 2074   element, with t
+0000fcb0: 6865 2061 7474 7269 6275 7465 7320 6173  he attributes as
+0000fcc0: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+0000fcd0: 6520 6172 6775 6d65 6e74 730a 0a20 2020  e arguments..   
+0000fce0: 2041 7267 733a 0a20 2020 2020 2020 2054   Args:.        T
+0000fcf0: 6865 2061 7267 756d 656e 7473 2063 6f72  he arguments cor
+0000fd00: 7265 7370 6f6e 6420 313a 3120 746f 2074  respond 1:1 to t
+0000fd10: 6865 2061 7474 7269 6275 7465 7320 6f66  he attributes of
+0000fd20: 2074 6865 203c 616e 6e6f 7461 7469 6f6e   the <annotation
+0000fd30: 3e20 656c 656d 656e 742e 0a0a 2020 2020  > element...    
+0000fd40: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0000fd50: 5761 726e 696e 673a 2069 6620 626f 7468  Warning: if both
+0000fd60: 2061 6e20 4152 4b20 616e 6420 616e 2049   an ARK and an I
+0000fd70: 5249 2061 7265 2070 726f 7669 6465 640a  RI are provided.
+0000fd80: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+0000fd90: 723a 2069 6620 7468 6520 6372 6561 7469  r: if the creati
+0000fda0: 6f6e 2064 6174 6520 6973 2069 6e76 616c  on date is inval
+0000fdb0: 6964 0a0a 2020 2020 5265 7475 726e 733a  id..    Returns:
+0000fdc0: 0a20 2020 2020 2020 2054 6865 2061 6e6e  .        The ann
+0000fdd0: 6f74 6174 696f 6e20 656c 656d 656e 742c  otation element,
+0000fde0: 2077 6974 686f 7574 2061 6e79 2063 6869   without any chi
+0000fdf0: 6c64 7265 6e2c 2062 7574 2077 6974 6820  ldren, but with 
+0000fe00: 7468 6520 6174 7472 6962 7574 6573 3a0a  the attributes:.
+0000fe10: 2020 2020 2020 2020 3c61 6e6e 6f74 6174          <annotat
+0000fe20: 696f 6e20 6c61 6265 6c3d 6c61 6265 6c20  ion label=label 
+0000fe30: 6964 3d69 6420 7065 726d 6973 7369 6f6e  id=id permission
+0000fe40: 733d 7065 726d 6973 7369 6f6e 7320 6172  s=permissions ar
+0000fe50: 6b3d 6172 6b20 6972 693d 6972 693e 3c2f  k=ark iri=iri></
+0000fe60: 616e 6e6f 7461 7469 6f6e 3e0a 0a20 2020  annotation>..   
+0000fe70: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+0000fe80: 2020 203e 3e3e 2061 6e6e 6f74 6174 696f     >>> annotatio
+0000fe90: 6e20 3d20 6578 6365 6c32 786d 6c2e 6d61  n = excel2xml.ma
+0000fea0: 6b65 5f61 6e6e 6f74 6174 696f 6e28 226c  ke_annotation("l
+0000feb0: 6162 656c 222c 2022 6964 2229 0a20 2020  abel", "id").   
+0000fec0: 2020 2020 203e 3e3e 2061 6e6e 6f74 6174       >>> annotat
+0000fed0: 696f 6e2e 6170 7065 6e64 2865 7863 656c  ion.append(excel
+0000fee0: 3278 6d6c 2e6d 616b 655f 7465 7874 5f70  2xml.make_text_p
+0000fef0: 726f 7028 2268 6173 436f 6d6d 656e 7422  rop("hasComment"
+0000ff00: 2c20 2254 6869 7320 6973 2061 2063 6f6d  , "This is a com
+0000ff10: 6d65 6e74 2229 290a 2020 2020 2020 2020  ment")).        
+0000ff20: 3e3e 3e20 616e 6e6f 7461 7469 6f6e 2e61  >>> annotation.a
+0000ff30: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+0000ff40: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+0000ff50: 2822 6973 416e 6e6f 7461 7469 6f6e 4f66  ("isAnnotationOf
+0000ff60: 222c 2022 7265 736f 7572 6365 5f30 2229  ", "resource_0")
+0000ff70: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
+0000ff80: 6f74 2e61 7070 656e 6428 616e 6e6f 7461  ot.append(annota
+0000ff90: 7469 6f6e 290a 0a20 2020 2053 6565 2068  tion)..    See h
+0000ffa0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
+0000ffb0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
+0000ffc0: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
+0000ffd0: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
+0000ffe0: 696c 652f 2361 6e6e 6f74 6174 696f 6e0a  ile/#annotation.
+0000fff0: 2020 2020 2222 220a 0a20 2020 206b 7761      """..    kwa
+00010000: 7267 7320 3d20 7b22 6c61 6265 6c22 3a20  rgs = {"label": 
+00010010: 6c61 6265 6c2c 2022 6964 223a 2069 642c  label, "id": id,
+00010020: 2022 7065 726d 6973 7369 6f6e 7322 3a20   "permissions": 
+00010030: 7065 726d 6973 7369 6f6e 732c 2022 6e73  permissions, "ns
+00010040: 6d61 7022 3a20 786d 6c5f 6e61 6d65 7370  map": xml_namesp
+00010050: 6163 655f 6d61 707d 0a20 2020 2069 6620  ace_map}.    if 
+00010060: 6172 6b3a 0a20 2020 2020 2020 206b 7761  ark:.        kwa
+00010070: 7267 735b 2261 726b 225d 203d 2061 726b  rgs["ark"] = ark
+00010080: 0a20 2020 2069 6620 6972 693a 0a20 2020  .    if iri:.   
+00010090: 2020 2020 206b 7761 7267 735b 2269 7269       kwargs["iri
+000100a0: 225d 203d 2069 7269 0a20 2020 2069 6620  "] = iri.    if 
+000100b0: 6172 6b20 616e 6420 6972 693a 0a20 2020  ark and iri:.   
+000100c0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+000100d0: 726e 280a 2020 2020 2020 2020 2020 2020  rn(.            
+000100e0: 6622 426f 7468 2041 524b 2061 6e64 2049  f"Both ARK and I
+000100f0: 5249 2077 6572 6520 7072 6f76 6964 6564  RI were provided
+00010100: 2066 6f72 2072 6573 6f75 7263 6520 277b   for resource '{
+00010110: 6c61 6265 6c7d 2720 287b 6964 7d29 2e20  label}' ({id}). 
+00010120: 5468 6520 4152 4b20 7769 6c6c 206f 7665  The ARK will ove
+00010130: 7272 6964 6520 7468 6520 4952 492e 222c  rride the IRI.",
+00010140: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00010150: 636b 6c65 7665 6c3d 322c 0a20 2020 2020  cklevel=2,.     
+00010160: 2020 2029 0a20 2020 2069 6620 6372 6561     ).    if crea
+00010170: 7469 6f6e 5f64 6174 653a 0a20 2020 2020  tion_date:.     
+00010180: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00010190: 2020 2020 4461 7465 5469 6d65 5374 616d      DateTimeStam
+000101a0: 7028 6372 6561 7469 6f6e 5f64 6174 6529  p(creation_date)
+000101b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000101c0: 4261 7365 4572 726f 723a 0a20 2020 2020  BaseError:.     
+000101d0: 2020 2020 2020 2072 6169 7365 2042 6173         raise Bas
+000101e0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000101f0: 2020 2020 2020 2020 6622 5468 6520 616e          f"The an
+00010200: 6e6f 7461 7469 6f6e 2027 7b6c 6162 656c  notation '{label
+00010210: 7d27 2028 4944 3a20 7b69 647d 2920 6861  }' (ID: {id}) ha
+00010220: 7320 616e 2069 6e76 616c 6964 2063 7265  s an invalid cre
+00010230: 6174 696f 6e20 6461 7465 2027 7b63 7265  ation date '{cre
+00010240: 6174 696f 6e5f 6461 7465 7d27 2e20 220a  ation_date}'. ".
+00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010260: 6622 4469 6420 796f 7520 7065 7268 6170  f"Did you perhap
+00010270: 7320 666f 7267 6574 2074 6865 2074 696d  s forget the tim
+00010280: 657a 6f6e 653f 220a 2020 2020 2020 2020  ezone?".        
+00010290: 2020 2020 2920 6672 6f6d 204e 6f6e 650a      ) from None.
+000102a0: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+000102b0: 6372 6561 7469 6f6e 5f64 6174 6522 5d20  creation_date"] 
+000102c0: 3d20 6372 6561 7469 6f6e 5f64 6174 650a  = creation_date.
+000102d0: 0a20 2020 2072 6574 7572 6e20 6574 7265  .    return etre
+000102e0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+000102f0: 2020 2022 7b25 737d 616e 6e6f 7461 7469     "{%s}annotati
+00010300: 6f6e 2220 2520 786d 6c5f 6e61 6d65 7370  on" % xml_namesp
+00010310: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
+00010320: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+00010330: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00010340: 5b61 7267 2d74 7970 655d 0a20 2020 2029  [arg-type].    )
+00010350: 0a0a 0a64 6566 206d 616b 655f 6c69 6e6b  ...def make_link
+00010360: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
+00010370: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
+00010380: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
+00010390: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
+000103a0: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
+000103b0: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
+000103c0: 6661 756c 7422 2c0a 2020 2020 6172 6b3a  fault",.    ark:
+000103d0: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+000103e0: 204e 6f6e 652c 0a20 2020 2069 7269 3a20   None,.    iri: 
+000103f0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00010400: 4e6f 6e65 2c0a 2020 2020 6372 6561 7469  None,.    creati
+00010410: 6f6e 5f64 6174 653a 204f 7074 696f 6e61  on_date: Optiona
+00010420: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
+00010430: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
+00010440: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
+00010450: 4372 6561 7465 7320 616e 2065 6d70 7479  Creates an empty
+00010460: 206c 696e 6b20 656c 656d 656e 742c 2077   link element, w
+00010470: 6974 6820 7468 6520 6174 7472 6962 7574  ith the attribut
+00010480: 6573 2061 7320 7370 6563 6966 6965 6420  es as specified 
+00010490: 6279 2074 6865 2061 7267 756d 656e 7473  by the arguments
+000104a0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000104b0: 2020 2020 5468 6520 6172 6775 6d65 6e74      The argument
+000104c0: 7320 636f 7272 6573 706f 6e64 2031 3a31  s correspond 1:1
+000104d0: 2074 6f20 7468 6520 6174 7472 6962 7574   to the attribut
+000104e0: 6573 206f 6620 7468 6520 3c6c 696e 6b3e  es of the <link>
+000104f0: 2065 6c65 6d65 6e74 2e0a 0a20 2020 2052   element...    R
+00010500: 6169 7365 733a 0a20 2020 2020 2020 2057  aises:.        W
+00010510: 6172 6e69 6e67 3a20 6966 2062 6f74 6820  arning: if both 
+00010520: 616e 2041 524b 2061 6e64 2061 6e20 4952  an ARK and an IR
+00010530: 4920 6172 6520 7072 6f76 6964 6564 0a20  I are provided. 
+00010540: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
+00010550: 3a20 6966 2074 6865 2063 7265 6174 696f  : if the creatio
+00010560: 6e20 6461 7465 2069 7320 696e 7661 6c69  n date is invali
+00010570: 640a 0a20 2020 2052 6574 7572 6e73 3a0a  d..    Returns:.
+00010580: 2020 2020 2020 2020 5468 6520 6c69 6e6b          The link
+00010590: 2065 6c65 6d65 6e74 2c20 7769 7468 6f75   element, withou
+000105a0: 7420 616e 7920 6368 696c 6472 656e 2c20  t any children, 
+000105b0: 6275 7420 7769 7468 2074 6865 2061 7474  but with the att
+000105c0: 7269 6275 7465 733a 0a20 2020 2020 2020  ributes:.       
+000105d0: 203c 6c69 6e6b 206c 6162 656c 3d6c 6162   <link label=lab
+000105e0: 656c 2069 643d 6964 2070 6572 6d69 7373  el id=id permiss
+000105f0: 696f 6e73 3d70 6572 6d69 7373 696f 6e73  ions=permissions
+00010600: 2061 726b 3d61 726b 2069 7269 3d69 7269   ark=ark iri=iri
+00010610: 3e3c 2f6c 696e 6b3e 0a0a 2020 2020 4578  ></link>..    Ex
+00010620: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00010630: 3e3e 3e20 6c69 6e6b 203d 2065 7863 656c  >>> link = excel
+00010640: 3278 6d6c 2e6d 616b 655f 6c69 6e6b 2822  2xml.make_link("
+00010650: 6c61 6265 6c22 2c20 2269 6422 290a 2020  label", "id").  
+00010660: 2020 2020 2020 3e3e 3e20 6c69 6e6b 2e61        >>> link.a
+00010670: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+00010680: 6d61 6b65 5f74 6578 745f 7072 6f70 2822  make_text_prop("
+00010690: 6861 7343 6f6d 6d65 6e74 222c 2022 5468  hasComment", "Th
+000106a0: 6973 2069 7320 6120 636f 6d6d 656e 7422  is is a comment"
+000106b0: 2929 0a20 2020 2020 2020 203e 3e3e 206c  )).        >>> l
+000106c0: 696e 6b2e 6170 7065 6e64 2865 7863 656c  ink.append(excel
+000106d0: 3278 6d6c 2e6d 616b 655f 7265 7370 7472  2xml.make_resptr
+000106e0: 5f70 726f 7028 2268 6173 4c69 6e6b 546f  _prop("hasLinkTo
+000106f0: 222c 205b 2272 6573 6f75 7263 655f 3022  ", ["resource_0"
+00010700: 2c20 2272 6573 6f75 7263 655f 3122 5d29  , "resource_1"])
+00010710: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
+00010720: 6f74 2e61 7070 656e 6428 6c69 6e6b 290a  ot.append(link).
+00010730: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+00010740: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
+00010750: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
+00010760: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
+00010770: 786d 6c2d 6461 7461 2d66 696c 652f 236c  xml-data-file/#l
+00010780: 696e 6b0a 2020 2020 2222 220a 0a20 2020  ink.    """..   
+00010790: 206b 7761 7267 7320 3d20 7b22 6c61 6265   kwargs = {"labe
+000107a0: 6c22 3a20 6c61 6265 6c2c 2022 6964 223a  l": label, "id":
+000107b0: 2069 642c 2022 7065 726d 6973 7369 6f6e   id, "permission
+000107c0: 7322 3a20 7065 726d 6973 7369 6f6e 732c  s": permissions,
+000107d0: 2022 6e73 6d61 7022 3a20 786d 6c5f 6e61   "nsmap": xml_na
+000107e0: 6d65 7370 6163 655f 6d61 707d 0a20 2020  mespace_map}.   
+000107f0: 2069 6620 6172 6b3a 0a20 2020 2020 2020   if ark:.       
+00010800: 206b 7761 7267 735b 2261 726b 225d 203d   kwargs["ark"] =
+00010810: 2061 726b 0a20 2020 2069 6620 6972 693a   ark.    if iri:
+00010820: 0a20 2020 2020 2020 206b 7761 7267 735b  .        kwargs[
+00010830: 2269 7269 225d 203d 2069 7269 0a20 2020  "iri"] = iri.   
+00010840: 2069 6620 6172 6b20 616e 6420 6972 693a   if ark and iri:
+00010850: 0a20 2020 2020 2020 2077 6172 6e69 6e67  .        warning
+00010860: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00010870: 2020 2020 6622 426f 7468 2041 524b 2061      f"Both ARK a
+00010880: 6e64 2049 5249 2077 6572 6520 7072 6f76  nd IRI were prov
+00010890: 6964 6564 2066 6f72 2072 6573 6f75 7263  ided for resourc
+000108a0: 6520 277b 6c61 6265 6c7d 2720 287b 6964  e '{label}' ({id
+000108b0: 7d29 2e20 5468 6520 4152 4b20 7769 6c6c  }). The ARK will
+000108c0: 206f 7665 7272 6964 6520 7468 6520 4952   override the IR
+000108d0: 492e 222c 0a20 2020 2020 2020 2020 2020  I.",.           
+000108e0: 2073 7461 636b 6c65 7665 6c3d 322c 0a20   stacklevel=2,. 
+000108f0: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
+00010900: 6372 6561 7469 6f6e 5f64 6174 653a 0a20  creation_date:. 
+00010910: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010920: 2020 2020 2020 2020 4461 7465 5469 6d65          DateTime
+00010930: 5374 616d 7028 6372 6561 7469 6f6e 5f64  Stamp(creation_d
+00010940: 6174 6529 0a20 2020 2020 2020 2065 7863  ate).        exc
+00010950: 6570 7420 4261 7365 4572 726f 723a 0a20  ept BaseError:. 
+00010960: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00010970: 2042 6173 6545 7272 6f72 280a 2020 2020   BaseError(.    
+00010980: 2020 2020 2020 2020 2020 2020 6622 5468              f"Th
+00010990: 6520 6c69 6e6b 2027 7b6c 6162 656c 7d27  e link '{label}'
+000109a0: 2028 4944 3a20 7b69 647d 2920 6861 7320   (ID: {id}) has 
+000109b0: 616e 2069 6e76 616c 6964 2063 7265 6174  an invalid creat
+000109c0: 696f 6e20 6461 7465 2027 7b63 7265 6174  ion date '{creat
+000109d0: 696f 6e5f 6461 7465 7d27 2e20 220a 2020  ion_date}'. ".  
+000109e0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000109f0: 4469 6420 796f 7520 7065 7268 6170 7320  Did you perhaps 
+00010a00: 666f 7267 6574 2074 6865 2074 696d 657a  forget the timez
+00010a10: 6f6e 653f 220a 2020 2020 2020 2020 2020  one?".          
+00010a20: 2020 2920 6672 6f6d 204e 6f6e 650a 2020    ) from None.  
+00010a30: 2020 2020 2020 6b77 6172 6773 5b22 6372        kwargs["cr
+00010a40: 6561 7469 6f6e 5f64 6174 6522 5d20 3d20  eation_date"] = 
+00010a50: 6372 6561 7469 6f6e 5f64 6174 650a 0a20  creation_date.. 
+00010a60: 2020 2072 6574 7572 6e20 6574 7265 652e     return etree.
+00010a70: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+00010a80: 2022 7b25 737d 6c69 6e6b 2220 2520 786d   "{%s}link" % xm
+00010a90: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
+00010aa0: 4e6f 6e65 5d2c 0a20 2020 2020 2020 202a  None],.        *
+00010ab0: 2a6b 7761 7267 732c 2020 2320 7479 7065  *kwargs,  # type
+00010ac0: 3a20 6967 6e6f 7265 5b61 7267 2d74 7970  : ignore[arg-typ
+00010ad0: 655d 0a20 2020 2029 0a0a 0a64 6566 2063  e].    )...def c
+00010ae0: 7265 6174 655f 6a73 6f6e 5f65 7863 656c  reate_json_excel
+00010af0: 5f6c 6973 745f 6d61 7070 696e 6728 0a20  _list_mapping(. 
+00010b00: 2020 2070 6174 685f 746f 5f6a 736f 6e3a     path_to_json:
+00010b10: 2073 7472 2c0a 2020 2020 6c69 7374 5f6e   str,.    list_n
+00010b20: 616d 653a 2073 7472 2c0a 2020 2020 6578  ame: str,.    ex
+00010b30: 6365 6c5f 7661 6c75 6573 3a20 4974 6572  cel_values: Iter
+00010b40: 6162 6c65 5b73 7472 5d2c 0a20 2020 2073  able[str],.    s
+00010b50: 6570 3a20 7374 7220 3d20 272b 222a c3a7  ep: str = '+"*..
+00010b60: 2526 2f28 293d 272c 0a20 2020 2063 6f72  %&/()=',.    cor
+00010b70: 7265 6374 696f 6e73 3a20 4f70 7469 6f6e  rections: Option
+00010b80: 616c 5b64 6963 745b 7374 722c 2073 7472  al[dict[str, str
+00010b90: 5d5d 203d 204e 6f6e 652c 0a29 202d 3e20  ]] = None,.) -> 
+00010ba0: 6469 6374 5b73 7472 2c20 7374 725d 3a0a  dict[str, str]:.
+00010bb0: 2020 2020 2222 220a 2020 2020 4f66 7465      """.    Ofte
+00010bc0: 6e2c 2064 6174 6120 736f 7572 6365 7320  n, data sources 
+00010bd0: 636f 6e74 6169 6e20 6c69 7374 2076 616c  contain list val
+00010be0: 7565 7320 7468 6174 2061 7265 6e27 7420  ues that aren't 
+00010bf0: 6964 656e 7469 6361 6c20 746f 2074 6865  identical to the
+00010c00: 206e 616d 6520 6f66 2074 6865 206e 6f64   name of the nod
+00010c10: 6520 696e 2074 6865 206c 6973 7420 6f66  e in the list of
+00010c20: 2074 6865 204a 534f 4e0a 2020 2020 7072   the JSON.    pr
+00010c30: 6f6a 6563 7420 6669 6c65 2028 636f 6c6c  oject file (coll
+00010c40: 6f71 7569 616c 6c79 3a20 6f6e 746f 6c6f  oquially: ontolo
+00010c50: 6779 292e 2049 6e20 6f72 6465 7220 746f  gy). In order to
+00010c60: 2063 7265 6174 6520 6120 636f 7272 6563   create a correc
+00010c70: 7420 584d 4c20 666f 7220 7468 6520 6064  t XML for the `d
+00010c80: 7370 2d74 6f6f 6c73 2078 6d6c 7570 6c6f  sp-tools xmluplo
+00010c90: 6164 602c 2061 206d 6170 7069 6e67 2069  ad`, a mapping i
+00010ca0: 730a 2020 2020 6e65 6365 7373 6172 792e  s.    necessary.
+00010cb0: 2054 6869 7320 6675 6e63 7469 6f6e 2074   This function t
+00010cc0: 616b 6573 2061 204a 534f 4e20 6c69 7374  akes a JSON list
+00010cd0: 2061 6e64 2061 6e20 4578 6365 6c20 636f   and an Excel co
+00010ce0: 6c75 6d6e 2063 6f6e 7461 696e 696e 6720  lumn containing 
+00010cf0: 6c69 7374 2d76 616c 7565 732c 2061 6e64  list-values, and
+00010d00: 2074 7269 6573 2074 6f20 6d61 7463 6820   tries to match 
+00010d10: 7468 656d 0a20 2020 2061 7574 6f6d 6174  them.    automat
+00010d20: 6963 616c 6c79 2062 6173 6564 206f 6e20  ically based on 
+00010d30: 7369 6d69 6c61 7269 7479 2e20 5468 6520  similarity. The 
+00010d40: 7265 7375 6c74 2069 7320 6120 6469 6374  result is a dict
+00010d50: 206f 6620 7468 6520 666f 726d 207b 6578   of the form {ex
+00010d60: 6365 6c5f 7661 6c75 653a 206c 6973 745f  cel_value: list_
+00010d70: 6e6f 6465 5f6e 616d 657d 2e0a 0a20 2020  node_name}...   
+00010d80: 2041 6c74 6572 6e61 7469 7665 6c79 2c20   Alternatively, 
+00010d90: 636f 6e73 6964 6572 2075 7369 6e67 2074  consider using t
+00010da0: 6865 2066 756e 6374 696f 6e20 6372 6561  he function crea
+00010db0: 7465 5f6a 736f 6e5f 6c69 7374 5f6d 6170  te_json_list_map
+00010dc0: 7069 6e67 2829 2c20 7768 6963 6820 616c  ping(), which al
+00010dd0: 736f 2062 7569 6c64 7320 6120 6469 6374  so builds a dict
+00010de0: 696f 6e61 7279 2c0a 2020 2020 6275 7420  ionary,.    but 
+00010df0: 6672 6f6d 2074 6865 206e 616d 6573 2061  from the names a
+00010e00: 6e64 206c 6162 656c 7320 696e 2074 6865  nd labels in the
+00010e10: 204a 534f 4e20 6c69 7374 2c20 7768 6963   JSON list, whic
+00010e20: 6820 6973 206c 6573 7320 6572 726f 722d  h is less error-
+00010e30: 7072 6f6e 6520 7468 616e 2074 6869 7320  prone than this 
+00010e40: 6675 6e63 7469 6f6e 2773 2061 7070 726f  function's appro
+00010e50: 6163 682e 2048 6f77 6576 6572 2c0a 2020  ach. However,.  
+00010e60: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+00010e70: 6861 7320 7468 6520 6164 7661 6e74 6167  has the advantag
+00010e80: 6520 7468 6174 2069 7420 6576 656e 2077  e that it even w
+00010e90: 6f72 6b73 2077 6865 6e20 796f 7572 2064  orks when your d
+00010ea0: 6174 6120 736f 7572 6365 2064 6f65 736e  ata source doesn
+00010eb0: 2774 2075 7365 2074 6865 206c 6973 7420  't use the list 
+00010ec0: 6c61 6265 6c73 2063 6f72 7265 6374 6c79  labels correctly
+00010ed0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00010ee0: 2020 2020 2070 6174 685f 746f 5f6a 736f       path_to_jso
+00010ef0: 6e3a 2070 6174 6820 746f 2074 6865 204a  n: path to the J
+00010f00: 534f 4e20 7072 6f6a 6563 7420 6669 6c65  SON project file
+00010f10: 0a20 2020 2020 2020 206c 6973 745f 6e61  .        list_na
+00010f20: 6d65 3a20 6e61 6d65 206f 6620 7468 6520  me: name of the 
+00010f30: 6c69 7374 2069 6e20 7468 6520 4a53 4f4e  list in the JSON
+00010f40: 2070 726f 6a65 6374 2066 696c 6520 2863   project file (c
+00010f50: 616e 2061 6c73 6f20 6265 2061 206e 6573  an also be a nes
+00010f60: 7465 6420 6c69 7374 290a 2020 2020 2020  ted list).      
+00010f70: 2020 6578 6365 6c5f 7661 6c75 6573 3a20    excel_values: 
+00010f80: 7468 6520 4578 6365 6c20 636f 6c75 6d6e  the Excel column
+00010f90: 2028 652e 672e 2061 7320 6c69 7374 2920   (e.g. as list) 
+00010fa0: 7769 7468 2074 6865 206c 6973 7420 7661  with the list va
+00010fb0: 6c75 6573 2069 6e20 6974 0a20 2020 2020  lues in it.     
+00010fc0: 2020 2073 6570 3a20 7365 7061 7261 746f     sep: separato
+00010fd0: 7220 7374 7269 6e67 2c20 6966 2074 6865  r string, if the
+00010fe0: 2063 656c 6c73 2069 6e20 7468 6520 4578   cells in the Ex
+00010ff0: 6365 6c20 636f 6e74 6169 6e20 6d6f 7265  cel contain more
+00011000: 2074 6861 6e20 6f6e 6520 6c69 7374 2065   than one list e
+00011010: 6e74 7279 0a20 2020 2020 2020 2063 6f72  ntry.        cor
+00011020: 7265 6374 696f 6e73 3a20 6469 6374 2077  rections: dict w
+00011030: 6974 6820 7772 6f6e 6720 656e 7472 6965  ith wrong entrie
+00011040: 732c 2065 6163 6820 706f 696e 7469 6e67  s, each pointing
+00011050: 2074 6f20 6974 7320 636f 7272 6563 7420   to its correct 
+00011060: 636f 756e 7465 7270 6172 740a 0a20 2020  counterpart..   
+00011070: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+00011080: 2057 6172 6e69 6e67 3a20 6966 2074 6865   Warning: if the
+00011090: 7265 2069 7320 616e 2045 7863 656c 2076  re is an Excel v
+000110a0: 616c 7565 2074 6861 7420 636f 756c 646e  alue that couldn
+000110b0: 2774 2062 6520 6d61 7463 6865 640a 2020  't be matched.  
+000110c0: 2020 2020 2020 4578 6365 7074 696f 6e3a        Exception:
+000110d0: 2069 6620 7468 6520 7061 7468 2064 6f65   if the path doe
+000110e0: 736e 2774 2070 6f69 6e74 2074 6f20 6120  sn't point to a 
+000110f0: 4a53 4f4e 2070 726f 6a65 6374 2066 696c  JSON project fil
+00011100: 650a 0a20 2020 2052 6574 7572 6e73 3a0a  e..    Returns:.
+00011110: 2020 2020 2020 2020 6469 6374 206f 6620          dict of 
+00011120: 7468 6520 666f 726d 2060 607b 6578 6365  the form ``{exce
+00011130: 6c5f 7661 6c75 653a 206c 6973 745f 6e6f  l_value: list_no
+00011140: 6465 5f6e 616d 657d 6060 2e0a 2020 2020  de_name}``..    
+00011150: 2020 2020 2020 2020 4576 6572 7920 6578          Every ex
+00011160: 6365 6c5f 7661 6c75 6520 6973 2073 7472  cel_value is str
+00011170: 6970 7065 642c 2061 6e64 2061 6c73 6f20  ipped, and also 
+00011180: 7072 6573 656e 7420 696e 2061 206c 6f77  present in a low
+00011190: 6572 6361 7365 2066 6f72 6d2e 0a0a 2020  ercase form...  
+000111a0: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+000111b0: 2020 2020 3e3e 3e20 6a73 6f6e 5f6c 6973      >>> json_lis
+000111c0: 745f 6e6f 6465 7320 3d20 5b0a 2020 2020  t_nodes = [.    
+000111d0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 2020 226e 616d 6522 3a20 2267 6972 6166    "name": "giraf
+00011200: 6665 222c 0a20 2020 2020 2020 2020 2020  fe",.           
+00011210: 2020 2020 2020 2020 2022 6c61 6265 6c73           "labels
+00011220: 223a 207b 2265 6e22 3a20 2267 6972 6166  ": {"en": "giraf
+00011230: 6665 227d 0a20 2020 2020 2020 2020 2020  fe"}.           
+00011240: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00011250: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00011260: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00011270: 616d 6522 3a20 2261 6e74 656c 6f70 6522  ame": "antelope"
+00011280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011290: 2020 2020 2020 226c 6162 656c 7322 3a20        "labels": 
+000112a0: 7b22 656e 223a 2022 616e 7465 6c6f 7065  {"en": "antelope
+000112b0: 227d 0a20 2020 2020 2020 2020 2020 2020  "}.             
+000112c0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000112d0: 205d 0a20 2020 2020 2020 203e 3e3e 2065   ].        >>> e
+000112e0: 7863 656c 5f72 6f77 5f31 203d 205b 2247  xcel_row_1 = ["G
+000112f0: 6972 6166 6665 6568 2022 2c20 2220 416e  iraffeeh ", " An
+00011300: 7469 6c6f 7570 6522 2c20 2247 6972 7261  tiloupe", "Girra
+00011310: 6666 6520 2c20 416e 7469 6c6f 7570 6520  ffe , Antiloupe 
+00011320: 225d 0a20 2020 2020 2020 203e 3e3e 206a  "].        >>> j
+00011330: 736f 6e5f 6578 6365 6c5f 6c69 7374 5f6d  son_excel_list_m
+00011340: 6170 7069 6e67 203d 207b 0a20 2020 2020  apping = {.     
+00011350: 2020 2020 2020 2020 2020 2022 4769 7261             "Gira
+00011360: 6666 6565 6822 3a20 2267 6972 6166 6665  ffeeh": "giraffe
+00011370: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00011380: 2020 2022 6769 7261 6666 6565 6822 3a20     "giraffeeh": 
+00011390: 2267 6972 6166 6665 222c 0a20 2020 2020  "giraffe",.     
+000113a0: 2020 2020 2020 2020 2020 2022 4769 7272             "Girr
+000113b0: 6166 6665 223a 2022 6769 7261 6666 6522  affe": "giraffe"
+000113c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000113d0: 2020 2267 6972 7261 6666 6522 3a20 2267    "girraffe": "g
+000113e0: 6972 6166 6665 222c 0a20 2020 2020 2020  iraffe",.       
+000113f0: 2020 2020 2020 2020 2022 416e 7469 6c6f           "Antilo
+00011400: 7570 6522 3a20 2261 6e74 656c 6f70 6522  upe": "antelope"
+00011410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011420: 2020 2261 6e74 696c 6f75 7065 223a 2022    "antiloupe": "
+00011430: 616e 7465 6c6f 7065 220a 2020 2020 2020  antelope".      
+00011440: 2020 2020 2020 7d0a 2020 2020 2222 220a        }.    """.
+00011450: 0a20 2020 2023 2061 766f 6964 206d 7574  .    # avoid mut
+00011460: 6162 6c65 2064 6566 6175 6c74 2061 7267  able default arg
+00011470: 756d 656e 740a 2020 2020 636f 7272 6563  ument.    correc
+00011480: 7469 6f6e 7320 3d20 636f 7272 6563 7469  tions = correcti
+00011490: 6f6e 7320 6f72 207b 7d0a 0a20 2020 2023  ons or {}..    #
+000114a0: 2073 706c 6974 2074 6865 2076 616c 7565   split the value
+000114b0: 732c 2069 6620 6e65 6365 7373 6172 790a  s, if necessary.
+000114c0: 2020 2020 6578 6365 6c5f 7661 6c75 6573      excel_values
+000114d0: 5f6e 6577 203d 205b 5d0a 2020 2020 666f  _new = [].    fo
+000114e0: 7220 7661 6c20 696e 2065 7863 656c 5f76  r val in excel_v
+000114f0: 616c 7565 733a 0a20 2020 2020 2020 2069  alues:.        i
+00011500: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
+00011510: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00011520: 2020 2020 6578 6365 6c5f 7661 6c75 6573      excel_values
+00011530: 5f6e 6577 2e65 7874 656e 6428 5b78 2e73  _new.extend([x.s
+00011540: 7472 6970 2829 2066 6f72 2078 2069 6e20  trip() for x in 
+00011550: 7661 6c2e 7370 6c69 7428 7365 7029 2069  val.split(sep) i
+00011560: 6620 785d 290a 0a20 2020 2023 2072 6561  f x])..    # rea
+00011570: 6420 7468 6520 6c69 7374 206f 6620 7468  d the list of th
+00011580: 6520 4a53 4f4e 2070 726f 6a65 6374 2028  e JSON project (
+00011590: 776f 726b 7320 616c 736f 2066 6f72 206e  works also for n
+000115a0: 6573 7465 6420 6c69 7374 7329 0a20 2020  ested lists).   
+000115b0: 2077 6974 6820 6f70 656e 2870 6174 685f   with open(path_
+000115c0: 746f 5f6a 736f 6e2c 2065 6e63 6f64 696e  to_json, encodin
+000115d0: 673d 2275 7466 2d38 2229 2061 7320 663a  g="utf-8") as f:
+000115e0: 0a20 2020 2020 2020 206a 736f 6e5f 6669  .        json_fi
+000115f0: 6c65 203d 206a 736f 6e2e 6c6f 6164 2866  le = json.load(f
+00011600: 290a 2020 2020 6a73 6f6e 5f73 7562 7365  ).    json_subse
+00011610: 7420 3d20 5b5d 0a20 2020 2066 6f72 2065  t = [].    for e
+00011620: 6c65 6d20 696e 206a 736f 6e5f 6669 6c65  lem in json_file
+00011630: 5b22 7072 6f6a 6563 7422 5d5b 226c 6973  ["project"]["lis
+00011640: 7473 225d 3a0a 2020 2020 2020 2020 6966  ts"]:.        if
+00011650: 2065 6c65 6d5b 226e 616d 6522 5d20 3d3d   elem["name"] ==
+00011660: 206c 6973 745f 6e61 6d65 3a0a 2020 2020   list_name:.    
+00011670: 2020 2020 2020 2020 6a73 6f6e 5f73 7562          json_sub
+00011680: 7365 7420 3d20 656c 656d 5b22 6e6f 6465  set = elem["node
+00011690: 7322 5d0a 2020 2020 6a73 6f6e 5f76 616c  s"].    json_val
+000116a0: 7565 7320 3d20 7365 7428 5f6e 6573 7465  ues = set(_neste
+000116b0: 645f 6469 6374 5f76 616c 7565 735f 6974  d_dict_values_it
+000116c0: 6572 6174 6f72 286a 736f 6e5f 7375 6273  erator(json_subs
+000116d0: 6574 2929 0a0a 2020 2020 2320 6275 696c  et))..    # buil
+000116e0: 6420 6469 6374 696f 6e61 7279 2077 6974  d dictionary wit
+000116f0: 6820 7468 6520 6d61 7070 696e 672c 2062  h the mapping, b
+00011700: 6173 6564 206f 6e20 7374 7269 6e67 2073  ased on string s
+00011710: 696d 696c 6172 6974 790a 2020 2020 7265  imilarity.    re
+00011720: 7320 3d20 7b7d 0a20 2020 2066 6f72 2065  s = {}.    for e
+00011730: 7863 656c 5f76 616c 7565 2069 6e20 6578  xcel_value in ex
+00011740: 6365 6c5f 7661 6c75 6573 5f6e 6577 3a0a  cel_values_new:.
+00011750: 2020 2020 2020 2020 6578 6365 6c5f 7661          excel_va
+00011760: 6c75 655f 636f 7272 6563 7465 6420 3d20  lue_corrected = 
+00011770: 636f 7272 6563 7469 6f6e 732e 6765 7428  corrections.get(
+00011780: 6578 6365 6c5f 7661 6c75 652c 2065 7863  excel_value, exc
+00011790: 656c 5f76 616c 7565 290a 2020 2020 2020  el_value).      
+000117a0: 2020 6578 6365 6c5f 7661 6c75 655f 7369    excel_value_si
+000117b0: 6d70 6c20 3d20 7369 6d70 6c69 6679 5f6e  mpl = simplify_n
+000117c0: 616d 6528 6578 6365 6c5f 7661 6c75 655f  ame(excel_value_
+000117d0: 636f 7272 6563 7465 6429 2020 2320 696e  corrected)  # in
+000117e0: 6372 6561 7365 206d 6174 6368 2070 726f  crease match pro
+000117f0: 6261 6269 6c69 7479 2062 7920 7265 6d6f  bability by remo
+00011800: 7669 6e67 2069 6c6c 6567 616c 2063 6861  ving illegal cha
+00011810: 7273 0a20 2020 2020 2020 2069 6620 6d61  rs.        if ma
+00011820: 7463 6865 7320 3a3d 2064 6966 666c 6962  tches := difflib
+00011830: 2e67 6574 5f63 6c6f 7365 5f6d 6174 6368  .get_close_match
+00011840: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
+00011850: 776f 7264 3d65 7863 656c 5f76 616c 7565  word=excel_value
+00011860: 5f73 696d 706c 2c0a 2020 2020 2020 2020  _simpl,.        
+00011870: 2020 2020 706f 7373 6962 696c 6974 6965      possibilitie
+00011880: 733d 6a73 6f6e 5f76 616c 7565 732c 0a20  s=json_values,. 
+00011890: 2020 2020 2020 2020 2020 206e 3d31 2c0a             n=1,.
+000118a0: 2020 2020 2020 2020 2020 2020 6375 746f              cuto
+000118b0: 6666 3d30 2e36 2c0a 2020 2020 2020 2020  ff=0.6,.        
+000118c0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000118d0: 6573 5b65 7863 656c 5f76 616c 7565 5d20  es[excel_value] 
+000118e0: 3d20 6d61 7463 6865 735b 305d 0a20 2020  = matches[0].   
+000118f0: 2020 2020 2020 2020 2072 6573 5b65 7863           res[exc
+00011900: 656c 5f76 616c 7565 2e6c 6f77 6572 2829  el_value.lower()
+00011910: 5d20 3d20 6d61 7463 6865 735b 305d 0a20  ] = matches[0]. 
+00011920: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00011930: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00011940: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00011950: 2020 2020 2020 2020 6622 4469 6420 6e6f          f"Did no
+00011960: 7420 6669 6e64 2061 2063 6c6f 7365 206d  t find a close m
+00011970: 6174 6368 2074 6f20 7468 6520 6578 6365  atch to the exce
+00011980: 6c20 6c69 7374 2065 6e74 7279 2027 7b65  l list entry '{e
+00011990: 7863 656c 5f76 616c 7565 7d27 2022 0a20  xcel_value}' ". 
+000119a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000119b0: 2261 6d6f 6e67 2074 6865 2076 616c 7565  "among the value
+000119c0: 7320 696e 2074 6865 204a 534f 4e20 7072  s in the JSON pr
+000119d0: 6f6a 6563 7420 6c69 7374 2027 7b6c 6973  oject list '{lis
+000119e0: 745f 6e61 6d65 7d27 222c 0a20 2020 2020  t_name}'",.     
+000119f0: 2020 2020 2020 2020 2020 2073 7461 636b             stack
+00011a00: 6c65 7665 6c3d 322c 0a20 2020 2020 2020  level=2,.       
+00011a10: 2020 2020 2029 0a0a 2020 2020 7265 7475       )..    retu
+00011a20: 726e 2072 6573 0a0a 0a64 6566 205f 6e65  rn res...def _ne
+00011a30: 7374 6564 5f64 6963 745f 7661 6c75 6573  sted_dict_values
+00011a40: 5f69 7465 7261 746f 7228 6469 6374 733a  _iterator(dicts:
+00011a50: 206c 6973 745b 6469 6374 5b73 7472 2c20   list[dict[str, 
+00011a60: 416e 795d 5d29 202d 3e20 4974 6572 6162  Any]]) -> Iterab
+00011a70: 6c65 5b73 7472 5d3a 0a20 2020 2022 2222  le[str]:.    """
+00011a80: 0a20 2020 2059 6965 6c64 2061 6c6c 2076  .    Yield all v
+00011a90: 616c 7565 7320 6f66 2061 206e 6573 7465  alues of a neste
+00011aa0: 6420 6469 6374 696f 6e61 7279 2e0a 0a20  d dictionary... 
+00011ab0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00011ac0: 2064 6963 7473 3a20 6c69 7374 206f 6620   dicts: list of 
+00011ad0: 6e65 7374 6564 2064 6963 7469 6f6e 6172  nested dictionar
+00011ae0: 6965 730a 0a20 2020 2059 6965 6c64 733a  ies..    Yields:
+00011af0: 0a20 2020 2020 2020 2076 616c 7565 7320  .        values 
+00011b00: 6f66 2074 6865 206e 6573 7465 6420 6469  of the nested di
+00011b10: 6374 696f 6e61 7269 6573 0a20 2020 2022  ctionaries.    "
+00011b20: 2222 0a20 2020 2023 2043 7265 6469 7473  "".    # Credits
+00011b30: 3a20 6874 7470 733a 2f2f 7468 6973 706f  : https://thispo
+00011b40: 696e 7465 722e 636f 6d2f 7079 7468 6f6e  inter.com/python
+00011b50: 2d69 7465 7261 7465 2d6c 6f6f 702d 6f76  -iterate-loop-ov
+00011b60: 6572 2d61 6c6c 2d6e 6573 7465 642d 6469  er-all-nested-di
+00011b70: 6374 696f 6e61 7279 2d76 616c 7565 732f  ctionary-values/
+00011b80: 0a20 2020 2066 6f72 205f 6469 6374 2069  .    for _dict i
+00011b90: 6e20 6469 6374 733a 0a20 2020 2020 2020  n dicts:.       
+00011ba0: 2069 6620 226e 6f64 6573 2220 696e 205f   if "nodes" in _
+00011bb0: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
+00011bc0: 2020 7969 656c 6420 6672 6f6d 205f 6e65    yield from _ne
+00011bd0: 7374 6564 5f64 6963 745f 7661 6c75 6573  sted_dict_values
+00011be0: 5f69 7465 7261 746f 7228 5f64 6963 745b  _iterator(_dict[
+00011bf0: 226e 6f64 6573 225d 290a 2020 2020 2020  "nodes"]).      
+00011c00: 2020 6966 2022 6e61 6d65 2220 696e 205f    if "name" in _
+00011c10: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
+00011c20: 2020 7969 656c 6420 5f64 6963 745b 226e    yield _dict["n
+00011c30: 616d 6522 5d0a 0a0a 6465 6620 6372 6561  ame"]...def crea
+00011c40: 7465 5f6a 736f 6e5f 6c69 7374 5f6d 6170  te_json_list_map
+00011c50: 7069 6e67 280a 2020 2020 7061 7468 5f74  ping(.    path_t
+00011c60: 6f5f 6a73 6f6e 3a20 7374 722c 0a20 2020  o_json: str,.   
+00011c70: 206c 6973 745f 6e61 6d65 3a20 7374 722c   list_name: str,
+00011c80: 0a20 2020 206c 616e 6775 6167 655f 6c61  .    language_la
+00011c90: 6265 6c3a 2073 7472 2c0a 2920 2d3e 2064  bel: str,.) -> d
+00011ca0: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
+00011cb0: 2020 2022 2222 0a20 2020 204f 6674 656e     """.    Often
+00011cc0: 2c20 6461 7461 2073 6f75 7263 6573 2063  , data sources c
+00011cd0: 6f6e 7461 696e 206c 6973 7420 7661 6c75  ontain list valu
+00011ce0: 6573 206e 616d 6564 2061 6674 6572 2074  es named after t
+00011cf0: 6865 2022 6c61 6265 6c22 206f 6620 7468  he "label" of th
+00011d00: 6520 4a53 4f4e 2070 726f 6a65 6374 206c  e JSON project l
+00011d10: 6973 7420 6e6f 6465 2c20 696e 7374 6561  ist node, instea
+00011d20: 6420 6f66 2074 6865 2022 6e61 6d65 220a  d of the "name".
+00011d30: 2020 2020 7768 6963 6820 6973 206e 6565      which is nee
+00011d40: 6465 6420 666f 7220 7468 6520 6064 7370  ded for the `dsp
+00011d50: 2d74 6f6f 6c73 2078 6d6c 7570 6c6f 6164  -tools xmlupload
+00011d60: 602e 2049 6e20 6f72 6465 7220 746f 2063  `. In order to c
+00011d70: 7265 6174 6520 6120 636f 7272 6563 7420  reate a correct 
+00011d80: 584d 4c2c 2079 6f75 206e 6565 6420 6120  XML, you need a 
+00011d90: 6469 6374 696f 6e61 7279 2074 6861 7420  dictionary that 
+00011da0: 6d61 7073 2074 6865 0a20 2020 2022 6c61  maps the.    "la
+00011db0: 6265 6c73 2220 746f 2074 6865 6972 2063  bels" to their c
+00011dc0: 6f72 7265 6374 2022 6e61 6d65 7322 2e0a  orrect "names"..
+00011dd0: 0a20 2020 2041 6c74 6572 6e61 7469 7665  .    Alternative
+00011de0: 6c79 2c20 636f 6e73 6964 6572 2075 7369  ly, consider usi
+00011df0: 6e67 2074 6865 206d 6574 686f 6420 6372  ng the method cr
+00011e00: 6561 7465 5f6a 736f 6e5f 6578 6365 6c5f  eate_json_excel_
+00011e10: 6c69 7374 5f6d 6170 7069 6e67 2829 2c20  list_mapping(), 
+00011e20: 7768 6963 6820 616c 736f 2063 7265 6174  which also creat
+00011e30: 6573 2061 2064 6963 7469 6f6e 6172 792c  es a dictionary,
+00011e40: 2062 7574 206d 6170 730a 2020 2020 7661   but maps.    va
+00011e50: 6c75 6573 2066 726f 6d20 796f 7572 2064  lues from your d
+00011e60: 6174 6120 736f 7572 6365 2074 6f20 6c69  ata source to li
+00011e70: 7374 206e 6f64 6520 6e61 6d65 7320 6672  st node names fr
+00011e80: 6f6d 2074 6865 204a 534f 4e20 7072 6f6a  om the JSON proj
+00011e90: 6563 7420 6669 6c65 2c20 6261 7365 6420  ect file, based 
+00011ea0: 6f6e 2073 696d 696c 6172 6974 792e 0a0a  on similarity...
+00011eb0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00011ec0: 2020 7061 7468 5f74 6f5f 6a73 6f6e 3a20    path_to_json: 
+00011ed0: 7061 7468 2074 6f20 6120 4a53 4f4e 2070  path to a JSON p
+00011ee0: 726f 6a65 6374 2066 696c 6520 2861 2e6b  roject file (a.k
+00011ef0: 2e61 2e20 6f6e 746f 6c6f 6779 290a 2020  .a. ontology).  
+00011f00: 2020 2020 2020 6c69 7374 5f6e 616d 653a        list_name:
+00011f10: 206e 616d 6520 6f66 2061 206c 6973 7420   name of a list 
+00011f20: 696e 2074 6865 204a 534f 4e20 7072 6f6a  in the JSON proj
+00011f30: 6563 7420 2877 6f72 6b73 2061 6c73 6f20  ect (works also 
+00011f40: 666f 7220 6e65 7374 6564 206c 6973 7473  for nested lists
+00011f50: 290a 2020 2020 2020 2020 6c61 6e67 7561  ).        langua
+00011f60: 6765 5f6c 6162 656c 3a20 7768 6963 6820  ge_label: which 
+00011f70: 6c61 6e67 7561 6765 206f 6620 7468 6520  language of the 
+00011f80: 6c61 6265 6c20 746f 2063 686f 6f73 650a  label to choose.
+00011f90: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00011fa0: 2020 2020 2020 6120 6469 6374 696f 6e61        a dictiona
+00011fb0: 7279 206f 6620 7468 6520 666f 726d 207b  ry of the form {
+00011fc0: 6c61 6265 6c3a 206e 616d 657d 0a20 2020  label: name}.   
+00011fd0: 2022 2222 0a20 2020 2077 6974 6820 6f70   """.    with op
+00011fe0: 656e 2870 6174 685f 746f 5f6a 736f 6e2c  en(path_to_json,
+00011ff0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00012000: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00012010: 206a 736f 6e5f 6669 6c65 203d 206a 736f   json_file = jso
+00012020: 6e2e 6c6f 6164 2866 290a 2020 2020 6a73  n.load(f).    js
+00012030: 6f6e 5f73 7562 7365 7420 3d20 5b78 2066  on_subset = [x f
+00012040: 6f72 2078 2069 6e20 6a73 6f6e 5f66 696c  or x in json_fil
+00012050: 655b 2270 726f 6a65 6374 225d 5b22 6c69  e["project"]["li
+00012060: 7374 7322 5d20 6966 2078 5b22 6e61 6d65  sts"] if x["name
+00012070: 225d 203d 3d20 6c69 7374 5f6e 616d 655d  "] == list_name]
+00012080: 0a20 2020 2023 206a 736f 6e5f 7375 6273  .    # json_subs
+00012090: 6574 2069 7320 6120 6c69 7374 2063 6f6e  et is a list con
+000120a0: 7461 696e 696e 6720 6f6e 6520 6974 656d  taining one item
+000120b0: 2c20 6e61 6d65 6c79 2074 6865 206a 736f  , namely the jso
+000120c0: 6e20 6f62 6a65 6374 2063 6f6e 7461 696e  n object contain
+000120d0: 696e 6720 7468 6520 656e 7469 7265 206a  ing the entire j
+000120e0: 736f 6e2d 6c69 7374 0a0a 2020 2020 7265  son-list..    re
+000120f0: 7320 3d20 7b7d 0a20 2020 2066 6f72 206c  s = {}.    for l
+00012100: 6162 656c 2c20 6e61 6d65 2069 6e20 5f6e  abel, name in _n
+00012110: 616d 655f 6c61 6265 6c5f 6d61 7070 6572  ame_label_mapper
+00012120: 5f69 7465 7261 746f 7228 6a73 6f6e 5f73  _iterator(json_s
+00012130: 7562 7365 742c 206c 616e 6775 6167 655f  ubset, language_
+00012140: 6c61 6265 6c29 3a0a 2020 2020 2020 2020  label):.        
+00012150: 6966 206e 616d 6520 213d 206c 6973 745f  if name != list_
+00012160: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+00012170: 2020 7265 735b 6c61 6265 6c5d 203d 206e    res[label] = n
+00012180: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+00012190: 7265 735b 6c61 6265 6c2e 7374 7269 7028  res[label.strip(
+000121a0: 292e 6c6f 7765 7228 295d 203d 206e 616d  ).lower()] = nam
+000121b0: 650a 0a20 2020 2072 6574 7572 6e20 7265  e..    return re
+000121c0: 730a 0a0a 6465 6620 5f6e 616d 655f 6c61  s...def _name_la
+000121d0: 6265 6c5f 6d61 7070 6572 5f69 7465 7261  bel_mapper_itera
+000121e0: 746f 7228 0a20 2020 206a 736f 6e5f 7375  tor(.    json_su
+000121f0: 6273 6574 3a20 6c69 7374 5b64 6963 745b  bset: list[dict[
+00012200: 7374 722c 2041 6e79 5d5d 2c0a 2020 2020  str, Any]],.    
+00012210: 6c61 6e67 7561 6765 5f6c 6162 656c 3a20  language_label: 
+00012220: 7374 722c 0a29 202d 3e20 4974 6572 6162  str,.) -> Iterab
+00012230: 6c65 5b74 7570 6c65 5b73 7472 2c20 7374  le[tuple[str, st
+00012240: 725d 5d3a 0a20 2020 2022 2222 0a20 2020  r]]:.    """.   
+00012250: 2047 6f20 7468 726f 7567 6820 6c69 7374   Go through list
+00012260: 206e 6f64 6573 206f 6620 6120 4a53 4f4e   nodes of a JSON
+00012270: 2070 726f 6a65 6374 2061 6e64 2079 6965   project and yie
+00012280: 6c64 2028 6c61 6265 6c2c 206e 616d 6529  ld (label, name)
+00012290: 2070 6169 7273 2e0a 0a20 2020 2041 7267   pairs...    Arg
+000122a0: 733a 0a20 2020 2020 2020 206a 736f 6e5f  s:.        json_
+000122b0: 7375 6273 6574 3a20 6c69 7374 206f 6620  subset: list of 
+000122c0: 4453 5020 6c69 7374 7320 2861 2044 5350  DSP lists (a DSP
+000122d0: 206c 6973 7420 6265 696e 6720 6120 6469   list being a di
+000122e0: 6374 696f 6e61 7279 2077 6974 6820 7468  ctionary with th
+000122f0: 6520 6b65 7973 2022 6e61 6d65 222c 2022  e keys "name", "
+00012300: 6c61 6265 6c73 2220 616e 6420 226e 6f64  labels" and "nod
+00012310: 6573 2229 0a20 2020 2020 2020 206c 616e  es").        lan
+00012320: 6775 6167 655f 6c61 6265 6c3a 2077 6869  guage_label: whi
+00012330: 6368 206c 616e 6775 6167 6520 6f66 2074  ch language of t
+00012340: 6865 206c 6162 656c 2074 6f20 6368 6f6f  he label to choo
+00012350: 7365 0a0a 2020 2020 5969 656c 6473 3a0a  se..    Yields:.
+00012360: 2020 2020 2020 2020 286c 6162 656c 2c20          (label, 
+00012370: 6e61 6d65 2920 7061 6972 730a 2020 2020  name) pairs.    
+00012380: 2222 220a 2020 2020 666f 7220 6e6f 6465  """.    for node
+00012390: 2069 6e20 6a73 6f6e 5f73 7562 7365 743a   in json_subset:
+000123a0: 0a20 2020 2020 2020 2023 206e 6f64 6520  .        # node 
+000123b0: 6973 2074 6865 206a 736f 6e20 6f62 6a65  is the json obje
+000123c0: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
+000123d0: 6520 656e 7469 7265 206a 736f 6e2d 6c69  e entire json-li
+000123e0: 7374 0a20 2020 2020 2020 2069 6620 226e  st.        if "n
+000123f0: 6f64 6573 2220 696e 206e 6f64 653a 0a20  odes" in node:. 
+00012400: 2020 2020 2020 2020 2020 2023 2022 6e6f             # "no
+00012410: 6465 7322 2069 7320 7468 6520 6a73 6f6e  des" is the json
+00012420: 2073 7562 2d6f 626a 6563 7420 636f 6e74   sub-object cont
+00012430: 6169 6e69 6e67 2074 6865 2065 6e74 7269  aining the entri
+00012440: 6573 206f 6620 7468 6520 6a73 6f6e 2d6c  es of the json-l
+00012450: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+00012460: 7969 656c 6420 6672 6f6d 205f 6e61 6d65  yield from _name
+00012470: 5f6c 6162 656c 5f6d 6170 7065 725f 6974  _label_mapper_it
+00012480: 6572 6174 6f72 286e 6f64 655b 226e 6f64  erator(node["nod
+00012490: 6573 225d 2c20 6c61 6e67 7561 6765 5f6c  es"], language_l
+000124a0: 6162 656c 290a 2020 2020 2020 2020 2020  abel).          
+000124b0: 2020 2320 6561 6368 2079 6965 6c64 6564    # each yielded
+000124c0: 2076 616c 7565 2069 7320 6120 286c 6162   value is a (lab
+000124d0: 656c 2c20 6e61 6d65 2920 7061 6972 206f  el, name) pair o
+000124e0: 6620 6120 7369 6e67 6c65 206c 6973 7420  f a single list 
+000124f0: 656e 7472 790a 2020 2020 2020 2020 6966  entry.        if
+00012500: 2022 6e61 6d65 2220 696e 206e 6f64 653a   "name" in node:
+00012510: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
+00012520: 6c64 2028 6e6f 6465 5b22 6c61 6265 6c73  ld (node["labels
+00012530: 225d 5b6c 616e 6775 6167 655f 6c61 6265  "][language_labe
+00012540: 6c5d 2c20 6e6f 6465 5b22 6e61 6d65 225d  l], node["name"]
+00012550: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00012560: 7468 6520 6163 7475 616c 2076 616c 7565  the actual value
+00012570: 7320 6f66 2074 6865 206e 616d 6520 616e  s of the name an
+00012580: 6420 7468 6520 6c61 6265 6c0a 0a0a 6465  d the label...de
+00012590: 6620 7772 6974 655f 786d 6c28 0a20 2020  f write_xml(.   
+000125a0: 2072 6f6f 743a 2065 7472 6565 2e5f 456c   root: etree._El
+000125b0: 656d 656e 742c 0a20 2020 2066 696c 6570  ement,.    filep
+000125c0: 6174 683a 2073 7472 207c 2050 6174 682c  ath: str | Path,
+000125d0: 0a29 202d 3e20 4e6f 6e65 3a0a 2020 2020  .) -> None:.    
+000125e0: 2222 220a 2020 2020 5772 6974 6520 7468  """.    Write th
+000125f0: 6520 6669 6e69 7368 6564 2058 4d4c 2074  e finished XML t
+00012600: 6f20 6120 6669 6c65 2e0a 0a20 2020 2041  o a file...    A
+00012610: 7267 733a 0a20 2020 2020 2020 2072 6f6f  rgs:.        roo
+00012620: 743a 2065 7472 6565 2045 6c65 6d65 6e74  t: etree Element
+00012630: 2077 6974 6820 7468 6520 656e 7469 7265   with the entire
+00012640: 2058 4d4c 2064 6f63 756d 656e 740a 2020   XML document.  
+00012650: 2020 2020 2020 6669 6c65 7061 7468 3a20        filepath: 
+00012660: 7768 6572 6520 746f 2073 6176 6520 7468  where to save th
+00012670: 6520 6669 6c65 0a0a 2020 2020 5761 726e  e file..    Warn
+00012680: 696e 673a 0a20 2020 2020 2020 2069 6620  ing:.        if 
+00012690: 7468 6520 584d 4c20 6973 206e 6f74 2076  the XML is not v
+000126a0: 616c 6964 2061 6363 6f72 6469 6e67 2074  alid according t
+000126b0: 6f20 7468 6520 7363 6865 6d61 0a20 2020  o the schema.   
+000126c0: 2022 2222 0a20 2020 2065 7472 6565 2e69   """.    etree.i
+000126d0: 6e64 656e 7428 726f 6f74 2c20 7370 6163  ndent(root, spac
+000126e0: 653d 2220 2020 2022 290a 2020 2020 786d  e="    ").    xm
+000126f0: 6c5f 7374 7269 6e67 203d 2065 7472 6565  l_string = etree
+00012700: 2e74 6f73 7472 696e 6728 0a20 2020 2020  .tostring(.     
+00012710: 2020 2072 6f6f 742c 0a20 2020 2020 2020     root,.       
+00012720: 2065 6e63 6f64 696e 673d 2275 6e69 636f   encoding="unico
+00012730: 6465 222c 0a20 2020 2020 2020 2070 7265  de",.        pre
+00012740: 7474 795f 7072 696e 743d 5472 7565 2c0a  tty_print=True,.
+00012750: 2020 2020 2020 2020 646f 6374 7970 653d          doctype=
+00012760: 273c 3f78 6d6c 2076 6572 7369 6f6e 3d22  '<?xml version="
+00012770: 312e 3022 2065 6e63 6f64 696e 673d 2255  1.0" encoding="U
+00012780: 5446 2d38 223f 3e27 2c0a 2020 2020 290a  TF-8"?>',.    ).
+00012790: 2020 2020 786d 6c5f 7374 7269 6e67 203d      xml_string =
+000127a0: 2078 6d6c 5f73 7472 696e 672e 7265 706c   xml_string.repl
+000127b0: 6163 6528 7222 5c27 222c 2022 2722 290a  ace(r"\'", "'").
+000127c0: 2020 2020 7769 7468 206f 7065 6e28 6669      with open(fi
+000127d0: 6c65 7061 7468 2c20 2277 222c 2065 6e63  lepath, "w", enc
+000127e0: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+000127f0: 7320 663a 0a20 2020 2020 2020 2066 2e77  s f:.        f.w
+00012800: 7269 7465 2878 6d6c 5f73 7472 696e 6729  rite(xml_string)
+00012810: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+00012820: 2020 7661 6c69 6461 7465 5f78 6d6c 2869    validate_xml(i
+00012830: 6e70 7574 5f66 696c 653d 6669 6c65 7061  nput_file=filepa
+00012840: 7468 290a 2020 2020 2020 2020 7072 696e  th).        prin
+00012850: 7428 6622 5468 6520 584d 4c20 6669 6c65  t(f"The XML file
+00012860: 2077 6173 2073 7563 6365 7373 6675 6c6c   was successfull
+00012870: 7920 7361 7665 6420 746f 207b 6669 6c65  y saved to {file
+00012880: 7061 7468 7d22 290a 2020 2020 6578 6365  path}").    exce
+00012890: 7074 2042 6173 6545 7272 6f72 2061 7320  pt BaseError as 
+000128a0: 6572 723a 0a20 2020 2020 2020 2077 6172  err:.        war
+000128b0: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
+000128c0: 2020 2020 2020 2020 6622 5468 6520 584d          f"The XM
+000128d0: 4c20 6669 6c65 2077 6173 2073 7563 6365  L file was succe
+000128e0: 7373 6675 6c6c 7920 7361 7665 6420 746f  ssfully saved to
+000128f0: 207b 6669 6c65 7061 7468 7d2c 2022 0a20   {filepath}, ". 
+00012900: 2020 2020 2020 2020 2020 2066 2262 7574             f"but
+00012910: 2074 6865 2066 6f6c 6c6f 7769 6e67 2053   the following S
+00012920: 6368 656d 6120 7661 6c69 6461 7469 6f6e  chema validation
+00012930: 2065 7272 6f72 2873 2920 6f63 6375 7272   error(s) occurr
+00012940: 6564 3a20 7b65 7272 2e6d 6573 7361 6765  ed: {err.message
+00012950: 7d22 0a20 2020 2020 2020 2029 0a         }".        ).
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import importlib.resources
 import json
+import warnings
 from pathlib import Path
 from typing import Any
 from typing import Union
 
 import jsonpath_ng
 import jsonpath_ng.ext
 import jsonschema
 import networkx as nx
 import regex
 
 from dsp_tools.commands.excel2json.lists import expand_lists_from_excel
+from dsp_tools.models.custom_warnings import DspToolsFutureWarning
 from dsp_tools.models.exceptions import BaseError
 
 
 def _check_for_duplicate_names(project_definition: dict[str, Any]) -> bool:
     """
     Check that the resource names and property names are unique.
 
@@ -205,14 +207,45 @@
         err_msg = "Your data model contains cardinalities with invalid propnames:\n" + "\n".join(
             f" - {loc}: {invalids}" for loc, invalids in errors.items()
         )
         raise BaseError(err_msg)
     return True
 
 
+def _check_for_deprecated_syntax(project_definition: dict[str, Any]) -> bool:
+    return _check_for_deprecated_isSequenceOf(project_definition)
+
+
+def _check_for_deprecated_isSequenceOf(project_definition: dict[str, Any]) -> bool:
+    ontos = project_definition["project"]["ontologies"]
+    isSequenceOf_matches = []
+    for index in range(len(ontos)):
+        pth = f"$.project.ontologies[{index}].properties[?super[*] == isSequenceOf]"
+        isSequenceOf_matches.extend(jsonpath_ng.ext.parse(pth).find(project_definition))
+
+    hasSequenceBounds_matches = []
+    for index in range(len(ontos)):
+        pth = f"$.project.ontologies[{index}].properties[?super[*] == hasSequenceBounds]"
+        hasSequenceBounds_matches.extend(jsonpath_ng.ext.parse(pth).find(project_definition))
+
+    sequence_resource_matches = []
+    for index in range(len(ontos)):
+        pth = f"$.project.ontologies[{index}].resources[?cardinalities.propname == isSequenceOf]"
+        sequence_resource_matches.extend(jsonpath_ng.ext.parse(pth).find(project_definition))
+
+    if any([isSequenceOf_matches, hasSequenceBounds_matches, sequence_resource_matches]):
+        msg = (
+            "Deprecation Warning: Your JSON project definition contains deprecated properties. "
+            "Support for the following properties will be removed soon: isSequenceOf, hasSequenceBounds"
+        )
+        warnings.warn(DspToolsFutureWarning(msg))
+
+    return True
+
+
 def validate_project(
     input_file_or_json: Union[dict[str, Any], str],
     expand_lists: bool = True,
 ) -> bool:
     """
     Validates a JSON project definition file.
 
@@ -276,14 +309,15 @@
         ) from None
 
     # make some checks that are too complex for JSON schema
     _check_for_undefined_super_property(project_definition)
     _check_for_undefined_super_resource(project_definition)
     _check_for_undefined_cardinalities(project_definition)
     _check_for_duplicate_names(project_definition)
+    _check_for_deprecated_syntax(project_definition)
 
     # cardinalities check for circular references
     return _check_cardinalities_of_circular_references(project_definition)
 
 
 def _check_cardinalities_of_circular_references(project_definition: dict[Any, Any]) -> bool:
     """
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/template.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlallow.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlpermission.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlproperty.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlresource.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/models/xmlvalue.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.1.3/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.1.3/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.1.3/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/models/langstring.py` & `dsp_tools-7.1.3/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.1.3/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.1.3/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.1.3/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/data.xsd`

 * *Files 1% similar despite different names*

#### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/data.xsd`

```diff
@@ -36,15 +36,15 @@
     <xs:restriction base="xs:token">
       <xs:pattern value="#([0-9a-fA-F]{3}){1,2}"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- data type for knora uri -->
   <xs:simpleType name="knorauri_type">
     <xs:restriction base="xs:string">
-      <xs:pattern value="([a-z][a-z0-9+.\-]*):(//([\w_.\-~:\[\]]+)(:\d{0,6})?)(/[\w_.\-~:%()]*)*(\?[\w_.,;/\-:%=*&amp;]+)*(#[\w_.\-~:/]*)?"/>
+      <xs:pattern value="([a-z][a-z0-9+.\-]*):(//([\w_.\-~:\[\]]+)(:\d{0,6})?)(/[\w_.\-~:%()]*)*(\?[\w_.,;/\-:%=*&amp;]+)*(#[\w_.\-,~:/]*)?"/>
     </xs:restriction>
   </xs:simpleType>
   <!-- data type for knora interval -->
   <xs:simpleType name="knorainterval_type">
     <xs:restriction base="xs:token">
       <xs:pattern value="([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+)):([+-]?([0-9]+([.][0-9]*)?|[.][0-9]+))"/>
     </xs:restriction>
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.1.3/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.1.3/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 ---
 
-version: "3.7"
-
 services:
 
   api:
     # on the verge of every deployment (fortnightly), update the "image" value from the "api" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/knora-api:v30.11.0
+    image: daschswiss/knora-api:v30.12.0
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
@@ -31,15 +29,15 @@
       - KNORA_WEBAPI_ALLOW_RELOAD_OVER_HTTP=true
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
       - DSP_API_LOG_LEVEL=INFO
 
   sipi:
     # on the verge of every deployment (fortnightly), take the same tag as DSP-API
-    image: daschswiss/knora-sipi:v30.11.0
+    image: daschswiss/knora-sipi:v30.12.0
     ports:
       - "1024:1024"
     volumes:
       - ./tmp:/tmp
       - .:/sipi/config
       - ./sipi/images:/sipi/images
     networks:
@@ -54,37 +52,37 @@
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/sipi/config/sipi.docker-config.lua
 
   app:
     # on the verge of every deployment (fortnightly), update the "image" value from the "app" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/dsp-app:v11.8.0
+    image: daschswiss/dsp-app:v11.9.0
     ports:
       - "4200:4200"
     networks:
       - knora-net
 
   db:
     # on the verge of every deployment (fortnightly), update the "image" value from the "db" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/apache-jena-fuseki:2.1.5
+    image: daschswiss/apache-jena-fuseki:5.0.0-1
     ports:
       - "3030:3030"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   ingest:
     # on the verge of every deployment (fortnightly), update the "image" value from the "ingest" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/dsp-ingest:v0.8.2
+    image: daschswiss/dsp-ingest:v0.8.3
     ports:
       - "3340:3340"
     volumes:
       - ./sipi/images:/opt/images
       - ./sipi/tmp-dsp-ingest:/opt/temp
     networks:
       - knora-net
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/connection_live.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/json_ld_util.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/json_ld_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/shared.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/xml_validation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import importlib.resources
+import warnings
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 from typing import Union
 
 import regex
 from loguru import logger
 from lxml import etree
 
+from dsp_tools.models.custom_warnings import DspToolsFutureWarning
 from dsp_tools.models.exceptions import InputError
 from dsp_tools.utils.xml_utils import parse_and_remove_comments_from_xml_file
 from dsp_tools.utils.xml_utils import remove_namespaces_from_xml
 from dsp_tools.utils.xml_validation_models import InconsistentTextValueEncodings
 from dsp_tools.utils.xml_validation_models import TextValueData
 
 separator = "\n    "
@@ -49,14 +51,16 @@
     if not all_good:
         problems.append(msg)
 
     all_good, msg = _find_mixed_encodings_in_one_text_prop(xml_no_namespace)
     if not all_good:
         problems.append(msg)
 
+    _check_for_deprecated_syntax(xml_no_namespace)
+
     if len(problems) > 0:
         err_msg = grand_separator.join(problems)
         logger.opt(exception=True).error(err_msg)
         raise InputError(err_msg)
 
     logger.info("The XML file is syntactically correct and passed validation.")
     print(f"{datetime.now()}: The XML file is syntactically correct and passed validation.")
@@ -137,14 +141,31 @@
     if df is not None:
         csv_path = Path(f"XML_syntax_errors_{datetime.now().strftime('%Y-%m-%d_%H%M%S')}.csv")
         msg = f"\nAll the problems are listed in the file: '{csv_path.absolute()}'" + msg
         df.to_csv(csv_path)
     return False, msg
 
 
+def _check_for_deprecated_syntax(data_xml: etree._Element) -> None:
+    _check_for_deprecated_isSequenceOf(data_xml)
+
+
+def _check_for_deprecated_isSequenceOf(data_xml: etree._Element) -> None:
+    isSequenceOf_matches = data_xml.findall("resource/resptr-prop")
+    isSequenceOf_matches = [x for x in isSequenceOf_matches if x.attrib.get("name") == "isSequenceOf"]
+    hasSequenceBounds_matches = data_xml.findall("resource/interval-prop")
+    hasSequenceBounds_matches = [x for x in hasSequenceBounds_matches if x.attrib.get("name") == "hasSequenceBounds"]
+    if any([isSequenceOf_matches, hasSequenceBounds_matches]):
+        msg = (
+            "Deprecation Warning: Your XML data file contains deprecated properties. "
+            "Support for the following properties will be removed soon: isSequenceOf, hasSequenceBounds"
+        )
+        warnings.warn(DspToolsFutureWarning(msg))
+
+
 def check_if_only_one_encoding_is_used_per_prop_in_root(
     root: etree._Element,
 ) -> list[TextValueData]:
     """
     Check if all the encodings in the <text> elements are consistent within one <text-prop>
 
     This is correct:
```

### Comparing `dsp_tools-7.1.2.post0/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.1.3/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.1.2.post0/PKG-INFO` & `dsp_tools-7.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.1.2.post0
+Version: 7.1.3
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

