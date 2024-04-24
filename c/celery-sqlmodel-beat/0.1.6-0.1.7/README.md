# Comparing `tmp/celery_sqlmodel_beat-0.1.6.tar.gz` & `tmp/celery_sqlmodel_beat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_sqlmodel_beat-0.1.6.tar", max compression
+gzip compressed data, was "celery_sqlmodel_beat-0.1.7.tar", max compression
```

## Comparing `celery_sqlmodel_beat-0.1.6.tar` & `celery_sqlmodel_beat-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2024-04-10 07:51:25.382208 celery_sqlmodel_beat-0.1.6/LICENSE
--rw-r--r--   0        0        0     1790 2024-04-10 09:04:57.596997 celery_sqlmodel_beat-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:59:12.511663 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/__init__.py
--rw-r--r--   0        0        0     1428 2024-03-26 06:59:12.511775 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/clockedschedule.py
--rw-r--r--   0        0        0    16421 2024-04-10 08:58:29.862538 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/models.py
--rw-r--r--   0        0        0    13249 2024-04-10 05:54:34.370412 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/schedulers.py
--rw-r--r--   0        0        0     2695 2024-04-10 07:41:25.226801 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/tzcrontab.py
--rw-r--r--   0        0        0      354 2024-04-10 07:42:01.484314 celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/util.py
--rw-r--r--   0        0        0      634 2024-04-10 09:06:28.580695 celery_sqlmodel_beat-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 celery_sqlmodel_beat-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-10 07:51:25.382208 celery_sqlmodel_beat-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1790 2024-04-10 09:04:57.596997 celery_sqlmodel_beat-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:59:12.511663 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/__init__.py
+-rw-r--r--   0        0        0     1428 2024-03-26 06:59:12.511775 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/clockedschedule.py
+-rw-r--r--   0        0        0    18079 2024-04-22 23:39:31.858415 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/models.py
+-rw-r--r--   0        0        0    13249 2024-04-10 05:54:34.370412 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/schedulers.py
+-rw-r--r--   0        0        0     2695 2024-04-10 07:41:25.226801 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/tzcrontab.py
+-rw-r--r--   0        0        0      354 2024-04-10 07:42:01.484314 celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/util.py
+-rw-r--r--   0        0        0      634 2024-04-24 21:01:08.160729 celery_sqlmodel_beat-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 celery_sqlmodel_beat-0.1.7/PKG-INFO
```

### Comparing `celery_sqlmodel_beat-0.1.6/LICENSE` & `celery_sqlmodel_beat-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_sqlmodel_beat-0.1.6/README.md` & `celery_sqlmodel_beat-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/clockedschedule.py` & `celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/models.py` & `celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from cron_descriptor import (
     FormatException,
     MissingFieldException,
     WrongArgumentException,
     get_description,
 )
 from pydantic import ValidationError, field_validator, model_validator
+from pydantic_core import InitErrorDetails, PydanticCustomError
 from sqlalchemy.event import listen
 from sqlmodel import Column, Field, Relationship, Session, SQLModel, select, BIGINT
 
 from .clockedschedule import clocked
 from .tzcrontab import TzAwareCrontab
 from .util import make_aware, nowfun
 
@@ -317,24 +318,24 @@
 class PeriodicTask(ModelMixin, table=True):
     """Model representing a periodic task."""
 
     name: str = Field(max_length=200, unique=True)
     task: str = Field(max_length=200)
 
     interval_id: Optional[int] = Field(sa_type=BIGINT, default=None, foreign_key="tasks_interval_schedule.id")
-    interval: Optional[IntervalSchedule] = Relationship(back_populates="periodic_task")
+    interval: Optional[IntervalSchedule] = Relationship(back_populates="periodic_task",sa_relationship_kwargs={"lazy": "selectin"},)
 
     crontab_id: Optional[int] = Field(sa_type=BIGINT, default=None, foreign_key="tasks_crontab_schedule.id")
-    crontab: Optional[CrontabSchedule] = Relationship(back_populates="periodic_task")
+    crontab: Optional[CrontabSchedule] = Relationship(back_populates="periodic_task",sa_relationship_kwargs={"lazy": "selectin"},)
 
     solar_id: Optional[int] = Field(sa_type=BIGINT, default=None, foreign_key="tasks_solar_schedule.id")
-    solar: Optional[SolarSchedule] = Relationship(back_populates="periodic_task")
+    solar: Optional[SolarSchedule] = Relationship(back_populates="periodic_task",sa_relationship_kwargs={"lazy": "selectin"},)
 
     clocked_id: Optional[int] = Field(sa_type=BIGINT, default=None, foreign_key="tasks_clocked_schedule.id")
-    clocked: Optional[ClockedSchedule] = Relationship(back_populates="periodic_task")
+    clocked: Optional[ClockedSchedule] = Relationship(back_populates="periodic_task",sa_relationship_kwargs={"lazy": "selectin"},)
 
     # These are JSON fields, so we can store any serializable data
     # For querying, we can use the JSON operators in SQLAlchemy
     # https://docs.sqlalchemy.org/en/14/dialects/postgresql.html#json-jsonb
     # Example:
     # .where(PeriodicTask.args.op("->>")(0).cast(Integer)== your_var)
     # This compares the first element of the args JSON array to your_var
@@ -374,44 +375,88 @@
         default=nowfun(),
     )
     description: str = Field(max_length=200, nullable=True)
 
     no_changes: bool = False
 
     @model_validator(mode="after")
-    @classmethod
-    def validate_unique(cls, values: dict):
-
-        schedule_types = ["interval", "crontab", "solar", "clocked"]
-        selected_schedule_types = [
-            s for s in schedule_types if values.get(s) is not None
-        ]
+    def validate_unique(self):
+        selected_schedule_types = list(
+            filter(
+                lambda element: element is not None,
+                [
+                    self.interval,
+                    self.crontab,
+                    self.solar,
+                    self.clocked,
+                ],
+            )
+        )
 
         if len(selected_schedule_types) == 0:
-            raise ValidationError(
-                "One of clocked, interval, crontab, or solar "
-                "must be set."  # pylint: disable=implicit-str-concat
+            raise ValidationError.from_exception_data(
+                title="Missing Schedule Type",
+                line_errors=[
+                    InitErrorDetails(
+                        input=self.name,
+                        type=PydanticCustomError(
+                            "String",
+                            "One of clocked, interval, crontab, or solar must be set.",
+                        ),
+                    )
+                ],
             )
 
-        err_msg = (
-            "Only one of clocked, interval, crontab, "
-            "or solar must be set"  # pylint: disable=implicit-str-concat
-        )
+        err_msg = "Only one of clocked, interval, crontab, or solar must be set"
         if len(selected_schedule_types) > 1:
             error_info = {}
             for selected_schedule_type in selected_schedule_types:
                 error_info[selected_schedule_type] = [err_msg]
-            raise ValidationError(f"{error_info}")
+            raise ValidationError.from_exception_data(
+                title="Schedule Conflict",
+                line_errors=[
+                    InitErrorDetails(
+                        input=self.name,
+                        type=PydanticCustomError(
+                            "String",
+                            f"{error_info}",
+                        ),
+                    )
+                ],
+            )
 
         # clocked must be one off task
-        if values["clocked"] and not values["one_off"]:
+        if self.clocked and not self.one_off:
             err_msg = "clocked must be one off, one_off must set True"
-            raise ValidationError(err_msg)
-        if (values["expires_seconds"] is not None) and (values["expires"] is not None):
-            raise ValidationError("Only one can be set, in expires and expire_seconds")
+            raise ValidationError.from_exception_data(
+                title="Clocked Error",
+                line_errors=[
+                    InitErrorDetails(
+                        input=self.name,
+                        type=PydanticCustomError(
+                            "String",
+                            f"{err_msg}",
+                        ),
+                    )
+                ],
+            )
+        if (self.expire_seconds is not None) and (self.expires is not None):
+            raise ValidationError.from_exception_data(
+                title="Expires Error",
+                line_errors=[
+                    InitErrorDetails(
+                        input=self.name,
+                        type=PydanticCustomError(
+                            "String",
+                            "Only one can be set, in expires and expire_seconds",
+                        ),
+                    )
+                ],
+            )
+        return self
 
     @property
     def expires_(self):
         return self.expires or self.expire_seconds
 
     def __str__(self):
         fmt = "{0.name}: {{no schedule}}"
```

### Comparing `celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/schedulers.py` & `celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/schedulers.py`

 * *Files identical despite different names*

### Comparing `celery_sqlmodel_beat-0.1.6/celery_sqlmodel_beat/tzcrontab.py` & `celery_sqlmodel_beat-0.1.7/celery_sqlmodel_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `celery_sqlmodel_beat-0.1.6/pyproject.toml` & `celery_sqlmodel_beat-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celery-sqlmodel-beat"
-version = "0.1.6"
+version = "0.1.7"
 authors = ["Cray"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "celery_sqlmodel_beat"}]
 description = "Celery Periodic Tasks backed by the sqlmodel"
 
 [project.urls]
```

### Comparing `celery_sqlmodel_beat-0.1.6/PKG-INFO` & `celery_sqlmodel_beat-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-sqlmodel-beat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Celery Periodic Tasks backed by the sqlmodel
 License: MIT
 Author: Cray
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

