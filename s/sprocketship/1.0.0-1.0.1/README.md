# Comparing `tmp/sprocketship-1.0.0.tar.gz` & `tmp/sprocketship-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-1.0.0.tar", last modified: Tue Apr 23 03:20:35 2024, max compression
+gzip compressed data, was "sprocketship-1.0.1.tar", last modified: Wed Apr 24 15:18:04 2024, max compression
```

## Comparing `sprocketship-1.0.0.tar` & `sprocketship-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 03:20:31.000000 sprocketship-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 03:20:31.000000 sprocketship-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 03:20:35.280539 sprocketship-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-23 03:20:31.000000 sprocketship-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-23 03:20:31.000000 sprocketship-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:20:35.280539 sprocketship-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.276539 sprocketship-1.0.0/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/templates/javascript.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-23 03:20:31.000000 sprocketship-1.0.0/sprocketship/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:20:35.280539 sprocketship-1.0.0/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 03:20:35.000000 sprocketship-1.0.0/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:18:04.374624 sprocketship-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 15:17:59.000000 sprocketship-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-24 15:17:59.000000 sprocketship-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-24 15:18:04.374624 sprocketship-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-04-24 15:17:59.000000 sprocketship-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 15:17:59.000000 sprocketship-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:18:04.374624 sprocketship-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:18:04.374624 sprocketship-1.0.1/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 15:17:59.000000 sprocketship-1.0.1/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:18:04.374624 sprocketship-1.0.1/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 15:17:59.000000 sprocketship-1.0.1/sprocketship/templates/javascript.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-24 15:17:59.000000 sprocketship-1.0.1/sprocketship/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:18:04.374624 sprocketship-1.0.1/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 15:18:04.000000 sprocketship-1.0.1/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-1.0.0/LICENSE` & `sprocketship-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-1.0.0/PKG-INFO` & `sprocketship-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: sprocketship
-Version: 1.0.0
-Summary: Better stored procedure management
-Author-email: Nicklaus Roach <nicklausroach@gmail.com>
-Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click
-Requires-Dist: snowflake-connector-python
-Requires-Dist: ABSQL
-Requires-Dist: ruamel.yaml
-Requires-Dist: jinja2
-
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -108,25 +90,27 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
+### Structure
+
+Currently, sprocketship expects a `.sprocketship.yml` file in a `procedures/` directory.
 
 ```
 ├── dbt_models
 │   ├── customers.sql
 │   ├── products.sql
 ├── procedures
-│   ├── admin
+│   ├── useradmin
 │   │   ├── create_database_writer_role.js
 │   │   ├── create_database_reader_role.js
-│   ├── development
+│   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
@@ -145,41 +129,86 @@
 
     - name: create_database_writer
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
+### Directory-level Default Parameters
+
+sprocketship allows providing default parameters at any given level of
+your project. These defaults will be applied recursively to any procedures
+defined in any of the subdirectories, unless overridden by a default in one
+of the subdirectories.
+
+```
+procedures:
+  # for all procedures, default to the below database and schema
+  +database: !env_var SNOWFLAKE_DATABASE
+  +schema: !env_var SNOWFLAKE_SCHEMA
+  development:
+    # for all procedures in the development directory,
+    # default to using the sysadmin role
+    +use_role: sysadmin
+    create_temp_database:
+      args:
+        - name: Name of argument
+          type: Type of argument
+          default: (Optional) default value for the argument
+      returns: varchar
+```
+
+### File Frontmatter
+
+Thanks to ABSQL, sprocketship also provides the ability to define parameters using file frontmatter. Suppose we have a file `create_database_writer_role.js`, we can define parameters for the stored procedure within the file using frontmatter:
+
+```js
+/*
+database: my_database
+schema: my_schema
+language: javascript
+execute_as: owner
+use_role: sysadmin
+*/
+```
+
+sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
+
+### Recommended Configuration
+
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+
+### Execution
+
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
 ```
-name: The name of the procedure
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
+use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
       type: Type of argument
       default: (Optional) default value for the argument
-returns: The return type
+returns: The return type, this can include the `NOT NULL` option
 comment: Explanation of the procedure
 ```
 
 ## Support
 
 sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
 
-* `RETURNS <result-data-type> NOT NULL`
 * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
 * `VOLATILE | IMMUTABLE` (deprecated)
 
 
 <!-- LICENSE -->
 ## License
```

#### html2text {}

```diff
@@ -1,19 +1,10 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.0 Summary: Better stored
-procedure management Author-email: Nicklaus Roach
-gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
-Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
-Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
-[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
-[linkedin-shield]][linkedin-url]
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -23,43 +14,64 @@
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Installation `pip install sprocketship` ## Usage
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
-` directory at the same level in a directory structure. ``` âââ
-dbt_models â âââ customers.sql â âââ products.sql âââ
-procedures â âââ admin â â âââ create_database_writer_role.js
-â â âââ create_database_reader_role.js â âââ development â
-â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
-path to each procedure in the `sprocketship.yml` should follow that of the
-paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
-create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
-SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
-run `$ sprocketship liftoff` from the project directory (or provide the
-directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
-launch your stored procedures into the given directory. ### Exhaustive Options
-for Stored Procedure Configuration ``` name: The name of the procedure
+## Getting Started ### Installation `pip install sprocketship` ## Usage ###
+Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
+`procedures/` directory. ``` âââ dbt_models â âââ customers.sql
+â âââ products.sql âââ procedures â âââ useradmin â â
+âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ sysadmin â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
+name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
+!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
+sprocketship allows providing default parameters at any given level of your
+project. These defaults will be applied recursively to any procedures defined
+in any of the subdirectories, unless overridden by a default in one of the
+subdirectories. ``` procedures: # for all procedures, default to the below
+database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+SNOWFLAKE_SCHEMA development: # for all procedures in the development
+directory, # default to using the sysadmin role +use_role: sysadmin
+create_temp_database: args: - name: Name of argument type: Type of argument
+default: (Optional) default value for the argument returns: varchar ``` ###
+File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
+define parameters using file frontmatter. Suppose we have a file
+`create_database_writer_role.js`, we can define parameters for the stored
+procedure within the file using frontmatter: ```js /* database: my_database
+schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
+``` sprocketship will automatically parse and apply the parameters defined in
+the frontmatter to the stored procedure. ### Recommended Configuration When
+setting up your sprocketship project, we recommend setting more general
+parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
+file, and anything that's specific to a given procedure should be defined in
+the file frontmatter of that procedure, such as the args or return type. ###
+Execution From here, simply run `$ sprocketship liftoff` from the project
+directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
+path`) and sprocketship will launch your stored procedures into the given
+directory. ### Exhaustive Options for Stored Procedure Configuration ```
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner args: - name:
-Name of argument type: Type of argument default: (Optional) default value for
-the argument returns: The return type comment: Explanation of the procedure ```
-## Support sprocketship currently only supports Javascript-based stored
-procedures (Python support coming soon!). Additionally, there are a few options
-from the `CREATE STORED PROCEDURE` function that are not yet supported: *
-`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
-STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
-the MIT License. See `LICENSE` for more information.
+language of the procedure definition execute_as: caller or owner use_role: The
+role you'd like to own the procedure args: - name: Name of argument type: Type
+of argument default: (Optional) default value for the argument returns: The
+return type, this can include the `NOT NULL` option comment: Explanation of the
+procedure ``` ## Support sprocketship currently only supports Javascript-based
+stored procedures (Python support coming soon!). Additionally, there are a few
+options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
+| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
+`LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-1.0.0/README.md` & `sprocketship-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sprocketship
+Version: 1.0.1
+Summary: Better stored procedure management
+Author-email: Nicklaus Roach <nicklausroach@gmail.com>
+Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: snowflake-connector-python
+Requires-Dist: ABSQL
+Requires-Dist: ruamel.yaml
+Requires-Dist: jinja2
+
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
 *** that would make this better, please fork the repo and create a pull request
 *** or simply open an issue with the tag "enhancement".
 *** Don't forget to give the project a star!
@@ -90,25 +108,27 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
+### Structure
+
+Currently, sprocketship expects a `.sprocketship.yml` file in a `procedures/` directory.
 
 ```
 ├── dbt_models
 │   ├── customers.sql
 │   ├── products.sql
 ├── procedures
-│   ├── admin
+│   ├── useradmin
 │   │   ├── create_database_writer_role.js
 │   │   ├── create_database_reader_role.js
-│   ├── development
+│   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
@@ -127,41 +147,86 @@
 
     - name: create_database_writer
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
+### Directory-level Default Parameters
+
+sprocketship allows providing default parameters at any given level of
+your project. These defaults will be applied recursively to any procedures
+defined in any of the subdirectories, unless overridden by a default in one
+of the subdirectories.
+
+```
+procedures:
+  # for all procedures, default to the below database and schema
+  +database: !env_var SNOWFLAKE_DATABASE
+  +schema: !env_var SNOWFLAKE_SCHEMA
+  development:
+    # for all procedures in the development directory,
+    # default to using the sysadmin role
+    +use_role: sysadmin
+    create_temp_database:
+      args:
+        - name: Name of argument
+          type: Type of argument
+          default: (Optional) default value for the argument
+      returns: varchar
+```
+
+### File Frontmatter
+
+Thanks to ABSQL, sprocketship also provides the ability to define parameters using file frontmatter. Suppose we have a file `create_database_writer_role.js`, we can define parameters for the stored procedure within the file using frontmatter:
+
+```js
+/*
+database: my_database
+schema: my_schema
+language: javascript
+execute_as: owner
+use_role: sysadmin
+*/
+```
+
+sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
+
+### Recommended Configuration
+
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+
+### Execution
+
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
 ```
-name: The name of the procedure
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
+use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
       type: Type of argument
       default: (Optional) default value for the argument
-returns: The return type
+returns: The return type, this can include the `NOT NULL` option
 comment: Explanation of the procedure
 ```
 
 ## Support
 
 sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
 
-* `RETURNS <result-data-type> NOT NULL`
 * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
 * `VOLATILE | IMMUTABLE` (deprecated)
 
 
 <!-- LICENSE -->
 ## License
```

#### html2text {}

```diff
@@ -1,10 +1,19 @@
-[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
-shield]][issues-url] [![LinkedIn][linkedin-shield]][linkedin-url]
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.1 Summary: Better stored
+procedure management Author-email: Nicklaus Roach
+gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
+Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
+Dist: ruamel.yaml Requires-Dist: jinja2 [![Contributors][contributors-shield]]
+[contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
+shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url]
                                   _â___ï_¸__ _ð___
                             ******** SSpprroocckkeettsshhiipp ********
                       Better stored procedure management
 Table of Contents
    1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
@@ -14,43 +23,64 @@
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Installation `pip install sprocketship` ## Usage
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
-` directory at the same level in a directory structure. ``` âââ
-dbt_models â âââ customers.sql â âââ products.sql âââ
-procedures â âââ admin â â âââ create_database_writer_role.js
-â â âââ create_database_reader_role.js â âââ development â
-â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
-path to each procedure in the `sprocketship.yml` should follow that of the
-paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
-create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
-SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
-run `$ sprocketship liftoff` from the project directory (or provide the
-directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
-launch your stored procedures into the given directory. ### Exhaustive Options
-for Stored Procedure Configuration ``` name: The name of the procedure
+## Getting Started ### Installation `pip install sprocketship` ## Usage ###
+Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
+`procedures/` directory. ``` âââ dbt_models â âââ customers.sql
+â âââ products.sql âââ procedures â âââ useradmin â â
+âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ sysadmin â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
+name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
+!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
+sprocketship allows providing default parameters at any given level of your
+project. These defaults will be applied recursively to any procedures defined
+in any of the subdirectories, unless overridden by a default in one of the
+subdirectories. ``` procedures: # for all procedures, default to the below
+database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+SNOWFLAKE_SCHEMA development: # for all procedures in the development
+directory, # default to using the sysadmin role +use_role: sysadmin
+create_temp_database: args: - name: Name of argument type: Type of argument
+default: (Optional) default value for the argument returns: varchar ``` ###
+File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
+define parameters using file frontmatter. Suppose we have a file
+`create_database_writer_role.js`, we can define parameters for the stored
+procedure within the file using frontmatter: ```js /* database: my_database
+schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
+``` sprocketship will automatically parse and apply the parameters defined in
+the frontmatter to the stored procedure. ### Recommended Configuration When
+setting up your sprocketship project, we recommend setting more general
+parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
+file, and anything that's specific to a given procedure should be defined in
+the file frontmatter of that procedure, such as the args or return type. ###
+Execution From here, simply run `$ sprocketship liftoff` from the project
+directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
+path`) and sprocketship will launch your stored procedures into the given
+directory. ### Exhaustive Options for Stored Procedure Configuration ```
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner args: - name:
-Name of argument type: Type of argument default: (Optional) default value for
-the argument returns: The return type comment: Explanation of the procedure ```
-## Support sprocketship currently only supports Javascript-based stored
-procedures (Python support coming soon!). Additionally, there are a few options
-from the `CREATE STORED PROCEDURE` function that are not yet supported: *
-`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
-STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
-the MIT License. See `LICENSE` for more information.
+language of the procedure definition execute_as: caller or owner use_role: The
+role you'd like to own the procedure args: - name: Name of argument type: Type
+of argument default: (Optional) default value for the argument returns: The
+return type, this can include the `NOT NULL` option comment: Explanation of the
+procedure ``` ## Support sprocketship currently only supports Javascript-based
+stored procedures (Python support coming soon!). Additionally, there are a few
+options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
+| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
+`LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

### Comparing `sprocketship-1.0.0/pyproject.toml` & `sprocketship-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Nicklaus Roach", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-1.0.0/sprocketship/cli.py` & `sprocketship-1.0.1/sprocketship/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 @main.command()
 @click.argument("dir", default=".")
 @click.option("--show", is_flag=True)
 def liftoff(dir, show):
     click.echo(click.style(f"🚀 Sprocketship lifting off!", fg="white", bold=True))
     data = render_file(
-        os.path.join(dir, "procedures", ".sprocketship.yml"), return_dict=True
+        os.path.join(dir, ".sprocketship.yml"), return_dict=True
     )
     con = connector.connect(**data["snowflake"])
     files = list(Path(dir).rglob("*.js"))
 
     err = False
     for file in files:
         proc = get_file_config(file, data, dir)
@@ -70,15 +70,15 @@
 def build(dir, target):
     click.echo(click.style(f"⚙️ Building sprocketship!", fg="white", bold=True))
     # Open config in current directory
 
     Path(os.path.join(dir, target)).mkdir(parents=True, exist_ok=True)
 
     data = render_file(
-        os.path.join(dir, "procedures", ".sprocketship.yml"), return_dict=True
+        os.path.join(dir, ".sprocketship.yml"), return_dict=True
     )
     files = list(Path(dir).rglob("*.js"))
 
     err = False
     for file in files:
         proc = get_file_config(file, data, dir)
         try:
```

### Comparing `sprocketship-1.0.0/sprocketship/utils.py` & `sprocketship-1.0.1/sprocketship/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         elif isinstance(value, dict):
             configs.update(extract_configs(value, new_path))
     return configs
 
 
 def get_file_config(path: Path, config: dict, dir: str):
     filename = path.stem
-    keys = str(path.relative_to(dir)).split("/")[:-1] + [filename]
+    keys = ["procedures"] + str(path.relative_to(dir)).split("/")[:-1] + [filename]
+    print(keys)
 
     file_config = {"path": str(path), "name": filename}
     curr_config = config
     for key in keys:
         file_config.update(
             {k[1:]: v for k, v in curr_config.items() if k.startswith("+")}
         )
```

### Comparing `sprocketship-1.0.0/sprocketship.egg-info/PKG-INFO` & `sprocketship-1.0.1/sprocketship.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 1.0.0
+Version: 1.0.1
 Summary: Better stored procedure management
 Author-email: Nicklaus Roach <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -108,25 +108,27 @@
 `pip install sprocketship`
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/` directory at the same level in a directory structure.
+### Structure
+
+Currently, sprocketship expects a `.sprocketship.yml` file in a `procedures/` directory.
 
 ```
 ├── dbt_models
 │   ├── customers.sql
 │   ├── products.sql
 ├── procedures
-│   ├── admin
+│   ├── useradmin
 │   │   ├── create_database_writer_role.js
 │   │   ├── create_database_reader_role.js
-│   ├── development
+│   ├── sysadmin
 │   │   ├── create_temp_database.js
 └── .sprocketship.yml
 ```
 
 The yaml path to each procedure in the `sprocketship.yml` should follow that of the paths to their corresponding files in the `procedures/` directory. 
 
 ```
@@ -145,41 +147,86 @@
 
     - name: create_database_writer
       database: !env_var SNOWFLAKE_DATABASE
       schema: !env_var SNOWFLAKE_SCHEMA
       ...
 ```
 
+### Directory-level Default Parameters
+
+sprocketship allows providing default parameters at any given level of
+your project. These defaults will be applied recursively to any procedures
+defined in any of the subdirectories, unless overridden by a default in one
+of the subdirectories.
+
+```
+procedures:
+  # for all procedures, default to the below database and schema
+  +database: !env_var SNOWFLAKE_DATABASE
+  +schema: !env_var SNOWFLAKE_SCHEMA
+  development:
+    # for all procedures in the development directory,
+    # default to using the sysadmin role
+    +use_role: sysadmin
+    create_temp_database:
+      args:
+        - name: Name of argument
+          type: Type of argument
+          default: (Optional) default value for the argument
+      returns: varchar
+```
+
+### File Frontmatter
+
+Thanks to ABSQL, sprocketship also provides the ability to define parameters using file frontmatter. Suppose we have a file `create_database_writer_role.js`, we can define parameters for the stored procedure within the file using frontmatter:
+
+```js
+/*
+database: my_database
+schema: my_schema
+language: javascript
+execute_as: owner
+use_role: sysadmin
+*/
+```
+
+sprocketship will automatically parse and apply the parameters defined in the frontmatter to the stored procedure.
+
+### Recommended Configuration
+
+When setting up your sprocketship project, we recommend setting more general parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml` file, and anything that's specific to a given procedure should be defined in the file frontmatter of that procedure, such as the args or return type.
+
+### Execution
+
 From here, simply run 
 
 `$ sprocketship liftoff` 
 
 from the project directory (or provide the directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will launch your stored procedures into the given directory. 
 
 ### Exhaustive Options for Stored Procedure Configuration
 
 ```
-name: The name of the procedure
 database: The name of the database where the procedure will be stored
 schema: The name of the schema where the procedure will be stored
 language: The language of the procedure definition
 execute_as: caller or owner
+use_role: The role you'd like to own the procedure
 args:
     - name: Name of argument
       type: Type of argument
       default: (Optional) default value for the argument
-returns: The return type
+returns: The return type, this can include the `NOT NULL` option
 comment: Explanation of the procedure
 ```
 
 ## Support
 
 sprocketship currently only supports Javascript-based stored procedures (Python support coming soon!). Additionally, there are a few options from the `CREATE STORED PROCEDURE` function that are not yet supported:
 
-* `RETURNS <result-data-type> NOT NULL`
 * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }`
 * `VOLATILE | IMMUTABLE` (deprecated)
 
 
 <!-- LICENSE -->
 ## License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 1.0.0 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 1.0.1 Summary: Better stored
 procedure management Author-email: Nicklaus Roach
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/nicklausroach/sprocketship/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake-connector-python Requires-Dist: ABSQL Requires-
@@ -23,43 +23,64 @@
 ## About The Project `sprocketship` makes it easy to develop, manage, and
 deploy stored procedures in Snowflake. Using the language of your choosing, you
 can write the contents of your stored procedure separately from its
 configurations (e.g., `EXECUTE AS`, `RETURN TYPE`, etc.). ### Built With_[_h_t_t_p_s_:
 _/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_p_i_p_e_l_i_n_e_-_t_o_o_l_s_/_A_B_S_Q_L_/
 _5_9_8_f_c_a_b_4_a_5_c_c_b_1_c_a_6_7_4_c_4_0_e_7_4_0_b_4_e_d_d_9_f_9_9_2_5_1_a_6_/_i_m_a_g_e_s_/_l_o_g_o___4_0_0_._s_v_g_]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started ### Installation `pip install sprocketship` ## Usage
-Currently, sprocketship expects a `.sprocketship.yml` file and a `procedures/
-` directory at the same level in a directory structure. ``` âââ
-dbt_models â âââ customers.sql â âââ products.sql âââ
-procedures â âââ admin â â âââ create_database_writer_role.js
-â â âââ create_database_reader_role.js â âââ development â
-â âââ create_temp_database.js âââ .sprocketship.yml ``` The yaml
-path to each procedure in the `sprocketship.yml` should follow that of the
-paths to their corresponding files in the `procedures/` directory. ```
-procedures: development: - name: create_temp_database database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name:
-create_database_reader database: !env_var SNOWFLAKE_DATABASE schema: !env_var
-SNOWFLAKE_SCHEMA ... - name: create_database_writer database: !env_var
-SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... ``` From here, simply
-run `$ sprocketship liftoff` from the project directory (or provide the
-directory, e.g. `sprocketship liftoff my/directory/path`) and sprocketship will
-launch your stored procedures into the given directory. ### Exhaustive Options
-for Stored Procedure Configuration ``` name: The name of the procedure
+## Getting Started ### Installation `pip install sprocketship` ## Usage ###
+Structure Currently, sprocketship expects a `.sprocketship.yml` file in a
+`procedures/` directory. ``` âââ dbt_models â âââ customers.sql
+â âââ products.sql âââ procedures â âââ useradmin â â
+âââ create_database_writer_role.js â â âââ
+create_database_reader_role.js â âââ sysadmin â â âââ
+create_temp_database.js âââ .sprocketship.yml ``` The yaml path to each
+procedure in the `sprocketship.yml` should follow that of the paths to their
+corresponding files in the `procedures/` directory. ``` procedures:
+development: - name: create_temp_database database: !env_var SNOWFLAKE_DATABASE
+schema: !env_var SNOWFLAKE_SCHEMA ... admin: - name: create_database_reader
+database: !env_var SNOWFLAKE_DATABASE schema: !env_var SNOWFLAKE_SCHEMA ... -
+name: create_database_writer database: !env_var SNOWFLAKE_DATABASE schema:
+!env_var SNOWFLAKE_SCHEMA ... ``` ### Directory-level Default Parameters
+sprocketship allows providing default parameters at any given level of your
+project. These defaults will be applied recursively to any procedures defined
+in any of the subdirectories, unless overridden by a default in one of the
+subdirectories. ``` procedures: # for all procedures, default to the below
+database and schema +database: !env_var SNOWFLAKE_DATABASE +schema: !env_var
+SNOWFLAKE_SCHEMA development: # for all procedures in the development
+directory, # default to using the sysadmin role +use_role: sysadmin
+create_temp_database: args: - name: Name of argument type: Type of argument
+default: (Optional) default value for the argument returns: varchar ``` ###
+File Frontmatter Thanks to ABSQL, sprocketship also provides the ability to
+define parameters using file frontmatter. Suppose we have a file
+`create_database_writer_role.js`, we can define parameters for the stored
+procedure within the file using frontmatter: ```js /* database: my_database
+schema: my_schema language: javascript execute_as: owner use_role: sysadmin */
+``` sprocketship will automatically parse and apply the parameters defined in
+the frontmatter to the stored procedure. ### Recommended Configuration When
+setting up your sprocketship project, we recommend setting more general
+parameters (e.g., database, schema, language, etc.) in the `.sprocketship.yml`
+file, and anything that's specific to a given procedure should be defined in
+the file frontmatter of that procedure, such as the args or return type. ###
+Execution From here, simply run `$ sprocketship liftoff` from the project
+directory (or provide the directory, e.g. `sprocketship liftoff my/directory/
+path`) and sprocketship will launch your stored procedures into the given
+directory. ### Exhaustive Options for Stored Procedure Configuration ```
 database: The name of the database where the procedure will be stored schema:
 The name of the schema where the procedure will be stored language: The
-language of the procedure definition execute_as: caller or owner args: - name:
-Name of argument type: Type of argument default: (Optional) default value for
-the argument returns: The return type comment: Explanation of the procedure ```
-## Support sprocketship currently only supports Javascript-based stored
-procedures (Python support coming soon!). Additionally, there are a few options
-from the `CREATE STORED PROCEDURE` function that are not yet supported: *
-`RETURNS NOT NULL` * `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT |
-STRICT }` * `VOLATILE | IMMUTABLE` (deprecated) ## License Distributed under
-the MIT License. See `LICENSE` for more information.
+language of the procedure definition execute_as: caller or owner use_role: The
+role you'd like to own the procedure args: - name: Name of argument type: Type
+of argument default: (Optional) default value for the argument returns: The
+return type, this can include the `NOT NULL` option comment: Explanation of the
+procedure ``` ## Support sprocketship currently only supports Javascript-based
+stored procedures (Python support coming soon!). Additionally, there are a few
+options from the `CREATE STORED PROCEDURE` function that are not yet supported:
+* `CALLED ON NULL INPUT | { RETURNS NULL ON NULL INPUT | STRICT }` * `VOLATILE
+| IMMUTABLE` (deprecated) ## License Distributed under the MIT License. See
+`LICENSE` for more information.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 [contributors-shield]: https://img.shields.io/github/contributors/
 nicklausroach/sprocketship.svg?style=for-the-badge [contributors-url]: https://
 github.com/nicklausroach/sprocketship/graphs/contributors [forks-shield]:
 https://img.shields.io/github/forks/nicklausroach/sprocketship.svg?style=for-
 the-badge [forks-url]: https://github.com/nicklausroach/sprocketship/network/
 members [stars-shield]: https://img.shields.io/github/stars/nicklausroach/
```

