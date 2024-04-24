# Comparing `tmp/mbtiles_util-1.0.0.tar.gz` & `tmp/mbtiles_util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbtiles_util-1.0.0.tar", last modified: Mon Apr 22 08:37:15 2024, max compression
+gzip compressed data, was "mbtiles_util-1.0.2.tar", last modified: Wed Apr 24 08:02:34 2024, max compression
```

## Comparing `mbtiles_util-1.0.0.tar` & `mbtiles_util-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:37:15.035109 mbtiles_util-1.0.0/
--rw-rw-rw-   0        0        0      579 2024-04-22 08:37:15.035109 mbtiles_util-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-04-22 08:16:08.000000 mbtiles_util-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 08:37:15.029599 mbtiles_util-1.0.0/mbtiles_util/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:34:15.000000 mbtiles_util-1.0.0/mbtiles_util/__init__.py
--rw-rw-rw-   0        0        0      928 2024-04-22 07:41:29.000000 mbtiles_util-1.0.0/mbtiles_util/latlong.py
--rw-rw-rw-   0        0        0     2757 2024-04-22 07:51:11.000000 mbtiles_util-1.0.0/mbtiles_util/mbtiles2folder.py
--rw-rw-rw-   0        0        0      541 2024-04-22 03:58:16.000000 mbtiles_util-1.0.0/mbtiles_util/vt2geo.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:37:15.035109 mbtiles_util-1.0.0/mbtiles_util.egg-info/
--rw-rw-rw-   0        0        0      579 2024-04-22 08:37:14.000000 mbtiles_util-1.0.0/mbtiles_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-22 08:37:14.000000 mbtiles_util-1.0.0/mbtiles_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:37:14.000000 mbtiles_util-1.0.0/mbtiles_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-22 08:37:14.000000 mbtiles_util-1.0.0/mbtiles_util.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-04-22 08:37:14.000000 mbtiles_util-1.0.0/mbtiles_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 08:37:15.035109 mbtiles_util-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      798 2024-04-22 08:36:44.000000 mbtiles_util-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:02:34.601915 mbtiles_util-1.0.2/
+-rw-rw-rw-   0        0        0    11524 2024-04-22 09:15:57.000000 mbtiles_util-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1122 2024-04-24 08:02:34.601915 mbtiles_util-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2024-04-23 07:42:20.000000 mbtiles_util-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:02:34.592347 mbtiles_util-1.0.2/mbtiles_util/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:34:15.000000 mbtiles_util-1.0.2/mbtiles_util/__init__.py
+-rw-rw-rw-   0        0        0     2963 2024-04-23 07:34:27.000000 mbtiles_util-1.0.2/mbtiles_util/mbtiles2folder.py
+-rw-rw-rw-   0        0        0     4047 2024-04-23 09:06:00.000000 mbtiles_util-1.0.2/mbtiles_util/mbtiles2s3.py
+-rw-rw-rw-   0        0        0     4389 2024-04-23 03:19:55.000000 mbtiles_util-1.0.2/mbtiles_util/mbtilesinfo.py
+-rw-rw-rw-   0        0        0     3755 2024-04-24 04:27:18.000000 mbtiles_util-1.0.2/mbtiles_util/osm2mbtiles.py
+-rw-rw-rw-   0        0        0     2093 2024-04-24 03:39:11.000000 mbtiles_util-1.0.2/mbtiles_util/pbfinfo.py
+-rw-rw-rw-   0        0        0      668 2024-04-22 09:14:25.000000 mbtiles_util-1.0.2/mbtiles_util/tileserve.py
+-rw-rw-rw-   0        0        0    15360 2024-04-22 12:20:34.000000 mbtiles_util-1.0.2/mbtiles_util/util.py
+-rw-rw-rw-   0        0        0      710 2024-04-24 04:27:43.000000 mbtiles_util-1.0.2/mbtiles_util/versatiles.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:02:34.600939 mbtiles_util-1.0.2/mbtiles_util.egg-info/
+-rw-rw-rw-   0        0        0     1122 2024-04-24 08:02:34.000000 mbtiles_util-1.0.2/mbtiles_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-24 08:02:34.000000 mbtiles_util-1.0.2/mbtiles_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:02:34.000000 mbtiles_util-1.0.2/mbtiles_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2024-04-24 08:02:34.000000 mbtiles_util-1.0.2/mbtiles_util.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 08:02:34.000000 mbtiles_util-1.0.2/mbtiles_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:02:34.601915 mbtiles_util-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1014 2024-04-24 08:02:13.000000 mbtiles_util-1.0.2/setup.py
```

### Comparing `mbtiles_util-1.0.0/mbtiles_util/mbtiles2folder.py` & `mbtiles_util-1.0.2/mbtiles_util/mbtiles2folder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,97 @@
-
 import os
-import sys
-import sqlite3, json
+import sqlite3
+import json
 import argparse
+from tqdm import tqdm
 
-######################################
-# Helper functions
-
-def safeMakeDir(d):
+def safe_makedir(d):
   if os.path.exists(d):
     return
   os.makedirs(d)
 
-def setDir(d):
-  safeMakeDir(d)
+def set_dir(d):
+  safe_makedir(d)
   os.chdir(d)
 
-######################################
-def main():
-  parser = argparse.ArgumentParser(description='Convert MBTiles file to folder')
-
-  # Add your command-line arguments/options here
-  parser.add_argument('-i', help='Input MBTiles file name')
-  parser.add_argument('-o', help='Output folder name')
-
-  # Parse the command-line arguments
-  args = parser.parse_args()
-
-  # if not len(sys.argv) == 3:
-  #   print ('Please provide  the mbtiles input filename and output folder')
-  #   exit()
-
-  if not args.i or not args.o:
-    print ('Please provide the mbtiles input filename and output folder name')
-    exit()
-
-
-  # Process input
-  # input_filename = sys.argv[1]
-  input_filename = args.i
-  # dirname = input_filename[0:input_filename.index('.')]
-  # dirname = sys.argv[2]
-  dirname = args.o
-  print ('Converting file "%s" into tiles in local directory "%s"' % (input_filename, dirname))
-
-  # This will fail if there is already a directory.
-  os.makedirs(dirname)
-
-  # Database connection boilerplate
-  connection = sqlite3.connect(input_filename)
-  cursor = connection.cursor()
-
+def extract_metadata(cursor):
+  """Extract metadata from MBTiles file."""
   cursor.execute("SELECT name, value FROM metadata")
   metadata_rows = cursor.fetchall()
-
-  # Extract metadata
   metadata = {}
   for name, value in metadata_rows:
       metadata[name] = value
+  return metadata
 
-  # Write metadata to JSON file
+def write_metadata_to_json(metadata, dirname):
+  """Write metadata to JSON file."""
   metadata_json_path = os.path.join(dirname, "metadata.json")
   with open(metadata_json_path, "w") as metadata_file:
       json.dump(metadata, metadata_file, indent=4)
-  print ("Writing metadata.json done!")
+  print("Writing metadata.json done!")
 
-  # Read format type from metadata
+def determine_tile_format(cursor):
+  """Determine tile format based on metadata."""
   cursor.execute("SELECT value FROM metadata WHERE name='format'")
   tile_format = cursor.fetchone()
-
   if tile_format:
       if tile_format[0] == 'png' or tile_format[0] == 'webp':
-          out_format = '.png'
+          return '.png'
       elif tile_format[0] == 'jpg':
-          out_format = '.jpg'
+          return '.jpg'
       elif tile_format[0] == 'pbf':
-          out_format = '.pbf'
-  else:
-      out_format = ''
-
-  # select all info in tiles view
-  cursor.execute('SELECT zoom_level, tile_column, tile_row, tile_data FROM tiles')
-
-  os.chdir(dirname)
-  for row in cursor:
-    setDir(str(row[0]))
-    setDir(str(row[1]))
-    # y = (2^row[0] - 1) - row[2]
-    output_file = open(str(row[2]) + out_format, 'wb')
-    # output_file = open(str(y) + out_format, 'wb')
-    output_file.write(row[3])
-    output_file.close()
-    os.chdir('..')
-    os.chdir('..')
+          return '.pbf'
+  return ''
+
+def count_total_tiles(cursor):
+  """Count total number of tiles."""
+  cursor.execute('SELECT COUNT(*) FROM tiles')
+  return cursor.fetchone()[0]
+
+def convert_mbtiles_to_folder(input_filename, output_folder):
+  """Convert MBTiles file to folder."""
+  os.makedirs(output_folder)
+  connection = sqlite3.connect(input_filename)
+  cursor = connection.cursor()  
+
+  
+  tile_format = determine_tile_format(cursor)
+  total_tiles = count_total_tiles(cursor)
+  metadata = extract_metadata(cursor)
+  write_metadata_to_json(metadata, output_folder)
+ 
+  os.chdir(output_folder)
+  cursor.execute('SELECT zoom_level, tile_column, tile_row, tile_data FROM tiles order by zoom_level')
+  with tqdm(total=total_tiles, desc="Progress", unit="tile") as pbar:      
+    for row in cursor:
+      set_dir(str(row[0]))
+      set_dir(str(row[1]))
+      output_file = open(str(row[2]) + tile_format, 'wb')
+      output_file.write(row[3])
+      output_file.close()
+      os.chdir('..')
+      os.chdir('..')
+      pbar.update(1)
+
+  print('Converting mbtiles to folder done!')
+  connection.close()
+
+def main():
+  parser = argparse.ArgumentParser(description='Convert MBTiles file to folder')
+  parser.add_argument('-i', help='Input MBTiles file name')
+  parser.add_argument('-o', help='Output folder name')
+  args = parser.parse_args()
+
+  if not args.i:
+    print('Please provide the mbtiles input filename.')
+    exit()
+  if not os.path.exists(args.i):
+    print('MBTiles file does not exist!. Please recheck and input a correct file path.')
+    exit()
+  if not args.o:
+    print('Please provide the output folder name.')
+    exit()
+  
+  convert_mbtiles_to_folder(args.i, args.o)
 
-  print ('Done!')
 if __name__ == "__main__":
     main()
```

### Comparing `mbtiles_util-1.0.0/setup.py` & `mbtiles_util-1.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # python setup.py sdist bdist_wheel
-#twine upload dist/*
+# twine upload dist/*
 
 
 from setuptools import setup, find_packages
 
 setup(
     name='mbtiles_util',
-    version='1.0.0',
+    version='1.0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
+            'mbtilesinfo = mbtiles_util.mbtilesinfo:main',
             'mbtiles2folder = mbtiles_util.mbtiles2folder:main',
+            'mbtiles2s3 = mbtiles_util.mbtiles2s3:main'            
         ],
     },
     description='MBTiles Utilities',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[],
     author='Thang Quach',
     author_email='quachdongthang@gmail.com',
     url='https://github.com/thangqd/mbtiles_util',
     classifiers=[
         'Programming Language :: Python :: 3',
+        'Environment :: Console',
+        'Topic :: Scientific/Engineering :: GIS',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

