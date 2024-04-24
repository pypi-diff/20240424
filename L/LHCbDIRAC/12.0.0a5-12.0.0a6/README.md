# Comparing `tmp/LHCbDIRAC-12.0.0a5.tar.gz` & `tmp/LHCbDIRAC-12.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LHCbDIRAC-12.0.0a5.tar", last modified: Thu Feb 15 16:00:24 2024, max compression
+gzip compressed data, was "LHCbDIRAC-12.0.0a6.tar", last modified: Wed Feb 21 18:07:04 2024, max compression
```

## Comparing `LHCbDIRAC-12.0.0a5.tar` & `LHCbDIRAC-12.0.0a6.tar`

### file list

```diff
@@ -1,553 +1,554 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.093639 LHCbDIRAC-12.0.0a5/
--rw-rw-rw-   0 root         (0) root         (0)     1809 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    32452 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2964 2024-02-15 16:00:24.093639 LHCbDIRAC-12.0.0a5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/lhcbdirac.cfg
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)    12745 2024-02-15 16:00:24.095639 LHCbDIRAC-12.0.0a5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.948640 LHCbDIRAC-12.0.0a5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.966640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.968640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.968640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.970640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/
--rw-rw-rw-   0 root         (0) root         (0)     1869 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2201 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.970640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/test/
--rw-rw-rw-   0 root         (0) root         (0)     2457 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.970640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.972640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/
--rw-rw-rw-   0 root         (0) root         (0)    17746 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    26536 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    10573 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    26244 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    15013 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.973640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/
--rw-rw-rw-   0 root         (0) root         (0)    29758 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    11739 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    16810 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py
--rw-rw-rw-   0 root         (0) root         (0)    34147 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.973640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.976640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    38872 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py
--rw-rw-rw-   0 root         (0) root         (0)    21141 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py
--rw-rw-rw-   0 root         (0) root         (0)     4744 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py
--rw-rw-rw-   0 root         (0) root         (0)     6597 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py
--rw-rw-rw-   0 root         (0) root         (0)    18511 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py
--rw-rw-rw-   0 root         (0) root         (0)    81682 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py
--rw-rw-rw-   0 root         (0) root         (0)    72651 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.977640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/
--rw-rw-rw-   0 root         (0) root         (0)     6316 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35461 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.981640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     3003 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py
--rw-rw-rw-   0 root         (0) root         (0)   241870 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py
--rw-rw-rw-   0 root         (0) root         (0)    12515 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py
--rw-rw-rw-   0 root         (0) root         (0)    16403 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py
--rw-rw-rw-   0 root         (0) root         (0)     4036 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py
--rwxrwxrwx   0 root         (0) root         (0)      842 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2967 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql
--rw-rw-rw-   0 root         (0) root         (0)    28034 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql
--rw-rw-rw-   0 root         (0) root         (0)     4705 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql
--rw-rw-rw-   0 root         (0) root         (0)    12638 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql
--rw-rw-rw-   0 root         (0) root         (0)    87437 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql
--rw-rw-rw-   0 root         (0) root         (0)    19607 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.982640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/
--rw-rw-rw-   0 root         (0) root         (0)    14289 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.984640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/
--rw-rw-rw-   0 root         (0) root         (0)     1271 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py
--rw-rw-rw-   0 root         (0) root         (0)     8490 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1942 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     5893 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py
--rw-rw-rw-   0 root         (0) root         (0)     2216 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)   294418 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.984640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    88288 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     2330 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.986640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.989640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py
--rw-rw-rw-   0 root         (0) root         (0)     3705 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py
--rw-rw-rw-   0 root         (0) root         (0)     1751 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1519 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13131 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.990640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2611 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py
--rw-rw-rw-   0 root         (0) root         (0)    28818 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:23.991640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/
--rw-rw-rw-   0 root         (0) root         (0)     7892 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.001640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1155 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py
--rwxrwxrwx   0 root         (0) root         (0)     3567 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py
--rwxrwxrwx   0 root         (0) root         (0)     4682 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py
--rwxrwxrwx   0 root         (0) root         (0)     4660 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py
--rwxrwxrwx   0 root         (0) root         (0)     1704 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     2291 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py
--rwxrwxrwx   0 root         (0) root         (0)     1954 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py
--rwxrwxrwx   0 root         (0) root         (0)     1479 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py
--rwxrwxrwx   0 root         (0) root         (0)     1799 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py
--rwxrwxrwx   0 root         (0) root         (0)     9413 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py
--rwxrwxrwx   0 root         (0) root         (0)     1610 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py
--rwxrwxrwx   0 root         (0) root         (0)     2009 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py
--rwxrwxrwx   0 root         (0) root         (0)     2128 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py
--rwxrwxrwx   0 root         (0) root         (0)     2006 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py
--rwxrwxrwx   0 root         (0) root         (0)     1871 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py
--rwxrwxrwx   0 root         (0) root         (0)     2442 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py
--rwxrwxrwx   0 root         (0) root         (0)     2003 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py
--rwxrwxrwx   0 root         (0) root         (0)     2460 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py
--rwxrwxrwx   0 root         (0) root         (0)     1791 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     1665 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py
--rwxrwxrwx   0 root         (0) root         (0)     2154 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py
--rwxrwxrwx   0 root         (0) root         (0)     6303 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py
--rwxrwxrwx   0 root         (0) root         (0)     3242 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py
--rwxrwxrwx   0 root         (0) root         (0)     3021 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py
--rwxrwxrwx   0 root         (0) root         (0)     2714 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py
--rwxrwxrwx   0 root         (0) root         (0)     3374 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py
--rwxrwxrwx   0 root         (0) root         (0)     2247 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py
--rwxrwxrwx   0 root         (0) root         (0)     3172 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     1597 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     2278 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py
--rwxrwxrwx   0 root         (0) root         (0)     7961 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py
--rwxrwxrwx   0 root         (0) root         (0)     3047 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py
--rwxrwxrwx   0 root         (0) root         (0)    10570 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py
--rwxrwxrwx   0 root         (0) root         (0)     2681 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py
--rwxrwxrwx   0 root         (0) root         (0)     2443 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py
--rwxrwxrwx   0 root         (0) root         (0)     4711 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py
--rwxrwxrwx   0 root         (0) root         (0)     2580 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py
--rwxrwxrwx   0 root         (0) root         (0)     2052 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4024 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_split_runs_for_prod.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.002640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.002640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.002640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/
--rw-rw-rw-   0 root         (0) root         (0)     5344 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.003640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/
--rw-rw-rw-   0 root         (0) root         (0)     9187 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.003640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4493 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.003640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.008640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     4891 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py
--rw-rw-rw-   0 root         (0) root         (0)     2424 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/File.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py
--rw-rw-rw-   0 root         (0) root         (0)     5658 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py
--rw-rw-rw-   0 root         (0) root         (0)    18183 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/HTML.py
--rw-rw-rw-   0 root         (0) root         (0)     4845 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py
--rw-rw-rw-   0 root         (0) root         (0)     5041 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/LogErr.py
--rw-rw-rw-   0 root         (0) root         (0)     6763 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)    14189 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ProductionData.py
--rw-rw-rw-   0 root         (0) root         (0)     4667 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ResolveSE.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/RunApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     3810 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLErr.py
--rw-rw-rw-   0 root         (0) root         (0)    23487 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py
--rw-rw-rw-   0 root         (0) root         (0)     4029 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.009640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py
--rw-rw-rw-   0 root         (0) root         (0)    21804 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py
--rw-rw-rw-   0 root         (0) root         (0)     4771 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py
--rw-rw-rw-   0 root         (0) root         (0)      885 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.012640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4387 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_architecture.py
--rwxrwxrwx   0 root         (0) root         (0)     1972 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     5967 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py
--rwxrwxrwx   0 root         (0) root         (0)     2958 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py
--rwxrwxrwx   0 root         (0) root         (0)     2648 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py
--rwxrwxrwx   0 root         (0) root         (0)     8040 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_loop.py
--rwxrwxrwx   0 root         (0) root         (0)     1601 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.012640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.015640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    14583 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    10773 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    15521 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.016640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-rw-rw-   0 root         (0) root         (0)     4512 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    64458 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    36134 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    29277 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9366 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.018640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    24689 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py
--rw-rw-rw-   0 root         (0) root         (0)    21905 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py
--rw-rw-rw-   0 root         (0) root         (0)    61334 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py
--rw-rw-rw-   0 root         (0) root         (0)    24499 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py
--rwxrwxrwx   0 root         (0) root         (0)    20145 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py
--rw-rw-rw-   0 root         (0) root         (0)     3539 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py
--rwxrwxrwx   0 root         (0) root         (0)    27390 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py
--rw-rw-rw-   0 root         (0) root         (0)    89812 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.019640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/test/
--rw-rw-rw-   0 root         (0) root         (0)     6621 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.020640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)    15896 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql
--rw-rw-rw-   0 root         (0) root         (0)    52321 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql
--rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.021640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     3124 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py
--rw-rw-rw-   0 root         (0) root         (0)     6906 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    16266 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    11871 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.022640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     2892 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.022640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.023640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/
--rw-rw-rw-   0 root         (0) root         (0)     6116 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.030640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2049 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
--rwxrwxrwx   0 root         (0) root         (0)     3160 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py
--rwxrwxrwx   0 root         (0) root         (0)     3026 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py
--rwxrwxrwx   0 root         (0) root         (0)     3631 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py
--rwxrwxrwx   0 root         (0) root         (0)     3885 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py
--rwxrwxrwx   0 root         (0) root         (0)     4627 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py
--rwxrwxrwx   0 root         (0) root         (0)     2424 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py
--rwxrwxrwx   0 root         (0) root         (0)    10410 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py
--rwxrwxrwx   0 root         (0) root         (0)     2470 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py
--rwxrwxrwx   0 root         (0) root         (0)     5753 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py
--rwxrwxrwx   0 root         (0) root         (0)     1684 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py
--rwxrwxrwx   0 root         (0) root         (0)     2409 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py
--rwxrwxrwx   0 root         (0) root         (0)     1684 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     1858 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py
--rwxrwxrwx   0 root         (0) root         (0)     2455 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py
--rwxrwxrwx   0 root         (0) root         (0)     1993 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py
--rwxrwxrwx   0 root         (0) root         (0)     2159 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     1752 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py
--rwxrwxrwx   0 root         (0) root         (0)     1733 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py
--rwxrwxrwx   0 root         (0) root         (0)     1744 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
--rwxrwxrwx   0 root         (0) root         (0)     2171 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
--rwxrwxrwx   0 root         (0) root         (0)     2482 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py
--rwxrwxrwx   0 root         (0) root         (0)     1953 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py
--rwxrwxrwx   0 root         (0) root         (0)     1874 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py
--rwxrwxrwx   0 root         (0) root         (0)     1851 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py
--rwxrwxrwx   0 root         (0) root         (0)     1873 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py
--rwxrwxrwx   0 root         (0) root         (0)    22127 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.030640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.031639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     2582 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.031639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.032640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/
--rwxrwxrwx   0 root         (0) root         (0)    42727 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py
--rw-rw-rw-   0 root         (0) root         (0)    40074 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/DiracProduction.py
--rwxrwxrwx   0 root         (0) root         (0)    26765 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/LHCbJob.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.033640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/test/
--rw-rw-rw-   0 root         (0) root         (0)     1722 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.038639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1145 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py
--rwxrwxrwx   0 root         (0) root         (0)     2841 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py
--rwxrwxrwx   0 root         (0) root         (0)     1718 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     2184 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py
--rwxrwxrwx   0 root         (0) root         (0)     2058 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py
--rwxrwxrwx   0 root         (0) root         (0)     2968 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     1999 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py
--rwxrwxrwx   0 root         (0) root         (0)     1887 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py
--rwxrwxrwx   0 root         (0) root         (0)     1783 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     1824 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py
--rwxrwxrwx   0 root         (0) root         (0)     1835 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py
--rwxrwxrwx   0 root         (0) root         (0)     1718 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py
--rwxrwxrwx   0 root         (0) root         (0)     1967 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py
--rwxrwxrwx   0 root         (0) root         (0)     2859 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py
--rwxrwxrwx   0 root         (0) root         (0)     1777 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py
--rwxrwxrwx   0 root         (0) root         (0)     1726 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.038639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.040639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    12249 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9490 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    27798 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    13625 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    44203 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     4656 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py
--rwxrwxrwx   0 root         (0) root         (0)      858 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.041639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/
--rw-rw-rw-   0 root         (0) root         (0)    10086 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py
--rw-rw-rw-   0 root         (0) root         (0)    16063 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9518 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.043640 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/
--rw-rw-rw-   0 root         (0) root         (0)    11609 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py
--rw-rw-rw-   0 root         (0) root         (0)     2105 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py
--rw-rw-rw-   0 root         (0) root         (0)    38156 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py
--rw-rw-rw-   0 root         (0) root         (0)    36845 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py
--rw-rw-rw-   0 root         (0) root         (0)    44341 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py
--rwxrwxrwx   0 root         (0) root         (0)      859 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.044639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/
--rw-rw-rw-   0 root         (0) root         (0)     1344 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py
--rw-rw-rw-   0 root         (0) root         (0)    97546 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py
--rw-rw-rw-   0 root         (0) root         (0)      864 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.048639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)    22135 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.sql
--rw-rw-rw-   0 root         (0) root         (0)     6783 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py
--rw-rw-rw-   0 root         (0) root         (0)     2294 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py
--rw-rw-rw-   0 root         (0) root         (0)     4118 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py
--rw-rw-rw-   0 root         (0) root         (0)     3866 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py
--rw-rw-rw-   0 root         (0) root         (0)     4301 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py
--rw-rw-rw-   0 root         (0) root         (0)    64737 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py
--rw-rw-rw-   0 root         (0) root         (0)     4189 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql
--rwxrwxrwx   0 root         (0) root         (0)      855 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.048639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/
--rw-rw-rw-   0 root         (0) root         (0)    25169 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.049639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     2271 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    14372 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    11119 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py
--rwxrwxrwx   0 root         (0) root         (0)      860 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.049639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2148 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.051639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/
--rw-rw-rw-   0 root         (0) root         (0)    15147 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py
--rw-rw-rw-   0 root         (0) root         (0)     9682 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py
--rw-rw-rw-   0 root         (0) root         (0)    15838 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py
--rw-rw-rw-   0 root         (0) root         (0)     8050 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/Sprucing_run.py
--rw-rw-rw-   0 root         (0) root         (0)     9633 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py
--rw-rw-rw-   0 root         (0) root         (0)    15180 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.053639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py
--rw-rw-rw-   0 root         (0) root         (0)    14396 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     6638 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py
--rw-rw-rw-   0 root         (0) root         (0)     5772 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py
--rw-rw-rw-   0 root         (0) root         (0)     9027 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.053639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/
--rw-rw-rw-   0 root         (0) root         (0)     3617 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/Test_production_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.054639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/
--rw-rw-rw-   0 root         (0) root         (0)     1848 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/ana_prod_1.yaml
--rw-rw-rw-   0 root         (0) root         (0)    32688 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/mc_1.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2746 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_1.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2062 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_2.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2156 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_3.yaml
--rwxrwxrwx   0 root         (0) root         (0)      852 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.055639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11476 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py
--rw-rw-rw-   0 root         (0) root         (0)     6931 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py
--rwxrwxrwx   0 root         (0) root         (0)    17423 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.056639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.057639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     2980 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9585 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     9662 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.058639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/
--rw-rw-rw-   0 root         (0) root         (0)     3837 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     3789 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.059639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/
--rw-rw-rw-   0 root         (0) root         (0)     2213 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)     5161 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.060639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.061639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/
--rw-rw-rw-   0 root         (0) root         (0)     8650 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py
--rw-rw-rw-   0 root         (0) root         (0)     2119 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py
--rw-rw-rw-   0 root         (0) root         (0)     2332 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.061639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/test/
--rw-rw-rw-   0 root         (0) root         (0)    28983 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py
--rw-rw-rw-   0 root         (0) root         (0)     4938 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.062639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.062639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/test/
--rw-rw-rw-   0 root         (0) root         (0)     8294 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.063639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.066639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)    19638 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    17711 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    17686 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     3540 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py
--rwxrwxrwx   0 root         (0) root         (0)     7069 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    99012 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py
--rwxrwxrwx   0 root         (0) root         (0)     6013 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
--rwxrwxrwx   0 root         (0) root         (0)      852 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.067639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/
--rw-rw-rw-   0 root         (0) root         (0)    14547 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    14181 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     5456 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py
--rw-rw-rw-   0 root         (0) root         (0)    20751 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.068639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.069639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/
--rw-rw-rw-   0 root         (0) root         (0)     3797 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py
--rw-rw-rw-   0 root         (0) root         (0)     5044 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py
--rw-rw-rw-   0 root         (0) root         (0)     5483 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py
--rw-rw-rw-   0 root         (0) root         (0)     5820 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py
--rw-rw-rw-   0 root         (0) root         (0)    95494 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py
--rwxrwxrwx   0 root         (0) root         (0)      934 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.070639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/test/
--rw-rw-rw-   0 root         (0) root         (0)    13054 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.071639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/
--rwxrwxrwx   0 root         (0) root         (0)    34602 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py
--rwxrwxrwx   0 root         (0) root         (0)     4120 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql
--rwxrwxrwx   0 root         (0) root         (0)      930 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.071639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
--rw-rw-rw-   0 root         (0) root         (0)    13013 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py
--rwxrwxrwx   0 root         (0) root         (0)      935 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.073639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)     5149 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py
--rw-rw-rw-   0 root         (0) root         (0)    87796 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.073639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/test/
--rw-rw-rw-   0 root         (0) root         (0)     3310 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py
--rwxrwxrwx   0 root         (0) root         (0)      927 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.078639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9400 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py
--rwxrwxrwx   0 root         (0) root         (0)    16558 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py
--rwxrwxrwx   0 root         (0) root         (0)     2479 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py
--rwxrwxrwx   0 root         (0) root         (0)     6835 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
--rwxrwxrwx   0 root         (0) root         (0)     6904 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py
--rwxrwxrwx   0 root         (0) root         (0)     1637 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py
--rwxrwxrwx   0 root         (0) root         (0)    21894 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py
--rwxrwxrwx   0 root         (0) root         (0)     4906 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
--rwxrwxrwx   0 root         (0) root         (0)     1773 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
--rwxrwxrwx   0 root         (0) root         (0)     1721 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
--rwxrwxrwx   0 root         (0) root         (0)     3127 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py
--rwxrwxrwx   0 root         (0) root         (0)     5972 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py
--rwxrwxrwx   0 root         (0) root         (0)     2651 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py
--rwxrwxrwx   0 root         (0) root         (0)     5057 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py
--rw-rw-rw-   0 root         (0) root         (0)     3621 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py
--rwxrwxrwx   0 root         (0) root         (0)     5390 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py
--rwxrwxrwx   0 root         (0) root         (0)     2734 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.078639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.084639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/
--rw-rw-rw-   0 root         (0) root         (0)     7856 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py
--rw-rw-rw-   0 root         (0) root         (0)    10256 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py
--rw-rw-rw-   0 root         (0) root         (0)    19732 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py
--rw-rw-rw-   0 root         (0) root         (0)     3055 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py
--rw-rw-rw-   0 root         (0) root         (0)     6567 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     5744 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/FileUsage.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py
--rw-rw-rw-   0 root         (0) root         (0)     5050 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/MergeMDF.py
--rw-rw-rw-   0 root         (0) root         (0)    47262 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)     9180 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py
--rw-rw-rw-   0 root         (0) root         (0)     4732 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py
--rw-rw-rw-   0 root         (0) root         (0)    16006 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadMC.py
--rw-rw-rw-   0 root         (0) root         (0)    21200 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py
--rw-rw-rw-   0 root         (0) root         (0)    15380 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py
--rwxrwxrwx   0 root         (0) root         (0)      838 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12324 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.086639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/
--rw-rw-rw-   0 root         (0) root         (0)     2784 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py
--rw-rw-rw-   0 root         (0) root         (0)     2397 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py
--rw-rw-rw-   0 root         (0) root         (0)     5275 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py
--rw-rw-rw-   0 root         (0) root         (0)    16821 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py
--rw-rw-rw-   0 root         (0) root         (0)    10434 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.087639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml
--rw-rw-rw-   0 root         (0) root         (0)     2185 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.088639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.088639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/
--rw-rw-rw-   0 root         (0) root         (0)     5420 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.089639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/
--rw-rw-rw-   0 root         (0) root         (0)     1281 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql
--rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.090639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Service/
--rw-rw-rw-   0 root         (0) root         (0)    15971 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.090639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.091639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Utilities/
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20517 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Workflow.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-15 16:00:02.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-15 16:00:24.091639 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2964 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28949 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    11341 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-15 16:00:22.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-15 16:00:23.000000 LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.408291 LHCbDIRAC-12.0.0a6/
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-02-21 18:07:04.408291 LHCbDIRAC-12.0.0a6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/lhcbdirac.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)    12745 2024-02-21 18:07:04.410291 LHCbDIRAC-12.0.0a6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.263291 LHCbDIRAC-12.0.0a6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.279291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.281291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.281291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.283291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2201 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.283291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2457 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.284291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.285291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/
+-rw-rw-rw-   0 root         (0) root         (0)    17746 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    26536 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10573 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    26244 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15013 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.287291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/
+-rw-rw-rw-   0 root         (0) root         (0)    29758 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    16810 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)    34147 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.287291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.290291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    39138 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py
+-rw-rw-rw-   0 root         (0) root         (0)    21141 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     4744 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6597 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    18511 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)    81681 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py
+-rw-rw-rw-   0 root         (0) root         (0)    72651 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.291291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BKQuery.py
+-rw-rw-rw-   0 root         (0) root         (0)     6316 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35461 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.295291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     3003 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)   245595 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py
+-rw-rw-rw-   0 root         (0) root         (0)    12515 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py
+-rw-rw-rw-   0 root         (0) root         (0)    16403 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     4036 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)      842 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2967 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql
+-rw-rw-rw-   0 root         (0) root         (0)    29670 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4705 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql
+-rw-rw-rw-   0 root         (0) root         (0)    12638 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql
+-rw-rw-rw-   0 root         (0) root         (0)    88601 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql
+-rw-rw-rw-   0 root         (0) root         (0)    19607 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.297291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/
+-rw-rw-rw-   0 root         (0) root         (0)    14289 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.298291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5893 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py
+-rw-rw-rw-   0 root         (0) root         (0)     2216 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)   294418 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.299291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)    88540 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2330 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.300291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.304291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1519 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13131 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.305291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py
+-rw-rw-rw-   0 root         (0) root         (0)    30245 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.305291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/
+-rw-rw-rw-   0 root         (0) root         (0)     8426 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.316291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1155 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py
+-rwxrwxrwx   0 root         (0) root         (0)     3567 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py
+-rwxrwxrwx   0 root         (0) root         (0)     4682 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py
+-rwxrwxrwx   0 root         (0) root         (0)     4660 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py
+-rwxrwxrwx   0 root         (0) root         (0)     1704 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     2291 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py
+-rwxrwxrwx   0 root         (0) root         (0)     1954 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py
+-rwxrwxrwx   0 root         (0) root         (0)     1479 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py
+-rwxrwxrwx   0 root         (0) root         (0)     1799 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py
+-rwxrwxrwx   0 root         (0) root         (0)     9413 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py
+-rwxrwxrwx   0 root         (0) root         (0)     1610 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py
+-rwxrwxrwx   0 root         (0) root         (0)     2009 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py
+-rwxrwxrwx   0 root         (0) root         (0)     2128 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py
+-rwxrwxrwx   0 root         (0) root         (0)     2006 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py
+-rwxrwxrwx   0 root         (0) root         (0)     1871 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     2442 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py
+-rwxrwxrwx   0 root         (0) root         (0)     2003 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py
+-rwxrwxrwx   0 root         (0) root         (0)     2460 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py
+-rwxrwxrwx   0 root         (0) root         (0)     1791 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     1665 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py
+-rwxrwxrwx   0 root         (0) root         (0)     2154 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py
+-rwxrwxrwx   0 root         (0) root         (0)     6303 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py
+-rwxrwxrwx   0 root         (0) root         (0)     3242 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py
+-rwxrwxrwx   0 root         (0) root         (0)     3021 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py
+-rwxrwxrwx   0 root         (0) root         (0)     2714 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     3374 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py
+-rwxrwxrwx   0 root         (0) root         (0)     2247 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py
+-rwxrwxrwx   0 root         (0) root         (0)     3172 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     1597 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     2278 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     7961 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py
+-rwxrwxrwx   0 root         (0) root         (0)     3047 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py
+-rwxrwxrwx   0 root         (0) root         (0)    10570 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py
+-rwxrwxrwx   0 root         (0) root         (0)     2681 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     2443 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py
+-rwxrwxrwx   0 root         (0) root         (0)     4711 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py
+-rwxrwxrwx   0 root         (0) root         (0)     2580 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py
+-rwxrwxrwx   0 root         (0) root         (0)     2052 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4024 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_split_runs_for_prod.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.316291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.316291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.317291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/
+-rw-rw-rw-   0 root         (0) root         (0)     5344 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.317291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/
+-rw-rw-rw-   0 root         (0) root         (0)     9187 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.318291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4493 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.318291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.323291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     4937 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     5711 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py
+-rw-rw-rw-   0 root         (0) root         (0)    18183 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/HTML.py
+-rw-rw-rw-   0 root         (0) root         (0)     4845 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     5041 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/LogErr.py
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)    14189 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ProductionData.py
+-rw-rw-rw-   0 root         (0) root         (0)     4667 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ResolveSE.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/RunApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     3810 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLErr.py
+-rw-rw-rw-   0 root         (0) root         (0)    23413 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.324291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py
+-rw-rw-rw-   0 root         (0) root         (0)    21800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py
+-rw-rw-rw-   0 root         (0) root         (0)     4771 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py
+-rw-rw-rw-   0 root         (0) root         (0)      885 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.327291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4387 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_architecture.py
+-rwxrwxrwx   0 root         (0) root         (0)     1972 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     5967 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py
+-rwxrwxrwx   0 root         (0) root         (0)     2958 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py
+-rwxrwxrwx   0 root         (0) root         (0)     2648 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py
+-rwxrwxrwx   0 root         (0) root         (0)     8040 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_loop.py
+-rwxrwxrwx   0 root         (0) root         (0)     1601 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.327291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.330291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    14583 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    10773 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    15521 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.331291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-rw-rw-   0 root         (0) root         (0)     4512 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    64458 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    36134 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    29277 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9366 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.334291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    24689 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py
+-rw-rw-rw-   0 root         (0) root         (0)    21905 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py
+-rw-rw-rw-   0 root         (0) root         (0)    61334 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py
+-rw-rw-rw-   0 root         (0) root         (0)    24909 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py
+-rwxrwxrwx   0 root         (0) root         (0)    20145 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3539 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py
+-rwxrwxrwx   0 root         (0) root         (0)    27390 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py
+-rw-rw-rw-   0 root         (0) root         (0)    89812 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.334291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/test/
+-rw-rw-rw-   0 root         (0) root         (0)     6621 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.335291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)    15896 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql
+-rw-rw-rw-   0 root         (0) root         (0)    52321 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql
+-rw-rw-rw-   0 root         (0) root         (0)      849 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.337291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6906 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    16266 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11871 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.337291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      907 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.338291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.338291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     6116 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.346291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2049 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     3160 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py
+-rwxrwxrwx   0 root         (0) root         (0)     3026 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py
+-rwxrwxrwx   0 root         (0) root         (0)     3631 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py
+-rwxrwxrwx   0 root         (0) root         (0)     3885 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py
+-rwxrwxrwx   0 root         (0) root         (0)     4627 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py
+-rwxrwxrwx   0 root         (0) root         (0)     2424 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py
+-rwxrwxrwx   0 root         (0) root         (0)    10410 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py
+-rwxrwxrwx   0 root         (0) root         (0)     2470 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py
+-rwxrwxrwx   0 root         (0) root         (0)     5753 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1684 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     2409 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py
+-rwxrwxrwx   0 root         (0) root         (0)     1684 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1858 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py
+-rwxrwxrwx   0 root         (0) root         (0)     2455 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py
+-rwxrwxrwx   0 root         (0) root         (0)     1993 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py
+-rwxrwxrwx   0 root         (0) root         (0)     2159 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1752 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1733 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py
+-rwxrwxrwx   0 root         (0) root         (0)     1744 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     2171 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
+-rwxrwxrwx   0 root         (0) root         (0)     2482 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py
+-rwxrwxrwx   0 root         (0) root         (0)     1953 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py
+-rwxrwxrwx   0 root         (0) root         (0)     1874 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py
+-rwxrwxrwx   0 root         (0) root         (0)     1851 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py
+-rwxrwxrwx   0 root         (0) root         (0)    22127 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.346291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.346291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     2582 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.347291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.348291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/
+-rwxrwxrwx   0 root         (0) root         (0)    42727 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py
+-rw-rw-rw-   0 root         (0) root         (0)    40074 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/DiracProduction.py
+-rwxrwxrwx   0 root         (0) root         (0)    26765 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/LHCbJob.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.348291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.353291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1145 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py
+-rwxrwxrwx   0 root         (0) root         (0)     2841 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py
+-rwxrwxrwx   0 root         (0) root         (0)     1718 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     2184 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py
+-rwxrwxrwx   0 root         (0) root         (0)     2058 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py
+-rwxrwxrwx   0 root         (0) root         (0)     2968 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     1999 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py
+-rwxrwxrwx   0 root         (0) root         (0)     1887 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py
+-rwxrwxrwx   0 root         (0) root         (0)     1783 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     1824 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py
+-rwxrwxrwx   0 root         (0) root         (0)     1835 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py
+-rwxrwxrwx   0 root         (0) root         (0)     1718 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py
+-rwxrwxrwx   0 root         (0) root         (0)     1967 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py
+-rwxrwxrwx   0 root         (0) root         (0)     2859 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py
+-rwxrwxrwx   0 root         (0) root         (0)     1777 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py
+-rwxrwxrwx   0 root         (0) root         (0)     1726 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.353291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.355291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    12249 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9490 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    27798 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    13625 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    44203 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4656 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py
+-rwxrwxrwx   0 root         (0) root         (0)      858 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.356291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/
+-rw-rw-rw-   0 root         (0) root         (0)    10086 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)    16063 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9518 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.358291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/
+-rw-rw-rw-   0 root         (0) root         (0)    11609 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    38156 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)    36845 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py
+-rw-rw-rw-   0 root         (0) root         (0)    44341 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py
+-rwxrwxrwx   0 root         (0) root         (0)      859 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.359291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)    97546 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.363291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)    22135 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.sql
+-rw-rw-rw-   0 root         (0) root         (0)     6783 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py
+-rw-rw-rw-   0 root         (0) root         (0)     2294 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     4118 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     3866 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     4301 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py
+-rw-rw-rw-   0 root         (0) root         (0)    64737 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py
+-rw-rw-rw-   0 root         (0) root         (0)     4189 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql
+-rwxrwxrwx   0 root         (0) root         (0)      855 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.363291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    25169 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.364291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    14372 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11119 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py
+-rwxrwxrwx   0 root         (0) root         (0)      860 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.365291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2148 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.366291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/
+-rw-rw-rw-   0 root         (0) root         (0)    15147 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     9682 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    15838 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     8050 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/Sprucing_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     9633 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    15180 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.368291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14396 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     6638 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5772 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py
+-rw-rw-rw-   0 root         (0) root         (0)     9027 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.368291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/Test_production_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.370291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/ana_prod_1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    32688 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/mc_1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2746 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_1.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_2.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_3.yaml
+-rwxrwxrwx   0 root         (0) root         (0)      852 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.371291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11476 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py
+-rw-rw-rw-   0 root         (0) root         (0)     6931 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py
+-rwxrwxrwx   0 root         (0) root         (0)    17423 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.371291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.372291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9585 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     9662 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.373291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/
+-rw-rw-rw-   0 root         (0) root         (0)     3837 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.374291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)     5161 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.375291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.376291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/
+-rw-rw-rw-   0 root         (0) root         (0)     8650 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2119 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2332 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.376291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/test/
+-rw-rw-rw-   0 root         (0) root         (0)    28983 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py
+-rw-rw-rw-   0 root         (0) root         (0)     4938 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.377291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.377291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/test/
+-rw-rw-rw-   0 root         (0) root         (0)     8294 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.378291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.380291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)    19638 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    17711 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    11910 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    17686 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py
+-rwxrwxrwx   0 root         (0) root         (0)     7069 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    99012 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py
+-rwxrwxrwx   0 root         (0) root         (0)     6013 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
+-rwxrwxrwx   0 root         (0) root         (0)      852 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.382291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/
+-rw-rw-rw-   0 root         (0) root         (0)    14547 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    14181 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5456 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)    20751 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.383291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.384291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3797 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py
+-rw-rw-rw-   0 root         (0) root         (0)     5044 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5483 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5820 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py
+-rw-rw-rw-   0 root         (0) root         (0)    95494 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py
+-rwxrwxrwx   0 root         (0) root         (0)      934 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.385291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/test/
+-rw-rw-rw-   0 root         (0) root         (0)    13054 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.385291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/
+-rwxrwxrwx   0 root         (0) root         (0)    34602 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py
+-rwxrwxrwx   0 root         (0) root         (0)     4120 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql
+-rwxrwxrwx   0 root         (0) root         (0)      930 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.386291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    13013 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py
+-rwxrwxrwx   0 root         (0) root         (0)      935 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.387291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    87796 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.388291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3310 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py
+-rwxrwxrwx   0 root         (0) root         (0)      927 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.393291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9400 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py
+-rwxrwxrwx   0 root         (0) root         (0)    16558 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py
+-rwxrwxrwx   0 root         (0) root         (0)     2479 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py
+-rwxrwxrwx   0 root         (0) root         (0)     6835 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
+-rwxrwxrwx   0 root         (0) root         (0)     6904 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py
+-rwxrwxrwx   0 root         (0) root         (0)     1638 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py
+-rwxrwxrwx   0 root         (0) root         (0)    21894 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)     4906 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     1773 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
+-rwxrwxrwx   0 root         (0) root         (0)     1721 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
+-rwxrwxrwx   0 root         (0) root         (0)     3127 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py
+-rwxrwxrwx   0 root         (0) root         (0)     5972 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2651 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py
+-rwxrwxrwx   0 root         (0) root         (0)     5057 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     3621 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py
+-rwxrwxrwx   0 root         (0) root         (0)     5390 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py
+-rwxrwxrwx   0 root         (0) root         (0)     2734 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.393291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.398291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/
+-rw-rw-rw-   0 root         (0) root         (0)     7856 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py
+-rw-rw-rw-   0 root         (0) root         (0)    19732 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py
+-rw-rw-rw-   0 root         (0) root         (0)     3055 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6567 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5744 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/FileUsage.py
+-rwxrwxrwx   0 root         (0) root         (0)     8615 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    47262 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     9180 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     5539 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py
+-rw-rw-rw-   0 root         (0) root         (0)    16003 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    11505 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    20952 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    15380 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py
+-rwxrwxrwx   0 root         (0) root         (0)      838 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.403291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/
+-rw-rw-rw-   0 root         (0) root         (0)     9013 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_AnalyseFileAccess.py
+-rw-rw-rw-   0 root         (0) root         (0)    23485 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_AnalyseXMLSummary.py
+-rw-rw-rw-   0 root         (0) root         (0)    24875 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py
+-rw-rw-rw-   0 root         (0) root         (0)     5674 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_CreateDataFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    17974 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ErrorLogging.py
+-rw-rw-rw-   0 root         (0) root         (0)    11129 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_FailoverRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6806 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_FileUsage.py
+-rw-rw-rw-   0 root         (0) root         (0)    70252 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py
+-rw-rw-rw-   0 root         (0) root         (0)     4291 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbScript.py
+-rw-rw-rw-   0 root         (0) root         (0)    17001 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py
+-rw-rw-rw-   0 root         (0) root         (0)     6662 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_RemoveInputData.py
+-rw-rw-rw-   0 root         (0) root         (0)     8955 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_StepAccounting.py
+-rw-rw-rw-   0 root         (0) root         (0)    16960 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadLogFile.py
+-rw-rw-rw-   0 root         (0) root         (0)    13803 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py
+-rw-rw-rw-   0 root         (0) root         (0)    26151 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadOutputData.py
+-rw-rw-rw-   0 root         (0) root         (0)    15279 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UserJobFinalization.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    12324 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/mock_Commons.py
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.404291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.404291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/
+-rw-rw-rw-   0 root         (0) root         (0)     5420 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.405291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql
+-rw-rw-rw-   0 root         (0) root         (0)      853 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.406291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.406291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20517 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-21 18:06:42.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 18:07:04.407291 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29154 2024-02-21 18:07:04.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    11341 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-02-21 18:07:03.000000 LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/top_level.txt
```

### Comparing `LHCbDIRAC-12.0.0a5/CONTRIBUTING.md` & `LHCbDIRAC-12.0.0a6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/LICENSE` & `LHCbDIRAC-12.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/PKG-INFO` & `LHCbDIRAC-12.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbDIRAC
-Version: 12.0.0a5
+Version: 12.0.0a6
 Summary: LHCbDIRAC is the LHCb extension of DIRAC
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbDIRAC-12.0.0a5/README.rst` & `LHCbDIRAC-12.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/setup.cfg` & `LHCbDIRAC-12.0.0a6/setup.cfg`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/DataStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/JobStep.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/Popularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/Storage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/UserStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/Types/test/Test_AS_Client_Types_DataStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/DataStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/JobStepPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/PopularityPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/StoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/UserStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_DataStoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_JobStepPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_PopularityPlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/Plotters/test/Test_AS_private_Plotters_StoragePlotter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/AccountingSystem/private/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/AccountingSystem/private/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/BKQuery.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,18 +231,23 @@
             bk = bkPath.split("/")[1:] + len(bkFields) * [""]
             for bpath in bk:
                 gLogger.verbose(
                     "buildBKQuery.1. Item #%d, Field %s, From Path %s, ProcessingPass %s"
                     % (i, bkFields[i], bpath, processingPass)
                 )
                 if bkFields[i] == "ProcessingPass":
+                    # TODO: This should be refactored to be more robust
                     if (
                         bpath != ""
                         and bpath.upper() != "ALL"
-                        and not bpath.split(",")[0].split(" ")[0].isdigit()
+                        and not (
+                            # Event types are always 8 digits
+                            bpath.split(",")[0].split(" ")[0].isdigit()
+                            and len(bpath.split(",")[0].split(" ")[0]) >= 8
+                        )
                         and not bpath.upper() in self.__bkFileTypes
                     ):
                         processingPass = os.path.join(processingPass, bpath)
                         continue
                     # Set the PP
                     if processingPass != "/":
                         bkQuery["ProcessingPass"] = processingPass
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/Help.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1835,15 +1835,15 @@
                         string += f"{self.comment} {i[0]} : {i[1]} \n"
         return string
 
     #############################################################################
     @staticmethod
     def __createFormatString(filesandformats):
         """It generates the Root format option file."""
-        string = "\nfrom Gaudi.Configuration import * "
+        string = "\nfrom Gaudi.Configuration import *"
         string += "\nfrom GaudiConf import IOHelper\n"
         for fileFormat, lfns in filesandformats.items():
             if fileFormat:
                 string += f"IOHelper('{fileFormat}').inputFiles([\n"
             else:
                 string += "IOHelper().inputFiles([\n"
             string += "\n".join(f"'LFN:{lfn}'," for lfn in lfns)
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/objects.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -1164,14 +1164,15 @@
         runnumbers=None,
         startRunID=None,
         endRunID=None,
         tcks=default,
         jobStart=None,
         jobEnd=None,
         selection=None,
+        smog2States=None,
     ):
         """For retrieving files with meta data.
 
         :param str configName: configuration name
         :param str configVersion: configuration version
         :param str conddescription: data taking or simulation description
         :param str processing: processing pass
@@ -1247,14 +1248,19 @@
             return retVal
         condition, tables = retVal["Value"]
 
         condition, tables = self.__buildEventType(evt, condition, tables, useMainTables=False)
 
         condition, tables = self.__buildFileTypes(filetype, condition, tables, useMainTables=False)
 
+        retVal = self._buildSMOG2Conditions(smog2States, condition, tables)
+        if not retVal["OK"]:
+            return retVal
+        condition, tables = retVal["Value"]
+
         command = (
             "SELECT %s FROM %s WHERE j.jobid=f.jobid AND ft.filetypeid=f.filetypeid AND f.qualityid=d.qualityid %s"
             % (selection, tables, condition)
         )
         return self.dbR_.query(command)
 
     #############################################################################
@@ -3557,14 +3563,15 @@
         runnumbers=None,
         replicaFlag=default,
         visible=default,
         filesize=False,
         tcks=None,
         jobStart=None,
         jobEnd=None,
+        smog2States=None,
     ):
         """returns a list of lfns.
 
         :param str simdesc: simulation condition description
         :param str datataking: data taking condition description
         :pram str procPass: processing pass
         :param str ftype: file type
@@ -3634,14 +3641,19 @@
         condition, tables = self.__buildVisibilityflag(visible, condition, tables)
 
         retVal = self._buildConditions(simdesc, datataking, condition, tables)
         if not retVal["OK"]:
             return retVal
         condition, tables = retVal["Value"]
 
+        retVal = self._buildSMOG2Conditions(smog2States, condition, tables)
+        if not retVal["OK"]:
+            return retVal
+        condition, tables = retVal["Value"]
+
         # hint = ''
         # if (not startDate and not endDate) and tables.strip() == 'files f,jobs j  ,filetypes ft':
         #  hint = '/*+INDEX(j JOBS_PRODUCTIONID) INDEX(f FILES_JOB_EVENT_FILETYPE) INDEX(ft FILETYPES_ID_NAME)*/'
 
         if nbofEvents:
             command = f"SELECT SUM(f.eventstat) FROM {tables} WHERE f.jobid= j.jobid {condition} "
         elif filesize:
@@ -4060,14 +4072,80 @@
             condition += retVal["Value"]
             if tables.upper().find("PRODUCTIONSCONTAINER") < 0:
                 tables += " , productionscontainer cont "
 
         return S_OK((condition, tables))
 
     #############################################################################
+    def _SMOG2States2SQL(self, smog2States):
+        """convert the list of possible states (or "Undefined") into SQL conditions.
+
+        :param list[str]: smog2state: the list of states, assumes OR.
+        """
+        if type(smog2States) is not list:
+            return S_ERROR("incorrect SMOG2 type, expected a list of strings")
+        cond = ",".join([f"'{state}'" for state in smog2States if state != "Undefined"])
+        if cond != "":
+            cond = f"(s2s.state in ({cond}))"
+        if "Undefined" in smog2States:
+            if cond != "":
+                cond = f" AND (s2s.id IS NULL OR {cond})"
+            else:
+                cond = " AND s2s.id IS NULL"
+        elif cond != "":
+            cond = f" AND {cond}"
+        return S_OK(f" AND runs.smog2_id = s2s.id (+) {cond}")
+
+    #############################################################################
+    def _buildSMOG2Conditions(self, smog2States, condition, tables):
+        """adds SMOG2 state condition to the query.
+        WARNING: depends from the previously defined conditions!
+        At the moment can be called ONLY from:
+            getFiles()
+            getFilesWithMetadata()
+            getFilesSummary()
+
+        :param list[str] smog2states: a list of SMOG2 states
+        """
+        if not smog2States:
+            return S_OK((condition, tables))  # don't wake the sleeping bear...
+
+        # we need the reference to runnumber, which explicitly exists in:
+        #   runstatus - O(runs*1), not used in targeted functions
+        #   newrunquality - O(runs*n), not used in targeted functions
+        #   prodrunview - O(prods = runs*m)
+        #   jobs - O(inf), has runnumber index, but partitioned by production
+        # note that some tables specify production only
+        #   productionscontainer - O(prods)
+        #   stepscontainer - O(prods*k)
+        #   productionoutputfiles - O(prods*l)
+        # and production in general works with many runs.
+        #
+        # So runs.smog2_id link shuld be jobs.runnumber = runs.runnumber (+) (AND state conditions),
+        # LEFT (OUTER) JOINT allows deal with "Undefined" case.
+        #
+        # If SMOG2= has to work in not jobs based (f.e. production) queries, that should
+        # be implemented separately, with proper grouping (f.e. prodrunview can easily
+        # multiply results and it is updated asyncroneously to file registration)
+
+        if not tables or "jobs j" not in tables.lower():
+            raise RuntimeError("No jobs to join SMOG2, exiting...")
+        if condition is None:
+            condition = ""  # all jobs for SMOG2 conditions... the list can be long...
+        condRet = self._SMOG2States2SQL(smog2States)
+        if not condRet["OK"]:
+            return condRet
+        if "smog2" not in tables.lower():
+            tables += " , smog2 s2s"
+        if "runs" not in tables.lower():
+            tables += " , runs"
+        condition += f" AND j.runnumber = runs.runnumber (+) {condRet['Value']} "
+        return S_OK((condition, tables))
+
+    #############################################################################
     def getVisibleFilesWithMetadata(
         self,
         simdesc,
         datataking,
         procPass,
         ftype,
         evt,
@@ -4154,14 +4232,15 @@
         startDate=None,
         endDate=None,
         runNumbers=None,
         replicaFlag=default,
         tcks=default,
         jobStart=None,
         jobEnd=None,
+        smog2States=None,
     ):
         """File summary for a given data set.
 
         :param str configName: configuration name
         :param str configVersion: configuration version
         :param str conddescription: simulation or data taking condition
         :param str processingPass: processing pass
@@ -4232,14 +4311,19 @@
         condition, tables = retVal["Value"]
 
         retVal = self.__buildDataquality(dataQuality, condition, tables)
         if not retVal["OK"]:
             return retVal
         condition, tables = retVal["Value"]
 
+        retVal = self._buildSMOG2Conditions(smog2States, condition, tables)
+        if not retVal["OK"]:
+            return retVal
+        condition, tables = retVal["Value"]
+
         command = (
             "SELECT COUNT(DISTINCT fileid), \
 SUM(f.EventStat), SUM(f.FILESIZE), \
 SUM(f.luminosity),SUM(f.instLuminosity) FROM  %s WHERE \
 j.jobid=f.jobid AND \
 prod.production=cont.production AND prod.filetypeid=f.filetypeid %s"
             % (tables, condition)
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,12 @@
 ###############################################################################
-# (c) Copyright 2023 CERN for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2019 CERN for the benefit of the LHCb Collaboration           #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-from DIRAC import gLogger
-from DIRAC.Core.Utilities.ReturnValues import DReturnType
-
-
-class NewOracleBookkeepingDB:
-    def __init__(self, *, dbW, dbR):
-        self.log = gLogger.getSubLogger("LegacyOracleBookkeepingDB")
-        self.dbW_ = dbW
-        self.dbR_ = dbR
-
-    def getAvailableFileTypes(self) -> DReturnType[list[str]]:
-        """Retrieve all available file types from the database."""
-        return self.dbR_.executeStoredProcedure("BOOKKEEPINGORACLEDB.getAvailableFileTypes", [])
+"""LHCbDIRAC.TransformationSystem package."""
+################################################################################
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/OracleDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/admin_tools.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema.sql`

 * *Files 4% similar despite different names*

```diff
@@ -319,14 +319,53 @@
 
 INSERT INTO dataquality (qualityid,dataqualityflag) SELECT 1,'UNCHECKED' FROM dual WHERE NOT EXISTS (SELECT * FROM dataquality WHERE (qualityid = 1 AND dataqualityflag = 'UNCHECKED'));
 INSERT INTO dataquality (qualityid,dataqualityflag) SELECT 2,'OK' FROM dual WHERE NOT EXISTS (SELECT * FROM dataquality WHERE (qualityid = 2 AND dataqualityflag = 'OK'));
 INSERT INTO dataquality (qualityid,dataqualityflag) SELECT 3,'BAD' FROM dual WHERE NOT EXISTS (SELECT * FROM dataquality WHERE (qualityid = 3 AND dataqualityflag = 'BAD'));
 COMMIT;
 
 ---------------------------------------------------------------------------------------
+CREATE TABLE smog2(
+    id       NUMBER,
+    state varchar2(64),
+    PRIMARY KEY (id)
+);
+
+CREATE INDEX smog2_state ON smog2 (state);
+INSERT INTO smog2 (id,state) VALUES (0,'Unknown');
+INSERT INTO smog2 (id,state) VALUES (1,'NoGas');
+INSERT INTO smog2 (id,state) VALUES (2,'Hydrogen');
+INSERT INTO smog2 (id,state) VALUES (3,'HydrogenUnstable');
+INSERT INTO smog2 (id,state) VALUES (4,'Deuterium');
+INSERT INTO smog2 (id,state) VALUES (5,'DeuteriumUnstable');
+INSERT INTO smog2 (id,state) VALUES (6,'Helium');
+INSERT INTO smog2 (id,state) VALUES (7,'HeliumUnstable');
+INSERT INTO smog2 (id,state) VALUES (8,'Nitrogen');
+INSERT INTO smog2 (id,state) VALUES (9,'NitrogenUnstable');
+INSERT INTO smog2 (id,state) VALUES (10,'Oxygen');
+INSERT INTO smog2 (id,state) VALUES (11,'OxygenUnstable');
+INSERT INTO smog2 (id,state) VALUES (12,'Neon');
+INSERT INTO smog2 (id,state) VALUES (13,'NeonUnstable');
+INSERT INTO smog2 (id,state) VALUES (14,'Argon');
+INSERT INTO smog2 (id,state) VALUES (15,'ArgonUnstable');
+INSERT INTO smog2 (id,state) VALUES (16,'Krypton');
+INSERT INTO smog2 (id,state) VALUES (17,'KryptonUnstable');
+INSERT INTO smog2 (id,state) VALUES (18,'Xenon');
+INSERT INTO smog2 (id,state) VALUES (19,'XenonUnstable');
+COMMIT;
+
+---------------------------------------------------------------------------------------
+CREATE TABLE runs(
+    runnumber       NUMBER,
+    smog2_id    NUMBER,
+    PRIMARY KEY (runnumber),
+    CONSTRAINT fk_runs_smog2_id FOREIGN KEY (smog2_id) REFERENCES smog2 (id)
+);
+CREATE INDEX runs_smog2_id ON runs (smog2_id);
+
+---------------------------------------------------------------------------------------
 CREATE TABLE eventtypes(
     description   varchar2(256),
     eventtypeid   NUMBER,
     PRIMARY       varchar2(256),
     PRIMARY KEY (eventtypeid)
 );
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/database_schema_cleaner.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/monitoring.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_schema_storedprocedures.sql`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 PROCEDURE updateluminosity(v_runnumber NUMBER);
 PROCEDURE updatedesluminosity(v_fileid NUMBER);
 PROCEDURE getfiledesjobid(v_filename VARCHAR2, a_cursor OUT udt_refcursor);
 FUNCTION getproducedevents(v_prodid NUMBER) RETURN NUMBER;
 PROCEDURE bulkgetidsfromfiles(lfns varchararray, a_cursor OUT udt_refcursor);
 PROCEDURE insertprodnoutputftypes(v_production NUMBER, v_stepid NUMBER, v_filetypeid NUMBER, v_visible char, v_eventtype NUMBER);
 FUNCTION getjobidwithoutreplicacheck(v_filename VARCHAR2) RETURN NUMBER;
+PROCEDURE setsmog2 (v_state VARCHAR2, v_update BOOLEAN, v_runs numberarray);
 END;
  /
 
 
 CREATE OR REPLACE PACKAGE BODY bookkeepingoracledb AS
 
 -------------------------------------------------------------------------------------------------------------------------------
@@ -2052,9 +2053,36 @@
     WHERE
       files.jobid = jobs.jobid AND
       files.filename = v_filename;
     RETURN (jid);
     EXCEPTION WHEN others THEN
   RETURN 0;
   END;
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------
+PROCEDURE setsmog2 (v_state VARCHAR2, v_update BOOLEAN, v_runs numberarray) IS
+v_stateid NUMBER := 0;
+v_cstateid NUMBER := 0;
+BEGIN
+  BEGIN
+    SELECT id INTO v_stateid FROM smog2 WHERE state = v_state;
+  EXCEPTION WHEN NO_DATA_FOUND THEN
+    raise_application_error(-20006, 'SMOG2 state ' || v_state || ' is unknown');
+  END;
+  FOR i IN v_runs.first .. v_runs.last LOOP
+    BEGIN
+      INSERT INTO runs (runnumber, smog2_id) VALUES (v_runs(i), v_stateid);
+    EXCEPTION WHEN dup_val_on_index THEN
+      SELECT smog2_id INTO v_cstateid FROM runs WHERE runnumber = v_runs(i);
+      IF v_cstateid != v_stateid THEN
+        IF v_update THEN
+          UPDATE runs SET smog2_id = v_stateid WHERE runnumber = v_runs(i);
+        ELSE
+          raise_application_error(-20007, 'Run ' || v_runs(i) || ' has different SMOG2 state');
+        END IF;
+      END IF; -- ELSE the state is the same
+    END;
+  END LOOP;
+  COMMIT;
+END;
+
 END;
 /
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/oracle_utilities_stored_procedures.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BKK_DB_OracleBookkeepingDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_filetypes.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/Test_proxying.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_BookkeepingDB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/Test_conditionString.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/conftest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/DB/test/dtc.json`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/BookkeepingManagerHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,14 +498,15 @@
             runNbs = [runNbs]
         replicaFlag = in_dict.get("ReplicaFlag", "Yes")
         visible = in_dict.get("Visible", default)
         filesize = in_dict.get("FileSize", False)
         tck = in_dict.get("TCK", [])
         jobStart = in_dict.get("JobStartDate", None)
         jobEnd = in_dict.get("JobEndDate", None)
+        smog2States = in_dict.get("SMOG2", None)
 
         if "ProductionID" in in_dict:
             cls.log.verbose("ProductionID will be removed. It will changed to Production")
 
         if "DataQualityFlag" in in_dict:
             cls.log.verbose("DataQualityFlag will be removed. It will changed to DataQuality")
 
@@ -530,14 +531,15 @@
             runNbs,
             replicaFlag,
             visible,
             filesize,
             tck,
             jobStart,
             jobEnd,
+            smog2States,
         )
         if not retVal["OK"]:
             return retVal
 
         return S_OK([i[0] for i in retVal["Value"]])
 
     #############################################################################
@@ -559,14 +561,15 @@
         endDate = in_dict.get("EndDate", None)
         runnumbers = in_dict.get("RunNumber", in_dict.get("RunNumbers", []))
         startRunID = in_dict.get("StartRun", None)
         endRunID = in_dict.get("EndRun", None)
         tcks = in_dict.get("TCK")
         jobStart = in_dict.get("JobStartDate", None)
         jobEnd = in_dict.get("JobEndDate", None)
+        smog2States = in_dict.get("SMOG2", None)
 
         if "EventTypeId" in in_dict:
             cls.log.verbose("The EventTypeId has to be replaced by EventType!")
 
         if "Quality" in in_dict:
             cls.log.verbose("The Quality has to be replaced by DataQuality!")
 
@@ -585,14 +588,16 @@
             endDate,
             runnumbers,
             startRunID,
             endRunID,
             tcks,
             jobStart,
             jobEnd,
+            None,
+            smog2States,
         )
         if not retVal["OK"]:
             return retVal
         records = []
         parameters = [
             "FileName",
             "EventStat",
@@ -679,14 +684,15 @@
         startDate = in_dict.get("StartDate", None)
         endDate = in_dict.get("EndDate", None)
         runNumbers = in_dict.get("RunNumber", in_dict.get("RunNumbers", []))
         replicaFlag = in_dict.get("ReplicaFlag", "Yes")
         tcks = in_dict.get("TCK")
         jobStart = in_dict.get("JobStartDate", None)
         jobEnd = in_dict.get("JobEndDate", None)
+        smog2States = in_dict.get("SMOG2", None)
 
         if "EventTypeId" in in_dict:
             self.log.verbose("The EventTypeId has to be replaced by EventType!")
 
         if "Quality" in in_dict:
             self.log.verbose("The Quality has to be replaced by DataQuality!")
 
@@ -705,14 +711,15 @@
             startDate=startDate,
             endDate=endDate,
             runNumbers=runNumbers,
             replicaFlag=replicaFlag,
             tcks=tcks,
             jobStart=jobStart,
             jobEnd=jobEnd,
+            smog2States=smog2States,
         )
         if not retVal["OK"]:
             return retVal
         records = []
         parameters = ["NbofFiles", "NumberOfEvents", "FileSize", "Luminosity", "InstLuminosity"]
         for record in retVal["Value"]:
             records += [[record[0], record[1], record[2], record[3], record[4]]]
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/TornadoBookkeepingManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/DataTakingConditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/File.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/FileParam.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/InputFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Job.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobConfiguration.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobOption.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/JobParameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/Quality.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/QualityParameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/SimulationConditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Job/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/JobReader.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/FileReplica.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/Replica.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/ReplicaParam.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/Replica/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/ReplicaReader.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/XMLFilesReaderManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,31 @@
         except NameError as ex:
             gLogger.error("XML reading error", filename)
             return S_ERROR(ex)
 
         return xmltype, doc, filename
 
     #############################################################################
+    @staticmethod
+    def smogInjectionSMOG2Gas(smogValue):
+        """converts RunDB/CondDB SMOG value format into BK format (currently SMOG2 only or NoGas)."""
+        fields = smogValue.split("_")
+        type = fields[0]
+        gas = fields[1] if len(fields) > 1 else ""
+        unstable = fields[2] if len(fields) > 2 else ""
+        if type == "NONE" or gas == "NONE":  # we set NoGas even when it is speicified for SMOG(1)
+            return "NoGas"
+        if type != "SMOG2":
+            return "Unknown"  # register the value, means "we know it is unknown"
+        if unstable not in ["", "Unstable"] or not gas:
+            gLogger.error(f"SMOG value '{smogValue}' has unexpected format")
+            return ""
+        return gas.capitalize() + unstable
+
+    #############################################################################
     def readXMLfromString(self, xmlString):
         """read the xml string."""
         try:
             doc = parseString(xmlString)
 
             docType = doc.doctype  # job or replica
             xmltype = docType.name
@@ -499,14 +516,23 @@
             if job.exists("DDDB"):
                 job.removeParam("DDDB")
 
             if not found:
                 self.log.error("Run number is missing!")
                 return S_ERROR("Run number is missing!")
 
+            if "SmogInjection" in datataking:
+                # "RunNumber" is checked several lines above (for production)
+                gas = self.smogInjectionSMOG2Gas(datataking["SmogInjection"])
+                if gas:
+                    retVal = self.db.setSMOG2State(gas, False, [production * -1])
+                    if not retVal["OK"]:
+                        self.log.error(f"Can't set SMOG2 state {gas} for run {production * -1}, will ignore...")
+                        # return S_ERROR("Can't set SMOG2 state for run") # TOCHANGE: Ignore till SMOG2 is checked
+
             retVal = self.db.getStepIdandNameForRUN(programName, programVersion, conddb, dddb)
 
             if not retVal["OK"]:
                 return retVal
 
             stepid = retVal["Value"][0]
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/book.dtd`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/replica.dtd`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/XMLReader/test/Test_XMLReader.py`

 * *Files 11% similar despite different names*

```diff
@@ -148,7 +148,16 @@
     xfrm = XMLFilesReaderManager()
     xfrm.db = MagicMock()
     xfrm.db.getProductionProcessingPassID.return_value = getProductionProcessingPassID_RV
     xfrm.db.getRunAndProcessingPassDataQuality.return_value = getRunAndProcessingPassDataQuality_RV
 
     res = xfrm._getDataQuality(prod, runNumber)
     assert res == expected
+
+
+def test_SMOG_Parser():
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("NONE") == "NoGas"
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("NONE_NONE") == "NoGas"
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("SMOG_ARGON") == "Unknown"
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("SMOG2_ARGON") == "Argon"
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("SMOG_HELIUM_Unstable") == "Unknown"
+    assert XMLFilesReaderManager.smogInjectionSMOG2Gas("SMOG2_HELIUM_Unstable") == "HeliumUnstable"
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_CLI.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_decays_path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_eventtype_mgt_update.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_file_path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_filetypes_list.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_fix_luminosity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_genXMLCatalog.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_conditions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_ancestors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_descendants.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_file_sisters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_processing_passes.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_run_ranges.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_runsWithAGivenDate.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_get_tck.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_getdataquality_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_job_input_output.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_prod4path.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_information.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_production_jobs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_productions_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_rejection_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_run_information.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_set_visibility.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_setdataquality_run_processing_pass.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_insert.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_simulationconditions_list.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_split_runs_for_prod.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/BookkeepingSystem/scripts/dirac_bookkeeping_split_runs_for_prod.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/Resources.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ConfigurationSystem/scripts/add_user_DFC.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/BookkeepingJobInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
             output_file.extend(
                 [ET.Element("Parameter", Name=k, Value=str(v)) for k, v in data.items() if v is not None]
             )
             root.append(output_file)
         if self.simulation_condition is not None:
             simulation_condition = ET.Element("SimulationCondition")
             simulation_condition.append(ET.Element("Parameter", Name="SimDescription", Value=self.simulation_condition))
+            root.append(simulation_condition)
         ET.indent(root, "    ")
         return b"\n".join(
             [
                 b'<?xml version="1.0" encoding="ISO-8859-1"?>\n',
                 b'<!DOCTYPE Job SYSTEM "book.dtd">\n',
                 ET.tostring(root, encoding="ISO-8859-1", method="xml", xml_declaration=False),
             ]
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/File.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/File.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/GangaDataFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/GeneratorLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,16 @@
         """converts the xml Generator Log into json format"""
         dictElements = dict()
         dictGenerator = dict()
 
         with open("GeneratorLog.xml") as fp:
             fileLines = fp.readlines()
 
-        fileLines = fileLines[fileLines.index("<generatorCounters>\n") : fileLines.index("</generatorCounters>\n") + 1]
+        fileLines = [line.strip() for line in fileLines]
+        fileLines = fileLines[fileLines.index("<generatorCounters>") : fileLines.index("</generatorCounters>") + 1]
         xmlText = "".join(fileLines)
         numberEventTypes = xmlText.count("<eventType>")
         if numberEventTypes > 1:
             # Taking the first set of nodes
             xmlText = (
                 xmlText.split("<eventType>")[0]
                 + "<eventType>"
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/HTML.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/HTML.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/LogErr.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/LogErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/NagiosConnector.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/OutputDataPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ProductionData.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ProductionData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ProductionOptions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/ResolveSE.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/RunApplication.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/RunApplication.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLErr.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLSummaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,17 +501,16 @@
         jsonTemp = dict()
         jsonFin = dict()
 
         with open(self.xmlFileName) as fp:
             # storing the lines in a list
             fileLines = fp.readlines()
         # keeping only the counters lines
-        fileLines = fileLines[fileLines.index("\t<counters>\n") : fileLines.index("\t</counters>\n") + 1]
-        # deleting the \t in the beginning of each line
-        countersLines = [counterLine[1:] for counterLine in fileLines]
+        fileLines = [line.strip() for line in fileLines]
+        countersLines = fileLines[fileLines.index("<counters>") : fileLines.index("</counters>") + 1]
         # replacing Theta with Eta in order to simplify the process. It will be replaced back at the end
         countersText = "".join(countersLines).replace("Theta", "Eta")
 
         # Transforming the xml data into a dictionary
         jsonData = xmltodict.parse(countersText)
         listCounters = jsonData["counters"]["counter"]
         lCategory1 = list()
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/XMLTreeParser.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_GeneratorLog.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_Utilities_Core.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,52 +60,52 @@
         gdf = GangaDataFile()
 
         res = gdf.generateDataFile(["foo", "bar"], persistency="ROOT")
         # Remove first line as it contains the date and time
         res = "\n".join(res.split("\n")[1:])
         root = (
             "\n"
-            + "from Gaudi.Configuration import * \n"
+            + "from Gaudi.Configuration import *\n"
             + "from GaudiConf import IOHelper\nIOHelper('ROOT').inputFiles([\n"
             + "'LFN:foo',\n'LFN:bar',\n], clear=True)\n"
             + "\nFileCatalog().Catalogs += [ 'xmlcatalog_file:pool_xml_catalog.xml' ]\n"
         )
         self.assertEqual(res, root)
 
         res = gdf.generateDataFile(["foo", "bar"])
         # Remove first line as it contains the date and time
         res = "\n".join(res.split("\n")[1:])
         root = (
             "\n"
-            + "from Gaudi.Configuration import * \n"
+            + "from Gaudi.Configuration import *\n"
             + "from GaudiConf import IOHelper\nIOHelper().inputFiles([\n"
             + "'LFN:foo',\n'LFN:bar',\n], clear=True)\n"
             + "\nFileCatalog().Catalogs += [ 'xmlcatalog_file:pool_xml_catalog.xml' ]\n"
         )
         self.assertEqual(res, root)
 
         gdf = GangaDataFile(xmlcatalog_file="")
 
         res = gdf.generateDataFile(["foo", "bar"], persistency="MDF")
         # Remove first line as it contains the date and time
         res = "\n".join(res.split("\n")[1:])
         root = (
             "\n"
-            + "from Gaudi.Configuration import * \n"
+            + "from Gaudi.Configuration import *\n"
             + "from GaudiConf import IOHelper\nIOHelper('MDF').inputFiles([\n"
             + "'LFN:foo',\n'LFN:bar',\n], clear=True)\n"
         )
         self.assertEqual(res, root)
 
         res = gdf.generateDataFile("foo", persistency="ROOT")
         # Remove first line as it contains the date and time
         res = "\n".join(res.split("\n")[1:])
         root = (
             "\n"
-            + "from Gaudi.Configuration import * \n"
+            + "from Gaudi.Configuration import *\n"
             + "from GaudiConf import IOHelper\nIOHelper('ROOT').inputFiles([\n"
             + "'LFN:foo',\n], clear=True)\n"
         )
         self.assertEqual(res, root)
 
 
 #################################################
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_XMLErr.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_XMLSummaries.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/Utilities/test/Test_entrypoints.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_architecture.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_architecture.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_analyse_XML_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_fix_file_guid.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_get_root_guid.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_lhcb_mc_eventtype_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/dirac_loop.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/dirac_loop.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Core/scripts/lhcb_proxy_init.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/PopularityAnalysisAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RAWIntegrityAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/LogUpload.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/WMSSecureOutputData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/SEUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/StorageHistoryAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/StorageUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageQuotaAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/UserStorageUsageAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/AddTransformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/CheckExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ConsistencyChecks.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DMScript.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,17 @@
         )
         Script.registerSwitch("", "DQFlags=", "   DQ flag used in query", self.setDQFlags)
         Script.registerSwitch("", "StartDate=", "   Start date for the BK query", self.setStartDate)
         Script.registerSwitch("", "EndDate=", "   End date for the BK query", self.setEndDate)
         Script.registerSwitch("", "Visibility=", "   Required visibility (Yes, No, All) [Yes]", self.setVisibility)
         Script.registerSwitch("", "ReplicaFlag=", "   Required replica flag (Yes, No, All) [Yes]", self.setReplicaFlag)
         Script.registerSwitch("", "TCK=", "   Get files with a given TCK", self.setTCK)
+        Script.registerSwitch(
+            "", "SMOG2=", "   Required SMOG2 (comma separated list, may include 'Undefined')", self.setSMOG2
+        )
 
     def registerNamespaceSwitches(self, action="search [ALL]"):
         """Register namespace switches."""
         Script.registerSwitch("D:", "Directory=", "   Directory to " + action, self.setDirectory)
 
     def registerSiteSwitches(self):
         """SE switches."""
@@ -345,14 +348,20 @@
 
     def setTCK(self, arg):
         """Setter."""
         tcks = arg.split(",")
         self.options["TCK"] = tcks
         return DIRAC.S_OK()
 
+    def setSMOG2(self, arg):
+        """Setter."""
+        states = arg.split(",")
+        self.options["SMOG2"] = states
+        return DIRAC.S_OK()
+
     def setVisibility(self, arg):
         """Setter."""
         if arg.lower() in ("yes", "no", "all"):
             self.options["Visibility"] = arg
         else:
             gLogger.error(f"Unknown visibility flag: {arg}")
             return DIRAC.exit(1)
@@ -556,14 +565,16 @@
             self.bkClientQuery.setOption("StartDate", self.options["StartDate"])
         if "EndDate" in self.options:
             self.bkClientQuery.setOption("EndDate", self.options["EndDate"])
         if "ReplicaFlag" in self.options:
             self.bkClientQuery.setOption("ReplicaFlag", self.options["ReplicaFlag"])
         if "TCK" in self.options:
             self.bkClientQuery.setOption("TCK", self.options["TCK"])
+        if "SMOG2" in self.options:
+            self.bkClientQuery.setOption("SMOG2", self.options["SMOG2"])
         return self.bkClientQuery
 
     def getRequestID(self, prod=None):
         """Get the request ID for a single production."""
         from DIRAC.TransformationSystem.Client.TransformationClient import TransformationClient
 
         if not prod:
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DataIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/DataUsageClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ScanPopularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/ScriptExecutors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/StorageUsageClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/RAWIntegrityDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/StorageUsageDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/DataUsageHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/RAWIntegrityHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/RunDBInterfaceHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/StorageUsageHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Utilities/FCUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/LHCbFTS3Plugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/private/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/private/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_add_transformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_bkk2fc.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_directory_integrity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2bkk.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_fc2se.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_file_integrity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_inputdata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_check_se.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_chown_directory.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_get_file.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_accessURL.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_lfn_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_list_directory.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_exists.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_pfn_metadata.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_register_bk2fc.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_disk_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replica_stats.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_lfn.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_replicate_to_run_destination.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_scan_popularity.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_set_problematic_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/DataManagementSystem/scripts/dirac_dms_storage_usage_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/DB/ProxyDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/FrameworkSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/FrameworkSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/DiracLHCb.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/DiracProduction.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/DiracProduction.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/LHCbJob.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/LHCbJob.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/API/test/Test_Interfaces.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_admin_grid_weather.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_action.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_application_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_change_status.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_status.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_file_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_get_id.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_job_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_list_id.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_logging_info.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_mc_extend.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_progress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_set_agent_type.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_site_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Interfaces/scripts/dirac_production_summary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/APSyncAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/DataProcessingProgressAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/HistogramMergingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/NotifyAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/ProductionStatusAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/RequestTrackingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_Agent_ProductionManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_HistogramMergingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Agent/test/Test_ProductionStatusAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/AnalysisProductionsClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/MCStatsClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProcessingProgress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/Production.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/ProductionRequestClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionManagementSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_Client_ProductionRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/Test_PMS_Client_ProcessingProgress.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Client/test/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/AnalysisProductionsObjects.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticApplicationSummaryDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticGeneratorLogDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticLogErrorsDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticMCStatsDBBase.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ElasticPrMonDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/ProductionRequestDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/extra_func.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/DB/tests/Test_AnalysisProductionsDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/MCStatsElasticDBHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/ProductionRequestHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/TornadoAnalysisProductionsHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Service/tests/Test_ProductionRequestHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/MCSimulation_simplified_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/RecoStripping_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/Sprucing_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/Sprucing_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/WGProds_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Templates/everyThingElse_run.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/APUtils.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/ModelCompatibility.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Models.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/Utils.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/Test_production_models.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/Test_production_models.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/ana_prod_1.yaml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/ana_prod_1.yaml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/mc_1.yaml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/mc_1.yaml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_1.yaml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_1.yaml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_2.yaml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_2.yaml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_3.yaml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/Utilities/test/example_yamls/sprucing_3.yaml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_run_local.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_request_submit.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ProductionManagementSystem/scripts/dirac_production_shifter.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/LHCbPRProxyAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/NagiosTopologyAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/ShiftDBAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/Configurations.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/JobWebSummaryEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/TransferQualityPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobWebSummaryEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_TransferQualityPolicy.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/ResourceStatusSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/ResourceStatusSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/BookkeepingDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/PoolXMLFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/RAWIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_BookkeepingDBClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Catalog/test/Test_Resources_Catalog_RAWIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/LHCbOnlineStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/Storage/test/Test_Resources_Storage_LHCbOnlineStorage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Resources/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/BookkeepingWatchAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/DataRecoveryAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/MCExtensionAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/MCSimulationTestingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCExtensionAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_MCSimulationTestingAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_Plugins.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/Test_TransformationCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Agent/test/testWF.xml`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/DataChallengeReplicationBody.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/RAWReplicationBody.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/BodyPlugin/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TaskManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TransformationClient.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/TransformationDebug.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Client/test/Test_TS_Client_TaskManager.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/TransformationDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/DB/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/TransformationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Service/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Service/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/PluginScript.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/PluginUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/Utilities/test/Test_Utilities_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,9 +4,7 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-"""LHCbDIRAC.TransformationSystem package."""
-################################################################################
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,7 +4,8 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
+"""LHCbDIRAC.WorkloadManagementSystem.DB package."""
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_ancestors.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_check_descendants.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_remove_output.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_set_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_production_verify_outputdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,19 @@
 def main():
     from DIRAC.Core.Base.Script import parseCommandLine
 
     parseCommandLine()
 
     import sys
 
-    transIDs = []
-    if len(sys.argv) < 2:
+    transIDs = Script.getPositionalArgs()
+    if not transIDs:
         print("Usage: dirac-production-verify-outputdata transID [transID] [transID]")
         sys.exit()
-    else:
-        transIDs = [int(arg) for arg in sys.argv[1:]]
+    transIDs = [int(arg) for arg in transIDs]
 
     from LHCbDIRAC.TransformationSystem.Agent.ValidateOutputDataAgent import ValidateOutputDataAgent
 
     agent = ValidateOutputDataAgent(
         "Transformation/ValidateOutputDataAgent",
         "Transformation/ValidateOutputDataAgent",
         "dirac-production-verify-outputdata",
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_test_plugin.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_archive.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_clean.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_debug.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_flush_runs.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_remove_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_reset_files.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_parameters.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_set_run_destination.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/TransformationSystem/scripts/dirac_transformation_targets.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/AnalyseFileAccess.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/AnalyseXMLSummary.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/FileUsage.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/FileUsage.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
             self._resolveInputVariables()
 
             self.log.info(
                 "Executing application %s %s for binary tag %s"
                 % (self.applicationName, self.applicationVersion, self.systemConfig)
             )
-            if self.jobType.lower() == "merge" in self.siteName:
+            if self.jobType.lower() == "merge" and self._WMSJob():
                 self._disableWatchdogCPUCheck()
 
             # Resolve options files
             if self.optionsFile.startswith("{"):
                 commandOptions = json.loads(self.optionsFile)
                 self.log.info("Found lbexec style configuration:", commandOptions)
             else:
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/LHCbScript.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/StepAccounting.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,17 @@
                 "OutputEvents": xf_o.outputEventsTotal,
             }
 
             jobStep.setValuesFromDict(dataDict)
 
             res = jobStep.checkValues()
             if not res["OK"]:
-                self.log.error("Values for StepAccounting are wrong", res["Message"], dataDict)
+                self.log.error(
+                    "Values for StepAccounting are wrong:", f"{res['Message']}. Here are the given data: {dataDict}"
+                )
                 return S_ERROR("Values for StepAccounting are wrong")
 
             if not self._enableModule():
                 self.log.info(f"Not enabled, would have accounted for {dataDict}")
                 return S_OK()
 
             self.dsc.addRegister(jobStep)
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
             try:
                 res = zipFiles(zipFileName, selectedFiles, str(self.prod_job_id))
                 if not res["OK"]:
                     self.log.error("Failed to create zip of log files", res["Message"])
                     self.setApplicationStatus("Failed to create zip of log files")
                     # We do not fail the job for this case
                     return S_OK()
-            except OSError:
-                self.log.error("Failed to create zip of log files", res["Message"])
+            except OSError as e:
+                self.log.error("Failed to create zip of log files", str(e))
                 self.setApplicationStatus("Failed to create zip of log files")
                 # We do not fail the job for this case
                 return S_OK()
 
             # Instantiate the failover transfer client with the global request object
             if not self.failoverTransfer:
                 self.failoverTransfer = FailoverTransfer(self.request)
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadMC.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadMC.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """Module to upload specified job output files according to the parameters
 defined in the production workflow."""
 import os
 import random
 import glob
 from operator import itemgetter
 
-from DIRAC import S_OK, S_ERROR, gLogger, gConfig
+from DIRAC import S_OK, S_ERROR, gLogger
 from DIRAC.Core.Utilities import DEncode
 from DIRAC.DataManagementSystem.Client.FailoverTransfer import FailoverTransfer
 from DIRAC.RequestManagementSystem.Client.Request import Request
 from DIRAC.RequestManagementSystem.Client.Operation import Operation
 from DIRAC.RequestManagementSystem.Client.File import File
 from DIRAC.Resources.Catalog.FileCatalog import FileCatalog
 
@@ -37,21 +37,14 @@
     #############################################################################
     def __init__(self, bkClient=None, dm=None):
         """Module initialization."""
 
         self.log = gLogger.getSubLogger("UploadOutputData")
         super().__init__(self.log, bkClientIn=bkClient, dm=dm)
 
-        self.commandTimeOut = 10 * 60
-        self.jobID = ""
-        self.existingCatalogs = []
-        result = gConfig.getSections("/Resources/FileCatalogs")
-        if result["OK"]:
-            self.existingCatalogs = result["Value"]
-
         # List all parameters here
         self.outputDataFileMask = ""
         self.outputMode = "Any"  # or 'Run', for Reco/Stripping case, or 'Local', e.g. for MCMerge
         self.outputList = []
         self.outputDataStep = ""
         self.request = None
         self.failoverTransfer = None
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/mock_Commons.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/mock_Commons.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbScript.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,37 +4,33 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-"""Unit tests for Workflow Modules utilities."""
+"""Unit tests for LHCbScript."""
 import unittest
 import copy
 import os
 
-from unittest.mock import MagicMock, patch
-
 from DIRAC import gLogger
 
-from LHCbDIRAC.Workflow.Modules.mock_Commons import (
+from LHCbDIRAC.Workflow.Modules.test.mock_Commons import (
     prod_id,
     prod_job_id,
     wms_job_id,
     workflowStatus,
     stepStatus,
     step_id,
     step_number,
     step_commons,
     wf_commons,
 )
 
-from LHCbDIRAC.Workflow.Modules.ErrorLogging import ErrorLogging
-
 
 class ModulesApplicationsTestCase(unittest.TestCase):
     """Base class for the Modules Applications test cases."""
 
     def setUp(self):
         gLogger.setLevel("DEBUG")
         self.maxDiff = None
@@ -113,34 +109,12 @@
             for s_cs in step_commons:
                 lhcbScript.workflow_commons = wf_cs
                 lhcbScript.step_commons = s_cs
                 res = lhcbScript.execute()
                 self.assertFalse(res["OK"])
 
 
-#############################################################################
-# ErrorLogging.py
-#############################################################################
-
-
-class ErrorLoggingSuccess(ModulesApplicationsTestCase):
-    @patch("LHCbDIRAC.Workflow.Modules.ModuleBase.RequestValidator", side_effect=MagicMock())
-    def test_excecute(self, _patch):
-        er = ErrorLogging()
-        er.jobType = "user"
-
-        # no errors, no input data
-        for wf_cs in copy.deepcopy(wf_commons):
-            for s_cs in step_commons:
-                self.assertTrue(
-                    er.execute(
-                        prod_id, prod_job_id, wms_job_id, workflowStatus, stepStatus, wf_cs, s_cs, step_number, step_id
-                    )["OK"]
-                )
-
-
 if __name__ == "__main__":
     suite = unittest.defaultTestLoader.loadTestsFromTestCase(ModulesApplicationsTestCase)
     suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(LHCbScriptSuccess))
     suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(LHCbScriptFailure))
-    suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(ErrorLoggingSuccess))
     testResult = unittest.TextTestRunner(verbosity=2).run(suite)
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
 """Test class for ModuleBase."""
 # pylint: disable=protected-access, missing-docstring, invalid-name
 import os
 from itertools import product
+from pathlib import Path
 from unittest.mock import MagicMock
 
 import pytest
 
 # mocks
 from DIRAC.DataManagementSystem.Client.test.mock_DM import dm_mock
 from LHCbDIRAC.BookkeepingSystem.Client.test.mock_BookkeepingClient import bkc_mock
-from LHCbDIRAC.Workflow.Modules.mock_Commons import (
+from LHCbDIRAC.Workflow.Modules.test.mock_Commons import (
     version,
     prod_id,
     prod_job_id,
     wms_job_id,
     workflowStatus,
     stepStatus,
     step_id,
@@ -384,14 +385,18 @@
     ]
     bkExp = ["BHADRON.DST"]
     mb.stepName = "someApp_1"
     out, bk = mb._findOutputs(stepOutput)
     assert out == outExp
     assert bk == bkExp
 
+    Path("aaa.Bhadron.dst").unlink(missing_ok=True)
+    Path("ccc.charm.mdst").unlink(missing_ok=True)
+    Path("prova.txt").unlink(missing_ok=True)
+
 
 def test_getFileMetadata(mocker):
     mocker.patch("LHCbDIRAC.Workflow.Modules.ModuleBase.RequestValidator", side_effect=MagicMock())
     mb = ModuleBase(bkClientIn=bkc_mock, dm=dm_mock)
 
     candidateFiles = {
         "foo_1.txt": {"lfn": "/lhcb/MC/2010/DST/00012345/0001/foo_1.txt", "type": "txt", "workflowSE": "SE1"},
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/Workflow/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/Workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,8 +4,13 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-"""LHCbDIRAC.WorkloadManagementSystem.DB package."""
+############################################################
+
+"""LHCbSystem package.
+
+This contains the LHCb specific plugins for DIRAC.
+"""
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/WorkloadManagementSystem/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Utilities/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 ###############################################################################
-# (c) Copyright 2019 CERN for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2021 CERN for the benefit of the LHCb Collaboration           #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
-# Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".   #
+# Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-############################################################
-
-"""LHCbSystem package.
-
-This contains the LHCb specific plugins for DIRAC.
-"""
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Utilities/__init__.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC/tests/Workflow.py` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC/tests/Workflow.py`

 * *Files identical despite different names*

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/PKG-INFO` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LHCbDIRAC
-Version: 12.0.0a5
+Version: 12.0.0a6
 Summary: LHCbDIRAC is the LHCb extension of DIRAC
 Home-page: https://gitlab.cern.ch/lhcb-dirac/LHCbDIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/SOURCES.txt` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/LHCbDIRAC/BookkeepingSystem/Client/JEncoder.py
 src/LHCbDIRAC/BookkeepingSystem/Client/LHCB_BKKDBClient.py
 src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingCLI.py
 src/LHCbDIRAC/BookkeepingSystem/Client/LHCbBookkeepingManager.py
 src/LHCbDIRAC/BookkeepingSystem/Client/ScriptExecutors.py
 src/LHCbDIRAC/BookkeepingSystem/Client/__init__.py
 src/LHCbDIRAC/BookkeepingSystem/Client/objects.py
+src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BKQuery.py
 src/LHCbDIRAC/BookkeepingSystem/Client/test/Test_BookkeepingClient.py
 src/LHCbDIRAC/BookkeepingSystem/Client/test/__init__.py
 src/LHCbDIRAC/BookkeepingSystem/Client/test/mock_BookkeepingClient.py
 src/LHCbDIRAC/BookkeepingSystem/DB/DataTakingConditionInterpreter.py
 src/LHCbDIRAC/BookkeepingSystem/DB/LegacyOracleBookkeepingDB.py
 src/LHCbDIRAC/BookkeepingSystem/DB/NewOracleBookkeepingDB.py
 src/LHCbDIRAC/BookkeepingSystem/DB/OracleBookkeepingDB.py
@@ -416,44 +417,46 @@
 src/LHCbDIRAC/Workflow/Modules/BookkeepingReport.py
 src/LHCbDIRAC/Workflow/Modules/CreateDataFile.py
 src/LHCbDIRAC/Workflow/Modules/ErrorLogging.py
 src/LHCbDIRAC/Workflow/Modules/FailoverRequest.py
 src/LHCbDIRAC/Workflow/Modules/FileUsage.py
 src/LHCbDIRAC/Workflow/Modules/GaudiApplication.py
 src/LHCbDIRAC/Workflow/Modules/LHCbScript.py
-src/LHCbDIRAC/Workflow/Modules/MergeMDF.py
 src/LHCbDIRAC/Workflow/Modules/ModuleBase.py
 src/LHCbDIRAC/Workflow/Modules/ModulesUtilities.py
 src/LHCbDIRAC/Workflow/Modules/RemoveInputData.py
 src/LHCbDIRAC/Workflow/Modules/StepAccounting.py
 src/LHCbDIRAC/Workflow/Modules/UploadLogFile.py
 src/LHCbDIRAC/Workflow/Modules/UploadMC.py
 src/LHCbDIRAC/Workflow/Modules/UploadOutputData.py
 src/LHCbDIRAC/Workflow/Modules/UserJobFinalization.py
 src/LHCbDIRAC/Workflow/Modules/__init__.py
-src/LHCbDIRAC/Workflow/Modules/mock_Commons.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_AnalyseFileAccess.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_AnalyseXMLSummary.py
 src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_BookkeepingReport.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_CreateDataFile.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ErrorLogging.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_FailoverRequest.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_FileUsage.py
 src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_GaudiApplication.py
-src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbAnalyse.py
-src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbApplications.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_LHCbScript.py
 src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_ModuleBase.py
-src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Others.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_RemoveInputData.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_StepAccounting.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadLogFile.py
 src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadMC.py
-src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Uploads.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UploadOutputData.py
+src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_UserJobFinalization.py
 src/LHCbDIRAC/Workflow/Modules/test/Test_Modules_Utilities.py
-src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/Test_Modules_AnalyseFileAccess.py
-src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/pool_xml_catalog.xml
-src/LHCbDIRAC/Workflow/Modules/test/test_analyseFileAccess/summary.xml
+src/LHCbDIRAC/Workflow/Modules/test/mock_Commons.py
 src/LHCbDIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
 src/LHCbDIRAC/WorkloadManagementSystem/__init__.py
 src/LHCbDIRAC/WorkloadManagementSystem/Agent/AncestorFilesAgent.py
 src/LHCbDIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
 src/LHCbDIRAC/WorkloadManagementSystem/Agent/__init__.py
 src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.py
 src/LHCbDIRAC/WorkloadManagementSystem/DB/JobDB.sql
 src/LHCbDIRAC/WorkloadManagementSystem/DB/__init__.py
-src/LHCbDIRAC/WorkloadManagementSystem/Service/WMSSecureGWHandler.py
-src/LHCbDIRAC/WorkloadManagementSystem/Service/__init__.py
 src/LHCbDIRAC/tests/Workflow.py
 src/LHCbDIRAC/tests/__init__.py
 src/LHCbDIRAC/tests/Utilities/__init__.py
 src/LHCbDIRAC/tests/Utilities/testJobDefinitions.py
```

### Comparing `LHCbDIRAC-12.0.0a5/src/LHCbDIRAC.egg-info/entry_points.txt` & `LHCbDIRAC-12.0.0a6/src/LHCbDIRAC.egg-info/entry_points.txt`

 * *Files identical despite different names*

