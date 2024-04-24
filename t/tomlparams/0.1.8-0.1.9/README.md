# Comparing `tmp/tomlparams-0.1.8.tar.gz` & `tmp/tomlparams-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomlparams-0.1.8.tar", max compression
+gzip compressed data, was "tomlparams-0.1.9.tar", max compression
```

## Comparing `tomlparams-0.1.8.tar` & `tomlparams-0.1.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0      420 2024-03-21 15:24:23.604065 tomlparams-0.1.8/AUTHORS
--rw-r--r--   0        0        0     1138 2024-03-21 15:24:23.604065 tomlparams-0.1.8/LICENSE
--rw-r--r--   0        0        0    16084 2024-03-21 15:24:23.604065 tomlparams-0.1.8/README.md
--rw-r--r--   0        0        0     1118 2024-03-21 15:24:23.604065 tomlparams-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      115 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/__init__.py
--rw-r--r--   0        0        0     1250 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/captureoutput.py
--rw-r--r--   0        0        0     1414 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/console.py
--rw-r--r--   0        0        0        0 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/__init__.py
--rw-r--r--   0        0        0       52 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/base.toml
--rw-r--r--   0        0        0      190 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/defaults.toml
--rw-r--r--   0        0        0      332 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/defaults2.toml
--rw-r--r--   0        0        0      116 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/hier.toml
--rw-r--r--   0        0        0       33 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/newparam.toml
--rw-r--r--   0        0        0      195 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/one.toml
--rw-r--r--   0        0        0      732 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/readme1.py
--rw-r--r--   0        0        0      711 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/readme2.py
--rw-r--r--   0        0        0      298 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/readme3.py
--rw-r--r--   0        0        0      310 2024-03-21 15:24:23.604065 tomlparams-0.1.8/tomlparams/examples/readme/readme4.py
--rw-r--r--   0        0        0      247 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/examples/readme/three.toml
--rw-r--r--   0        0        0      149 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/examples/readme/two.toml
--rw-r--r--   0        0        0     2932 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/params_group.py
--rw-r--r--   0        0        0     7294 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/parse_helpers.py
--rw-r--r--   0        0        0        0 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/__init__.py
--rw-r--r--   0        0        0    27059 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/test_tomlparams.py
--rw-r--r--   0        0        0       80 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/deep.toml
--rw-r--r--   0        0        0       48 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/one.toml
--rw-r--r--   0        0        0      129 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/self.toml
--rw-r--r--   0        0        0      130 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/three.toml
--rw-r--r--   0        0        0      128 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/two.toml
--rw-r--r--   0        0        0      135 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/unchanged.toml
--rw-r--r--   0        0        0        6 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/expected/user_only.toml
--rw-r--r--   0        0        0        0 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/base.toml
--rw-r--r--   0        0        0       48 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/deep.toml
--rw-r--r--   0        0        0       35 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/birds.toml
--rw-r--r--   0        0        0       41 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/fish/salmon.toml
--rw-r--r--   0        0        0       39 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/fish/tuna.toml
--rw-r--r--   0        0        0       38 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/fungi/ascomycota.toml
--rw-r--r--   0        0        0       43 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/fungi/chytridiomycota.toml
--rw-r--r--   0        0        0       27 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir/human.toml
--rw-r--r--   0        0        0       27 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir_repeated_keys/human.toml
--rw-r--r--   0        0        0       27 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_dir_repeated_keys/stinky-human.toml
--rw-r--r--   0        0        0      228 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/defaults_as_file.toml
--rw-r--r--   0        0        0       31 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/five.toml
--rw-r--r--   0        0        0       49 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/four.toml
--rw-r--r--   0        0        0       48 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/one.toml
--rw-r--r--   0        0        0       67 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/self.toml
--rw-r--r--   0        0        0       45 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/table_array_defaults.toml
--rw-r--r--   0        0        0       40 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/three.toml
--rw-r--r--   0        0        0       47 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/two.toml
--rw-r--r--   0        0        0       18 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/type_check_dates.toml
--rw-r--r--   0        0        0       46 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/type_check_deeper_level.toml
--rw-r--r--   0        0        0       17 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/type_check_list.toml
--rw-r--r--   0        0        0       17 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/type_check_root_level.toml
--rw-r--r--   0        0        0       34 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/tomlparams/type_check_shallow.toml
--rw-r--r--   0        0        0       74 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/usertomlparams/table_array_longer.toml
--rw-r--r--   0        0        0       49 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/usertomlparams/table_array_same_length.toml
--rw-r--r--   0        0        0       24 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/usertomlparams/table_array_shorter.toml
--rw-r--r--   0        0        0        6 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tests/testdata/usertomlparams/user_only.toml
--rw-r--r--   0        0        0    17245 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/tomlparams.py
--rw-r--r--   0        0        0     1999 2024-03-21 15:24:23.608065 tomlparams-0.1.8/tomlparams/utils.py
--rw-r--r--   0        0        0    16621 1970-01-01 00:00:00.000000 tomlparams-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      420 2024-03-21 15:33:13.652173 tomlparams-0.1.9/AUTHORS
+-rw-r--r--   0        0        0     1138 2024-03-21 15:33:13.652173 tomlparams-0.1.9/LICENSE
+-rw-r--r--   0        0        0    16084 2024-03-21 15:33:13.652173 tomlparams-0.1.9/README.md
+-rw-r--r--   0        0        0     1118 2024-03-21 15:33:13.652173 tomlparams-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/__init__.py
+-rw-r--r--   0        0        0     1250 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/captureoutput.py
+-rw-r--r--   0        0        0     1414 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/console.py
+-rw-r--r--   0        0        0        0 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/__init__.py
+-rw-r--r--   0        0        0       52 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/base.toml
+-rw-r--r--   0        0        0      190 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/defaults.toml
+-rw-r--r--   0        0        0      332 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/defaults2.toml
+-rw-r--r--   0        0        0      116 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/hier.toml
+-rw-r--r--   0        0        0       33 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/newparam.toml
+-rw-r--r--   0        0        0      195 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/one.toml
+-rw-r--r--   0        0        0      732 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/readme1.py
+-rw-r--r--   0        0        0      711 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/readme2.py
+-rw-r--r--   0        0        0      298 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/readme3.py
+-rw-r--r--   0        0        0      310 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/readme4.py
+-rw-r--r--   0        0        0      247 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/three.toml
+-rw-r--r--   0        0        0      149 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/examples/readme/two.toml
+-rw-r--r--   0        0        0     2932 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/params_group.py
+-rw-r--r--   0        0        0     7294 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/parse_helpers.py
+-rw-r--r--   0        0        0        0 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/__init__.py
+-rw-r--r--   0        0        0    27059 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/test_tomlparams.py
+-rw-r--r--   0        0        0       80 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/deep.toml
+-rw-r--r--   0        0        0       48 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/one.toml
+-rw-r--r--   0        0        0      129 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/self.toml
+-rw-r--r--   0        0        0      130 2024-03-21 15:33:13.652173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/three.toml
+-rw-r--r--   0        0        0      128 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/two.toml
+-rw-r--r--   0        0        0      135 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/unchanged.toml
+-rw-r--r--   0        0        0        6 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/expected/user_only.toml
+-rw-r--r--   0        0        0        0 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/base.toml
+-rw-r--r--   0        0        0       48 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/deep.toml
+-rw-r--r--   0        0        0       35 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/birds.toml
+-rw-r--r--   0        0        0       41 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/fish/salmon.toml
+-rw-r--r--   0        0        0       39 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/animals/fish/tuna.toml
+-rw-r--r--   0        0        0       38 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/fungi/ascomycota.toml
+-rw-r--r--   0        0        0       43 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/fungi/chytridiomycota.toml
+-rw-r--r--   0        0        0       27 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir/human.toml
+-rw-r--r--   0        0        0       27 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir_repeated_keys/human.toml
+-rw-r--r--   0        0        0       27 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_dir_repeated_keys/stinky-human.toml
+-rw-r--r--   0        0        0      228 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/defaults_as_file.toml
+-rw-r--r--   0        0        0       31 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/five.toml
+-rw-r--r--   0        0        0       49 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/four.toml
+-rw-r--r--   0        0        0       48 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/one.toml
+-rw-r--r--   0        0        0       67 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/self.toml
+-rw-r--r--   0        0        0       45 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/table_array_defaults.toml
+-rw-r--r--   0        0        0       40 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/three.toml
+-rw-r--r--   0        0        0       47 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/two.toml
+-rw-r--r--   0        0        0       18 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/type_check_dates.toml
+-rw-r--r--   0        0        0       46 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/type_check_deeper_level.toml
+-rw-r--r--   0        0        0       17 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/type_check_list.toml
+-rw-r--r--   0        0        0       17 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/type_check_root_level.toml
+-rw-r--r--   0        0        0       34 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/tomlparams/type_check_shallow.toml
+-rw-r--r--   0        0        0       74 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/usertomlparams/table_array_longer.toml
+-rw-r--r--   0        0        0       49 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/usertomlparams/table_array_same_length.toml
+-rw-r--r--   0        0        0       24 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/usertomlparams/table_array_shorter.toml
+-rw-r--r--   0        0        0        6 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tests/testdata/usertomlparams/user_only.toml
+-rw-r--r--   0        0        0    17245 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/tomlparams.py
+-rw-r--r--   0        0        0     2002 2024-03-21 15:33:13.656173 tomlparams-0.1.9/tomlparams/utils.py
+-rw-r--r--   0        0        0    16621 1970-01-01 00:00:00.000000 tomlparams-0.1.9/PKG-INFO
```

### Comparing `tomlparams-0.1.8/LICENSE` & `tomlparams-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/README.md` & `tomlparams-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/pyproject.toml` & `tomlparams-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomlparams"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = [
   "Smart Data Foundry <datascience@smartdatafoundry.com>",
   "Paola Arce <paola.arce@smartdatafoundry.com>",
   "Victor Diaz <victor.diaz@smartdatafoundry.com>",
   "Eric Janto <eric.janto@smartdatafoundry.com>",
   "Del Middlemiss <derek.middlemiss@smartdatafoundry.com>",
```

### Comparing `tomlparams-0.1.8/tomlparams/captureoutput.py` & `tomlparams-0.1.9/tomlparams/captureoutput.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/console.py` & `tomlparams-0.1.9/tomlparams/console.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/examples/readme/readme1.py` & `tomlparams-0.1.9/tomlparams/examples/readme/readme1.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/examples/readme/readme2.py` & `tomlparams-0.1.9/tomlparams/examples/readme/readme2.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/params_group.py` & `tomlparams-0.1.9/tomlparams/params_group.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/parse_helpers.py` & `tomlparams-0.1.9/tomlparams/parse_helpers.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/tests/test_tomlparams.py` & `tomlparams-0.1.9/tomlparams/tests/test_tomlparams.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/tomlparams.py` & `tomlparams-0.1.9/tomlparams/tomlparams.py`

 * *Files identical despite different names*

### Comparing `tomlparams-0.1.8/tomlparams/utils.py` & `tomlparams-0.1.9/tomlparams/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,10 +64,10 @@
                 yield key1 + sep + key2, value2
         elif isinstance(value1, list):
             for list_index, list_item in enumerate(value1):
                 if isinstance(list_item, dict):
                     for key3, value3 in concatenate_keys(list_item, sep=sep):
                         yield f'{key1}{sep}{list_index}{sep}{key3}', value3
                 else:
-                    yield f'{key1}{sep}{list_index}', value2
+                    yield f'{key1}{sep}{list_index}', list_item
         else:
             yield key1, value1
```

### Comparing `tomlparams-0.1.8/PKG-INFO` & `tomlparams-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomlparams
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Smart Data Foundry
 Author-email: datascience@smartdatafoundry.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

