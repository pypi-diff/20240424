# Comparing `tmp/furthrmind-0.1b8.tar.gz` & `tmp/furthrmind-0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furthrmind-0.1b8.tar", max compression
+gzip compressed data, was "furthrmind-0.1b9.tar", max compression
```

## Comparing `furthrmind-0.1b8.tar` & `furthrmind-0.1b9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b8/LICENSE
--rwxr-xr-x   0        0        0     3326 2024-04-16 07:37:32.310043 furthrmind-0.1b8/README.md
--rwxr-xr-x   0        0        0     2351 2024-04-17 09:15:00.906435 furthrmind-0.1b8/furthrmind/__init__.py
--rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b8/furthrmind/collection/__init__.py
--rwxr-xr-x   0        0        0    20492 2024-04-22 15:48:32.328925 furthrmind-0.1b8/furthrmind/collection/baseclass.py
--rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b8/furthrmind/collection/category.py
--rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b8/furthrmind/collection/column.py
--rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b8/furthrmind/collection/comboboxentry.py
--rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b8/furthrmind/collection/datatable.py
--rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b8/furthrmind/collection/experiment.py
--rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b8/furthrmind/collection/field.py
--rwxr-xr-x   0        0        0    10608 2024-04-17 09:15:00.899484 furthrmind-0.1b8/furthrmind/collection/fielddata.py
--rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b8/furthrmind/collection/file.py
--rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b8/furthrmind/collection/group.py
--rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b8/furthrmind/collection/import_collection.py
--rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b8/furthrmind/collection/project.py
--rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b8/furthrmind/collection/researchitem.py
--rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b8/furthrmind/collection/sample.py
--rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b8/furthrmind/collection/unit.py
--rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b8/furthrmind/file_loader.py
--rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b8/furthrmind/utils.py
--rwxr-xr-x   0        0        0      723 2024-04-22 15:49:14.499344 furthrmind-0.1b8/pyproject.toml
--rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 furthrmind-0.1b8/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b9/LICENSE
+-rwxr-xr-x   0        0        0     3326 2024-04-16 07:37:32.310043 furthrmind-0.1b9/README.md
+-rwxr-xr-x   0        0        0     2351 2024-04-17 09:15:00.906435 furthrmind-0.1b9/furthrmind/__init__.py
+-rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b9/furthrmind/collection/__init__.py
+-rwxr-xr-x   0        0        0    28494 2024-04-23 08:49:15.009846 furthrmind-0.1b9/furthrmind/collection/baseclass.py
+-rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b9/furthrmind/collection/category.py
+-rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b9/furthrmind/collection/column.py
+-rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b9/furthrmind/collection/comboboxentry.py
+-rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b9/furthrmind/collection/datatable.py
+-rwxr-xr-x   0        0        0     6370 2024-04-23 07:29:50.464069 furthrmind-0.1b9/furthrmind/collection/experiment.py
+-rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b9/furthrmind/collection/field.py
+-rwxr-xr-x   0        0        0    10608 2024-04-17 09:15:00.899484 furthrmind-0.1b9/furthrmind/collection/fielddata.py
+-rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b9/furthrmind/collection/file.py
+-rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b9/furthrmind/collection/group.py
+-rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b9/furthrmind/collection/import_collection.py
+-rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b9/furthrmind/collection/project.py
+-rwxr-xr-x   0        0        0     9459 2024-04-23 09:15:12.481013 furthrmind-0.1b9/furthrmind/collection/researchitem.py
+-rwxr-xr-x   0        0        0     6315 2024-04-23 07:29:50.453039 furthrmind-0.1b9/furthrmind/collection/sample.py
+-rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b9/furthrmind/collection/unit.py
+-rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b9/furthrmind/file_loader.py
+-rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b9/furthrmind/utils.py
+-rwxr-xr-x   0        0        0      723 2024-04-23 10:06:03.012252 furthrmind-0.1b9/pyproject.toml
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 furthrmind-0.1b9/PKG-INFO
```

### Comparing `furthrmind-0.1b8/LICENSE` & `furthrmind-0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/README.md` & `furthrmind-0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/__init__.py` & `furthrmind-0.1b9/furthrmind/__init__.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/baseclass.py` & `furthrmind-0.1b9/furthrmind/collection/baseclass.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from furthrmind.utils import furthr_wrap, instance_overload
 from typing_extensions import List, Self, Any, Dict, TYPE_CHECKING
 from inspect import isclass
 import os
 
 if TYPE_CHECKING:
-    from furthrmind.collection import File, FieldData, Experiment
+    from furthrmind.collection import File, FieldData, Experiment, Sample, ResearchItem
 
 class BaseClass:
     _data = {}
     _fetched = False
     _id = None
     fm = None
 
@@ -533,8 +533,229 @@
                     break
 
             if not group_id:
                 raise ValueError("No group with Name was found")
 
         data = {"name": name, "groups": [{"id": group_id}]}
 
-        return data
+        return data
+
+class BaseClassWithLinking(BaseClass):
+    id: str = ""
+    linked_samples: List["Sample"] = []
+    linked_experiments: List["Experiment"] = []
+    linked_researchitems: Dict[str, List["ResearchItem"]] = []
+
+    def __init__(self, id=None, data=None):
+        super().__init__(id, data)
+
+    def add_linked_experiment(self, experiment_id=None, experiment_name=None):
+        """
+        This method is to link an experiment to the current item
+        Args:
+            experiment_id: id to the experiment you want to link, either id or name must be given
+            experiment_name: name of the experiment you want to link, either name or name must be given
+
+        Returns:
+            the id of the item
+        """
+        from furthrmind.collection import Experiment
+        assert experiment_id or experiment_name, "Either experiment_id or experiment_name must be specified"
+
+        if experiment_name:
+            exp = Experiment.get(name = experiment_name)
+            if not exp:
+                raise ValueError("No exp found with the given name")
+            experiment_id = exp.id
+        else:
+            exp = Experiment.get(experiment_id)
+
+        experiment_id_list = [item.id for item in self.linked_experiments]
+        if experiment_id not in experiment_id_list:
+            experiment_id_list.append(experiment_id)
+
+        linked_experiment = [{"id": exp_id} for exp_id in experiment_id_list]
+        data = {
+            "id": self.id,
+                "experiments": linked_experiment
+        }
+
+        self.post(data=data)
+        self.linked_experiments.append(exp)
+        return self.id
+
+    def remove_linked_experiment(self, experiment_id=None, experiment_name=None):
+        """
+        This method is to remove link a linked experiment from the current item
+        Args:
+            experiment_id: id to the experiment you want to remove the linkage, either id or name must be given
+            experiment_name: name of the experiment you want to remove the linkage, either name or name must be given
+
+        Returns:
+            the id of the item
+        """
+        from furthrmind.collection import Experiment
+        assert experiment_id or experiment_name, "Either experiment_id or experiment_name must be specified"
+
+        if experiment_name:
+            exp = Experiment.get(name = experiment_name)
+            if not exp:
+                raise ValueError("No exp found with the given name")
+            experiment_id = exp.id
+
+        experiment_id_list = []
+        new_linked_items = []
+        for item in self.linked_experiments:
+            if item.id == experiment_id:
+                continue
+            new_linked_items.append(item)
+            experiment_id_list.append(item.id)
+
+        linked_experiment = [{"id": exp_id} for exp_id in experiment_id_list]
+        data = {
+            "id": self.id,
+                "experiments": linked_experiment
+        }
+
+        self.post(data=data)
+        self.linked_experiments = new_linked_items
+        return self.id
+
+    def add_linked_sample(self, sample_id=None, sample_name=None):
+        """
+        This method is to link a sample to the current item
+        Args:
+            sample_id: id to the sample you want to link, either id or name must be given
+            sample_name: name of the sample you want to link, either name or name must be given
+
+        Returns:
+            the id of the item
+        """
+        from furthrmind.collection import Sample
+        assert sample_id or sample_name, "Either sample_id or sample_name must be specified"
+
+        if sample_name:
+            s = Sample.get(name=sample_name)
+            if not s:
+                raise ValueError("No sample found with the given name")
+            sample_id = s.id
+        else:
+            s = Sample.get(sample_id)
+
+        sample_id_list = [item.id for item in self.linked_samples]
+        if sample_id not in sample_id_list:
+            sample_id_list.append(sample_id)
+
+        linked_samples = [{"id": s_id} for s_id in sample_id_list]
+
+        data = {
+            "id": self.id,
+            "samples": linked_samples
+        }
+
+        self.post(data=data)
+        self.linked_samples.append(s)
+        return self.id
+
+    def remove_linked_sample(self, sample_id=None, sample_name=None):
+        """
+        This method is to remove a linked sample from the current item
+        Args:
+            sample_id: id of the sample you want to remove the linkage, either id or name must be given
+            sample_name: name of the sample you want to remove linkage, either name or name must be given
+
+        Returns:
+            the id of the item
+        """
+        from furthrmind.collection import Sample
+        assert sample_id or sample_name, "Either sample_id or sample_name must be specified"
+
+        if sample_name:
+            s = Sample.get(name=sample_name)
+            if not s:
+                raise ValueError("No sample found with the given name")
+            sample_id = s.id
+
+        sample_id_list = []
+        new_linked_items = []
+        for item in self.linked_samples:
+            if item.id == sample_id:
+                continue
+            new_linked_items.append(item)
+            sample_id_list.append(item.id)
+
+        linked_samples = [{"id": s_id} for s_id in sample_id_list]
+
+        data = {
+            "id": self.id,
+            "samples": linked_samples
+        }
+        self.post(data=data)
+        self.linked_samples = new_linked_items
+        return self.id
+
+    def add_linked_researchitem(self, researchitem_id=None):
+        """
+        This method is to link an experiment to the current item
+        Args:
+            researchitem_id: id to the researchitem you want to link
+
+        Returns:
+            the id of the item
+        """
+        assert researchitem_id, "Either experiment_id or experiment_name must be specified"
+
+        researchitem_id_list = []
+        for cat in self.linked_researchitems:
+            researchitem_id_list.extend([ri_id for ri_id in self.linked_researchitems[cat]])
+
+        if researchitem_id not in researchitem_id_list:
+            researchitem_id_list.append(researchitem_id)
+
+        linked_researchitems = [{"id": ri_id} for ri_id in researchitem_id_list]
+
+
+        data = {
+            "id": self.id,
+            "researchitems": linked_researchitems
+        }
+
+        self.post(data=data)
+        ri = ResearchItem.get(id=researchitem_id)
+        self.linked_researchitems[ri.category.name].append(ri)
+        return self.id
+
+    def remove_linked_researchitem(self, researchitem_id=None):
+        """
+        This method is to link an experiment to the current item
+        Args:
+            researchitem_id: id to the researchitem you want to remove the linkage
+
+        Returns:
+            the id of the item
+        """
+        assert researchitem_id, "Either experiment_id or experiment_name must be specified"
+
+        researchitem_id_list = []
+        new_linked_items = {}
+        for cat in self.linked_researchitems:
+            for item in self.linked_researchitems[cat]:
+                if item.id == researchitem_id:
+                    continue
+                if cat not in new_linked_items:
+                    new_linked_items[cat] = []
+                new_linked_items[cat].append(item)
+                researchitem_id_list.append(item.id)
+
+        if researchitem_id in researchitem_id_list:
+            researchitem_id_list.remove(researchitem_id)
+
+        linked_researchitems = [{"id": ri_id} for ri_id in researchitem_id_list]
+
+        data = {
+            "id": self.id,
+            "researchitems": linked_researchitems
+        }
+
+        self.post(data=data)
+        self.linked_researchitems = new_linked_items
+        return self.id
```

### Comparing `furthrmind-0.1b8/furthrmind/collection/category.py` & `furthrmind-0.1b9/furthrmind/collection/category.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/column.py` & `furthrmind-0.1b9/furthrmind/collection/column.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/comboboxentry.py` & `furthrmind-0.1b9/furthrmind/collection/comboboxentry.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/datatable.py` & `furthrmind-0.1b9/furthrmind/collection/datatable.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/experiment.py` & `furthrmind-0.1b9/furthrmind/collection/experiment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-from furthrmind.collection.baseclass import BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup, BaseClass
-from typing_extensions import Self, List, Dict, TYPE_CHECKING
 from inspect import isclass
+
+from typing_extensions import Self, List, Dict, TYPE_CHECKING
+
+from furthrmind.collection.baseclass import (BaseClassWithFieldData,
+                                             BaseClassWithFiles,
+                                             BaseClassWithGroup,
+                                             BaseClassWithLinking,
+                                             BaseClass
+                                             )
+
 if TYPE_CHECKING:
     from furthrmind.collection import FieldData, Sample, Group, ResearchItem, DataTable, File
 
-class Experiment(BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup):
+
+class Experiment(BaseClassWithFieldData, BaseClassWithFiles,
+                 BaseClassWithGroup, BaseClassWithLinking):
     id = ""
     name = ""
     neglect = False
     shortid = ""
     files: List["File"] = []
     fielddata: List["FieldData"] = []
     linked_samples: List["Sample"] = []
     linked_experiments: List[Self] = []
     groups: List["Group"] = []
     linked_researchitems: Dict[str, List["ResearchItem"]] = []
     datatables: List["DataTable"] = []
 
-
     _attr_definition = {
         "files": {"class": "File"},
         "fielddata": {"class": "FieldData"},
         "linked_samples": {"class": "Sample"},
         "linked_experiments": {"class": "Experiment"},
         "groups": {"class": "Group"},
         "linked_researchitems": {"class": "ResearchItem", "nested_dict": True},
@@ -39,15 +48,15 @@
     @classmethod
     def _get_url_class(cls, id, project_id=None):
         project_url = cls.fm.get_project_url(project_id)
         url = f"{project_url}/experiments/{id}"
         return url
 
     @classmethod
-    def _get_all_url(cls, project_id:str = None) -> str:
+    def _get_all_url(cls, project_id: str = None) -> str:
         project_url = cls.fm.get_project_url(project_id)
         url = f"{project_url}/experiments"
         return url
 
     @classmethod
     def _post_url(cls, project_id=None):
         project_url = cls.fm.get_project_url(project_id)
@@ -59,37 +68,37 @@
         """
         Method to get all one experiment by it's id or short_id
         If called on an instance of the class, the id of the class is used
         :param str id: id or short_id of requested experiment 
         :param str name: name of requested experiment 
         :return Self: Instance of experiment class
         """
-        
+
         if isclass(cls):
             if id is None:
                 id = name
             assert id is not None or name is not None, "Either id or name must be specified"
             return cls._get_class_method(id)
         else:
             self = cls
             data = self._get_instance_method()
             return data
-    
+
     @classmethod
     def get_all(cls, project_id=None) -> List[Self]:
         """
         Method to get all experiment belonging to one project
         :param str project_id: Optionally to get experiments from another project as the furthrmind sdk was initiated with, defaults to None
         :return List[Self]: List with instances of experiment class
         """
         return super().get_all(project_id)
 
     @classmethod
     @BaseClass._create_instances_decorator
-    def create(cls, name, group_name = None, group_id=None, project_id=None) -> Self:
+    def create(cls, name, group_name=None, group_id=None, project_id=None) -> Self:
         """
         Method to create a new experiment
 
         :param name: the name of the item to be created
         :param group_name: The name of the group where the new item will belong to. group name can be only considered
             for groups that are not subgroups. Either group_name or group_id must be specified
         :param group_id: the id of the group where the new item will belong to. Either group_name or group_id must be specified
@@ -115,15 +124,15 @@
         :param project_id: Optionally to create an item in another project as the furthrmind sdk was initiated with
         :return list with instance of the experiment class
 
         """
 
         return Experiment._create_many(data_list, project_id)
 
-    def add_datatable(self, name: str, columns: List[Dict], project_id=None ) -> "DataTable":
+    def add_datatable(self, name: str, columns: List[Dict], project_id=None) -> "DataTable":
         """
         Method to create a new datatable within this experiment
 
         :param name: name of the datatable
         :param columns: a list of columns that should be added to the datatable. List with dicts with the following keys:
             - name: name of the column
             - type: Type of the column, Either "Text" or "Numeric". Data must fit to type, for Text all data
@@ -135,8 +144,7 @@
         :return: instance of column datatable class
 
         """
 
         from furthrmind.collection import DataTable
         datatable = DataTable.create(name, experiment_id=self.id, columns=columns, project_id=project_id)
         return datatable
-
```

### Comparing `furthrmind-0.1b8/furthrmind/collection/field.py` & `furthrmind-0.1b9/furthrmind/collection/field.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/fielddata.py` & `furthrmind-0.1b9/furthrmind/collection/fielddata.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/file.py` & `furthrmind-0.1b9/furthrmind/collection/file.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/group.py` & `furthrmind-0.1b9/furthrmind/collection/group.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/project.py` & `furthrmind-0.1b9/furthrmind/collection/project.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/collection/researchitem.py` & `furthrmind-0.1b9/furthrmind/collection/researchitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from ..utils import furthr_wrap
-from furthrmind.collection.baseclass import BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup, BaseClass
+from furthrmind.collection.baseclass import (BaseClassWithFieldData, BaseClassWithFiles,
+                                             BaseClassWithGroup, BaseClass,
+                                             BaseClassWithLinking)
 from typing_extensions import List, Dict, Self, TYPE_CHECKING
 from inspect import isclass
 
 if TYPE_CHECKING:
     from furthrmind.collection import *
 
-class ResearchItem(BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup, BaseClass):
+class ResearchItem(BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup, BaseClassWithLinking, BaseClass ):
     id = ""
     name = ""
     neglect = False
     shortid = ""
     files: List["File"] = []
     fielddata: List["FieldData"] = []
     linked_experiments: List["Experiment"] = []
@@ -79,20 +81,18 @@
         Method to get all researchitems belonging to one project
         :param str project_id: Optionally to get researchitems from another project as the furthrmind sdk was initiated with, defaults to None
         :return List[Self]: List with instances of researchitem class
         """
         return super().get_all(project_id)
 
     @classmethod
-    def get_by_name(cls, name, category_name, project_id=None):
+    def get_by_name(cls, name, category_name, project_id=None) -> Self:
         return cls._get_by_name_class_method(name, category_name, project_id)
 
     @classmethod
-    @BaseClass._create_instances_decorator
-    @furthr_wrap(force_list=False)
     def _get_by_name_class_method(cls, name, category_name, project_id):
         all_data = cls.get_all(project_id)
         for d in all_data:
             if d.category.name.lower() == category_name.lower():
                 if d.name.lower() == name.lower():
                     return d
```

### Comparing `furthrmind-0.1b8/furthrmind/collection/sample.py` & `furthrmind-0.1b9/furthrmind/collection/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from furthrmind.collection.baseclass import BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup, BaseClass
+from furthrmind.collection.baseclass import (BaseClassWithFieldData, BaseClassWithFiles,
+                                             BaseClassWithGroup, BaseClass,
+                                             BaseClassWithLinking)
 from typing_extensions import Self, Dict, List, TYPE_CHECKING
 from furthrmind.utils import instance_overload
 from inspect import isclass
 if TYPE_CHECKING:
     from furthrmind.collection import *
 
 
-class Sample(BaseClassWithFieldData, BaseClassWithFiles, BaseClassWithGroup):
+class Sample(BaseClassWithFieldData,
+             BaseClassWithFiles, BaseClassWithGroup,
+             BaseClassWithLinking, BaseClass):
     id = ""
     name = ""
     neglect = False
     shortid = ""
     files: List["File"] = []
     fielddata: List["FieldData"] = []
     linked_experiments: List["Experiment"] = []
```

### Comparing `furthrmind-0.1b8/furthrmind/collection/unit.py` & `furthrmind-0.1b9/furthrmind/collection/unit.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/file_loader.py` & `furthrmind-0.1b9/furthrmind/file_loader.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/furthrmind/utils.py` & `furthrmind-0.1b9/furthrmind/utils.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b8/pyproject.toml` & `furthrmind-0.1b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furthrmind"
-version = "0.1b8"
+version = "0.1b9"
 description = "Official python wrapper for the FURTHRmind rest api."
 authors = ["Daniel Menne"]
 license = "GNU GENERAL PUBLIC LICENSE Version 3"
 readme = "README.md"
 repository = "https://github.com/FURTHRresearch/furthrmind-sdk"
 
 [tool.poetry.dependencies]
```

### Comparing `furthrmind-0.1b8/PKG-INFO` & `furthrmind-0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furthrmind
-Version: 0.1b8
+Version: 0.1b9
 Summary: Official python wrapper for the FURTHRmind rest api.
 Home-page: https://github.com/FURTHRresearch/furthrmind-sdk
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Author: Daniel Menne
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

