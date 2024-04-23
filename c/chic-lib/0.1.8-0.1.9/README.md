# Comparing `tmp/chic-lib-0.1.8.tar.gz` & `tmp/chic-lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chic-lib-0.1.8.tar", last modified: Mon Feb 26 09:57:41 2024, max compression
+gzip compressed data, was "chic-lib-0.1.9.tar", last modified: Tue Apr 23 17:09:01 2024, max compression
```

## Comparing `chic-lib-0.1.8.tar` & `chic-lib-0.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-02-26 09:57:41.368993 chic-lib-0.1.8/
--rw-rw-r--   0 tcnicholas   (503) staff       (20)    35149 2023-03-03 14:29:31.000000 chic-lib-0.1.8/LICENSE
--rw-rw-r--   0 tcnicholas   (503) staff       (20)        0 2023-03-03 14:29:31.000000 chic-lib-0.1.8/MANIFEST.in
--rw-r--r--   0 tcnicholas   (503) staff       (20)     1797 2024-02-26 09:57:41.368569 chic-lib-0.1.8/PKG-INFO
--rw-rw-r--   0 tcnicholas   (503) staff       (20)     1250 2023-10-25 16:55:57.000000 chic-lib-0.1.8/README.md
-drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-02-26 09:57:41.365204 chic-lib-0.1.8/chic/
--rw-r--r--   0 tcnicholas   (503) staff       (20)      482 2024-02-26 09:56:52.000000 chic-lib-0.1.8/chic/__init__.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    18485 2024-02-23 13:37:43.000000 chic-lib-0.1.8/chic/atomic_cluster.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     4090 2023-10-14 21:09:53.000000 chic-lib-0.1.8/chic/bonds.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    11980 2024-02-03 13:47:17.000000 chic-lib-0.1.8/chic/cif.py
-drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-02-26 09:57:41.365904 chic-lib-0.1.8/chic/coarse_graining_methods/
--rw-r--r--   0 tcnicholas   (503) staff       (20)        0 2023-07-30 18:30:14.000000 chic-lib-0.1.8/chic/coarse_graining_methods/__init__.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     2872 2024-02-03 13:29:23.000000 chic-lib-0.1.8/chic/coarse_graining_methods/defaults.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     5537 2024-02-21 18:40:20.000000 chic-lib-0.1.8/chic/decorate.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    15468 2023-11-09 17:52:03.000000 chic-lib-0.1.8/chic/gulp.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    22670 2024-02-23 10:42:53.000000 chic-lib-0.1.8/chic/lammps.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    32497 2024-02-23 10:04:27.000000 chic-lib-0.1.8/chic/net.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     4269 2024-02-23 09:58:00.000000 chic-lib-0.1.8/chic/rattle.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     9553 2023-11-02 16:20:13.000000 chic-lib-0.1.8/chic/scatty.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     2473 2023-08-11 12:59:59.000000 chic-lib-0.1.8/chic/sort_sites.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    75669 2024-02-23 14:56:50.000000 chic-lib-0.1.8/chic/structure.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    18914 2024-02-26 09:56:16.000000 chic-lib-0.1.8/chic/templates.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)      716 2023-07-27 17:56:01.000000 chic-lib-0.1.8/chic/tidy.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)    14315 2023-10-26 10:43:24.000000 chic-lib-0.1.8/chic/utils.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     3868 2023-10-14 19:48:13.000000 chic-lib-0.1.8/chic/vasp.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     2986 2024-01-19 10:09:07.000000 chic-lib-0.1.8/chic/vector.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     1322 2023-10-14 19:48:39.000000 chic-lib-0.1.8/chic/xyz.py
--rw-r--r--   0 tcnicholas   (503) staff       (20)     4681 2023-10-14 19:56:27.000000 chic-lib-0.1.8/chic/zif.py
-drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-02-26 09:57:41.367925 chic-lib-0.1.8/chic_lib.egg-info/
--rw-r--r--   0 tcnicholas   (503) staff       (20)     1797 2024-02-26 09:57:41.000000 chic-lib-0.1.8/chic_lib.egg-info/PKG-INFO
--rw-r--r--   0 tcnicholas   (503) staff       (20)      566 2024-02-26 09:57:41.000000 chic-lib-0.1.8/chic_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tcnicholas   (503) staff       (20)        1 2024-02-26 09:57:41.000000 chic-lib-0.1.8/chic_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tcnicholas   (503) staff       (20)       47 2024-02-26 09:57:41.000000 chic-lib-0.1.8/chic_lib.egg-info/requires.txt
--rw-r--r--   0 tcnicholas   (503) staff       (20)        5 2024-02-26 09:57:41.000000 chic-lib-0.1.8/chic_lib.egg-info/top_level.txt
--rw-r--r--   0 tcnicholas   (503) staff       (20)       38 2024-02-26 09:57:41.369145 chic-lib-0.1.8/setup.cfg
--rw-r--r--   0 tcnicholas   (503) staff       (20)      999 2024-02-26 09:56:54.000000 chic-lib-0.1.8/setup.py
+drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-04-23 17:09:01.878347 chic-lib-0.1.9/
+-rw-rw-r--   0 tcnicholas   (503) staff       (20)    35149 2023-03-03 14:29:31.000000 chic-lib-0.1.9/LICENSE
+-rw-rw-r--   0 tcnicholas   (503) staff       (20)        0 2023-03-03 14:29:31.000000 chic-lib-0.1.9/MANIFEST.in
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     1934 2024-04-23 17:09:01.877905 chic-lib-0.1.9/PKG-INFO
+-rw-rw-r--   0 tcnicholas   (503) staff       (20)     1250 2023-10-25 16:55:57.000000 chic-lib-0.1.9/README.md
+drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-04-23 17:09:01.873768 chic-lib-0.1.9/chic/
+-rw-r--r--   0 tcnicholas   (503) staff       (20)      574 2024-04-23 17:08:30.000000 chic-lib-0.1.9/chic/__init__.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    18485 2024-04-12 21:55:57.000000 chic-lib-0.1.9/chic/atomic_cluster.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     4090 2023-10-14 21:09:53.000000 chic-lib-0.1.9/chic/bonds.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    12078 2024-04-14 16:31:29.000000 chic-lib-0.1.9/chic/cif.py
+drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-04-23 17:09:01.874691 chic-lib-0.1.9/chic/coarse_graining_methods/
+-rw-r--r--   0 tcnicholas   (503) staff       (20)        0 2023-07-30 18:30:14.000000 chic-lib-0.1.9/chic/coarse_graining_methods/__init__.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     2872 2024-02-03 13:29:23.000000 chic-lib-0.1.9/chic/coarse_graining_methods/defaults.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     5537 2024-02-21 18:40:20.000000 chic-lib-0.1.9/chic/decorate.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    15468 2023-11-09 17:52:03.000000 chic-lib-0.1.9/chic/gulp.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    22670 2024-03-26 14:19:01.000000 chic-lib-0.1.9/chic/lammps.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    32774 2024-03-01 23:59:45.000000 chic-lib-0.1.9/chic/net.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     4269 2024-02-23 09:58:00.000000 chic-lib-0.1.9/chic/rattle.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     9553 2023-11-02 16:20:13.000000 chic-lib-0.1.9/chic/scatty.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     2473 2023-08-11 12:59:59.000000 chic-lib-0.1.9/chic/sort_sites.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    78409 2024-04-23 17:04:22.000000 chic-lib-0.1.9/chic/structure.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    18925 2024-03-08 15:28:26.000000 chic-lib-0.1.9/chic/templates.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)      716 2023-07-27 17:56:01.000000 chic-lib-0.1.9/chic/tidy.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)    14315 2023-10-26 10:43:24.000000 chic-lib-0.1.9/chic/utils.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     3868 2023-10-14 19:48:13.000000 chic-lib-0.1.9/chic/vasp.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     2986 2024-01-19 10:09:07.000000 chic-lib-0.1.9/chic/vector.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     1322 2023-10-14 19:48:39.000000 chic-lib-0.1.9/chic/xyz.py
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     4681 2023-10-14 19:56:27.000000 chic-lib-0.1.9/chic/zif.py
+drwxr-xr-x   0 tcnicholas   (503) staff       (20)        0 2024-04-23 17:09:01.877384 chic-lib-0.1.9/chic_lib.egg-info/
+-rw-r--r--   0 tcnicholas   (503) staff       (20)     1934 2024-04-23 17:09:01.000000 chic-lib-0.1.9/chic_lib.egg-info/PKG-INFO
+-rw-r--r--   0 tcnicholas   (503) staff       (20)      566 2024-04-23 17:09:01.000000 chic-lib-0.1.9/chic_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 tcnicholas   (503) staff       (20)        1 2024-04-23 17:09:01.000000 chic-lib-0.1.9/chic_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 tcnicholas   (503) staff       (20)       47 2024-04-23 17:09:01.000000 chic-lib-0.1.9/chic_lib.egg-info/requires.txt
+-rw-r--r--   0 tcnicholas   (503) staff       (20)        5 2024-04-23 17:09:01.000000 chic-lib-0.1.9/chic_lib.egg-info/top_level.txt
+-rw-r--r--   0 tcnicholas   (503) staff       (20)       38 2024-04-23 17:09:01.878451 chic-lib-0.1.9/setup.cfg
+-rw-r--r--   0 tcnicholas   (503) staff       (20)      999 2024-04-23 17:06:59.000000 chic-lib-0.1.9/setup.py
```

### Comparing `chic-lib-0.1.8/LICENSE` & `chic-lib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/PKG-INFO` & `chic-lib-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: chic-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of tools for coarse-graining and back-mapping frameworks.
 Home-page: https://github.com/tcnicholas/chic
 Author: Thomas C Nicholas
 Author-email: thomas.nicholas@chem.ox.ac.uk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: pymatgen
+Requires-Dist: ase
+Requires-Dist: networkx
 
 # CHIC
 **C**oarse-graining **H**ybrid **I**organic **C**rystals.
 
 ![Schematic of decorating and coarse-graining the sodalite (**sod**) net](/bin/images/sod-decoration.png)
```

### Comparing `chic-lib-0.1.8/README.md` & `chic-lib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/atomic_cluster.py` & `chic-lib-0.1.9/chic/atomic_cluster.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/bonds.py` & `chic-lib-0.1.9/chic/bonds.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/cif.py` & `chic-lib-0.1.9/chic/cif.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 27.07.23
 @tcnicholas
 Handling CIFs.
 """
 
 import warnings
 from pathlib import Path
+from datetime import datetime
 from typing import Tuple, Dict, Union
 
 import numpy as np
 from scipy.spatial import cKDTree
 from pymatgen.io.cif import CifParser
 
 from .bonds import Bonding
@@ -277,16 +278,20 @@
 
 
     def _header(self) -> str:
         """
         Generates the header of file string.
         """
         form = f"'{self._parent_structure.composition.anonymized_formula}'"
-        return (f"data_{self._name}\n"
-            f"_chemical_formula_sum {form:>{60-len('_chemical_formula_sum')}}\n")
+        date = datetime.now().strftime('%Y-%m-%d')
+        return (
+            f"data_{self._name}\n"
+            f"_audit_creation_date {date:>{60-len('_audit_creation_date')}}\n"
+            f"_chemical_formula_sum {form:>{60-len('_chemical_formula_sum')}}\n"
+        )
 
 
     def _cell_loop(self) -> str:
         """
         Writes unit cell loop to file string.
         """
         cell_params = np.ravel(self._parent_structure.lattice.parameters)
@@ -296,62 +301,66 @@
         cell_string = (f"_cell_length_a\t\t\t{cell_params[0]:.5f}\n"
                        f"_cell_length_b\t\t\t{cell_params[1]:.5f}\n"
                        f"_cell_length_c\t\t\t{cell_params[2]:.5f}\n"
                        f"_cell_angle_alpha\t\t{cell_params[3]:.5f}\n"
                        f"_cell_angle_beta\t\t{cell_params[4]:.5f}\n"
                        f"_cell_angle_gamma\t\t{cell_params[5]:.5f}\n"
                        f"_cell_volume\t\t\t{volume:.5f}\n"
-                       f"_cell_formula_units_Z\t\t{int(Z)}\n"
-                       "_symmetry_space_group_name_H-M\t'P 1'\n"
-                       "_symmetry_Int_Tables_number\t1\n"
+                       f"_cell_formula_units_z\t\t{int(Z)}\n"
+                       "_symmetry_space_group_name_h-m\t'P 1'\n"
+                       "_symmetry_int_tables_number\t1\n"
                        "loop_\n"
-                       "_symmetry_equiv_pos_site_id\n"
-                       "_symmetry_equiv_pos_as_xyz\n"
+                       "_space_group_symop_id\n"
+                       "_space_group_symop_operation_xyz\n"
                        "1 x,y,z\n")
 
         return cell_string
 
 
     def _positions_loop(self) -> str:
         """
         Writes atom positions loop.
         """
-        positions = ["loop_\n",
-                     "_atom_site_label\n",
-                     "_atom_site_type_symbol\n",
-                     "_atom_site_symmetry_multiplicity\n",
-                     "_atom_site_fract_x\n",
-                     "_atom_site_fract_y\n",
-                     "_atom_site_fract_z\n",
-                     "_atom_site_occupancy\n"]
+        positions = [
+            "loop_\n",
+            "_atom_site_label\n",
+            "_atom_site_type_symbol\n",
+            "_atom_site_symmetry_multiplicity\n",
+            "_atom_site_fract_x\n",
+            "_atom_site_fract_y\n",
+            "_atom_site_fract_z\n",
+            "_atom_site_occupancy\n"
+        ]
 
         positions.extend(
             bead.to_topocif_string() + "\n" for bead in self._beads.values()
         )
         return ''.join(positions)
 
 
     def _bonds_loop(self) -> str:
         """
         Writes bonds loop to file string in the TopoCIF format.
         """
-        bonds = ["loop_\n",
-                 "_topol_link.node_label_1\n",
-                 "_topol_link.node_label_2\n",
-                 "_topol_link.distance\n",
-                 "_topol_link.site_symmetry_symop_1\n",
-                 "_topol_link.site_symmetry_translation_1_x\n",
-                 "_topol_link.site_symmetry_translation_1_y\n",
-                 "_topol_link.site_symmetry_translation_1_z\n",
-                 "_topol_link.site_symmetry_symop_2\n",
-                 "_topol_link.site_symmetry_translation_2_x\n",
-                 "_topol_link.site_symmetry_translation_2_y\n",
-                 "_topol_link.site_symmetry_translation_2_z\n",
-                 "_topol_link.type\n",
-                 "_topol_link.multiplicity\n"]
+        bonds = [
+            "loop_\n",
+            "_topol_link.node_label_1\n",
+            "_topol_link.node_label_2\n",
+            "_topol_link.distance\n",
+            "_topol_link.site_symmetry_symop_1\n",
+            "_topol_link.site_symmetry_translation_1_x\n",
+            "_topol_link.site_symmetry_translation_1_y\n",
+            "_topol_link.site_symmetry_translation_1_z\n",
+            "_topol_link.site_symmetry_symop_2\n",
+            "_topol_link.site_symmetry_translation_2_x\n",
+            "_topol_link.site_symmetry_translation_2_y\n",
+            "_topol_link.site_symmetry_translation_2_z\n",
+            "_topol_link.type\n",
+            "_topol_link.multiplicity\n"
+        ]
 
         for edge, images in self._bead_bonds.items():
             atom1 = self._beads[edge[0]].label
             atom2 = self._beads[edge[1]].label
             for image in images:
                 bonds.append(format_bond(
                     atom1,
```

### Comparing `chic-lib-0.1.8/chic/coarse_graining_methods/defaults.py` & `chic-lib-0.1.9/chic/coarse_graining_methods/defaults.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/decorate.py` & `chic-lib-0.1.9/chic/decorate.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/gulp.py` & `chic-lib-0.1.9/chic/gulp.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/lammps.py` & `chic-lib-0.1.9/chic/lammps.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/net.py` & `chic-lib-0.1.9/chic/net.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,14 +237,15 @@
         ] if fallbacks is not None else []
         all_templates = [template] if fallbacks is None else [template] + fallback_templates
 
         # if we allow for multiple templates, we need to be able to call them for
         # each unit when outputting the structures.
         self._templates = all_templates
         self._template_names = []
+        this_template = all_templates[0]
 
         atom_id = 1
         for mol_id, (label, ix) in enumerate(self._label_index.items(), 1):
 
             centroid = self[ix].coords
 
             if 'Si' in label:
@@ -259,14 +260,15 @@
                     1,
                     template.property_by_symbol('Zn', 'charge'),
                     *list(centroid)
                 ])
                 atom_id += 1
                 self._formula["A"] += 1
                 self._template_names.append(template.name)
+                
             
             elif 'O' in label:
 
                 fb = 0
                 placement_ok = False
                 num_fallbacks = 1 if fallbacks is None else len(all_templates)
                 while (fb < num_fallbacks) and not placement_ok:
@@ -289,21 +291,26 @@
                     coords = place_linker(
                         this_template,
                         centroid,
                         self._bonding.bond_by_label(label)
                     )
 
                     # now check distance constraints.
-                    f1 = self._lattice.get_fractional_coords(coords)
-                    f2 = self._lattice.get_fractional_coords(
-                        np.array(self._decorated_atoms)[:,-3:]
-                    )
-                    d = self._lattice.get_all_distances(f1,f2)
-                    if not np.any(d < closest_approach):
+                    placement_ok = False
+                    if not len(self._decorated_atoms):
                         placement_ok = True
+                    else:
+                        f1 = self._lattice.get_fractional_coords(coords)
+                        f2 = self._lattice.get_fractional_coords(
+                            np.array(self._decorated_atoms)[:,-3:]
+                        )
+                        d = self._lattice.get_all_distances(f1,f2)
+                        if not np.any(d < closest_approach):
+                            placement_ok = True
+                        
 
                     fb += 1
 
                 atom_data = zip(*[
                     this_template.atom_types, this_template.atom_charges, coords
                 ])
```

### Comparing `chic-lib-0.1.8/chic/rattle.py` & `chic-lib-0.1.9/chic/rattle.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/scatty.py` & `chic-lib-0.1.9/chic/scatty.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/sort_sites.py` & `chic-lib-0.1.9/chic/sort_sites.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/structure.py` & `chic-lib-0.1.9/chic/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,15 @@
         self._min_intra_bond_length = None
         self._max_intra_bond_length = None
         self._minimum_coordination_numbers = None
         self._maximum_coordination_numbers = None
         self._beads = None
         self._bead_bonds = defaultdict(list)
         self._bead_neighbour_list = defaultdict(list)
+        self._bead2cluster = defaultdict(str)
         
         # whether to default pickle.
         self.__pickle_dir__ = None
         self.__allow_pickle__ = allow_pickle
         self.__setup_pickle__()
 
 
@@ -314,15 +315,15 @@
         # set the CrystalNN kwargs.
         cnn_kwargs = {
             'weighted_cn': True,
             'cation_anion': False,
             'distance_cutoffs': (0.5, 1),
             'x_diff_weight': 0,
             'porous_adjustment': True,
-            'search_cutoff': 7.0,
+            'search_cutoff': 10.0,
             'fingerprint_length': None
         }
         cnn_kwargs.update(kwargs)
 
         # compute the neighbourlist. we hide the warnings because CrystalNN
         # throws a lot of them.
         with warnings.catch_warnings():
@@ -402,14 +403,46 @@
                     )
         
         if self.__allow_pickle__:
             with open(self.__pickle_dir__ / 'nl.pickle', 'wb') as f:
                 pickle.dump(self._neighbour_list, f, pickle.HIGHEST_PROTOCOL)
 
 
+    def get_neighbours_by_cutoff(self, rcut: float = 1.8) -> None:
+        """
+        Compute the neighbourlist with a single radial cut-off for all atoms.
+
+        Arguments:
+            rcut: the radial cut-off to apply for neighbour searching.
+        """
+
+        # use Pymatgen's neighbourlist function to compute it. This returns a 
+        # list of PeriodicNeighbors for each atom.
+        ns = self.get_all_neighbors(rcut)
+
+        # Re-format for cluster analysis.
+        nl = defaultdict(list)
+        for i, neighbours in enumerate(ns):
+            
+            # We need to keep sites with no neighbours!
+            if not neighbours:
+                nl[i] = []
+
+            for neighbour in neighbours:
+                nl[i].append({
+                    'site': neighbour,
+                    'image': neighbour.image,
+                    'weight': 1.0,
+                    'site_index': neighbour.index
+                })
+
+        # sort the dictionary by atom index.
+        self._neighbour_list = dict(sorted(nl.items()))
+
+
     @classmethod
     def from_structure(cls, 
         structure: PymatgenStructure, 
         atomic_clusters=None,
         **kwargs
     ) -> 'Structure':
         """
@@ -614,24 +647,24 @@
         self._min_intra_weight = parse_arguments(
             0.2, min_intra_weight, self._all_sites
         )
         self._min_intra_bond_length = parse_arguments(
             0.0, min_intra_bond_length, self._all_sites
         )
         self._max_intra_bond_length = parse_arguments(
-            2.0, max_intra_bond_length, self._all_sites
+            2.5, max_intra_bond_length, self._all_sites
         )
         self._min_inter_weight = parse_arguments(
             0.4, min_inter_weight, self._all_sites
         )
         self._min_inter_bond_length = parse_arguments(
             0.0, min_inter_bond_length, self._all_sites
         )
         self._max_inter_bond_length = parse_arguments(
-            None, max_inter_bond_length, self._all_sites
+            3.0, max_inter_bond_length, self._all_sites
         )
 
         # compute adjacency matrix using the neighbourlist and any constraints.
         adjacency_matrix = self._get_adjacency_matrix()
 
         # identify clusters
         clusters = self._identify_clusters(adjacency_matrix)
@@ -847,14 +880,15 @@
 
         def default_factory() -> int:
             """ Start the defaultdict counter at 1. """
             return 1
         
         all_beads = {}
         bead_mol_id = 1
+        self._bead2cluster = defaultdict(str)
         number_of_species = defaultdict(default_factory)
         for label, cluster in self._atomic_clusters.items():
             
             # first, check if the cluster should be skipped.
             if skip_non_framework and cluster.skip:
                 continue
             
@@ -905,14 +939,15 @@
                     bead_id, 
                     bead_mol_id,
                     frac_coord,
                     energy=elocal,
                     force=fcm
                 )
                 number_of_species[species] += 1
+                self._bead2cluster[bead_id] = label
 
             # increment the bead mol ID.
             bead_mol_id += 1
 
         # store the beads.
         self._beads = all_beads
 
@@ -1254,16 +1289,15 @@
         
         # gather beads.
         self.get_beads({'a': 'H', 'b': 'O'})
 
         # select keywords. opti conp bond property molq phon eigenmodes
         if keywords is None:
             keywords = [
-                'conp', 'bond', 'property', 'molq', 'phon', 
-                'eigenmodes'
+                'conp', 'bond', 'property', 'molq', 'phon', 'eigenmodes'
             ]
         
         # we cam now proceed to reduce the net to the framework nodes and write
         # to a GULP input file.
         _gulp_kwargs = {
             'sub_elem': 'H',
             'rattle': 0.0,
@@ -1472,14 +1506,52 @@
 
         :param filename: name of file to write.
         """
         if not self._neighbour_list:
             raise 
 
 
+    def _get_adjacency_matrix_new(self) -> csr_matrix:
+        """
+        Compute a global adjacency matrix for all intra-unit bonds.
+        """
+        data = []
+        i_indices = []
+        j_indices = []
+        
+        for site_index, site_neighbours in self._neighbour_list.items():
+            this_site = self[site_index]
+            this_site_type = self._get_site_type_index(this_site.specie.symbol)
+            
+            # Use a list comprehension to filter neighbours based on conditions
+            filtered_neighbours = [
+                neighbour for neighbour in site_neighbours
+                if self._get_site_type_index(neighbour['site'].specie.symbol) == this_site_type
+                and self._check_neighbour_conditions('intra', neighbour, self._all_sites[this_site_type])
+            ]
+            
+            for neighbour in filtered_neighbours:
+                data.append(1)
+                i_indices.append(site_index)
+                j_indices.append(neighbour['site_index'])
+                
+            # Update the neighbour list with only the filtered neighbours
+            self._neighbour_list[site_index] = filtered_neighbours
+
+        # Construct the CSR matrix using the data and indices
+        adjacency_matrix = csr_matrix(
+            (data, (i_indices, j_indices)), 
+            shape=(self.num_sites, self.num_sites)
+        ).maximum(
+            csr_matrix((data, (j_indices, i_indices)), 
+            shape=(self.num_sites, self.num_sites))
+        )
+        return adjacency_matrix
+
+
     def _get_adjacency_matrix(self) -> csr_matrix:
         """
         Compute a global adjacency matrix for all intra-unit bonds.
         """
         data = []
         i_indices = []
         j_indices = []
@@ -1501,15 +1573,16 @@
                 
                 site_type = self._all_sites[this_site_type]                
                 if self._check_neighbour_conditions('intra',neighbour,site_type):
                     data.append(1)
                     i_indices.append(site_index)
                     j_indices.append(neighbour['site_index'])
                 else:
-                    site_neighbours.remove(neighbour)
+                    pass
+                    #site_neighbours.remove(neighbour)
 
         adjacency_matrix = csr_matrix(
             (data, (i_indices, j_indices)), 
             shape=(self.num_sites, self.num_sites)
         ).maximum(
             csr_matrix((data, (j_indices, i_indices)), 
             shape=(self.num_sites, self.num_sites))
@@ -1626,14 +1699,15 @@
                     neighbor_index = neighbor['site_index']
                     if neighbor_index in images:
                         # Use the visited neighbor's image and relative image to
                         # assign the new image
                         neighbor_image = neighbor['image']
                         images[site_index] = images[neighbor_index] + neighbor_image
                         break
+
                 if site_index not in images:
                     # If no visited neighbor with image was found, raise error.
                     raise ValueError(
                         f"No image found for site index {site_index}, "
                         "and no visited neighbor with an image to use as "
                         "a reference."
                     )
```

### Comparing `chic-lib-0.1.8/chic/templates.py` & `chic-lib-0.1.9/chic/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
         [-1.12928266,       0.37738000,      -0.00024851],  # N(b)      [4]
         [ 1.41029730,      -1.77527570,      -0.01096395],  # H1(a)     [5]
         [-1.41030640,      -1.77527599,      -0.01098257],  # H1(b)     [6]
         [-0.00000493,       2.22845998,      -0.01704101],  # H2        [7]
     ], dtype=np.float64)
     
     # updated coordinates from VEJYUF (ZIF-4) experimental structure.
-    coordinates = np.array([
+    coordinates_experiment = np.array([
         [-0.00259284,       1.09794768,      -0.00748570],  # C2        [0]
         [-0.67922515,      -0.91839665,      -0.00155239],  # C1(a)     [1]
         [ 0.68361712,      -0.92484814,      -0.00264092],  # C1(b)     [2]
         [-1.11273746,       0.37477594,       0.00550580],  # N(a)      [3]
         [ 1.11093832,       0.37052117,       0.00617321],  # N(b)      [4]
         [-1.22963442,      -1.67977267,      -0.00552243],  # H1(a)     [5]
         [ 1.23315722,      -1.68711056,      -0.00644115],  # H1(b)     [6]
```

### Comparing `chic-lib-0.1.8/chic/tidy.py` & `chic-lib-0.1.9/chic/tidy.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/utils.py` & `chic-lib-0.1.9/chic/utils.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/vasp.py` & `chic-lib-0.1.9/chic/vasp.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/vector.py` & `chic-lib-0.1.9/chic/vector.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/xyz.py` & `chic-lib-0.1.9/chic/xyz.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic/zif.py` & `chic-lib-0.1.9/chic/zif.py`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/chic_lib.egg-info/PKG-INFO` & `chic-lib-0.1.9/chic_lib.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 Metadata-Version: 2.1
 Name: chic-lib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A set of tools for coarse-graining and back-mapping frameworks.
 Home-page: https://github.com/tcnicholas/chic
 Author: Thomas C Nicholas
 Author-email: thomas.nicholas@chem.ox.ac.uk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: pymatgen
+Requires-Dist: ase
+Requires-Dist: networkx
 
 # CHIC
 **C**oarse-graining **H**ybrid **I**organic **C**rystals.
 
 ![Schematic of decorating and coarse-graining the sodalite (**sod**) net](/bin/images/sod-decoration.png)
```

### Comparing `chic-lib-0.1.8/chic_lib.egg-info/SOURCES.txt` & `chic-lib-0.1.9/chic_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chic-lib-0.1.8/setup.py` & `chic-lib-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='chic-lib',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'scikit-learn',
         'pymatgen',
         'ase',
```

