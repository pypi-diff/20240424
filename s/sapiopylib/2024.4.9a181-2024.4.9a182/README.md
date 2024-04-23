# Comparing `tmp/sapiopylib-2024.4.9a181.tar.gz` & `tmp/sapiopylib-2024.4.9a182.tar.gz`

## Comparing `sapiopylib-2024.4.9a181.tar` & `sapiopylib-2024.4.9a182.tar`

### file list

```diff
@@ -1,129 +1,130 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/PyCspFieldMap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/__init__.py
--rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
--rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
--rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/QQPlotComputer.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0    13374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ClientCallbackService.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataService.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/GroupManagerService.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/MessengerService.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/ReportManager.py
--rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/UserManagerService.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Message.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/UserInfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/field_set.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/protocol_template.py
--rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/CompresionUtil.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/autopaging.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recorddatasinks.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    28845 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    44895 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/ancestry.py
--rw-r--r--   0        0        0    18003 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/properties.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/src/sapiopylib/utils/string.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/EmailAttachmentDataTest.py
--rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51536_test.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51549_test.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51551_test.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51635_test.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51821_test.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51846_test.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51847_test.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-51849_test.py
--rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/FR-52100_test.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51537_test.py
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51547.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51842_test.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51853_test.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51856_test.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/PR-51964_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/__init__.py
--rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/data_type_models.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/resources/NAC28735.fa
--rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/tests/resources/fr-51846.ssg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/LICENSE
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/README.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/pyproject.toml
--rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a181/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36931 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     4304 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/jarvis/QQPlotComputer.py
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0    13374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/ClientCallbackService.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataService.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/GroupManagerService.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/MessengerService.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/ReportManager.py
+-rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/UserManagerService.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    25254 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Message.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/UserInfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25239 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    21882 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    62485 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    26958 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/field_set.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/protocol_template.py
+-rw-r--r--   0        0        0    17530 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    24025 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     5549 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     8809 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/CompresionUtil.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    23715 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/autopaging.py
+-rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recorddatasinks.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    28845 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    46989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    13800 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/ancestry.py
+-rw-r--r--   0        0        0    21628 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/properties.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/src/sapiopylib/utils/string.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/EmailAttachmentDataTest.py
+-rw-r--r--   0        0        0    10694 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51536_test.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51549_test.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51551_test.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51635_test.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51821_test.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51846_test.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51847_test.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-51849_test.py
+-rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-52100_test.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/FR-52133_test.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51537_test.py
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51547.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51842_test.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51853_test.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51856_test.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/PR-51964_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/__init__.py
+-rw-r--r--   0        0        0  1468866 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/data_type_models.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/resources/NAC28735.fa
+-rw-r--r--   0        0        0    12255 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/tests/resources/fr-51846.ssg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/LICENSE
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/README.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/pyproject.toml
+-rw-r--r--   0        0        0     6455 2020-02-02 00:00:00.000000 sapiopylib-2024.4.9a182/PKG-INFO
```

### Comparing `sapiopylib-2024.4.9a181/INSTALL.md` & `sapiopylib-2024.4.9a182/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/PyCspFieldMap.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/PyCspFieldMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspData.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/PlotlyCspData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/jarvis/QQPlotComputer.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/jarvis/QQPlotComputer.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ClientCallbackService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/ClientCallbackService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/GroupManagerService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/GroupManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/MessengerService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/MessengerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/ReportManager.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/ReportManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/User.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/UserManagerService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/UserManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Message.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Message.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/UserInfo.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/UserInfo.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnEntryPosition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/field_set.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/field_set.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/eln/protocol_template.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/eln/protocol_template.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/CompresionUtil.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/CompresionUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/autopaging.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/autopaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recorddatasinks.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recorddatasinks.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from sapiopylib.rest.utils.DataTypeCacheManager import DataTypeCacheManager
 from sapiopylib.rest.utils.MultiMap import SetMultimap
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import PyRecordModel, SapioRecordModelException, \
     RecordModelReverseSideLinkCacheKey
 from sapiopylib.rest.utils.recordmodel.RecordModelEventBus import RecordModelEventBus
 from sapiopylib.rest.utils.recordmodel.RecordModelEvents import RecordAddedEvent, RecordDeletedEvent, \
     FieldChangeEvent, ChildAddedEvent, ChildRemovedEvent, CommitEvent, RollbackEvent, SideLinkChangedEvent
-from sapiopylib.rest.utils.recordmodel.RelationshipPath import RelationshipPath, RelationshipPathDir
+from sapiopylib.rest.utils.recordmodel.RelationshipPath import RelationshipPath, RelationshipNodeType, RelationshipNode
 
 
 class RecordModelManager:
     """
     Record Model Manager helps to keep track of a user session changes and attempt to batch record changes
     into one call.
 
@@ -609,35 +609,69 @@
     def load_path(self, root_records: List[PyRecordModel], rel_path: RelationshipPath) -> None:
         """
         Load an entire path of records that we need to load along this path.
         If any parents or children for any records along this way are already loaded, it will not attempt to reload.
         :param root_records: root records list.
         :param rel_path: the relationship path to load.
         """
-        path: List[Tuple[RelationshipPathDir, str]] = rel_path.path
-        cur_records: List[PyRecordModel] = root_records
-        for direction, dt_name in path:
+        import sapiopylib.rest.utils.recordmodel.ancestry as ancestry
+        path: List[RelationshipNode] = rel_path.path
+        cur_records: List[PyRecordModel] =  RecordModelWrapperUtil.unwrap_list(root_records)
+        visited: Set[PyRecordModel] = set()
+        for node in path:
+            for x in cur_records:
+                visited.add(x)
+            direction = node.direction
+            dt_name = node.data_type_name
+            data_field_name = node.data_field_name
             next_records: List[PyRecordModel] = []
-            if direction == RelationshipPathDir.PARENT:
+            if direction == RelationshipNodeType.PARENT:
                 self.load_parents(cur_records, dt_name)
                 for record in cur_records:
                     parents = record.get_parents_of_type(dt_name)
                     for parent in parents:
                         if parent not in next_records:
                             next_records.append(parent)
-            elif direction == RelationshipPathDir.CHILD:
+            elif direction == RelationshipNodeType.CHILD:
                 self.load_children(cur_records, dt_name)
                 for record in cur_records:
                     children = record.get_children_of_type(dt_name)
                     for child in children:
                         if child not in next_records:
                             next_records.append(child)
+            elif direction == RelationshipNodeType.ANCESTOR:
+                # Avoiding circular imports here...
+                rec_man = self._record_model_manager
+                ancestor_man = ancestry.RecordModelAncestorManager(rec_man)
+                ancestor_man.load_ancestors_of_type(cur_records, dt_name)
+                for record in cur_records:
+                    ancestors = ancestor_man.get_ancestors_of_type(record, dt_name)
+                    next_records.extend(ancestors)
+            elif direction == RelationshipNodeType.DESCENDANT:
+                # Avoiding circular imports here...
+                rec_man = self._record_model_manager
+                ancestor_man = ancestry.RecordModelAncestorManager(rec_man)
+                ancestor_man.load_descendant_of_type(cur_records, dt_name)
+                for record in cur_records:
+                    descendants = ancestor_man.get_descendant_of_type(record, dt_name)
+                    next_records.extend(descendants)
+            elif direction == RelationshipNodeType.FORWARD_SIDE_LINK:
+                self.load_forward_side_links(cur_records, data_field_name)
+                for record in cur_records:
+                    forward = record.get_forward_side_link(data_field_name)
+                    if forward is not None:
+                        next_records.append(forward)
+            elif direction == RelationshipNodeType.REVERSE_SIDE_LINK:
+                self.load_reverse_side_links(cur_records, dt_name, data_field_name)
+                for record in cur_records:
+                    backwards = record.get_reverse_side_link(dt_name, data_field_name)
+                    next_records.extend(backwards)
             else:
                 raise ValueError("Unsupported direction: " + direction.name)
-            cur_records = next_records
+            cur_records = list(set([x for x in next_records if x not in visited and x is not None]))
 
 
 class _RelationshipSideLinkHandler(EventHandler[SideLinkChangedEvent]):
     _rel_man: RecordModelRelationshipManager
 
     def __init__(self, rel_man: RecordModelRelationshipManager):
         self._rel_man = rel_man
```

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/ancestry.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/ancestry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/rest/utils/recordmodel/properties.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/rest/utils/recordmodel/properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from typing import Optional, Type, List, Union, Iterable, TypeVar, Generic
 
 from sapiopylib.rest.utils.recordmodel.PyRecordModel import AbstractRecordModelPropertyGetter, PyRecordModel, \
     AbstractRecordModelPropertyAdder, \
-    AbstractRecordModelPropertyRemover
+    AbstractRecordModelPropertyRemover, RecordModelPropertyType, AbstractRecordModelPropertySetter
 from sapiopylib.rest.utils.recordmodel.RecordModelManager import RecordModelManager
 from sapiopylib.rest.utils.recordmodel.RecordModelWrapper import WrappedRecordModel, RecordModelWrapperUtil
 from sapiopylib.rest.utils.recordmodel.ancestry import RecordModelAncestorManager
 
 # Record Model Specific Property Type. This is known from static constructors of each property.
 _RMSPT = TypeVar("_RMSPT", bound=Union[PyRecordModel, WrappedRecordModel])
 
+
 class _ParentsGetterProperty(AbstractRecordModelPropertyGetter[List[_RMSPT]], Generic[_RMSPT]):
     _parent_type_name: str
     wrap_results_type: Optional[Type[_RMSPT]]
 
     def __init__(self, parent_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._parent_type_name = parent_type_name
         self.wrap_results_type = wrap_results_type
@@ -101,14 +102,15 @@
         return _ParentsCreatorProperty[PyRecordModel](parent_type_name, num_records_to_create)
 
     @staticmethod
     def create(parent_type: Type[WrappedRecordModel], num_records_to_create: int):
         return _ParentsCreatorProperty[parent_type](parent_type.get_wrapper_data_type_name(),
                                                     num_records_to_create, parent_type)
 
+
 class _ParentGetterProperty(AbstractRecordModelPropertyGetter[_RMSPT], Generic[_RMSPT]):
     _parent_type_name: str
     wrap_results_type: Optional[Type[WrappedRecordModel]]
 
     def __init__(self, parent_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._parent_type_name = parent_type_name
         self.wrap_results_type = wrap_results_type
@@ -117,26 +119,28 @@
         model: Optional[PyRecordModel] = model.get_parent_of_type(self._parent_type_name)
         if not model:
             return None
         if not self.wrap_results_type:
             return model
         return RecordModelWrapperUtil.wrap(model, self.wrap_results_type)
 
+
 class _ParentModProperty(AbstractRecordModelPropertyAdder[None], AbstractRecordModelPropertyRemover[None]):
     value: PyRecordModel
 
     def __init__(self, value: Union[PyRecordModel, WrappedRecordModel]):
         self.value = RecordModelWrapperUtil.unwrap_list([value])[0]
 
     def remove_value(self, remove_from: PyRecordModel) -> None:
         remove_from.remove_parent(self.value)
 
     def add_value(self, add_to: PyRecordModel) -> None:
         add_to.add_parent(self.value)
 
+
 class _ParentCreatorProperty(AbstractRecordModelPropertyAdder[_RMSPT]):
     _parent_type_name: str
     wrap_results_type: Optional[Type[WrappedRecordModel]]
 
     def __init__(self, parent_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._parent_type_name = parent_type_name
         self.wrap_results_type = wrap_results_type
@@ -146,18 +150,20 @@
         inst_man = rec_man.instance_manager
         new_record = inst_man.add_new_record(self._parent_type_name)
         add_to.add_parent(new_record)
         if self.wrap_results_type:
             return RecordModelWrapperUtil.wrap(new_record, self.wrap_results_type)
         return new_record
 
+
 class Parent:
     """
     Property getters to obtain or modify single parent of record model
     """
+
     @staticmethod
     def of_type(parent_type: Type[WrappedRecordModel]):
         """
         Get the property getter of parent of specified wrapped record model's data type represented in wrapper class.
         """
         return _ParentGetterProperty[parent_type](parent_type.get_wrapper_data_type_name(), parent_type)
 
@@ -185,14 +191,15 @@
     @staticmethod
     def create(parent_type: Type[WrappedRecordModel]):
         """
         Creator of new parent.
         """
         return _ParentCreatorProperty[parent_type](parent_type.get_wrapper_data_type_name(), parent_type)
 
+
 class _ChildrenGetterProperty(AbstractRecordModelPropertyGetter[List[_RMSPT]]):
     _children_type_name: str
     wrap_results_type: Optional[Type[WrappedRecordModel]]
 
     def __init__(self, children_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._children_type_name = children_type_name
         self.wrap_results_type = wrap_results_type
@@ -238,14 +245,15 @@
         inst_man = rec_man.instance_manager
         new_records = inst_man.add_new_records(self._children_data_type_name, self._num_to_create)
         add_to.add_children(new_records)
         if self.wrap_results_type:
             return RecordModelWrapperUtil.wrap_list(new_records, self.wrap_results_type)
         return new_records
 
+
 class Children:
     """
     Property getters to obtain or modify children of record model
     """
 
     @staticmethod
     def of_type(child_type: Type[WrappedRecordModel]):
@@ -279,14 +287,15 @@
     def create(children_type: Type[WrappedRecordModel], num_records_to_create: int):
         """
         Creator of new children.
         """
         return _ChildrenCreatorProperty[children_type](children_type.get_wrapper_data_type_name(),
                                                        num_records_to_create, children_type)
 
+
 class _ChildGetterProperty(AbstractRecordModelPropertyGetter[_RMSPT]):
     _child_type_name: str
     wrap_results_type: Optional[Type[WrappedRecordModel]]
 
     def __init__(self, child_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._child_type_name = child_type_name
         self.wrap_results_type = wrap_results_type
@@ -295,26 +304,28 @@
         model: Optional[PyRecordModel] = model.get_child_of_type(self._child_type_name)
         if not model:
             return None
         if not self.wrap_results_type:
             return model
         return RecordModelWrapperUtil.wrap(model, self.wrap_results_type)
 
+
 class _ChildModProperty(AbstractRecordModelPropertyAdder[None], AbstractRecordModelPropertyRemover[None]):
     value: PyRecordModel
 
     def __init__(self, value: Union[PyRecordModel, WrappedRecordModel]):
         self.value = RecordModelWrapperUtil.unwrap_list([value])[0]
 
     def remove_value(self, remove_from: PyRecordModel) -> None:
         remove_from.remove_child(self.value)
 
     def add_value(self, add_to: PyRecordModel) -> None:
         add_to.add_child(self.value)
 
+
 class _ChildCreatorProperty(AbstractRecordModelPropertyAdder[_RMSPT]):
     _child_type_name: str
     wrap_results_type: Optional[Type[WrappedRecordModel]]
 
     def __init__(self, child_type_name: str, wrap_results_type: Optional[Type[WrappedRecordModel]] = None):
         self._child_type_name = child_type_name
         self.wrap_results_type = wrap_results_type
@@ -329,14 +340,15 @@
         return new_record
 
 
 class Child:
     """
     Property getters to obtain or modify single child of record model
     """
+
     @staticmethod
     def of_type(child_type: Type[WrappedRecordModel]):
         """
         Get the property getter of child of specified wrapped record model's data type represented in wrapper class.
         """
         return _ChildGetterProperty[child_type](child_type.get_wrapper_data_type_name(), child_type)
 
@@ -429,7 +441,94 @@
 
     def get_value(self, model: PyRecordModel) -> List[_RMSPT]:
         ancestor_man = RecordModelAncestorManager(model.record_model_manager)
         models: List[PyRecordModel] = list(ancestor_man.get_descendant_of_type(model, self._desc_type_name))
         if not self.wrap_results_type:
             return models
         return RecordModelWrapperUtil.wrap_list(models, self.wrap_results_type)
+
+
+class _ForwardSideLinkGetterProperty(AbstractRecordModelPropertyGetter[_RMSPT | None]):
+    """
+    Property to obtain a forward side link record.
+    """
+    forward_field_name: str
+    wrap_results_type: Optional[Type[WrappedRecordModel]]
+
+    def __init__(self, forward_field_name: str, wrap_result_type: Type[WrappedRecordModel] | None = None):
+        self.forward_field_name = forward_field_name
+        self.wrap_results_type = wrap_result_type
+
+    @staticmethod
+    def of_field(field_name: str, side_link_type: Type[WrappedRecordModel] | None = None):
+        return _ForwardSideLinkGetterProperty(field_name, side_link_type)
+
+    def get_value(self, model: PyRecordModel) -> _RMSPT | None:
+        ret: PyRecordModel | None = model.get_forward_side_link(self.forward_field_name)
+        if not ret or not self.wrap_results_type:
+            return ret
+        return RecordModelWrapperUtil.wrap(ret, self.wrap_results_type)
+
+
+class _ForwardSideLinkSetterProperty(AbstractRecordModelPropertySetter[None]):
+    field_name: str
+    value: PyRecordModel | None
+
+    def __init__(self, field_name: str, value: PyRecordModel | None):
+        self.field_name = field_name
+        self.value = value
+
+    def set_value(self, set_to: PyRecordModel) -> None:
+        set_to.set_field_value(self.field_name, self.value.record_id)
+
+
+class ForwardSideLink:
+    """
+    Obtaining properties for forward side links.
+    """
+
+    @staticmethod
+    def of(forward_field_name: str, wrap_result_type: Type[WrappedRecordModel] | None = None):
+        """
+        Obtain a getter property for the forward side link on this record's particular field.
+        """
+        return _ForwardSideLinkGetterProperty(forward_field_name, wrap_result_type)
+
+    @staticmethod
+    def ref(forward_field_name: str, value: PyRecordModel | WrappedRecordModel | None):
+        """
+        Obtain a setter property for the forward side link on tihs record's particular field.
+        """
+        if value is None:
+            return _ForwardSideLinkSetterProperty(forward_field_name, None)
+        return _ForwardSideLinkSetterProperty(forward_field_name, RecordModelWrapperUtil.unwrap(value))
+
+
+class _ReverseSideLinkGetterProperty(AbstractRecordModelPropertyGetter[list[_RMSPT]]):
+    reverse_data_type_name: str
+    reverse_field_name: str
+    wrap_results_type: Type[WrappedRecordModel] | None
+
+    def __init__(self, reverse_data_type_name: str, reverse_field_name: str,
+                 wrap_results_type: Type[WrappedRecordModel] | None = None):
+        self.reverse_data_type_name = reverse_data_type_name
+        self.reverse_field_name = reverse_field_name
+        self.wrap_results_type = wrap_results_type
+
+    def get_value(self, model: PyRecordModel) -> list[_RMSPT]:
+        reverse_side_links = model.get_reverse_side_link(self.reverse_data_type_name, self.reverse_field_name)
+        if not self.wrap_results_type:
+            return reverse_side_links
+        return RecordModelWrapperUtil.wrap_list(reverse_side_links, self.wrap_results_type)
+
+
+class ReverseSideLink:
+    """
+    Getter for reverse side link property.
+    """
+    @staticmethod
+    def of(reverse_data_type_name: str, reverse_data_field_name: str):
+        return _ReverseSideLinkGetterProperty(reverse_data_type_name, reverse_data_field_name)
+
+    @staticmethod
+    def of_type(reverse_data_type: Type[WrappedRecordModel], reverse_data_field_name: str):
+        return _ReverseSideLinkGetterProperty(reverse_data_type.get_wrapper_data_type_name(), reverse_data_field_name, reverse_data_type)
```

### Comparing `sapiopylib-2024.4.9a181/src/sapiopylib/utils/string.py` & `sapiopylib-2024.4.9a182/src/sapiopylib/utils/string.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/EmailAttachmentDataTest.py` & `sapiopylib-2024.4.9a182/tests/EmailAttachmentDataTest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51536_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51536_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51549_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51549_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51551_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51551_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51635_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51635_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51821_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51821_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51846_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51846_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51847_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51847_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-51849_test.py` & `sapiopylib-2024.4.9a182/tests/FR-51849_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/FR-52100_test.py` & `sapiopylib-2024.4.9a182/tests/FR-52100_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51537_test.py` & `sapiopylib-2024.4.9a182/tests/PR-51537_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51547.py` & `sapiopylib-2024.4.9a182/tests/PR-51547.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51842_test.py` & `sapiopylib-2024.4.9a182/tests/PR-51842_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51853_test.py` & `sapiopylib-2024.4.9a182/tests/PR-51853_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51856_test.py` & `sapiopylib-2024.4.9a182/tests/PR-51856_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/PR-51964_test.py` & `sapiopylib-2024.4.9a182/tests/PR-51964_test.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/data_type_models.py` & `sapiopylib-2024.4.9a182/tests/data_type_models.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/resources/NAC28735.fa` & `sapiopylib-2024.4.9a182/tests/resources/NAC28735.fa`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/tests/resources/fr-51846.ssg` & `sapiopylib-2024.4.9a182/tests/resources/fr-51846.ssg`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/LICENSE` & `sapiopylib-2024.4.9a182/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/README.md` & `sapiopylib-2024.4.9a182/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2024.4.9a181/pyproject.toml` & `sapiopylib-2024.4.9a182/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2024.04.09a181'
+version='2024.04.09a182'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sapiopylib-2024.4.9a181/PKG-INFO` & `sapiopylib-2024.4.9a182/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sapiopylib
-Version: 2024.4.9a181
+Version: 2024.4.9a182
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.9a181 Summary: Official
+Metadata-Version: 2.3 Name: sapiopylib Version: 2024.4.9a182 Summary: Official
 Sapio Informatics Platform Python API Project-URL: Homepage, https://
 github.com/sapiosciences Project-URL: Bug Tracker, https://github.com/
 sapiosciences/sapio-py-tutorials/issues Author-email: Yechen Qiao
 sapiosciences.com> License-Expression: MPL-2.0 License-File: LICENSE Keywords:
 eln,lims,rest,sapio Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Healthcare Industry Classifier: Intended Audience :: Science/Research
```

