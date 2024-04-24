# Comparing `tmp/cosmicfrog-0.3.8.tar.gz` & `tmp/cosmicfrog-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicfrog-0.3.8.tar", last modified: Tue Aug 22 23:07:32 2023, max compression
+gzip compressed data, was "cosmicfrog-0.3.9.tar", last modified: Wed Aug 23 23:12:04 2023, max compression
```

## Comparing `cosmicfrog-0.3.8.tar` & `cosmicfrog-0.3.9.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.387335 cosmicfrog-0.3.8/
--rw-r--r--   0 gordonhart   (501) staff       (20)      352 2023-08-22 23:07:32.387194 cosmicfrog-0.3.8/PKG-INFO
--rw-r--r--   0 gordonhart   (501) staff       (20)      486 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/README.md
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.327622 cosmicfrog-0.3.8/cosmicfrog/
--rw-r--r--   0 gordonhart   (501) staff       (20)      209 2023-08-22 21:57:18.000000 cosmicfrog-0.3.8/cosmicfrog/__init__.py
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.324442 cosmicfrog-0.3.8/cosmicfrog/anura/
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.386172 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/
--rw-r--r--   0 gordonhart   (501) staff       (20)     8022 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2629 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Analytics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5905 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2198 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10838 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6637 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6430 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13497 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    17710 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12342 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18271 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6525 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13321 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18203 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Customers.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12984 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    31026 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Facilities.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    23117 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7737 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13103 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7405 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13263 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13438 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13943 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4504 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    11840 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5179 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Groups.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2401 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Histograms.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9384 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InputFactors.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10320 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9604 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    37919 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    39657 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6883 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Lookups.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3239 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Maps.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5949 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7320 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    19168 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9656 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9469 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3602 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5317 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4329 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2583 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Organizations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6687 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2796 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Periods.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    28592 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Processes.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    26042 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12346 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15370 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    14833 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16683 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3296 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13669 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13977 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12389 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12870 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13999 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15546 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13797 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Products.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7335 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12348 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15376 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16715 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18561 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3189 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3278 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4718 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2879 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5353 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4340 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Scenarios.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6460 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10685 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Shipments.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5798 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_StepCosts.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4536 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6481 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5864 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    11580 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Suppliers.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6647 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3162 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TableFilters.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16686 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18492 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9955 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9181 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    22940 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    21819 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    32814 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    30886 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9956 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4705 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5569 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4111 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4092 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3647 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    25027 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6574 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13974 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15701 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9490 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7661 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18790 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18860 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10171 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkResources.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    11935 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     8862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10784 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3526 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    20156 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7056 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16396 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16803 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    21094 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7914 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    34222 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    22234 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9424 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6017 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10219 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6970 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    17471 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12634 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9490 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4522 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10498 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5722 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4787 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6799 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    14082 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16823 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6246 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    28983 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    14164 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4063 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12557 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5709 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4864 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9345 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6767 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12537 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9475 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4764 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     1961 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6460 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7043 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15917 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    17090 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    34065 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    33862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18726 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    18541 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7903 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7715 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    39373 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    40023 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    20366 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    20172 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2128 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2969 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2411 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    55257 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    55033 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    32669 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    32484 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7506 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7319 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    63682 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    63410 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    26655 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    26664 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    14419 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    14419 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10273 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10109 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6316 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4594 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     8524 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     8551 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4040 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7970 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7997 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12980 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    13007 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5341 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5368 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    60336 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    60255 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    31510 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    31476 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     2944 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5725 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5764 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    10657 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    16391 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    11893 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    11920 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3619 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     3646 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     7968 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6540 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6364 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    12327 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6846 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6885 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6204 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6263 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     8923 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     8950 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     5664 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     4045 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6275 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     6302 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9604 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
--rw-r--r--   0 gordonhart   (501) staff       (20)     9631 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.386821 cosmicfrog-0.3.8/cosmicfrog/anura/table_masterlists/
--rw-r--r--   0 gordonhart   (501) staff       (20)    57001 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    25920 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
--rw-r--r--   0 gordonhart   (501) staff       (20)    15890 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/frog_data.py
--rw-r--r--   0 gordonhart   (501) staff       (20)      288 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/frog_excel.py
--rw-r--r--   0 gordonhart   (501) staff       (20)     2424 2023-08-22 21:57:44.000000 cosmicfrog-0.3.8/cosmicfrog/frog_launcher.py
--rw-r--r--   0 gordonhart   (501) staff       (20)     1384 2023-08-22 17:11:57.000000 cosmicfrog-0.3.8/cosmicfrog/frog_log.py
--rw-r--r--   0 gordonhart   (501) staff       (20)     2445 2023-08-22 20:33:02.000000 cosmicfrog-0.3.8/cosmicfrog/frog_params.py
--rw-r--r--   0 gordonhart   (501) staff       (20)     2295 2023-08-22 17:12:08.000000 cosmicfrog-0.3.8/cosmicfrog/frog_platform.py
--rw-r--r--   0 gordonhart   (501) staff       (20)     3315 2023-08-21 21:26:06.000000 cosmicfrog-0.3.8/cosmicfrog/frog_security.py
--rw-r--r--   0 gordonhart   (501) staff       (20)      277 2023-08-22 21:41:27.000000 cosmicfrog-0.3.8/cosmicfrog/suppress_stdio.py
-drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-22 23:07:32.330355 cosmicfrog-0.3.8/cosmicfrog.egg-info/
--rw-r--r--   0 gordonhart   (501) staff       (20)      352 2023-08-22 23:07:32.000000 cosmicfrog-0.3.8/cosmicfrog.egg-info/PKG-INFO
--rw-r--r--   0 gordonhart   (501) staff       (20)    16641 2023-08-22 23:07:32.000000 cosmicfrog-0.3.8/cosmicfrog.egg-info/SOURCES.txt
--rw-r--r--   0 gordonhart   (501) staff       (20)        1 2023-08-22 23:07:32.000000 cosmicfrog-0.3.8/cosmicfrog.egg-info/dependency_links.txt
--rw-r--r--   0 gordonhart   (501) staff       (20)      114 2023-08-22 23:07:32.000000 cosmicfrog-0.3.8/cosmicfrog.egg-info/requires.txt
--rw-r--r--   0 gordonhart   (501) staff       (20)       11 2023-08-22 23:07:32.000000 cosmicfrog-0.3.8/cosmicfrog.egg-info/top_level.txt
--rw-r--r--   0 gordonhart   (501) staff       (20)       38 2023-08-22 23:07:32.387380 cosmicfrog-0.3.8/setup.cfg
--rw-r--r--   0 gordonhart   (501) staff       (20)      899 2023-08-22 23:04:57.000000 cosmicfrog-0.3.8/setup.py
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.917924 cosmicfrog-0.3.9/
+-rw-r--r--   0 gordonhart   (501) staff       (20)      352 2023-08-23 23:12:04.917797 cosmicfrog-0.3.9/PKG-INFO
+-rw-r--r--   0 gordonhart   (501) staff       (20)      486 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/README.md
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.874277 cosmicfrog-0.3.9/cosmicfrog/
+-rw-r--r--   0 gordonhart   (501) staff       (20)      208 2023-08-23 23:11:24.000000 cosmicfrog-0.3.9/cosmicfrog/__init__.py
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.872686 cosmicfrog-0.3.9/cosmicfrog/anura/
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.916810 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8022 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2629 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Analytics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5905 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2198 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10838 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6637 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6430 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13497 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    17710 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12342 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18271 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6525 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13321 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18203 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Customers.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12984 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    31026 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Facilities.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    23117 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7737 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13103 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7405 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13263 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13438 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13943 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4504 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    11840 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5179 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Groups.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2401 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Histograms.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9384 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InputFactors.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10320 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9604 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    37919 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    39657 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6883 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Lookups.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3239 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Maps.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5949 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7320 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    19168 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9656 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9469 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3602 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5317 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4329 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2583 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Organizations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6687 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2796 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Periods.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    28592 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Processes.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    26042 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12346 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15370 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    14833 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16683 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3296 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13669 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13977 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12389 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12870 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13999 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15546 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13797 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Products.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7335 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12348 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15376 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16715 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18561 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3189 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3278 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4718 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2879 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5353 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4340 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Scenarios.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6460 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10685 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Shipments.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5798 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_StepCosts.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4536 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6481 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5864 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    11580 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Suppliers.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6647 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3162 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TableFilters.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16686 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18492 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9955 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9181 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    22940 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    21819 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    32814 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    30886 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9956 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4705 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5569 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4111 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4092 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3647 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    25027 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6574 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13974 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15701 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9490 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7661 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18790 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18860 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10171 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkResources.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    11935 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10784 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3526 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    20156 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7056 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16396 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16803 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    21094 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7914 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    34222 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    22234 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9424 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6017 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10219 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6970 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    17471 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12634 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9490 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4522 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10498 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5722 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4787 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6799 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    14082 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16823 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6246 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    28983 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    14164 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4063 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12557 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5709 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4864 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9345 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6767 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12537 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9475 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4764 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     1961 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6460 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7043 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15917 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    17090 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    34065 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    33862 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18726 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    18541 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7903 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7715 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    39373 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    40023 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    20366 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    20172 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2128 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2969 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2411 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    55257 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    55033 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    32669 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    32484 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7506 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7319 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    63682 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    63410 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    26655 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    26664 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    14419 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    14419 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10273 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10109 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6316 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4594 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8524 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8551 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4040 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7970 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7997 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12980 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    13007 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5341 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5368 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    60336 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    60255 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    31510 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    31476 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2944 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5725 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5764 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    10657 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16391 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    11893 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    11920 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3619 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3646 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     7968 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6540 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6364 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    12327 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6846 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6885 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6204 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6263 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8923 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     8950 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     5664 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     4045 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6275 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     6302 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9604 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)     9631 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.917358 cosmicfrog-0.3.9/cosmicfrog/anura/table_masterlists/
+-rw-r--r--   0 gordonhart   (501) staff       (20)    57001 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    25920 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
+-rw-r--r--   0 gordonhart   (501) staff       (20)    15890 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/frog_data.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)      288 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/frog_excel.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3242 2023-08-23 23:04:43.000000 cosmicfrog-0.3.9/cosmicfrog/frog_launcher.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)     1384 2023-08-22 17:11:57.000000 cosmicfrog-0.3.9/cosmicfrog/frog_log.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2435 2023-08-23 21:38:59.000000 cosmicfrog-0.3.9/cosmicfrog/frog_params.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)     2819 2023-08-23 22:10:16.000000 cosmicfrog-0.3.9/cosmicfrog/frog_platform.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)     3315 2023-08-21 21:26:06.000000 cosmicfrog-0.3.9/cosmicfrog/frog_security.py
+-rw-r--r--   0 gordonhart   (501) staff       (20)      277 2023-08-22 21:41:27.000000 cosmicfrog-0.3.9/cosmicfrog/suppress_stdio.py
+drwxr-xr-x   0 gordonhart   (501) staff       (20)        0 2023-08-23 23:12:04.875158 cosmicfrog-0.3.9/cosmicfrog.egg-info/
+-rw-r--r--   0 gordonhart   (501) staff       (20)      352 2023-08-23 23:12:04.000000 cosmicfrog-0.3.9/cosmicfrog.egg-info/PKG-INFO
+-rw-r--r--   0 gordonhart   (501) staff       (20)    16641 2023-08-23 23:12:04.000000 cosmicfrog-0.3.9/cosmicfrog.egg-info/SOURCES.txt
+-rw-r--r--   0 gordonhart   (501) staff       (20)        1 2023-08-23 23:12:04.000000 cosmicfrog-0.3.9/cosmicfrog.egg-info/dependency_links.txt
+-rw-r--r--   0 gordonhart   (501) staff       (20)      114 2023-08-23 23:12:04.000000 cosmicfrog-0.3.9/cosmicfrog.egg-info/requires.txt
+-rw-r--r--   0 gordonhart   (501) staff       (20)       11 2023-08-23 23:12:04.000000 cosmicfrog-0.3.9/cosmicfrog.egg-info/top_level.txt
+-rw-r--r--   0 gordonhart   (501) staff       (20)       38 2023-08-23 23:12:04.917965 cosmicfrog-0.3.9/setup.cfg
+-rw-r--r--   0 gordonhart   (501) staff       (20)      899 2023-08-22 23:17:58.000000 cosmicfrog-0.3.9/setup.py
```

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Analytics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Analytics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_BusinessHours.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_BusinessHours.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Customers.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Customers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Facilities.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Facilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Groups.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Groups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Histograms.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Histograms.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InputFactors.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Lookups.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Lookups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Maps.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Maps.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelInfo.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelInfo.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ModelSettings.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ModelSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Organizations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Organizations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_OutputFactors.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_OutputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Periods.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Periods.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Processes.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Processes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Products.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Products.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Scenarios.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Scenarios.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Shipments.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Shipments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_StepCosts.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_StepCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_Suppliers.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_Suppliers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TableFilters.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TableFilters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationModes.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationModes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_TransportationRates.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_TransportationRates.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCenters.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCenters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkResources.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkResources.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json` & `cosmicfrog-0.3.9/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/frog_data.py` & `cosmicfrog-0.3.9/cosmicfrog/frog_data.py`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/frog_log.py` & `cosmicfrog-0.3.9/cosmicfrog/frog_log.py`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog/frog_params.py` & `cosmicfrog-0.3.9/cosmicfrog/frog_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from enum import Enum
 
 
 POSSIBLE_TYPES = ["int",        # User enters an integer
                    "double",    # User enters a double
                    "string"     # User enters a string
                  ]
@@ -21,20 +20,21 @@
         Methods
         -------
         add - Adds a new parameter
         result - Returns all added parameters as a string
     """
 
     def __init__(self, params : str = None):
+        
         self.__params = []
 
         # Note: No validation on params passed here, is responsibility of the running script to validate
         if params:
             self.__loaded_params = params
-            self.connection_string = self.__loaded_params.pop(0)
+            self.model_name = self.__loaded_params.pop(0)
 
     def __getitem__(self, index):
         return self.__loaded_params[index]
     
     def __is_valid_param_type(self, param_type: str) -> bool:
 
         if param_type in POSSIBLE_TYPES:
```

### Comparing `cosmicfrog-0.3.8/cosmicfrog/frog_platform.py` & `cosmicfrog-0.3.9/cosmicfrog/frog_platform.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,64 @@
+import os
 import json
 import logging
 import optilogic
 import time
 
-# Functions to facilitate interactions with Optilogic platform - Use 'optilogic' library
-
-#TODO: rename database=model, storage_name=model_name etc for cf library
-#TODO: use optilogic library where possible
+# Functions to facilitate interactions with Optilogic platform using 'optilogic' library
 
 class OptilogicClient():
     """
-    wrapper for optilogic module for consumption in cosmic frog services
+    Wrapper for optilogic module for consumption in Cosmic Frog services
     """
-    def __init__(self, username, appkey, logger = logging.getLogger()):
-        self.api = optilogic.pioneer.Api(auth_legacy=False, appkey=appkey, un=username)
+    def __init__(self, username = None, appkey = None, logger = logging.getLogger()):
+
+        # Detect if being run in Andromeda
+        job_app_key = os.environ.get('OPTILOGIC_JOB_APPKEY')
+        job_id = os.environ.get('JOB_KEY')
+
+        if appkey and not username:
+            # Use supplied key
+            self.api = optilogic.pioneer.Api(auth_legacy=False, appkey=appkey)  
+        elif appkey and username:
+            # Use supplied key & name
+            self.api = optilogic.pioneer.Api(auth_legacy=False, appkey=appkey, un=username)
+        elif job_app_key and job_id:
+            # Running on Andromeda
+            self.api = optilogic.pioneer.Api(auth_legacy=False)
+        else:
+            raise ValueError("OptilogicClient could not authenticate")
+
         self.logger = logger
 
     def model_exists(self, model_name):
         """
-        returns True if a given model exists, False otherwise
+        Returns True if a given model exists, False otherwise
         """
         try:
             return self.api.storagename_database_exists(model_name)
-        except Exception:
+        except Exception as e:
+            self.logger.error( f'Exception in cosmicfrog: {e}')
             return False
 
     def get_connection_string(self, model_name):
         try:
-            status = "error"
             rv = {"message" : "error getting connection string"}
-            if self.api.storagename_database_exists(model_name):
-                connections = self.api.sql_connection_info(model_name)
-                rv = connections
-                status = "success"
-            else:
-                rv = {"message" : f"model {model_name} does not exist"}
-                
-            return status, rv
+            if not self.api.storagename_database_exists(model_name):
+                return False, ""
+            
+            connection_info = self.api.sql_connection_info(model_name)
+
+            return True, connection_info['connectionStrings']['url']
+
         except Exception as e:
-            return "exception", e
-    
+            self.logger.error( f'Exception in cosmicfrog: {e}')
+            return False, ""
+        
+   
     def create_model_synchronous(self, model_name, model_template):
         try:
             new_model = self.api.database_create(name=model_name, template=model_template)
 
             status = "success"
             rv = {}
             if "crash" in new_model:
```

### Comparing `cosmicfrog-0.3.8/cosmicfrog/frog_security.py` & `cosmicfrog-0.3.9/cosmicfrog/frog_security.py`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/cosmicfrog.egg-info/SOURCES.txt` & `cosmicfrog-0.3.9/cosmicfrog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.8/setup.py` & `cosmicfrog-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cosmicfrog",
     
     include_package_data=True,
 
-    version="0.3.8",
+    version="0.3.9",
     description='Helpful utilities for working with Cosmic Frog models',
     url='https://cosmicfrog.com',
     author='Optilogic',
     packages=['cosmicfrog'],
     package_data={
         'cosmicfrog': ['anura/table_definitions/*.json',
                         'anura/table_masterlists/*.json'
```

