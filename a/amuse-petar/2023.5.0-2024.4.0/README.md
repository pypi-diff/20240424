# Comparing `tmp/amuse-petar-2023.5.0.tar.gz` & `tmp/amuse-petar-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-petar-2023.5.0.tar", last modified: Wed May 17 10:19:23 2023, max compression
+gzip compressed data, was "amuse-petar-2024.4.0.tar", last modified: Wed Apr 24 16:32:41 2024, max compression
```

## Comparing `amuse-petar-2023.5.0.tar` & `amuse-petar-2024.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.170067 amuse-petar-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-petar-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2023-05-17 10:19:23.169904 amuse-petar-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       58 2022-11-22 11:55:14.000000 amuse-petar-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.165634 amuse-petar-2023.5.0/amuse_petar.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2023-05-17 10:19:21.000000 amuse-petar-2023.5.0/amuse_petar.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      666 2023-05-17 10:19:23.000000 amuse-petar-2023.5.0/amuse_petar.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:21.000000 amuse-petar-2023.5.0/amuse_petar.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:19:21.000000 amuse-petar-2023.5.0/amuse_petar.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:19:21.000000 amuse-petar-2023.5.0/amuse_petar.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-petar-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:23.170112 amuse-petar-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1770 2022-11-22 11:55:14.000000 amuse-petar-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.163960 amuse-petar-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.164009 amuse-petar-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.164060 amuse-petar-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.168192 amuse-petar-2023.5.0/src/amuse/community/petar/
--rw-r--r--   0 rieder     (501) staff       (20)     2610 2023-04-17 09:09:36.000000 amuse-petar-2023.5.0/src/amuse/community/petar/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/src/amuse/community/petar/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)     3782 2023-05-11 09:04:53.000000 amuse-petar-2023.5.0/src/amuse/community/petar/download.py
--rw-r--r--   0 rieder     (501) staff       (20)    34712 2023-05-04 12:36:05.000000 amuse-petar-2023.5.0/src/amuse/community/petar/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)     3280 2023-04-17 08:13:01.000000 amuse-petar-2023.5.0/src/amuse/community/petar/interface.h
--rw-r--r--   0 rieder     (501) staff       (20)    16287 2023-04-17 09:06:51.000000 amuse-petar-2023.5.0/src/amuse/community/petar/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:21.000000 amuse-petar-2023.5.0/src/amuse/community/petar/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:23.169669 amuse-petar-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-petar-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-petar-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-petar-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.775871 amuse-petar-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-petar-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1214 2024-04-24 16:32:41.775658 amuse-petar-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       58 2022-11-22 11:55:14.000000 amuse-petar-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.775374 amuse-petar-2024.4.0/amuse_petar.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1214 2024-04-24 16:32:40.000000 amuse-petar-2024.4.0/amuse_petar.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      667 2024-04-24 16:32:41.000000 amuse-petar-2024.4.0/amuse_petar.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:40.000000 amuse-petar-2024.4.0/amuse_petar.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:40.000000 amuse-petar-2024.4.0/amuse_petar.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:40.000000 amuse-petar-2024.4.0/amuse_petar.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-petar-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:41.775928 amuse-petar-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1575 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.771230 amuse-petar-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.771281 amuse-petar-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.771333 amuse-petar-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.773750 amuse-petar-2024.4.0/src/amuse/community/petar/
+-rw-r--r--   0 rieder     (501) staff       (20)     2552 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/src/amuse/community/petar/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/src/amuse/community/petar/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:40.000000 amuse-petar-2024.4.0/src/amuse/community/petar/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     3983 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/src/amuse/community/petar/download.py
+-rw-r--r--   0 rieder     (501) staff       (20)    35542 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/src/amuse/community/petar/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)     3279 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/src/amuse/community/petar/interface.h
+-rw-r--r--   0 rieder     (501) staff       (20)    18167 2024-04-24 15:35:29.000000 amuse-petar-2024.4.0/src/amuse/community/petar/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:41.775161 amuse-petar-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-petar-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-petar-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-petar-2024.4.0/support/version.py
```

### Comparing `amuse-petar-2023.5.0/PKG-INFO` & `amuse-petar-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-petar
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - PeTar
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
 
 This package installs the PeTar community code for AMUSE.
```

### Comparing `amuse-petar-2023.5.0/amuse_petar.egg-info/PKG-INFO` & `amuse-petar-2024.4.0/amuse_petar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-petar
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - PeTar
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
 
 This package installs the PeTar community code for AMUSE.
```

### Comparing `amuse-petar-2023.5.0/amuse_petar.egg-info/SOURCES.txt` & `amuse-petar-2024.4.0/amuse_petar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 amuse_petar.egg-info/PKG-INFO
 amuse_petar.egg-info/SOURCES.txt
 amuse_petar.egg-info/dependency_links.txt
 amuse_petar.egg-info/requires.txt
 amuse_petar.egg-info/top_level.txt
 src/amuse/community/petar/Makefile
 src/amuse/community/petar/__init__.py
+src/amuse/community/petar/_version.py
 src/amuse/community/petar/download.py
 src/amuse/community/petar/interface.cc
 src/amuse/community/petar/interface.h
 src/amuse/community/petar/interface.py
-src/amuse/community/petar/version.py
 support/__init__.py
 support/classifiers.py
 support/config.py
 support/generate_main.py
 support/getsp.class
 support/getsp.java
 support/misc.py
```

### Comparing `amuse-petar-2023.5.0/setup.py` & `amuse-petar-2024.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.petar.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/petar/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/petar/_version.py",
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
         'amuse.community.petar': 'src/amuse/community/petar',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-petar-2023.5.0/src/amuse/community/petar/Makefile` & `amuse-petar-2024.4.0/src/amuse/community/petar/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -36,55 +36,53 @@
 CXXFLAGS += -D INTERFACE_DEBUG_PRINT
 CXXFLAGS += -D INTERFACE_DEBUG
 
 LDFLAGS  += -lm $(MUSE_LD_FLAGS)
 
 OBJS = interface.o 
 
-FILELIST=interface.cc interface.py interface.h
+DIRLIST=src/PeTar src/SDAR src/FDPS
 
 CODELIB = 
 
 all: petar_worker __init__.py
 
 clean:
 	$(RM) -rf __pycache__
 	$(RM) -f *.so *.o *.pyc worker_code.cc worker_code.h 
 	$(RM) *~ petar_worker worker_code.cc
 #	make -C src clean
 
 distclean: clean
-	rm -rf src $(FILELIST)
+	rm -rf src
 
 #$(CODELIB):
 #	make -C src all
 
 DOWNLOAD_FROM_WEB = $(PYTHON) ./download.py
 
-download:
-	$(RM) -Rf .pc
-	$(RM) -Rf src
-	mkdir src
+$(DIRLIST):
+#	$(RM) -Rf .pc
+#	$(RM) -Rf src
+#       mkdir src
 	$(DOWNLOAD_FROM_WEB)
 
 __init__.py:
 	touch $@
 
-$(FILELIST): |download
-
-src/PeTar/src/get_version.hpp: src/PeTar/src/get_version.hpp.in |src/PeTar
+src/PeTar/src/get_version.hpp: |src/PeTar
 	sed 's/@VERSION@/'`cat src/PeTar/VERSION`'_'`cat src/SDAR/VERSION`'/g' src/PeTar/src/get_version.hpp.in >src/PeTar/src/get_version.hpp
 
 test_interface: $(OBJS) test_interface.o
 	$(MPICXX) $(CXXFLAGS) $(OBJS) test_interface.o -o $@
 
 worker_code.cc: interface.py
 	$(CODE_GENERATOR) --type=c interface.py petarInterface -o $@
 
 worker_code.h: interface.py 
 	$(CODE_GENERATOR) --type=H -i amuse.community.interface.stopping_conditions.StoppingConditionInterface interface.py petarInterface -o $@
 
 petar_worker: worker_code.cc worker_code.h $(CODELIB) $(OBJS) interface.h
 	$(MPICXX) $(CXXFLAGS) $(SC_FLAGS) $(AM_CFLAGS) $(LDFLAGS) $< $(OBJS) $(CODELIB) -o $@ $(SC_MPI_CLIBS) $(LIBS) $(AM_LIBS)
 
-interface.o: interface.cc src/PeTar/src/get_version.hpp 
+interface.o: interface.cc src/PeTar/src/get_version.hpp |$(DIRLIST)
 	$(MPICXX) $(CXXFLAGS) $(SC_FLAGS) -c -o $@ $<
```

### Comparing `amuse-petar-2023.5.0/src/amuse/community/petar/download.py` & `amuse-petar-2024.4.0/src/amuse/community/petar/download.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,29 +43,33 @@
                 name
             ],
             cwd=os.path.join(self.src_directory())
         )
         print("done")
 
     def start(self):
-        if os.path.exists('src'):
-            counter = 0
-            while os.path.exists('src.{0}'.format(counter)):
-                counter += 1
-                if counter > 100:
-                    print("too many backup directories")
-                    break
-            os.rename('src', 'src.{0}'.format(counter))
-
-        os.mkdir('src')
+        if not os.path.exists('src'):
+            os.mkdir('src')
+#            if not update_flag:
+#                return
+#            counter = 0
+#            while os.path.exists('src.{0}'.format(counter)):
+#                counter += 1
+#                if counter > 100:
+#                    print("too many backup directories")
+#                    break
+#            os.rename('src', 'src.{0}'.format(counter))
 
         for i, url_template in enumerate(self.url_template):
             url = url_template.format(version=self.version[i])
             filename = self.filename_template.format(version=self.version[i])
             filepath = os.path.join(self.src_directory(), filename)
+            if os.path.exists('src/'+self.name[i]):
+                print("src/%s exist" % self.name[i])
+                continue
             print(
                 "downloading version", self.version[i],
                 "from", url, "to", filename
             )
             if which('wget') is not None:
                 arguments = ['wget', url]
                 subprocess.call(
```

### Comparing `amuse-petar-2023.5.0/src/amuse/community/petar/interface.cc` & `amuse-petar-2024.4.0/src/amuse/community/petar/interface.cc`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #else
     static CalcForcePPNoSimd<ParticleBase,FPSoft> fcalc;
 #endif
     static int n_particle_in_interrupt_connected_cluster_glb; // 
 
     // flags
     static bool particle_list_change_flag=true;
+    static bool initial_particle_flag=false;
 
     // common
 
     int initialize_code() {
         PeTar::initial_fdps_flag = true;
         ptr = new PeTar;
 
@@ -98,14 +99,16 @@
     }
 
     int recommit_parameters() {
 #ifdef INTERFACE_DEBUG_PRINT
         if(ptr->my_rank==0) std::cout<<"PETAR: recommit_parameters start\n";
 #endif
         ptr->input_parameters.n_glb.value = ptr->stat.n_real_glb;
+        ptr->input_parameters.update_changeover_flag = true;
+        ptr->input_parameters.update_rsearch_flag = true;
         ptr->initialParameters();
         ptr->initial_step_flag = false;
 
         // set stopping condtions support
         set_support_for_condition(COLLISION_DETECTION);
         set_support_for_condition(PAIR_DETECTION);
 
@@ -119,14 +122,23 @@
         return 0;
     }
 
     // GravitationalDynamicsInterface
 
     int new_particle(int* index_of_the_particle,  double mass, double x, double y, double z, double vx, double vy, double vz, double radius) {
         // if not yet initial the system
+#ifdef INTERFACE_DEBUG_PRINT
+        if (!ptr->read_data_flag && ptr->my_rank==0) {
+            std::cout<<"New particle, rank "<<ptr->my_rank<<std::endl;
+            std::cout<<std::setw(20)<<"ID";
+            ParticleBase::printColumnTitle(std::cout);
+            std::cout<<std::endl;
+        }
+#endif
+
         ptr->read_data_flag = true;
         
         PS::S64 id_offset = ptr->input_parameters.id_offset.value;
         PS::S64 n_glb = ptr->stat.n_real_glb;
         PS::S64 n_loc = ptr->stat.n_real_loc;
 #ifdef INTERFACE_DEBUG
         assert(n_loc == ptr->system_soft.getNumberOfParticleLocal());
@@ -148,18 +160,33 @@
             p.id = n_glb+1;
             if (p.id>=id_offset) return -1;
             p.group_data.artificial.setParticleTypeToSingle();
 
             p.rank_org = ptr->my_rank;
             p.adr = n_loc;
 
+            if (initial_particle_flag) {
+                PS::F64 m_fac = p.mass*Ptcl::mean_mass_inv;
+                PS::F64 r_out = ptr->input_parameters.r_out.value;
+                PS::F64 r_in = r_out*ptr->input_parameters.ratio_r_cut.value;
+                p.changeover.setR(m_fac, r_in, r_out);
+                p.calcRSearch(ptr->input_parameters.dt_soft.value);
+            }
+            
             ptr->system_soft.addOneParticle(p);
 
             ptr->stat.n_real_loc++;
             *index_of_the_particle = p.id;
+#ifdef INTERFACE_DEBUG_PRINT
+            std::cout<<std::setprecision(14);
+            std::cout<<std::setw(20)<<p.id;
+            p.ParticleBase::printColumn(std::cout);
+            std::cout<<std::endl;
+#endif
+
         }
         ptr->stat.n_real_glb++;
 
         particle_list_change_flag = true;
 
         return 0;
     }
@@ -502,32 +529,14 @@
             *az = p->acc.z;
         }    
         else return -1;
 #endif
         return 0;
     }
 
-    int set_acceleration(int index_of_the_particle, double ax, double ay, double az) {
-        reconstruct_particle_list();
-        int index = ptr->getParticleAdrFromID(index_of_the_particle);
-        if (index>=0) {
-            FPSoft* p = &(ptr->system_soft[index]);
-            p->acc.x = ax; 
-            p->acc.y = ay; 
-            p->acc.z = az; 
-        }    
-#ifdef PARTICLE_SIMULATOR_MPI_PARALLEL
-        int check = PS::Comm::getMaxValue(index);
-        if (check==-1) return -1;
-#else
-        else return -1;
-#endif
-        return 0;
-    }
-
     int get_potential(int index_of_the_particle, double * potential) {
         reconstruct_particle_list();
         int index = ptr->getParticleAdrFromID(index_of_the_particle);
 #ifdef PARTICLE_SIMULATOR_MPI_PARALLEL
         double pot_local = 0.0;
         if (index>=0) {
             FPSoft* p = &(ptr->system_soft[index]);
@@ -544,15 +553,15 @@
         else return -1;
 #endif
         return 0;
     }
 
     int evolve_model(double time_next) {
 #ifdef INTERFACE_DEBUG_PRINT
-        if(ptr->my_rank==0) std::cout<<"PETAR: evolve models start\n";
+        if(ptr->my_rank==0) std::cout<<"PETAR: evolve models to "<<time_next<< "start\n";
 #endif
 
         if (ptr->stat.n_real_glb==0) {// escape if no particle
 #ifdef INTERFACE_DEBUG_PRINT
             if(ptr->my_rank==0) std::cout<<"PETAR: evolve models end\n";
 #endif
             return 0;
@@ -727,14 +736,15 @@
         if (!ptr->read_parameters_flag) return -1;
         if (!ptr->read_data_flag) return -1;
         ptr->input_parameters.n_glb.value = ptr->stat.n_real_glb;
         ptr->initialParameters();
         ptr->initialStep();
         ptr->reconstructIdAdrMap();
         particle_list_change_flag = false;
+        initial_particle_flag = true;
 #ifdef INTERFACE_DEBUG_PRINT
         if(ptr->my_rank==0) std::cout<<"PETAR: commit_particles end\n";
 #endif
         return 0;
     }
 
     int synchronize_model() {
@@ -855,14 +865,25 @@
     }
 
     int get_tree_step(double* dt_soft) {
         *dt_soft = ptr->input_parameters.dt_soft.value;
         return 0;
     }
 
+    int set_output_step(double dt_snap) {
+        ptr->input_parameters.dt_snap.value = dt_snap;
+        return 0;
+    }
+
+    int get_output_step(double* dt_snap) {
+        *dt_snap = ptr->input_parameters.dt_snap.value;
+        return 0;
+    }
+
+
     //// set gravitational constant
     //int set_gravitational_constant(double G) {
     //    ptr->input_parameters.unit_set.value=-1;
     //    ptr->input_parameters.gravitational_constant.value = G;
     //    return 0;
     //}
     //
```

### Comparing `amuse-petar-2023.5.0/src/amuse/community/petar/interface.h` & `amuse-petar-2024.4.0/src/amuse/community/petar/interface.h`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 
 int get_velocity(int index_of_the_particle, double * vx, double * vy, double * vz);
 
 int set_velocity(int index_of_the_particle, double vx, double vy, double vz);
 
 int get_acceleration(int index_of_the_particle, double * ax, double * ay, double * az);
 
-int set_acceleration(int index_of_the_particle, double ax, double ay, double az);
-
 int get_potential(int index_of_the_particle, double * potential);
 
 int evolve_model(double time);
 
 int commit_particles();
 
 int synchronize_model();
@@ -83,14 +81,18 @@
 
 int set_rsearch_min(double r_search_min);
 
 int get_tree_step(double * dt_soft);
 
 int set_tree_step(double dt_soft);
 
+int get_output_step(double * dt_output);
+
+int set_output_step(double dt_output);
+
 int get_kinetic_energy(double * kinetic_energy);
 
 int get_potential_energy(double * potential_energy);
 
 int get_time(double * time);
 
 int get_begin_time(double * time);
```

### Comparing `amuse-petar-2023.5.0/src/amuse/community/petar/interface.py` & `amuse-petar-2024.4.0/src/amuse/community/petar/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -352,14 +352,56 @@
         0 - OK
             the parameter was set
         -1 - ERROR
             could not set parameter
         """
         return function
 
+    @legacy_function
+    def get_output_step():
+        """
+        Get dt_output, the PeTar internal output time step (0.125)
+        """
+        function = LegacyFunctionSpecification()
+        function.addParameter(
+            'dt_output', dtype='float64', direction=function.OUT,
+            description=(
+                "dt_output, the PeTar internal output time step (0.125)"
+            )
+        )
+        function.result_type = 'int32'
+        function.result_doc = """
+        0 - OK
+            the parameter was retrieved
+        -1 - ERROR
+            could not retrieve parameter
+        """
+        return function
+
+    @legacy_function
+    def set_output_step():
+        """
+        Set dt_output, the PeTar internal output time step (0.125)
+        """
+        function = LegacyFunctionSpecification()
+        function.addParameter(
+            'dt_output', dtype='float64', direction=function.IN,
+            description=(
+                "dt_output, the PeTar internal output time step (0.125)"
+            )
+        )
+        function.result_type = 'int32'
+        function.result_doc = """
+        0 - OK
+            the parameter was set
+        -1 - ERROR
+            could not set parameter
+        """
+        return function
+
 
 class petar(GravitationalDynamics, GravityFieldCode):
 
     def __init__(self, convert_nbody=None, **keyword_arguments):
         self.stopping_conditions = StoppingConditions(self)
 
         GravitationalDynamics.__init__(
@@ -439,14 +481,22 @@
             "get_tree_step",
             "set_tree_step",
             "dt_soft",
             "Tree time step (if zero, auto-determine)",
             default_value=0.0 | nbody_system.time
         )
 
+        handler.add_method_parameter(
+            "get_output_step",
+            "set_output_step",
+            "dt_output",
+            "PeTar internal output time step (0.125)",
+            default_value=0.125 | nbody_system.time
+        )
+
     def define_methods(self, handler):
         GravitationalDynamics.define_methods(self, handler)
         self.stopping_conditions.define_methods(handler)
 
         handler.add_method(
             "set_eps2",
             (
@@ -538,14 +588,33 @@
             (),
             (
                 nbody_system.time,
                 handler.ERROR_CODE,
             )
         )
 
+        handler.add_method(
+            "set_output_step",
+            (
+                nbody_system.time,
+            ),
+            (
+                handler.ERROR_CODE,
+            )
+        )
+
+        handler.add_method(
+            "get_output_step",
+            (),
+            (
+                nbody_system.time,
+                handler.ERROR_CODE,
+            )
+        )
+
     def define_particle_sets(self, handler):
         GravitationalDynamics.define_particle_sets(self, handler)
         self.stopping_conditions.define_particle_set(handler)
 
 
 PetarInterface = petarInterface
 Petar = petar
```

### Comparing `amuse-petar-2023.5.0/support/__init__.py` & `amuse-petar-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/classifiers.py` & `amuse-petar-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/config.py` & `amuse-petar-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/generate_main.py` & `amuse-petar-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/getsp.class` & `amuse-petar-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/getsp.java` & `amuse-petar-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/misc.py` & `amuse-petar-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-petar-2023.5.0/support/setup_codes.py` & `amuse-petar-2024.4.0/support/setup_codes.py`

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

