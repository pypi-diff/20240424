# Comparing `tmp/eflips_model-3.2.0.tar.gz` & `tmp/eflips_model-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_model-3.2.0.tar", max compression
+gzip compressed data, was "eflips_model-3.3.0.tar", max compression
```

## Comparing `eflips_model-3.2.0.tar` & `eflips_model-3.3.0.tar`

### file list

```diff
@@ -1,21 +1,40 @@
--rw-r--r--   0        0        0    34260 2024-01-25 14:04:47.012623 eflips_model-3.2.0/LICENSE.md
--rw-r--r--   0        0        0     6274 2024-02-13 18:22:20.940626 eflips_model-3.2.0/README.md
--rw-r--r--   0        0        0     2522 2024-02-13 18:22:20.941222 eflips_model-3.2.0/eflips/model/__init__.py
--rw-r--r--   0        0        0     3556 2024-02-13 18:22:20.941461 eflips_model-3.2.0/eflips/model/alembic.ini
--rw-r--r--   0        0        0    11793 2024-04-17 07:02:23.238136 eflips_model-3.2.0/eflips/model/depot.py
--rw-r--r--   0        0        0    34829 2024-04-17 07:02:23.259349 eflips_model-3.2.0/eflips/model/general.py
--rw-r--r--   0        0        0     2772 2024-03-15 12:08:31.037325 eflips_model-3.2.0/eflips/model/migrations/env.py
--rw-r--r--   0        0        0      635 2024-02-13 18:22:20.942988 eflips_model-3.2.0/eflips/model/migrations/script.py.mako
--rw-r--r--   0        0        0      969 2024-03-25 15:41:52.646712 eflips_model-3.2.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py
--rw-r--r--   0        0        0      938 2024-02-13 18:22:20.943365 eflips_model-3.2.0/eflips/model/migrations/versions/126892076499_v2_0_0.py
--rw-r--r--   0        0        0     1187 2024-03-18 18:50:34.912225 eflips_model-3.2.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py
--rw-r--r--   0        0        0     1316 2024-02-14 17:51:30.276962 eflips_model-3.2.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py
--rw-r--r--   0        0        0      665 2024-02-13 18:22:20.943781 eflips_model-3.2.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py
--rw-r--r--   0        0        0     1497 2024-02-13 18:22:20.944022 eflips_model-3.2.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py
--rw-r--r--   0        0        0     1048 2024-03-18 18:50:34.912522 eflips_model-3.2.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py
--rw-r--r--   0        0        0      798 2024-02-27 15:24:32.595397 eflips_model-3.2.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py
--rw-r--r--   0        0        0    15938 2024-03-18 18:50:34.913013 eflips_model-3.2.0/eflips/model/network.py
--rw-r--r--   0        0        0        0 2024-01-25 14:06:07.781569 eflips_model-3.2.0/eflips/model/py.typed
--rw-r--r--   0        0        0    14194 2024-03-18 18:50:34.913435 eflips_model-3.2.0/eflips/model/schedule.py
--rw-r--r--   0        0        0      920 2024-04-17 07:02:50.829619 eflips_model-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     7245 1970-01-01 00:00:00.000000 eflips_model-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-01-25 14:04:47.012623 eflips_model-3.3.0/LICENSE.md
+-rw-r--r--   0        0        0     6274 2024-02-13 18:22:20.940626 eflips_model-3.3.0/README.md
+-rw-r--r--   0        0        0     6148 2024-04-24 14:53:08.400858 eflips_model-3.3.0/eflips/model/.DS_Store
+-rw-r--r--   0        0        0     2625 2024-04-24 14:44:48.525377 eflips_model-3.3.0/eflips/model/__init__.py
+-rw-r--r--   0        0        0     3556 2024-02-13 18:22:20.941461 eflips_model-3.3.0/eflips/model/alembic.ini
+-rw-r--r--   0        0        0    12308 2024-04-24 15:13:59.248339 eflips_model-3.3.0/eflips/model/depot.py
+-rw-r--r--   0        0        0    35392 2024-04-24 15:13:59.375400 eflips_model-3.3.0/eflips/model/general.py
+-rw-r--r--   0        0        0     3386 2024-03-15 12:08:48.064334 eflips_model-3.3.0/eflips/model/migrations/__pycache__/env.cpython-312.pyc
+-rw-r--r--   0        0        0     2772 2024-03-15 12:08:31.037325 eflips_model-3.3.0/eflips/model/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-02-13 18:22:20.942988 eflips_model-3.3.0/eflips/model/migrations/script.py.mako
+-rw-r--r--   0        0        0      969 2024-03-25 15:41:52.646712 eflips_model-3.3.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py
+-rw-r--r--   0        0        0      938 2024-02-13 18:22:20.943365 eflips_model-3.3.0/eflips/model/migrations/versions/126892076499_v2_0_0.py
+-rw-r--r--   0        0        0     1187 2024-03-18 18:50:34.912225 eflips_model-3.3.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py
+-rw-r--r--   0        0        0     1316 2024-02-14 17:51:30.276962 eflips_model-3.3.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py
+-rw-r--r--   0        0        0      665 2024-02-13 18:22:20.943781 eflips_model-3.3.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py
+-rw-r--r--   0        0        0     1570 2024-03-19 12:21:35.362459 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/0548463664b4_3_0_1.cpython-312.pyc
+-rw-r--r--   0        0        0     1570 2024-04-24 14:27:14.874317 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/0548463664b4_3_1_0.cpython-312.pyc
+-rw-r--r--   0        0        0     1654 2024-02-14 17:16:24.703966 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/126892076499_v2_0_0.cpython-312.pyc
+-rw-r--r--   0        0        0     1735 2024-03-19 09:52:18.829425 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/1e9e14c3cd74_3_0_1.cpython-312.pyc
+-rw-r--r--   0        0        0     1757 2024-03-19 09:52:18.544803 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/6ac022147397_3_0_0.cpython-312.pyc
+-rw-r--r--   0        0        0     2128 2024-02-14 17:53:32.629291 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/7483339ae654_v2_2_0.cpython-312.pyc
+-rw-r--r--   0        0        0      945 2024-02-14 17:16:24.704753 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/9e29124f8ce6_v1_1_6.cpython-312.pyc
+-rw-r--r--   0        0        0     1893 2024-02-14 17:16:24.705520 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/a06c97c98d2c_v2_1_0.cpython-312.pyc
+-rw-r--r--   0        0        0     1430 2024-03-19 09:52:18.546779 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/a9f1c33488b6_3_0_0.cpython-312.pyc
+-rw-r--r--   0        0        0     1280 2024-03-05 11:15:25.192568 eflips_model-3.3.0/eflips/model/migrations/versions/__pycache__/baef3598b52c_v2_3_0.cpython-312.pyc
+-rw-r--r--   0        0        0     1497 2024-02-13 18:22:20.944022 eflips_model-3.3.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py
+-rw-r--r--   0        0        0     1048 2024-03-18 18:50:34.912522 eflips_model-3.3.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py
+-rw-r--r--   0        0        0      798 2024-02-27 15:24:32.595397 eflips_model-3.3.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py
+-rw-r--r--   0        0        0    15938 2024-03-18 18:50:34.913013 eflips_model-3.3.0/eflips/model/network.py
+-rw-r--r--   0        0        0        0 2024-01-25 14:06:07.781569 eflips_model-3.3.0/eflips/model/py.typed
+-rw-r--r--   0        0        0    14194 2024-03-18 18:50:34.913435 eflips_model-3.3.0/eflips/model/schedule.py
+-rw-r--r--   0        0        0     6148 2024-04-24 14:53:08.399899 eflips_model-3.3.0/eflips/model/util/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-24 09:45:42.576370 eflips_model-3.3.0/eflips/model/util/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-24 14:39:09.510692 eflips_model-3.3.0/eflips/model/util/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0    13052 2024-04-24 15:32:43.319739 eflips_model-3.3.0/eflips/model/util/__pycache__/export.cpython-312.pyc
+-rw-r--r--   0        0        0     4263 2024-04-24 15:03:48.073244 eflips_model-3.3.0/eflips/model/util/__pycache__/import.cpython-312.pyc
+-rwxr-xr-x   0        0        0    12099 2024-04-24 15:38:03.293955 eflips_model-3.3.0/eflips/model/util/export.py
+-rwxr-xr-x   0        0        0     3630 2024-04-24 15:13:59.211863 eflips_model-3.3.0/eflips/model/util/import.py
+-rw-r--r--   0        0        0      956 2024-04-24 15:07:12.977847 eflips_model-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7245 1970-01-01 00:00:00.000000 eflips_model-3.3.0/PKG-INFO
```

### Comparing `eflips_model-3.2.0/LICENSE.md` & `eflips_model-3.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/README.md` & `eflips_model-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/__init__.py` & `eflips_model-3.3.0/eflips/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 from eflips.model.general import BatteryType as BatteryType
 from eflips.model.general import Scenario as Scenario
 from eflips.model.general import Vehicle as Vehicle
 from eflips.model.general import VehicleClass as VehicleClass
 from eflips.model.general import VehicleType as VehicleType
 from eflips.model.general import Event as Event
 from eflips.model.general import EventType as EventType
+from eflips.model.general import (
+    AssocVehicleTypeVehicleClass as AssocVehicleTypeVehicleClass,
+)
 
 from eflips.model.network import ChargeType as ChargeType
 from eflips.model.network import Line as Line
 from eflips.model.network import Route as Route
 from eflips.model.network import Station as Station
 from eflips.model.network import VoltageLevel as VoltageLevel
 from eflips.model.network import AssocRouteStation as AssocRouteStation
```

### Comparing `eflips_model-3.2.0/eflips/model/alembic.ini` & `eflips_model-3.3.0/eflips/model/alembic.ini`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/depot.py` & `eflips_model-3.3.0/eflips/model/depot.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,19 @@
     processes: Mapped[List["Process"]] = relationship(
         "Process", secondary="AssocAreaProcess", back_populates="areas"
     )
 
     events: Mapped[List["Event"]] = relationship("Event", back_populates="area")
     """The events that happened in this area."""
 
+    assoc_area_processes: Mapped[List["AssocAreaProcess"]] = relationship(
+        "AssocAreaProcess", viewonly=True
+    )
+    """The association between this area and its processes."""
+
     _table_args_list.append(capacity_constraint)
 
     __table_args__ = tuple(_table_args_list)
 
     def __repr__(self) -> str:
         return f"<Area(id={self.id}, name={self.name}, area_type={self.area_type}, capacity={self.capacity})>"
 
@@ -236,14 +241,18 @@
 
     areas: Mapped[List["Area"]] = relationship(
         "Area",
         secondary="AssocAreaProcess",
         back_populates="processes",
     )
 
+    assoc_area_processes: Mapped[List["AssocAreaProcess"]] = relationship(
+        "AssocAreaProcess", viewonly=True
+    )
+
     # This constraint verifies that the process actually does something
     _table_args_list.append(
         CheckConstraint(
             "(duration IS NULL) OR"
             "(duration IS NOT NULL AND duration >= '00:00:00') OR"
             "(electric_power IS NULL) OR"
             "(electric_power IS NOT NULL AND electric_power >= 0)",
@@ -295,13 +304,17 @@
     __tablename__ = "AssocAreaProcess"
 
     id = mapped_column(BigInteger, primary_key=True)
     """The unique identifier of the association. Auto-incremented. Needed for django."""
 
     area_id: Mapped[int] = mapped_column(ForeignKey("Area.id"))
     """The unique identifier of the area. Foreign key to :attr:`Area.id`."""
+    area: Mapped["Area"] = relationship("Area", overlaps="areas,processes")
+    """The area."""
 
     process_id: Mapped[int] = mapped_column(ForeignKey("Process.id"))
     """The unique identifier of the process. Foreign key to :attr:`Process.id`."""
+    process: Mapped["Process"] = relationship("Process", overlaps="areas,processes")
+    """The process."""
 
     def __repr__(self) -> str:
         return f"<AssocAreaProcess(id={self.id}, area_id={self.area_id}, process_id={self.process_id})>"
```

### Comparing `eflips_model-3.2.0/eflips/model/general.py` & `eflips_model-3.3.0/eflips/model/general.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,14 +564,18 @@
 
     events: Mapped[List["Event"]] = relationship("Event", back_populates="vehicle_type")
     """A list of events."""
 
     areas: Mapped[List["Area"]] = relationship("Area", back_populates="vehicle_type")
     """A list of areas."""
 
+    assoc_vehicle_type_vehicle_classes: Mapped[
+        "AssocVehicleTypeVehicleClass"
+    ] = relationship("AssocVehicleTypeVehicleClass", viewonly=True)
+
     __table_args__ = tuple(_table_args_list)
 
     def __repr__(self) -> str:
         return f"<VehicleType(id={self.id}, name={self.name})>"
 
 
 class BatteryType(Base):
@@ -673,14 +677,18 @@
 
     vehicle_types: Mapped[List["VehicleType"]] = relationship(
         "VehicleType",
         secondary="AssocVehicleTypeVehicleClass",
         back_populates="vehicle_classes",
     )
 
+    assoc_vehicle_type_vehicle_classes: Mapped[
+        "AssocVehicleTypeVehicleClass"
+    ] = relationship("AssocVehicleTypeVehicleClass", viewonly=True)
+
     def __repr__(self) -> str:
         return f"<VehicleClass(id={self.id}, name={self.name})>"
 
 
 class AssocVehicleTypeVehicleClass(Base):
     """
     The association table for the many-to-many relationship between vehicles and classes.
@@ -688,17 +696,23 @@
 
     __tablename__ = "AssocVehicleTypeVehicleClass"
     id = mapped_column(BigInteger, primary_key=True)
     """Not the primary key and not used in SQLAlchemy, but required by Django."""
 
     vehicle_type_id: Mapped[int] = mapped_column(ForeignKey("VehicleType.id"))
     """The unique identifier of the vehicle type. Foreign key to :attr:`VehicleType.id`."""
+    vehicle_type: Mapped[VehicleType] = relationship(
+        "VehicleType", overlaps="vehicle_classes,vehicle_types"
+    )
 
     vehicle_class_id: Mapped[int] = mapped_column(ForeignKey("VehicleClass.id"))
     """The unique identifier of the vehicle class. Foreign key to :attr:`VehicleClass.id`."""
+    vehicle_class: Mapped[VehicleClass] = relationship(
+        "VehicleClass", overlaps="vehicle_classes,vehicle_types"
+    )
 
     def __repr__(self) -> str:
         return f"<AssocVehicleTypeVehicleClass(id={self.id}, vehicle_type_id={self.vehicle_type_id}, vehicle_class_id={self.vehicle_class_id})>"
 
 
 class EventType(PyEnum):
     """
```

### Comparing `eflips_model-3.2.0/eflips/model/migrations/env.py` & `eflips_model-3.3.0/eflips/model/migrations/env.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/script.py.mako` & `eflips_model-3.3.0/eflips/model/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/0548463664b4_3_1_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/126892076499_v2_0_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/126892076499_v2_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/6ac022147397_3_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/7483339ae654_v2_2_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/9e29124f8ce6_v1_1_6.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/a06c97c98d2c_v2_1_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/a9f1c33488b6_3_0_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py` & `eflips_model-3.3.0/eflips/model/migrations/versions/baef3598b52c_v2_3_0.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/network.py` & `eflips_model-3.3.0/eflips/model/network.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/eflips/model/schedule.py` & `eflips_model-3.3.0/eflips/model/schedule.py`

 * *Files identical despite different names*

### Comparing `eflips_model-3.2.0/pyproject.toml` & `eflips_model-3.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-model"
-version = "3.2.0"
+version = "3.3.0"
 description = "A common data model for the eflips family of electric vehicle simulation & optimization tools."
 authors = [
 	"Ludger Heide <ludger.heide@tu-berlin.de>",
 	"Shuyao Guo <shuyao.guo@tu-berlin.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
@@ -25,12 +25,13 @@
 mypy = "^1.7.1"
 black = "^23.11.0"
 sphinx-autoapi = "^3.0.0"
 pytest = "^7.4.3"
 pytest-pycharm = "^0.7.0"
 pre-commit = "^3.5.0"
 sphinx-paramlinks = "^0.6.0"
+types-psycopg2 = "^2.9.21.20240417"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eflips_model-3.2.0/PKG-INFO` & `eflips_model-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-model
-Version: 3.2.0
+Version: 3.3.0
 Summary: A common data model for the eflips family of electric vehicle simulation & optimization tools.
 Home-page: https://github.com/mpm-tu-berlin/eflips-model
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@tu-berlin.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

