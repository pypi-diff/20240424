# Comparing `tmp/auto_classification_generator-1.1.2.tar.gz` & `tmp/auto_classification_generator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_classification_generator-1.1.2.tar", last modified: Thu Apr  4 10:33:14 2024, max compression
+gzip compressed data, was "auto_classification_generator-1.1.3.tar", last modified: Sun Apr 21 19:15:36 2024, max compression
```

## Comparing `auto_classification_generator-1.1.2.tar` & `auto_classification_generator-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.2/LICENSE.md
--rw-rw-rw-   0        0        0      642 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5494 2024-02-20 15:40:54.000000 auto_classification_generator-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.006857 auto_classification_generator-1.1.2/auto_classification_generator/
--rw-rw-rw-   0        0        0      408 2024-02-20 15:29:18.000000 auto_classification_generator-1.1.2/auto_classification_generator/__init__.py
--rw-rw-rw-   0        0        0    14871 2024-04-04 09:56:06.000000 auto_classification_generator-1.1.2/auto_classification_generator/classification_generator.py
--rw-rw-rw-   0        0        0     2619 2024-04-04 10:31:14.000000 auto_classification_generator-1.1.2/auto_classification_generator/cli.py
--rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.2/auto_classification_generator/common.py
--rw-rw-rw-   0        0        0     1011 2024-03-24 00:10:19.000000 auto_classification_generator-1.1.2/auto_classification_generator/hash.py
--rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.2/auto_classification_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-04 10:31:21.000000 auto_classification_generator-1.1.2/auto_classification_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/
--rw-rw-rw-   0        0        0      642 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-04 10:33:13.000000 auto_classification_generator-1.1.2/auto_classification_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      791 2024-04-04 10:31:27.000000 auto_classification_generator-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 10:33:14.053861 auto_classification_generator-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0      642 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8408 2024-04-21 18:05:12.000000 auto_classification_generator-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.567937 auto_classification_generator-1.1.3/auto_classification_generator/
+-rw-rw-rw-   0        0        0      451 2024-04-21 18:40:21.000000 auto_classification_generator-1.1.3/auto_classification_generator/__init__.py
+-rw-rw-rw-   0        0        0    15384 2024-04-21 18:04:22.000000 auto_classification_generator-1.1.3/auto_classification_generator/classification_generator.py
+-rw-rw-rw-   0        0        0     2618 2024-04-21 18:40:30.000000 auto_classification_generator-1.1.3/auto_classification_generator/cli.py
+-rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.3/auto_classification_generator/common.py
+-rw-rw-rw-   0        0        0      978 2024-04-12 13:13:37.000000 auto_classification_generator-1.1.3/auto_classification_generator/hash.py
+-rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.3/auto_classification_generator/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-04-21 18:52:54.000000 auto_classification_generator-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 19:15:36.629979 auto_classification_generator-1.1.3/setup.cfg
```

### Comparing `auto_classification_generator-1.1.2/LICENSE.md` & `auto_classification_generator-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.2/PKG-INFO` & `auto_classification_generator-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator/classification_generator.py` & `auto_classification_generator-1.1.3/auto_classification_generator/classification_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 author: Christopher Prince
 license: Apache License 2.0"
 """
 
 from auto_classification_generator.common import *
 from auto_classification_generator.hash import *
-import os, stat
+import os
+import stat
 import pandas as pd
 from datetime import datetime
 import time
 
 class ClassificationGenerator():
     def __init__(self,
                  root: str,
@@ -25,254 +26,294 @@
                  start_ref: int = 1,
                  fixity: str = None,
                  empty_flag: bool = False,
                  skip_flag: bool = False,
                  accession_flag: bool = False,
                  meta_dir_flag: bool = True,
                  hidden_flag: bool = False,
-                 output_format: str ="xlsx"):
-        
+                 output_format: str = "xlsx"):
+
         self.root = os.path.abspath(root)
         self.root_level = self.root.count(os.sep)
-        self.root_path = os.path.dirname(self.root)         
+        self.root_path = os.path.dirname(self.root)
         self.output_path = output_path
         self.output_format = output_format
         self.empty_flag = empty_flag
         self.skip_flag = skip_flag
         self.hidden_flag = hidden_flag
         self.prefix = prefix
         self.start_ref = start_ref
         self.fixity = fixity
         self.reference_list = []
         self.record_list = []
         self.accession_flag = accession_flag
         self.accession_list = []
         self.accession_count = start_ref
-        if accprefix: self.accession_prefix = accprefix
-        else: self.accession_prefix = prefix
+        if accprefix:
+            self.accession_prefix = accprefix
+        else:
+            self.accession_prefix = prefix
         self.empty_list = []
         self.meta_dir_flag = meta_dir_flag
-    
+        self.start_time = datetime.now()
+
+    def print_running_time(self):
+        print(f'\nRunning time: {datetime.now() - self.start_time}')
+
     def remove_empty_directories(self):
         """
-        Remove's empty directories with a warning.
+        Remove empty directories with a warning.
         """
         confirm_delete = input('\n***WARNING*** \
-                               \n\nYou have selected the Remove Empty Folder\'s Option. \
+                               \n\nYou have selected the Remove Empty Folders Option. \
                                \nThis process is NOT reversible! \
-                               \n\nPlease confirm this by typing in "Y" \
-                               \nTyping in any other character will cause this program to self destruct... \
+                               \n\nPlease confirm this by typing: "Y" \
+                               \nTyping any other character will abort the program... \
                                \n\nPlease confirm your choice: ')
-        if not confirm_delete in {"Y","y"}:
-            print('Running self destruct program...\n')
-            for n in reversed(range(10)):
-                print(f'Self destruction in: {n}',end="\r")
-                time.sleep(1)
-                raise SystemExit()
-        walk = list(os.walk(self.root))
-        for path, _, _ in walk[::-1]:
-            if len(os.listdir(path)) == 0:
-                self.empty_list.append(path)
-                os.rmdir(path)
-                print(f'Removed Directory: {path}')
-        if self.empty_list: 
-            output_txt = define_output_file(self.output_path,self.root,self.meta_dir_flag,output_suffix="_EmptyDirectoriesRemoved",output_format="txt")
-            export_list_txt(self.empty_list, output_txt)
-        else: print('No directories removed!')
-
-    def filter_directories(self,directory):
-        """Sorts the list Alphabetically and filters out certain files.
-        
-        Currently hardcoded to ignore:
-        1. Hidden Directories starting with '.'
-        2. '.opex' files
-        3. Folders titled 'meta'
-        4. Script file
-        5. Output file
-        
-        Look to make dynamic and customisable...
-        """ 
-        if not self.hidden_flag:
-            list_directories = sorted([f for f in os.listdir(directory) \
-                if not f.startswith('.') \
-                and not bool(os.stat(os.path.join(directory,f)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN) \
-                and not f.endswith('.opex') \
-                and f != 'meta'\
-                and f != os.path.basename(__file__)],key=str.casefold)
-        else: list_directories = sorted([f for f in os.listdir(directory) \
-                if not f.endswith('.opex') \
-                and f != 'meta' \
-                and f != os.path.basename(__file__)],key=str.casefold)
-        return list_directories
-    
-    def parse_directory_dict(self,file_path: str, level: str, ref: int):
-        """
-        Parse's directory / file data into a dict which is then appended to a list
-        """
-        full_path = os.path.abspath(file_path)
-        file_stats = os.stat(file_path)                               
-        if self.accession_flag:                                                   
-            acc_ref = self.accession_running_number(file_path)
-            self.accession_list.append(acc_ref)
-        if os.path.isdir(file_path): file_type = "Dir"
-        else: file_type = "File"
-        class_dict = {'RelativeName': str(file_path).replace(self.root_path,""),
-                        'FullName':str(full_path),
+        if confirm_delete.lower() != "y":
+            print('Aborting...')
+            time.sleep(1)
+            raise SystemExit()
+        empty_dirs = []
+        for dirpath, dirnames, filenames in os.walk(self.root, topdown=False):
+            if not any((dirnames, filenames)):
+                empty_dirs.append(dirpath)
+                try:
+                    os.rmdir(dirpath)
+                    print(f'Removed Directory: {dirpath}')
+                except OSError as e:
+                    print(f"Error removing directory '{dirpath}': {e}")
+        if empty_dirs:
+            output_txt = define_output_file(self.output_path, self.root, self.meta_dir_flag,
+                                            output_suffix="_EmptyDirectoriesRemoved",output_format="txt")
+            export_list_txt(empty_dirs, output_txt)
+        else:
+            print('No directories removed!')
+
+    def filter_directories(self, directory):
+        """
+        Sorts the list alphabetically and filters out certain files.
+        """
+        try:
+            if not self.hidden_flag:
+                list_directories = sorted([f.name for f in os.scandir(directory)
+                                            if not f.name.startswith('.')
+                                            and not bool(os.stat(win_256_check(os.path.join(directory, f.name))).st_file_attributes &
+                                                        stat.FILE_ATTRIBUTE_HIDDEN)
+                                            and not f.name.endswith('.opex')
+                                            and f.name != 'meta'
+                                            and f.name != os.path.basename(__file__)], key=str.casefold)
+            else:
+                list_directories = sorted([f.name for f in os.scandir(directory)
+                                            if not f.name.endswith('.opex')
+                                            and f.name != 'meta'
+                                            and f.name != os.path.basename(__file__)], key=str.casefold)
+            return list_directories
+        except Exception as e:
+            print('Failed to Filter')
+            print(e)
+            raise SystemError()
+
+    def parse_directory_dict(self, file_path: str, level: str, ref: int):
+        """
+        Parses directory / file data into a dict which is then appended to a list
+        """
+        try:
+            if file_path.startswith(u'\\\\?\\'):
+                parse_path = file_path.replace(u'\\\\?\\', "")
+            else: 
+                parse_path = file_path
+            file_stats = os.stat(file_path)
+            if self.accession_flag:
+                acc_ref = self.accession_running_number(parse_path)
+                self.accession_list.append(acc_ref)
+            if os.path.isdir(file_path):
+                file_type = "Dir"
+            else:
+                file_type = "File"
+            class_dict = {'RelativeName': str(parse_path).replace(self.root_path, ""),
+                        'FullName': str(os.path.abspath(parse_path)),
                         'Basename': os.path.splitext(os.path.basename(file_path))[0],
                         'Extension': os.path.splitext(file_path)[1],
-                        'Parent': os.path.abspath(os.path.join(full_path, os.pardir)),
-                        'Attribute':file_type,
-                        'Size':file_stats.st_size,
-                        'CreateDate':datetime.fromtimestamp(file_stats.st_ctime),
+                        'Parent': os.path.abspath(os.path.join(os.path.abspath(parse_path), os.pardir)),
+                        'Attribute': file_type,
+                        'Size': file_stats.st_size,
+                        'CreateDate': datetime.fromtimestamp(file_stats.st_ctime),
                         'ModifiedDate': datetime.fromtimestamp(file_stats.st_mtime),
-                        'AccessDate':datetime.fromtimestamp(file_stats.st_atime),
-                        'Level':level,
-                        'Ref_Section':ref}
-        if self.fixity and not os.path.isdir(file_path):
-            hash = HashGenerator(self.fixity).hash_generator(win_256_check(file_path))
-            class_dict.update({"Algorithm":self.fixity,"Hash":hash})
-        self.record_list.append(class_dict)
-        return class_dict
-        
-    def list_directories(self,directory: str, ref: int = 1):
+                        'AccessDate': datetime.fromtimestamp(file_stats.st_atime),
+                        'Level': level,
+                        'Ref_Section': ref}
+            if self.fixity and not os.path.isdir(file_path):
+                hash = HashGenerator(self.fixity).hash_generator(file_path)
+                class_dict.update({"Algorithm": self.fixity, "Hash": hash})
+            self.record_list.append(class_dict)
+            return class_dict
+        except:
+            print('Failed to Parse')
+            raise SystemError()
+
+
+    def list_directories(self, directory: str, ref: int = 1):
         """
-        Generates a list of directories. Also calculate's level and the reference number utilised in lookups.
+        Generates a list of directories. Also calculates level and a running reference number.
         """
         ref = int(ref)
         try:
             list_directory = self.filter_directories(directory)
-            if directory.startswith(u'\\\\?\\'): level = directory.replace(u'\\\\?\\',"").count(os.sep) - self.root_level + 1
-            else: level = directory.count(os.sep) - self.root_level + 1
+            if directory.startswith(u'\\\\?\\'):
+                level = directory.replace(u'\\\\?\\', "").count(os.sep) - self.root_level + 1
+            else:
+                level = directory.count(os.sep) - self.root_level + 1
             for file in list_directory:
-                file_path = os.path.join(directory,file)
-                file_path_256 = win_256_check(file_path)
-                self.parse_directory_dict(file_path,level,ref)
+                file_path = win_256_check(os.path.join(directory, file))
+                self.parse_directory_dict(file_path, level, ref)
                 ref = int(ref) + int(1)
-                if os.path.isdir(file_path): self.list_directories(file_path_256,ref=1)
+                if os.path.isdir(file_path):
+                    self.list_directories(file_path, ref=1)
         except Exception as e:
             print(e)
-            print("Error occured for directory/file: {}".format(list_directory))
-            raise SystemExit()
+            print("Error occurred for directory/file: {}".format(list_directory))
+            raise SystemError()
             pass
-        
+
     def init_dataframe(self):
         """
-        The directories are listed which are listed and form dicts from above two functions.
-        This looks up and pulls through the Parent row's data to the Child Row.
-        The dataframe is merged on itself, Parent is merged 'left' on FullName to pull through the Parent's data (lookup is based on File Path's), and unnecessary data is dropped.
-        Any errors are turned to 0 and the result are based to the reference loop init. 
-        """
-        self.parse_directory_dict(file_path=self.root,level=0,ref=0)
-        self.list_directories(self.root,self.start_ref)
-        df = pd.DataFrame(self.record_list)                                                                            
-        df = df.merge(df[['FullName','Ref_Section']],how='left',left_on='Parent',right_on='FullName')              
-        df = df.drop(['FullName_y'], axis=1)                                                                            
-        df = df.rename(columns={'Ref_Section_x':'Ref_Section','Ref_Section_y':'Parent_Ref','FullName_x':'FullName'})    # Rename occurs to realign columns
-        df['Parent_Ref'] = df['Parent_Ref'].fillna(0)                                                                   # Any Blank rows in Parent Ref set to 0                                                      
-        df = df.astype({'Parent_Ref': int})                                                                             # Parent Ref is set as Type int
-        df.index.name = "Index"
-        self.list_loop = df[['Ref_Section','Parent','Level']].values.tolist()                                           # Reference Section, Parent and Levels are exported to lists for iterating in ref_loop
-        self.df = df
-        if self.skip_flag: pass
-        else: self.init_reference_loop()
+        Lists the directories and forms dicts from the above two functions.
+        Looks up and pulls through the Parent row's data to the Child Row.
+        Merges the dataframe on itself, Parent is merged 'left' on FullName to pull through the Parent's data
+        (lookup is based on File Path's), and unnecessary data is dropped.
+        Any errors are turned to 0 and the result are based on the reference loop initialisation.
+        """
+        self.parse_directory_dict(file_path=self.root, level=0, ref=0)
+        self.list_directories(self.root, self.start_ref)
+        self.df = pd.DataFrame(self.record_list)
+        self.df = self.df.merge(self.df[['FullName', 'Ref_Section']], how='left', left_on='Parent',
+                                right_on='FullName')
+        self.df = self.df.drop(['FullName_y'], axis=1)
+        self.df = self.df.rename(columns={'Ref_Section_x': 'Ref_Section', 'Ref_Section_y': 'Parent_Ref',
+                                          'FullName_x': 'FullName'})
+        self.df['Parent_Ref'] = self.df['Parent_Ref'].fillna(0)
+        self.df = self.df.astype({'Parent_Ref': int})
+        self.df.index.name = "Index"
+        self.list_loop = self.df[['Ref_Section', 'Parent', 'Level']].values.tolist()
+        if self.skip_flag:
+            pass
+        else:
+            self.init_reference_loop()
         return self.df
-    
+
     def init_reference_loop(self):
         """
-        Inits the Reference loop. Sets some of the pre-variables necessary for the loop.
+        Initialises the Reference loop. Sets some of the pre-variables necessary for the loop.
         """
-        c = 0                       
+        c = 0
         tot = len(self.list_loop)
-        for REF,PARENT,LEVEL in self.list_loop:
+        for REF, PARENT, LEVEL in self.list_loop:
             c += 1
             print(f"Generating Auto Classification for: {c} / {tot}",end="\r")
             TRACK = 1  
             self.reference_loop(REF,PARENT,TRACK,LEVEL)
 
         self.df['Archive_Reference'] = self.reference_list
         if self.accession_flag:
             self.df['Accession_Reference'] = self.accession_list
         return self.df
-    
+
     def reference_loop(self, REF, PARENT, TRACK, LEVEL, NEWREF=None):
         """
-        Note that the Reference loop is acting inside the for loop of the init step.
+        The Reference loop works upwards, running an "index lookup" against the parent folder until it reaches the top.
 
-        REF is the reference section derived from the list in the list_directories function. [Stay's Constant]
-        PARENT is the parent folder of the child. [Vary's]
-        TRACK is an iteration tracker to distinguish between first and later iterations. [Vary's]
-        LEVEL is the level of the folder, 0 being the root. [Stay's Constant]
+        REF is the reference section derived from the list in the list_directories function. [Stays Constant]
+        PARENT is the parent folder of the child. [Varies]
+        TRACK is an iteration tracker to distinguish between first and later iterations. [Varies]
+        LEVEL is the level of the folder, 0 being the root. [Stays Constant]
 
-        NEWREF is the important variable here and is archive reference constructed during this loop.
+        NEWREF is the archive reference constructed during this loop.
 
-        To do this the reference loop works upwards, running an "index lookup" against the parent folder until it reaches the top.
-        
+        To do this, the reference loop works upwards, running an "index lookup" against the parent folder until it reaches the top.
         1) To start, the reference loop indexes from the dataframe established by listing the directories.
         2) The index compares FullName against the Parent (So acting on the Basis of File Path's)
         3) If the index fails / is 0, then the top has been reached.
         4) In that event if LEVEL is also 0 IE the top-most item is being looked at (normally the first thing). NEWREF is set to REF
         5) Otherwise the top-most level has been reached and, NEWREF is simply NEWREF.
         6) If the index does matches, then top level has not yet been reached. In this case we also account for the PARENT's Reference, to avoid an error at the 2nd to top layer.
         7) PARENTREF is looked up, by Indexing the Dataframe. Then if PARENTREF is 0, IE we're on the 2nd top layer. We check the TRACK.
         8) If TRACK is 1, IE the first iteration on the 2nd layer, NEWREF is just REF.
-        9) If TRACK isn't 1, IE subsquent iteration's on the 2nd layer, NEWREF is just itself.
+        9) If TRACK isn't 1, IE subsequent iterations on the 2nd layer, NEWREF is just itself.
         10) If PARENTREF isn't 0, then we concatenate the PARENTREF with either REF or NEWREF.
         11) If TRACK is 1, NEWREF is PARENTREF + REF.
         12) If TRACK isn't 1, NEWREF is PARENTREF + NEWREF.
         13) At the end of the process the PARENT of the current folder is looked up and SUBPARENT replace's the PARENT variable. TRACK is also advanced.
-        14) Then function is then called on recusrively. In this way the loop will work through until it reaches the top. 
-        15) this is only called upon if the index does not fail. If it does fail, then the top-level is reached and the loop escaped.
+        14) Then the function is then called upon recursively. In this way the loop will work through until it reaches the top.
+        15) This is only called upon if the index does not fail. If it does fail, then the top-level is reached and the loop escaped.
         16) As this is acting within the Loop from the init stage, this will operate on all files within a list.
         """
         try:
-            idx = self.df.index[self.df['FullName'] == PARENT]
+            idx = self.df['FullName'][self.df['FullName'] == PARENT].index
             if idx.size == 0:
                 if LEVEL == 0:
                     NEWREF = str(REF)
-                    if self.prefix: NEWREF = str(self.prefix)
+                    if self.prefix:
+                        NEWREF = str(self.prefix)
                 else:
                     NEWREF = str(NEWREF)
-                    if self.prefix: NEWREF = str(self.prefix) + "/" + str(NEWREF)
+                    if self.prefix:
+                        NEWREF = str(self.prefix) + "/" + str(NEWREF)
                 self.reference_list.append(NEWREF)
             else:
-                PARENTREF = self.df.loc[idx].Ref_Section.item() 
+                PARENTREF = self.df['Ref_Section'].loc[idx].item()
                 if PARENTREF == 0:
-                    if TRACK == 1: NEWREF = str(REF)            
-                    else: NEWREF = str(NEWREF)                       
+                    if TRACK == 1:
+                        NEWREF = str(REF)
+                    else:
+                        NEWREF = str(NEWREF)
                 else:
-                    if TRACK == 1: NEWREF = str(PARENTREF) + "/" + str(REF)         
-                    else: NEWREF = str(PARENTREF) + "/" + str(NEWREF)              
-                    
-                SUBPARENT = self.df.loc[idx].Parent.item() 
+                    if TRACK == 1:
+                        NEWREF = str(PARENTREF) + "/" + str(REF)
+                    else:
+                        NEWREF = str(PARENTREF) + "/" + str(NEWREF)
+
+                SUBPARENT = self.df['Parent'].loc[idx].item()
                 PARENT = SUBPARENT
-                TRACK = TRACK+1
+                TRACK = TRACK + 1
                 self.reference_loop(REF, PARENT, TRACK, LEVEL, NEWREF)
 
         except Exception as e:
             print('Passed?')
             print(e)
-            pass 
+            pass
 
     def accession_running_number(self,file_path):
         """
         Generates a Running Number / Accession Code, can be set to 3 different "modes", counting Files, Directories or Both
         """
 
         if self.accession_flag == "File":
-            if os.path.isdir(file_path): accession_ref = self.accession_prefix + "-Dir"
-            else: accession_ref = accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
+            if os.path.isdir(file_path):
+                accession_ref = self.accession_prefix + "-Dir"
+            else:
+                accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                self.accession_count += 1
         elif self.accession_flag == "Dir":
-            if os.path.isdir(file_path): accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
-            else: accession_ref = accession_ref = self.accession_prefix + "-File"
+            if os.path.isdir(file_path):
+                accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                self.accession_count += 1
+            else:
+                accession_ref = self.accession_prefix + "-File"
         elif self.accession_flag == "All":
-            accession_ref = self.accession_prefix + "-" + str(self.accession_count); self.accession_count += 1
+            accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+            self.accession_count += 1
         return accession_ref
-            
+
     def main(self):
         """
         Runs Program :)
         """
         if self.empty_flag: self.remove_empty_directories()
         self.init_dataframe()
-        output_file = define_output_file(self.output_path,self.root,meta_dir_flag=self.meta_dir_flag,output_format=self.output_format)
-        if self.output_format == "xlsx": export_xl(df=self.df,output_filename=output_file)
-        elif self.output_format == "csv": export_csv(df=self.df,output_filename=output_file)
+        output_file = define_output_file(self.output_path, self.root, meta_dir_flag=self.meta_dir_flag,
+                                         output_format=self.output_format)
+        if self.output_format == "xlsx":
+            export_xl(df=self.df, output_filename=output_file)
+        elif self.output_format == "csv":
+            export_csv(df=self.df, output_filename=output_file)
+        self.print_running_time()
```

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator/cli.py` & `auto_classification_generator-1.1.3/auto_classification_generator/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from auto_classification_generator.classification_generator import ClassificationGenerator
-from auto_classification_generator.version import __version__
 import argparse
 import os
+import importlib.metadata
 
 def parse_args():
     parser = argparse.ArgumentParser(description="OPEX Manifest Generator for Preservica Uploads")
     parser.add_argument('root',nargs='?', default=os.getcwd())
     parser.add_argument("-p","--prefix",required=False, nargs='?')
     parser.add_argument("-accp", "--acc-prefix",required=False, nargs='?')
     parser.add_argument("-rm","--empty",required=False,action='store_true')
@@ -13,24 +13,24 @@
     parser.add_argument("-o","--output",required=False,nargs='?')
     parser.add_argument("-s","--start-ref",required=False,nargs='?',default=1)
     parser.add_argument("--meta-dir",required=False,action='store_true',default=True)
     parser.add_argument("--skip",required=False,action='store_true',default=False)
     parser.add_argument("--hidden",required=False,action='store_true',default=False)
     parser.add_argument("-fmt","--output-format",required=False,default="xlsx",choices=['xlsx','csv'])
     parser.add_argument("-fx","--fixity",required=False,nargs='?', const="SHA-1",default=None,choices=['NONE','MD5','SHA-1','SHA-256','SHA-512'],type=str.upper)
-    parser.add_argument("-v", "--version", action='version',version='%(prog)s {version}'.format(version=__version__))
+    parser.add_argument("-v", "--version", action='version',version='%(prog)s {version}'.format(version=importlib.metadata.version("auto_classification_generator")))
     args = parser.parse_args()
     return args
 
 def run_cli():
     args = parse_args()
     if isinstance(args.root,str): args.root = args.root.strip("\"").rstrip("\\")
     if not args.output:
         args.output = os.path.abspath(args.root)
-        print(f'No output path selected, defaulting to root Directory: {args.output}')
+        print(f'Output path defaulting to root directory: {args.output}')
     else:
         args.output = os.path.abspath(args.output)
         print(f'Output path set to: {args.output}')
     
     ClassificationGenerator(args.root,
                             output_path = args.output,
                             prefix=args.prefix,
```

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator/common.py` & `auto_classification_generator-1.1.3/auto_classification_generator/common.py`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator/hash.py` & `auto_classification_generator-1.1.3/auto_classification_generator/hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,9 +21,8 @@
         else: hash = hashlib.sha1()
         print(f'Generating Fixity using {self.algorithm} for: {file_path}')#,end="\r") 
         with open(file_path,"rb") as f:
             buff = f.read(self.buffer)
             while buff:
                 hash.update(buff)
                 buff = f.read(self.buffer)
-        print(hash.hexdigest())
         return hash.hexdigest().upper()
```

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator.egg-info/PKG-INFO` & `auto_classification_generator-1.1.3/auto_classification_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.2
+Version: 1.1.3
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.2/auto_classification_generator.egg-info/SOURCES.txt` & `auto_classification_generator-1.1.3/auto_classification_generator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 pyproject.toml
 auto_classification_generator/__init__.py
 auto_classification_generator/classification_generator.py
 auto_classification_generator/cli.py
 auto_classification_generator/common.py
 auto_classification_generator/hash.py
 auto_classification_generator/test_cli.py
-auto_classification_generator/version.py
 auto_classification_generator.egg-info/PKG-INFO
 auto_classification_generator.egg-info/SOURCES.txt
 auto_classification_generator.egg-info/dependency_links.txt
 auto_classification_generator.egg-info/entry_points.txt
 auto_classification_generator.egg-info/requires.txt
 auto_classification_generator.egg-info/top_level.txt
```

### Comparing `auto_classification_generator-1.1.2/pyproject.toml` & `auto_classification_generator-1.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2261 7574 6f5f 636c  .name = "auto_cl
 00000070: 6173 7369 6669 6361 7469 6f6e 5f67 656e  assification_gen
 00000080: 6572 6174 6f72 220d 0a76 6572 7369 6f6e  erator"..version
-00000090: 203d 2022 312e 312e 3222 0d0a 6175 7468   = "1.1.2"..auth
+00000090: 203d 2022 312e 312e 3322 0d0a 6175 7468   = "1.1.3"..auth
 000000a0: 6f72 7320 3d20 5b0d 0a20 2020 207b 6e61  ors = [..    {na
 000000b0: 6d65 3d22 4368 7269 7374 6f70 6865 7220  me="Christopher 
 000000c0: 5072 696e 6365 222c 2065 6d61 696c 3d22  Prince", email="
 000000d0: 632e 706a 2e70 7269 6e63 6540 676d 6169  c.pj.prince@gmai
 000000e0: 6c2e 636f 6d22 7d0d 0a20 2020 205d 0d0a  l.com"}..    ]..
 000000f0: 6465 7363 7269 7074 696f 6e20 3d20 2241  description = "A
 00000100: 7574 6f20 436c 6173 7369 6669 6361 7469  uto Classificati
@@ -43,8 +43,15 @@
 000002a0: 494e 4345 2f61 7574 6f5f 636c 6173 7369  INCE/auto_classi
 000002b0: 6669 6361 7469 6f6e 5f67 656e 6572 6174  fication_generat
 000002c0: 6f72 2f69 7373 7565 7322 0d0a 5b70 726f  or/issues"..[pro
 000002d0: 6a65 6374 2e73 6372 6970 7473 5d0d 0a61  ject.scripts]..a
 000002e0: 7574 6f5f 636c 6173 7320 3d20 2261 7574  uto_class = "aut
 000002f0: 6f5f 636c 6173 7369 6669 6361 7469 6f6e  o_classification
 00000300: 5f67 656e 6572 6174 6f72 2e63 6c69 3a72  _generator.cli:r
-00000310: 756e 5f63 6c69 22                        un_cli"
+00000310: 756e 5f63 6c69 220d 0a0d 0a5b 746f 6f6c  un_cli"....[tool
+00000320: 2e73 6574 7570 746f 6f6c 732e 7061 636b  .setuptools.pack
+00000330: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000340: 6520 3d20 5b27 2e27 5d0d 0a69 6e63 6c75  e = ['.']..inclu
+00000350: 6465 203d 205b 2761 7574 6f5f 636c 6173  de = ['auto_clas
+00000360: 7369 6669 6361 7469 6f6e 5f67 656e 6572  sification_gener
+00000370: 6174 6f72 275d 0d0a 6578 636c 7564 6520  ator']..exclude 
+00000380: 3d20 5b5d                                = []
```

