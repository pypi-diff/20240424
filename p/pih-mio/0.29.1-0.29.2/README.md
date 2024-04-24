# Comparing `tmp/pih-mio-0.29.1.tar.gz` & `tmp/pih-mio-0.29.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-0.29.1.tar", last modified: Mon Apr 22 04:12:03 2024, max compression
+gzip compressed data, was "pih-mio-0.29.2.tar", last modified: Wed Apr 24 03:32:59 2024, max compression
```

## Comparing `pih-mio-0.29.1.tar` & `pih-mio-0.29.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 04:12:03.135127 pih-mio-0.29.1/
-drwxrwxrwx   0        0        0        0 2024-04-22 04:12:02.690916 pih-mio-0.29.1/MobileHelperService/
--rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.1/MobileHelperService/__init__.py
--rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.1/MobileHelperService/__main__.py
--rw-rw-rw-   0        0        0   374073 2024-04-22 03:14:50.000000 pih-mio-0.29.1/MobileHelperService/api.py
--rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.1/MobileHelperService/client.py
--rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.1/MobileHelperService/collection.py
--rw-rw-rw-   0        0        0     4465 2024-04-22 04:11:21.000000 pih-mio-0.29.1/MobileHelperService/const.py
--rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.1/MobileHelperService/service.py
--rw-rw-rw-   0        0        0    16542 2024-04-10 05:18:33.000000 pih-mio-0.29.1/MobileHelperService/service_api.py
--rw-rw-rw-   0        0        0      331 2024-04-22 04:12:03.088251 pih-mio-0.29.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 04:12:03.056998 pih-mio-0.29.1/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      331 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-22 04:12:02.000000 pih-mio-0.29.1/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 04:12:01.000000 pih-mio-0.29.1/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 04:12:03.166460 pih-mio-0.29.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 03:32:59.452346 pih-mio-0.29.2/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:32:58.552842 pih-mio-0.29.2/MobileHelperService/
+-rw-rw-rw-   0        0        0        0 2024-01-09 05:16:13.000000 pih-mio-0.29.2/MobileHelperService/__init__.py
+-rw-rw-rw-   0        0        0      208 2024-02-09 05:31:09.000000 pih-mio-0.29.2/MobileHelperService/__main__.py
+-rw-rw-rw-   0        0        0   371457 2024-04-24 03:32:14.000000 pih-mio-0.29.2/MobileHelperService/api.py
+-rw-rw-rw-   0        0        0     5945 2024-04-10 05:33:19.000000 pih-mio-0.29.2/MobileHelperService/client.py
+-rw-rw-rw-   0        0        0      100 2024-02-20 01:16:51.000000 pih-mio-0.29.2/MobileHelperService/collection.py
+-rw-rw-rw-   0        0        0     4465 2024-04-24 03:32:22.000000 pih-mio-0.29.2/MobileHelperService/const.py
+-rw-rw-rw-   0        0        0      635 2024-02-14 02:40:54.000000 pih-mio-0.29.2/MobileHelperService/service.py
+-rw-rw-rw-   0        0        0    16542 2024-04-23 06:08:38.000000 pih-mio-0.29.2/MobileHelperService/service_api.py
+-rw-rw-rw-   0        0        0      331 2024-04-24 03:32:59.421108 pih-mio-0.29.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 03:32:59.341974 pih-mio-0.29.2/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      331 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-24 03:32:57.000000 pih-mio-0.29.2/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:32:59.500324 pih-mio-0.29.2/setup.cfg
```

### Comparing `pih-mio-0.29.1/MobileHelperService/api.py` & `pih-mio-0.29.2/MobileHelperService/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,18 +68,18 @@
     nnb,
     nnl,
     escs,
     if_else,
     while_not_do,
 )
 from pih.consts import (
-    CheckableSections,
+    Tags,
     Actions,
     JournalType,
-    Tags,
+    CheckableSections,
     EmailVerificationMethods,
 )
 from MobileHelperService.collection import MobileHelperUserSettings
 from pih.consts.polibase import PolibaseDocumentTypes
 from pih.consts.ssh_hosts import SSHHosts
 from MobileHelperService.const import *
 
@@ -109,14 +109,21 @@
 
     def i(self, value: str) -> str:
         return i(value)
 
 
 SIMPLE_OUTPUT: MobileOutputBase = MobileOutputBase()
 
+def format_given_name(
+    session: Session, output: Output, name: str | None = None
+) -> str | None:
+    if e(session.login):
+        return None
+    return output.bold(name or session.user_given_name)
+
 
 def get_wappi_status(space: str, value: A.CT_ME_WH_W.Profiles) -> str:
     lines: list[str] = A.D_F.wappi_status(value, SIMPLE_OUTPUT).splitlines()
     return jnl(
         (
             j((" ", A.CT_V.BLUE_ROMB, " ", lines[0])),
             jnl((A.D.map(lambda item: j((space, " ", item)), lines[1:]))),
@@ -1102,32 +1109,27 @@
     user: list[CommandNode] | None = None
     journals: list[CommandNode] | None = None
     marketer_unit: list[CommandNode] | None = None
 
 
 @dataclass
 class KEYWORDS:
-    flag: FLAG_KEYWORDS = FLAG_KEYWORDS
-    command: COMMAND_KEYWORDS = COMMAND_KEYWORDS
+    flag = FLAG_KEYWORDS
+    command = COMMAND_KEYWORDS
     FROM_FILE_REDIRECT: str = FROM_FILE_REDIRECT_SYMBOL
 
 
 def get_file_pattern_index(value: str | None) -> int | None:
     if e(value):
         return None
     for file_pattern_index, pattern in enumerate(FILE_PATTERN_LIST):
         if nnt(value).find(pattern) == 0:
             return file_pattern_index
     return None
 
-
-def check_for_arg_is_file(self, value: str) -> bool:
-    return nn(get_file_pattern_index(value))
-
-
 class MobileHelper(OutputStub):
 
     command_base_name_collection: tuple[str, ...] | None = None
     command_node_name_collection: tuple[str, ...] | None = None
     allowed_group_collection: set[Groups] | None = None
 
     def flag_string_represent(self, value: Flags, all: bool = True) -> str:
@@ -5517,15 +5519,17 @@
         def show_settings() -> None:
             self.write_line(
                 js(
                     (
                         "Состояние:",
                         self.output.bold(
                             ["Выключен", "Включен"][
-                                A.S.get(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON)
+                                A.S.get(
+                                    A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON
+                                )
                             ]
                         ),
                     )
                 )
             )
             self.write_line(
                 js(
@@ -5535,115 +5539,62 @@
                             A.S.get(
                                 A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME,
                             )
                         ),
                     )
                 )
             )
+
         show_settings()
         if self.yes_no("Запустить мастер настройки"):
-            if self.set_variable_value(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON):
-                self.set_variable_value(A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME)
+            if self.set_variable_value(
+                A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_IS_ON
+            ):
+                self.set_variable_value(
+                    A.CT_S.POLIBASE_PERSON_REVIEW_NOTIFICATION_START_TIME
+                )
             self.output.good("Настройка завершена")
             show_settings()
 
     def set_variable_value(self, value: A.CT_S) -> Any:
         return self.variable_value_getter_and_setter_handler(
             False, variable_name=A.D.get(value).key_name, silence=True
         )
 
     def time_tracking_report_handler(self, for_me_report_only: bool = False) -> None:
-        def get_date_format(value: str) -> str:
-            value = value.strip()
-            return (
-                A.CT.YEARLESS_DATE_FORMAT
-                if value.count(A.CT.DATE_PART_DELIMITER) == 1 or value.count(" ") == 1
-                else A.CT.DATE_FORMAT
-            )
-
         today: date = A.D.today()
         if for_me_report_only:
             if self.argless and self.yes_no(
                 "Получить отчет в период с начала месяца до сегодняшнего дня"
             ):
                 now: datetime = A.D.now()
                 self.arg_list.append(jp((1, now.month, today.year)))
                 self.arg_list.append(jp((now.day, now.month, today.year)))
-        value: str | None = self.arg()
-        format: str | None = None if e(value) else get_date_format(value)
-        start_date: datetime | None = A.D_Ex.datetime(value, format)
-        if ne(start_date):
-            if format == A.CT.YEARLESS_DATE_FORMAT:
-                start_date = start_date.replace(today.year)
-        value = self.arg(1)
-        format = None if e(value) else get_date_format(value)
-        end_date: datetime | None = A.D_Ex.datetime(value, format)
-        if ne(end_date):
-            if format == A.CT.YEARLESS_DATE_FORMAT:
-                end_date = end_date.replace(today.year)
-        while True:
-            if e(start_date):
-                value = self.input.input(
-                    j(
-                        (
-                            "Введите начало периода, в формате ",
-                            self.output.bold("ДЕНЬ.МЕСЯЦ"),
-                            ", например ",
-                            A.D.today_string(A.CT.YEARLESS_DATE_FORMAT),
-                        )
-                    )
-                )
-                value = A.D_F.to_date(value)
-                format = get_date_format(value)
-                if format == A.CT.YEARLESS_DATE_FORMAT:
-                    value = jp((value, today.year))
-                start_date = A.D_Ex.datetime(value, A.CT.DATE_FORMAT)
-                if e(start_date) or start_date.date() > today:
-                    continue
-            if e(end_date) or start_date > end_date:
-                if not self.yes_no(
-                    "Использовать сегодняшнюю дату",
-                    no_label=j(
-                        (
-                            "Введите окончание периода, в формате ",
-                            self.output.bold("ДЕНЬ.МЕСЯЦ"),
-                            ", например ",
-                            A.D.today_string(A.CT.YEARLESS_DATE_FORMAT),
-                        )
-                    ),
-                ):
-                    value = A.D_F.to_date(self.input.answer)
-                    format = get_date_format(value)
-                    if format == A.CT.YEARLESS_DATE_FORMAT:
-                        value = jp((value, today.year))
-                    end_date = A.D_Ex.datetime(value, A.CT.DATE_FORMAT)
-                    if e(end_date):
-                        continue
-                else:
-                    end_date = A.D.today(as_datetime=True)
-            if not (e(start_date) or e(end_date)):
-                break
+
+        start_date, end_date = self.input.start_and_end_date(self.arg(), self.arg(1))
         start_date_string: str = A.D.date_to_string(
             start_date, A.CT.YEARLESS_DATE_FORMAT
         )
         end_date_string: str = A.D.date_to_string(end_date, A.CT.YEARLESS_DATE_FORMAT)
+
         report_file_name: str = A.PTH.add_extension(
             j([self.session.login, start_date_string, end_date_string], "_"),
             A.CT_F_E.EXCEL_NEW,
         )
         report_file_path: str = A.PTH.join(
             A.PTH.MOBILE_HELPER.TIME_TRACKING_REPORT_FOLDER, report_file_name
         )
         allowed_report_for_all_persons: bool = (
             not for_me_report_only
             and not self.is_forced
             and A.C_A.by_group(
                 Groups.TimeTrackingReport, False, self.session, True, False
             )
         )
+
         if A.A_TT.save_report(
             report_file_path,
             start_date,
             end_date,
             (
                 None
                 if allowed_report_for_all_persons
```

### Comparing `pih-mio-0.29.1/MobileHelperService/client.py` & `pih-mio-0.29.2/MobileHelperService/client.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.29.1/MobileHelperService/const.py` & `pih-mio-0.29.2/MobileHelperService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 NAME: str = "MobileHelper"
 
 DEFAULT_COUNT = 100
 ADMIN_ALIAS: str = "admin"
 COUNT_ALIAS: str = "count"
-VERSION: str = "0.29.1"
+VERSION: str = "0.29.2"
 
 HOST = Hosts.WS255
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Mobile helper service",
     host=HOST.NAME,
```

### Comparing `pih-mio-0.29.1/MobileHelperService/service.py` & `pih-mio-0.29.2/MobileHelperService/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-0.29.1/MobileHelperService/service_api.py` & `pih-mio-0.29.2/MobileHelperService/service_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     MobileUserInput,
     MobileMarkInput,
     get_wappi_status,
     InternalInterrupt,
     MobileHelper as Api,
     AddressedInterruption,
 )
+from pih.console_api import LINE
 from pih.consts.errors import NotFound
 from MobileHelperService.const import *
-from pih.console_api import LINE
 from pih import A, PIH, Stdin, PIHThread
 from pih.tools import (
     j,
     b,
     n,
     i,
     e,
```

