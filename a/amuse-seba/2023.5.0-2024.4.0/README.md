# Comparing `tmp/amuse-seba-2023.5.0.tar.gz` & `tmp/amuse-seba-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-seba-2023.5.0.tar", last modified: Wed May 17 10:19:32 2023, max compression
+gzip compressed data, was "amuse-seba-2024.4.0.tar", last modified: Wed Apr 24 16:32:47 2024, max compression
```

## Comparing `amuse-seba-2023.5.0.tar` & `amuse-seba-2024.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.767240 amuse-seba-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-seba-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1180 2023-05-17 10:19:32.767062 amuse-seba-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       57 2022-11-22 11:55:14.000000 amuse-seba-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.763614 amuse-seba-2023.5.0/amuse_seba.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1180 2023-05-17 10:19:31.000000 amuse-seba-2023.5.0/amuse_seba.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      617 2023-05-17 10:19:32.000000 amuse-seba-2023.5.0/amuse_seba.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:31.000000 amuse-seba-2023.5.0/amuse_seba.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:31.000000 amuse-seba-2023.5.0/amuse_seba.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:31.000000 amuse-seba-2023.5.0/amuse_seba.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-seba-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:32.767401 amuse-seba-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1763 2022-11-22 11:55:14.000000 amuse-seba-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.762005 amuse-seba-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.762058 amuse-seba-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.762106 amuse-seba-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.765458 amuse-seba-2023.5.0/src/amuse/community/seba/
--rw-r--r--   0 rieder     (501) staff       (20)     1576 2023-03-14 13:48:49.000000 amuse-seba-2023.5.0/src/amuse/community/seba/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       28 2023-03-14 13:48:49.000000 amuse-seba-2023.5.0/src/amuse/community/seba/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3014 2023-03-16 12:25:06.000000 amuse-seba-2023.5.0/src/amuse/community/seba/download.py
--rw-r--r--   0 rieder     (501) staff       (20)    30377 2023-03-14 13:48:49.000000 amuse-seba-2023.5.0/src/amuse/community/seba/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)    45633 2023-03-14 13:48:49.000000 amuse-seba-2023.5.0/src/amuse/community/seba/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:31.000000 amuse-seba-2023.5.0/src/amuse/community/seba/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:32.766839 amuse-seba-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-seba-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-seba-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-seba-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.419443 amuse-seba-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-seba-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1211 2024-04-24 16:32:47.419241 amuse-seba-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       57 2022-11-22 11:55:14.000000 amuse-seba-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.418988 amuse-seba-2024.4.0/amuse_seba.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1211 2024-04-24 16:32:46.000000 amuse-seba-2024.4.0/amuse_seba.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      618 2024-04-24 16:32:47.000000 amuse-seba-2024.4.0/amuse_seba.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:46.000000 amuse-seba-2024.4.0/amuse_seba.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:46.000000 amuse-seba-2024.4.0/amuse_seba.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:46.000000 amuse-seba-2024.4.0/amuse_seba.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-seba-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:47.419511 amuse-seba-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1569 2024-04-24 15:35:29.000000 amuse-seba-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.415154 amuse-seba-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.415204 amuse-seba-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.415255 amuse-seba-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.417447 amuse-seba-2024.4.0/src/amuse/community/seba/
+-rw-r--r--   0 rieder     (501) staff       (20)     1576 2023-03-14 13:48:49.000000 amuse-seba-2024.4.0/src/amuse/community/seba/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       28 2023-03-14 13:48:49.000000 amuse-seba-2024.4.0/src/amuse/community/seba/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:46.000000 amuse-seba-2024.4.0/src/amuse/community/seba/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3014 2024-04-24 15:35:29.000000 amuse-seba-2024.4.0/src/amuse/community/seba/download.py
+-rw-r--r--   0 rieder     (501) staff       (20)    33144 2024-04-24 15:35:29.000000 amuse-seba-2024.4.0/src/amuse/community/seba/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)    50340 2024-04-24 15:35:29.000000 amuse-seba-2024.4.0/src/amuse/community/seba/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:47.418797 amuse-seba-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-seba-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-seba-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-seba-2024.4.0/support/version.py
```

### Comparing `amuse-seba-2023.5.0/PKG-INFO` & `amuse-seba-2024.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-seba
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SeBa
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the SeBa community code for AMUSE.
```

### Comparing `amuse-seba-2023.5.0/amuse_seba.egg-info/PKG-INFO` & `amuse-seba-2024.4.0/amuse_seba.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-seba
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - SeBa
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the SeBa community code for AMUSE.
```

### Comparing `amuse-seba-2023.5.0/amuse_seba.egg-info/SOURCES.txt` & `amuse-seba-2024.4.0/amuse_seba.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 amuse_seba.egg-info/PKG-INFO
 amuse_seba.egg-info/SOURCES.txt
 amuse_seba.egg-info/dependency_links.txt
 amuse_seba.egg-info/requires.txt
 amuse_seba.egg-info/top_level.txt
 src/amuse/community/seba/Makefile
 src/amuse/community/seba/__init__.py
+src/amuse/community/seba/_version.py
 src/amuse/community/seba/download.py
 src/amuse/community/seba/interface.cc
 src/amuse/community/seba/interface.py
-src/amuse/community/seba/version.py
 support/__init__.py
 support/classifiers.py
 support/config.py
 support/generate_main.py
 support/getsp.class
 support/getsp.java
 support/misc.py
```

### Comparing `amuse-seba-2023.5.0/setup.py` & `amuse-seba-2024.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.seba.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/seba/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/seba/_version.py",
+}
 
 setup(
     name=name,
     use_scm_version=use_scm_version,
     setup_requires=setup_requires,
-    version=version,
     classifiers=classifiers,
     url=url,
     author_email=author_email,
     author=author,
     license=license_,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     install_requires=install_requires,
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     cmdclass=mapping_from_command_name_to_command_class,
     ext_modules=extensions,
     package_dir={
         'amuse.community.seba': 'src/amuse/community/seba',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-seba-2023.5.0/src/amuse/community/seba/Makefile` & `amuse-seba-2024.4.0/src/amuse/community/seba/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/src/amuse/community/seba/download.py` & `amuse-seba-2024.4.0/src/amuse/community/seba/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     instance.start()
 
 
 def new_option_parser():
     result = OptionParser()
     result.add_option(
         "--seba-version",
-        default='2f6e7f37a53167b4b0dcd6c723dff7b5ee1aecba',
+        default='94e9b1d6ba1466d288a12e3afaa1eba5bca6ddca',
         dest="seba_version",
         help="SeBa commit hash to download",
         type="string"
     )
     return result
```

### Comparing `amuse-seba-2023.5.0/src/amuse/community/seba/interface.cc` & `amuse-seba-2024.4.0/src/amuse/community/seba/interface.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#include "node.h"
 #include "single_star.h"
 #include "main_sequence.h"
 #include "worker_code.h"
 #include "double_star.h"
 
 // AMUSE STOPPING CONDITIONS SUPPORT
 #include <stopcond.h>
@@ -185,14 +184,59 @@
     case Double:
     case no_of_stellar_type:
       return -1;
   }
 }
 
 
+local stellar_type translate_int_to_stellar_type(int type_number) {
+
+  switch (type_number) {
+    case 19:
+      return Brown_Dwarf;
+    case 0:
+    case 1:
+      return Main_Sequence;
+    case 2:
+      return Hertzsprung_Gap;
+    case 3:
+      return Sub_Giant;
+    case 4:
+      return Horizontal_Branch;
+    case 5:
+    case 6:
+      return Super_Giant;
+//      return Hyper_Giant;
+    case 7:
+      return Helium_Star;
+    case 8:
+    case 9:
+      return Helium_Giant;
+    case 10:
+      return Helium_Dwarf;
+    case 11:
+      return Carbon_Dwarf;
+    case 12:
+      return Oxygen_Dwarf;
+    case 13:
+      return Neutron_Star;
+    case 14:
+      return Black_Hole;
+    case 15:
+      return Disintegrated;
+    case 17:
+      return Proto_Star;
+    case 18:
+      return Planet;
+    case -1:
+      return no_of_stellar_type;
+  }
+}
+
+
 
 local int translate_binary_type_to_int(binary_type btp) {
   switch (btp) {
     case Strong_Encounter:
         return -1;
     case Unknown_Binary_Type:
         return 0;
@@ -415,14 +459,55 @@
     *index_of_the_star = next_seba_id;
     
     next_seba_id++;
     
     return 0;
 }
 
+
+int new_advanced_particle(int * index_of_the_star, double mass,  double relative_mass, int type_number,  double age, double core_mass, double COcore_mass,  double radius){
+
+    if (relative_mass == 0) return new_particle(index_of_the_star, mass);
+    if (age < 0) return -1;
+ 
+    node * new_node = new node();
+    new_node->set_label(next_seba_id);
+    new_node->set_parent(seba_root);
+    new_node->set_mass(mass);
+    mapping_from_id_to_node[next_seba_id] = new_node;
+    
+    if(seba_insertion_point == 0) {
+        seba_insertion_point = new_node;
+        seba_root->set_oldest_daughter(new_node);
+    } else {
+        seba_insertion_point->set_younger_sister(new_node);
+        new_node->set_elder_sister(seba_insertion_point);
+        seba_insertion_point = new_node;
+    }
+    
+    stellar_type seba_stellar_type = translate_int_to_stellar_type(type_number);    
+
+    addstar(new_node, seba_time, seba_stellar_type, seba_metallicity, 0, false);
+    new_node->get_starbase()->set_time_offset(seba_time);
+    *index_of_the_star = next_seba_id;
+    
+    next_seba_id++;
+    
+    new_node->get_starbase()->set_relative_age(age);
+    new_node->get_starbase()->set_core_mass(core_mass);
+    new_node->get_starbase()->set_COcore_mass(COcore_mass);
+    new_node->get_starbase()->set_effective_radius(radius);
+    
+    
+    return 0;
+}
+
+
+
+
 int delete_star(int index_of_the_star){
     
     map<int, nodeptr>::iterator i = mapping_from_id_to_node.find(index_of_the_star);
     if(i == mapping_from_id_to_node.end()) {
         return -1;
     } else {
         node * node_to_remove = i->second;
@@ -724,14 +809,15 @@
     if(error_code < 0) {return error_code;}
     *wind_mass_loss_rate = seba_node->get_starbase()->get_wind_constant()*-1.;
     return error_code;
 }
 
 
 
+
 int evolve_one_step(int index_of_the_star){
     int error_code = 0;
     int n_steps_per_phase = 10;
     node * seba_node = get_seba_node_from_index(index_of_the_star, &error_code);
     if(error_code < 0) {return error_code;}
     
     double out_time = seba_node->get_starbase()->get_current_time();
@@ -962,7 +1048,23 @@
     int error_code = 0;
     node * seba_node = get_seba_node_from_index(index_of_the_star, &error_code);
     if(error_code < 0) {return error_code;}
     seba_node->get_starbase()->set_rotation_period(value);
     return error_code;
 }
 
+int get_binary_type(int index_of_the_star, double * value){
+    int error_code = 0;
+    node * seba_node = get_seba_node_from_index(index_of_the_star, &error_code);
+    if(error_code < 0) {return error_code;}
+    *value= seba_node->get_starbase()->get_bin_type();
+    return error_code;
+}
+
+int get_mass_transfer_type(int index_of_the_star, double * value){
+    int error_code = 0;
+    node * seba_node = get_seba_node_from_index(index_of_the_star, &error_code);
+    if(error_code < 0) {return error_code;}
+    *value= seba_node->get_starbase()->get_current_mass_transfer_type();
+    return error_code;
+}
+
```

### Comparing `amuse-seba-2023.5.0/src/amuse/community/seba/interface.py` & `amuse-seba-2024.4.0/src/amuse/community/seba/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,62 @@
         function.addParameter('time_step', dtype='float64', direction=function.OUT)
         function.addParameter('stellar_type', dtype='int32', direction=function.OUT)
         function.result_type = 'int32'
         function.can_handle_array = True
         return function
 
     @legacy_function
+    def new_advanced_particle():
+        """
+        Define a new star in the code. The star will start with the given mass.
+        """
+        function = LegacyFunctionSpecification()
+        function.can_handle_array = True
+        function.addParameter(
+            'index_of_the_star', dtype='int32', direction=function.OUT,
+            description=(
+                "The new index for the star. This index can be used to refer "
+                "to this star in other functions"
+            )
+        )
+        function.addParameter(
+            'mass', dtype='float64', direction=function.IN,
+            description="The initial mass of the star")
+        function.addParameter(
+            'relative_mass', dtype='float64', direction=function.IN, default=0,
+            description="The initial relative mass of the star")
+        function.addParameter(
+            'stellar_type', dtype='int32', direction=function.IN, default=0,
+            description="The initial stellar type of the star")
+        function.addParameter(
+            'age', dtype='float64', direction=function.IN, default=0,
+            description="The initial age of the star")
+        function.addParameter(
+            'core_mass', dtype='float64', direction=function.IN, default=0, 
+            description="The initial core mass of the star")
+        function.addParameter(
+            'COcore_mass', dtype='float64', direction=function.IN, default=0,
+            description="The initial CO core mass of the star")
+        function.addParameter(
+            'radius', dtype='float64', direction=function.IN, default=0,
+            description="The initial radius of the star")
+        # function.addParameter(
+        #     'age_tag', dtype='float64', direction=function.IN,
+        #     description="Starting age of the star *to be specified exactly*")
+        function.result_type = 'int32'
+        function.result_doc = """
+        0 - OK
+            New star was loaded and the index_of_the_star parameter set.
+        -1 - ERROR
+            New star could not be created.
+        """
+        return function
+
+
+    @legacy_function
     def new_binary():
         """
         Define a new star in the code. The star will start with the given mass.
         """
         function = LegacyFunctionSpecification()
         function.can_handle_array = True
         function.addParameter('index_of_the_star', dtype='int32', direction=function.OUT
@@ -141,14 +189,55 @@
         function.result_doc = """
         0 - OK
             The value has been set.
         -1 - ERROR
             A binary with the given index was not found.
         """
         return function
+        
+    @legacy_function
+    def get_binary_type():
+        """
+        Retrieve the current binary type of the binary star.
+        """
+        function = LegacyFunctionSpecification()
+        function.can_handle_array = True
+        function.addParameter('index_of_the_star', dtype='int32', direction=function.IN
+            , description="The index of the star to get the value of")
+        function.addParameter('value', dtype='float64', direction=function.OUT
+            , description="The current binary type.")
+        function.result_type = 'int32'
+        function.result_doc = """
+        0 - OK
+            The value has been set.
+        -1 - ERROR
+            A binary with the given index was not found.
+        """
+        return function
+
+    @legacy_function
+    def get_mass_transfer_type():
+        """
+        Retrieve the current mass transfer type of the binary star.
+        """
+        function = LegacyFunctionSpecification()
+        function.can_handle_array = True
+        function.addParameter('index_of_the_star', dtype='int32', direction=function.IN
+            , description="The index of the star to get the value of")
+        function.addParameter('value', dtype='float64', direction=function.OUT
+            , description="The current mass transfer type.")
+        function.result_type = 'int32'
+        function.result_doc = """
+        0 - OK
+            The value has been set.
+        -1 - ERROR
+            A binary with the given index was not found.
+        """
+        return function
+        
 
     @legacy_function
     def get_core_mass():
         """
         Retrieve the current core mass of a star
         """
         function = LegacyFunctionSpecification()
@@ -247,16 +336,14 @@
         0 - OK
             The value has been set.
         -1 - ERROR
             A binary with the given index was not found.
         """
         return function
 
-
-
     @legacy_function
     def refresh_memory():
         """
         Refresh the memory of SeBa. Update previous parameters in SeBa to current values. 
         """
         function = LegacyFunctionSpecification()
         function.can_handle_array = True
@@ -872,14 +959,19 @@
         )
         handler.add_method(
             "evolve_system",
             (units.Myr,),
             (handler.ERROR_CODE,)
         )
         handler.add_method(
+            "new_advanced_particle",
+            (units.MSun, units.MSun, units.stellar_type, units.Myr, units.MSun, units.MSun, units.RSun),
+            (handler.INDEX, handler.ERROR_CODE)
+        )        
+        handler.add_method(
             "new_binary",
             (units.RSun, handler.NO_UNIT, handler.LINK('particles'), handler.LINK('particles')),
             (handler.INDEX, handler.ERROR_CODE,)
         )
         handler.add_method(
             "delete_binary",
             (handler.INDEX,),
@@ -892,14 +984,24 @@
         )
         handler.add_method(
             "get_semi_major_axis",
             (handler.INDEX,),
             (units.RSun, handler.ERROR_CODE,)
         )
         handler.add_method(
+            "get_binary_type",
+            (handler.INDEX,),
+            (handler.NO_UNIT, handler.ERROR_CODE,)
+        )
+        handler.add_method(
+            "get_mass_transfer_type",
+            (handler.INDEX,),
+            (handler.NO_UNIT, handler.ERROR_CODE,)
+        )        
+        handler.add_method(
             "get_core_mass",
             (handler.INDEX,),
             (units.MSun, handler.ERROR_CODE,)
         )
         handler.add_method(
             "get_COcore_mass",
             (handler.INDEX,),
@@ -1071,30 +1173,33 @@
 
         self.stopping_conditions.define_parameters(handler)
 
 
     def define_particle_sets(self, handler):
 
         handler.define_set('particles', 'index_of_the_star')
-        handler.set_new('particles', 'new_particle')
+#        handler.set_new('particles', 'new_particle')
+        handler.set_new('particles', 'new_advanced_particle')        
         handler.set_delete('particles', 'delete_star')
-
+        
+        
         handler.add_getter('particles', 'get_radius', names = ('radius',))
         handler.add_getter('particles', 'get_stellar_type', names = ('stellar_type',))
         handler.add_getter('particles', 'get_mass', names = ('mass',))
         handler.add_getter('particles', 'get_core_mass', names = ('core_mass',))
-        handler.add_getter('particles', 'get_COcore_mass', names = ('CO_core_mass',))
+        handler.add_getter('particles', 'get_COcore_mass', names = ('COcore_mass',))
         handler.add_getter('particles', 'get_envelope_mass', names = ('envelope_mass',))
         handler.add_getter('particles', 'get_core_radius', names = ('core_radius',))
         handler.add_getter('particles', 'get_age', names = ('age',))
         handler.add_getter('particles', 'get_time_step', names = ('time_step',))
         #handler.add_getter('particles', 'get_spin', names = ('spin',))
         handler.add_getter('particles', 'get_luminosity', names = ('luminosity',))
         handler.add_getter('particles', 'get_temperature', names = ('temperature',))
         handler.add_getter('particles', 'get_natal_kick_velocity', names = ('natal_kick_x','natal_kick_y','natal_kick_z'))
+        
         handler.add_getter('particles', 'get_convective_envelope_mass', names = ('convective_envelope_mass',))
         handler.add_getter('particles', 'get_convective_envelope_radius', names = ('convective_envelope_radius',))
         handler.add_getter('particles', 'get_gyration_radius', names = ('gyration_radius',))
         handler.add_getter('particles', 'get_apsidal_motion_constant', names = ('apsidal_motion_constant',))        
         handler.add_getter('particles', 'get_zeta_thermal', names = ('zeta_thermal',))        
         handler.add_getter('particles', 'get_zeta_adiabatic', names = ('zeta_adiabatic',))        
         handler.add_getter('particles', 'get_rotation_period', names = ('rotation_period',))
@@ -1116,26 +1221,35 @@
         
 
         handler.define_set('binaries', 'index_of_the_star')
         handler.set_new('binaries', 'new_binary')
         handler.set_delete('binaries', 'delete_binary')
 
         handler.add_getter('binaries', 'get_semi_major_axis', names = ('semi_major_axis',))
+        handler.add_setter('binaries', 'set_semi_major_axis', names = ('semi_major_axis',))
         handler.add_getter('binaries', 'get_eccentricity', names = ('eccentricity',))
+        handler.add_setter('binaries', 'set_eccentricity', names = ('eccentricity',))
+
         handler.add_getter('binaries', 'get_mass', names = ('mass',))
         handler.add_getter('binaries', 'get_time_step', names = ('time_step',))
         handler.add_getter('binaries', 'get_age', names = ('age',))
         handler.add_getter("binaries", 'get_children_of_binary')
-        handler.add_setter('binaries', 'set_semi_major_axis', names = ('semi_major_axis',))
-        handler.add_setter('binaries', 'set_eccentricity', names = ('eccentricity',))
+        handler.add_getter('binaries', 'get_binary_type', names = ('binary_type',))
+        handler.add_getter('binaries', 'get_mass_transfer_type', names = ('mass_transfer_type',))
+
         handler.add_method('binaries', 'merge_the_binary')
         
 
         
     def define_state(self, handler):
         se.StellarEvolution.define_state(self, handler)
         
         self.stopping_conditions.define_state(handler)
+        
+        handler.add_method('EDIT', 'new_advanced_particle')
+        handler.add_method('UPDATE', 'new_advanced_particle')
+        handler.add_transition('RUN', 'UPDATE', 'new_advanced_particle', False)
+
 
 
 
 Seba = SeBa
```

### Comparing `amuse-seba-2023.5.0/support/__init__.py` & `amuse-seba-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/classifiers.py` & `amuse-seba-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/config.py` & `amuse-seba-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/generate_main.py` & `amuse-seba-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/getsp.class` & `amuse-seba-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/getsp.java` & `amuse-seba-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/misc.py` & `amuse-seba-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-seba-2023.5.0/support/setup_codes.py` & `amuse-seba-2024.4.0/support/setup_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import configparser
 
 from subprocess import Popen, PIPE, STDOUT
 
 from glob import glob
 
 from distutils.dir_util import create_tree
-# from distutils import log
-import logging
+from distutils import log
 from distutils import spawn
 from distutils import file_util
 from distutils.errors import DistutilsError
 from distutils.command.clean import clean
 from setuptools.command.install import install
 from setuptools import Command
 from setuptools.command.build import build
@@ -556,37 +555,37 @@
         if not os.path.exists(lib_binbuilddir):
             self.mkpath(lib_binbuilddir)
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
-                # self.announce("will copy worker: {0}".format(name), level = logging.INFO)
+                # self.announce("will copy worker: {0}".format(name), level = log.INFO)
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_binbuilddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -599,19 +598,19 @@
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
@@ -620,15 +619,15 @@
                         continue
 
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -712,15 +711,15 @@
         result = list(set(result))
 
         return result
 
     def call(self, arguments, buildlogfile=None, **keyword_arguments):
         stringio = []
 
-        self.announce(' '.join(arguments), logging.DEBUG)
+        self.announce(' '.join(arguments), log.DEBUG)
 
         process = Popen(
             arguments,
             stdout=PIPE,
             stderr=STDOUT,
             **keyword_arguments
         )
@@ -728,24 +727,24 @@
         while True:
             line = process.stdout.readline()
             if len(line) == 0:
                 break
 
             if buildlogfile is not None:
                 buildlogfile.write(line)
-            self.announce(line[:-1].decode("utf-8"), logging.DEBUG)
+            self.announce(line[:-1].decode("utf-8"), log.DEBUG)
             stringio.append(str(line, 'utf-8'))
 
         result = process.wait()
         content = ''.join(stringio)
 
         if result != 0:
-            self.announce("error in call, tail output:\n", logging.INFO)
-            self.announce(''.join(stringio[-100:]), logging.INFO)
-            self.announce("-"*80, logging.INFO)
+            self.announce("error in call, tail output:\n", log.INFO)
+            self.announce(''.join(stringio[-100:]), log.INFO)
+            self.announce("-"*80, log.INFO)
 
         return result, content
 
     def build_environment(self):
         environment = self.environment.copy()
         environment.update(os.environ)
         path = os.path.join(environment["MUSE_PACKAGE_DIR"], "src")
@@ -880,16 +879,16 @@
         build = list()
         lib_build = list()
         lib_not_build = list()
         environment = self.build_environment()
 
         buildlog = 'build.log'
 
-        self.announce("building libraries and community codes", level=logging.INFO)
-        self.announce("build, for logging, see '{0}'".format(buildlog), level=logging.INFO)
+        self.announce("building libraries and community codes", level=log.INFO)
+        self.announce("build, for logging, see '{0}'".format(buildlog), level=log.INFO)
 
         with open(buildlog, "w") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building libraries and codes\n')
             output.write('*'*100)
             output.write('\n')
@@ -898,28 +897,28 @@
             self.copy_build_prereq_to_build_dir()
             self.copy_lib_to_build_dir()
 
         for x in self.makefile_paths(self.lib_dir):
 
             shortname = x[len(self.lib_dir) + 1:] + '-library'
             starttime = datetime.datetime.now()
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
 
             endtime = datetime.datetime.now()
             if returncode == 2:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=logging.DEBUG)
+                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=log.DEBUG)
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(x[len(self.lib_dir) + 1:])
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(x[len(self.lib_dir) + 1:])
                 else:
                     lib_not_build.append(shortname)
             else:
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=logging.DEBUG)
+                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=log.DEBUG)
                 lib_build.append(shortname)
 
         if not self.codes_dir == self.codes_src_dir:
             self.copy_codes_to_build_dir()
 
         # environment.update(self.environment)
         makefile_paths = list(self.makefile_paths(self.codes_dir))
@@ -933,24 +932,24 @@
             # to distribute mesa, it will make the
             # download size from about 100mb size
             # to > 1Gb size.
             #
             # Could we remove some of the data files from mesa?
             #
             if not self.inplace and shortname == 'mesa':
-                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=logging.INFO)
+                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=log.INFO)
                 continue
 
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
             endtime = datetime.datetime.now()
             if returncode > 0:
                 self.announce(
                     "[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(shortname)
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(shortname)
                 elif self.are_python_imports_needed(outputlog):
                     are_python_imports_needed.append(shortname)
@@ -960,40 +959,40 @@
                 if self.is_mpi_enabled():
                     continue
             else:
                 build.append(shortname)
                 is_built = True
                 self.announce(
                     "[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
 
             if not self.variant:
                 continue
 
             special_targets = self.get_special_targets(shortname, x, environment)
             for target, target_name in special_targets:
                 starttime = datetime.datetime.now()
                 self.announce(
                     "[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 returncode, outputlog = self.run_make_on_directory(shortname, x, target, environment)
                 endtime = datetime.datetime.now()
                 if returncode > 0:
                     specials_list = not_build_special.setdefault(shortname,[])
                     specials_list.append(target_name)
                     self.announce(
                         "[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog, endtime),
-                        level=logging.DEBUG
+                        level=log.DEBUG
                     )
                 else:
                     build_to_special_targets.setdefault(shortname, list()).append(target_name)
                     self.announce(
-                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=logging.DEBUG
+                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=log.DEBUG
                     )
 
         # if supportrc["framework_install"]:
         #     self.copy_config_to_build_dir()
 
         if not self.codes_dir == self.codes_src_dir:
             # self.copy_worker_codes_to_build_dir()
@@ -1028,17 +1027,17 @@
             not_build
             or not_build_special
             or is_download_needed
             or is_cuda_needed
             or are_python_imports_needed
         ):
             if not_build:
-                level = logging.WARN
+                level = log.WARN
             else:
-                level = logging.INFO
+                level = log.INFO
             if not_build:
                 self.announce(
                     "Community codes not built (because of errors/ missing libraries):",
                     level=level
                 )
                 self.announce("="*80,  level=level)
                 for x in not_build:
@@ -1061,26 +1060,26 @@
                     self.announce(
                         f' * {x} , make {x}.code DOWNLOAD_CODES=1', level=level
                     )
 
             self.announce("="*80,  level=level)
 
         if build:
-            level = logging.INFO
+            level = log.INFO
             self.announce("Community codes built",  level=level)
             self.announce("="*80,  level=level)
             for x in build:
                 if x in build_to_special_targets:
                     y = build_to_special_targets[x]
                     self.announce('* {0} ({1})'.format(x, ','.join(y)), level=level)
                 else:
                     self.announce('* {0}'.format(x),  level=level)
             self.announce("="*80,  level=level)
 
-        level = logging.INFO
+        level = log.INFO
         self.announce(
             "{0} out of {1} codes built, {2} out of {3} libraries built".format(
                 len(build), 
                 len(build) + len(not_build), 
                 len(lib_build), 
                 len(lib_build) + len(lib_not_build)
             ),
```

