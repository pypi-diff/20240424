# Comparing `tmp/edc-appointment-0.4.8.tar.gz` & `tmp/edc-appointment-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-appointment-0.4.8.tar", last modified: Sat Jan  6 03:42:29 2024, max compression
+gzip compressed data, was "edc-appointment-0.4.9.tar", last modified: Wed Jan 24 05:30:45 2024, max compression
```

## Comparing `edc-appointment-0.4.8.tar` & `edc-appointment-0.4.9.tar`

### file list

```diff
@@ -1,208 +1,210 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.831697 edc-appointment-0.4.8/
--rw-r--r--   0 erikvw     (501) staff       (20)      243 2023-08-01 04:05:04.000000 edc-appointment-0.4.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 14:15:00.000000 edc-appointment-0.4.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.793171 edc-appointment-0.4.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.799265 edc-appointment-0.4.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     2091 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-05-02 18:44:30.000000 edc-appointment-0.4.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-appointment-0.4.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      362 2020-03-04 23:12:07.000000 edc-appointment-0.4.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)     2435 2023-09-22 02:23:07.000000 edc-appointment-0.4.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 23:11:42.000000 edc-appointment-0.4.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      156 2023-09-22 02:23:07.000000 edc-appointment-0.4.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     9365 2024-01-06 03:42:29.831600 edc-appointment-0.4.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     8521 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 22:57:31.000000 edc-appointment-0.4.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.803671 edc-appointment-0.4.8/edc_appointment/
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-10-15 23:22:52.000000 edc-appointment-0.4.8/edc_appointment/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.805545 edc-appointment-0.4.8/edc_appointment/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-07-18 12:12:49.000000 edc-appointment-0.4.8/edc_appointment/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2514 2022-07-18 12:12:49.000000 edc-appointment-0.4.8/edc_appointment/admin/actions.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8848 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment/admin/appointment_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-11-01 12:53:23.000000 edc-appointment-0.4.8/edc_appointment/admin/list_filters.py
--rw-r--r--   0 erikvw     (501) staff       (20)      175 2021-05-12 12:28:28.000000 edc-appointment-0.4.8/edc_appointment/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8189 2023-09-22 02:23:07.000000 edc-appointment-0.4.8/edc_appointment/appointment_reason_updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1753 2022-09-25 16:15:58.000000 edc-appointment-0.4.8/edc_appointment/appointment_status_updater.py
--rw-r--r--   0 erikvw     (501) staff       (20)      561 2022-08-25 03:20:20.000000 edc-appointment-0.4.8/edc_appointment/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      296 2023-08-01 04:05:04.000000 edc-appointment-0.4.8/edc_appointment/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-08-01 04:05:04.000000 edc-appointment-0.4.8/edc_appointment/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1114 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1009 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/constants.py
--rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-08-25 03:20:20.000000 edc-appointment-0.4.8/edc_appointment/context_processors.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.806851 edc-appointment-0.4.8/edc_appointment/creators/
--rw-r--r--   0 erikvw     (501) staff       (20)      491 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/creators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9229 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/creators/appointment_creator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3659 2023-11-22 02:29:32.000000 edc-appointment-0.4.8/edc_appointment/creators/appointments_creator.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10272 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/creators/unscheduled_appointment_creator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/creators/utils.py
--rw-r--r--   0 erikvw     (501) staff       (20)      689 2022-10-26 02:01:25.000000 edc-appointment-0.4.8/edc_appointment/exceptions.py
--rw-r--r--   0 erikvw     (501) staff       (20)      329 2023-11-30 05:10:38.000000 edc-appointment-0.4.8/edc_appointment/form_runners.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.807519 edc-appointment-0.4.8/edc_appointment/form_validator_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      180 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/form_validator_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3181 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/form_validator_mixins/next_appointment_crf_form_validator_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4256 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment/form_validator_mixins/window_period_form_validator_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.808118 edc-appointment-0.4.8/edc_appointment/form_validators/
--rw-r--r--   0 erikvw     (501) staff       (20)      195 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/form_validators/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)    24113 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/form_validators/appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)      318 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/form_validators/next_appointment_crf_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3138 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/form_validators/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.808547 edc-appointment-0.4.8/edc_appointment/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1328 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/forms/appointment_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      926 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/list_data.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.808649 edc-appointment-0.4.8/edc_appointment/management/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 01:04:14.000000 edc-appointment-0.4.8/edc_appointment/management/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.809224 edc-appointment-0.4.8/edc_appointment/management/commands/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 01:04:14.000000 edc-appointment-0.4.8/edc_appointment/management/commands/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1830 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/management/commands/close_appointments.py
--rw-r--r--   0 erikvw     (501) staff       (20)      567 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment/management/commands/update_appointment_status.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2293 2023-09-27 03:22:15.000000 edc-appointment-0.4.8/edc_appointment/management/commands/update_skipped_appointments.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9288 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment/managers.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.817299 edc-appointment-0.4.8/edc_appointment/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)      844 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    20411 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0002_auto_20161126_1156.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1454 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0003_auto_20161127_2226.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1094 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0004_auto_20161210_1408.py
--rw-r--r--   0 erikvw     (501) staff       (20)      710 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0005_auto_20161221_2135.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3687 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0006_auto_20170106_2118.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1656 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0007_auto_20170302_2220.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6350 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0008_auto_20171115_1601.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1044 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0009_auto_20171119_1032.py
--rw-r--r--   0 erikvw     (501) staff       (20)      798 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0010_auto_20171124_1120.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2076 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0011_auto_20171128_1054.py
--rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0012_auto_20171128_2153.py
--rw-r--r--   0 erikvw     (501) staff       (20)      248 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0013_delete_holiday.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1193 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0014_auto_20180116_1411.py
--rw-r--r--   0 erikvw     (501) staff       (20)      513 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0015_auto_20180706_1519.py
--rw-r--r--   0 erikvw     (501) staff       (20)      495 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0016_auto_20181108_0353.py
--rw-r--r--   0 erikvw     (501) staff       (20)      679 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0017_auto_20190201_0446.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3583 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0018_auto_20190305_0123.py
--rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0019_auto_20190627_2257.py
--rw-r--r--   0 erikvw     (501) staff       (20)      575 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0020_auto_20190922_0439.py
--rw-r--r--   0 erikvw     (501) staff       (20)      601 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0021_auto_20191024_1000.py
--rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0022_auto_20200729_2310.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2852 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0023_auto_20200821_2119.py
--rw-r--r--   0 erikvw     (501) staff       (20)      553 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0024_auto_20200911_0425.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1300 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0025_auto_20210624_0225.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4159 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0026_auto_20220501_1548.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1290 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0027_appointment_document_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0028_appointment_document_status_comments_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      655 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0029_appointment_ignore_window_period_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2881 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0030_alter_appointment_appt_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      818 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0031_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)      826 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0032_alter_appointment_unique_together.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2463 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0033_alter_appointment_appt_reason_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4224 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0034_appointmenttype_alter_appointment_appt_type_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      939 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0035_rename_appointment_appt_type.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1235 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0036_auto_20230124_1822.py
--rw-r--r--   0 erikvw     (501) staff       (20)      472 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/migrations/0037_remove_appointment_appt_type_old_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)      770 2023-07-10 03:30:01.000000 edc-appointment-0.4.8/edc_appointment/migrations/0038_alter_appointment_options.py
--rw-r--r--   0 erikvw     (501) staff       (20)      424 2023-08-03 05:09:25.000000 edc-appointment-0.4.8/edc_appointment/migrations/0039_appointmenttype_extra_value.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-08-22 03:04:53.000000 edc-appointment-0.4.8/edc_appointment/migrations/0040_appointment_appt_type_other_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2626 2023-08-22 03:04:53.000000 edc-appointment-0.4.8/edc_appointment/migrations/0041_alter_appointment_appt_reason_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2817 2023-08-23 01:29:06.000000 edc-appointment-0.4.8/edc_appointment/migrations/0042_alter_appointment_device_created_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3217 2023-09-22 02:23:07.000000 edc-appointment-0.4.8/edc_appointment/migrations/0043_alter_appointment_appt_status_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1522 2023-09-25 23:04:21.000000 edc-appointment-0.4.8/edc_appointment/migrations/0044_alter_appointment_appt_reason_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1986 2023-09-27 03:22:15.000000 edc-appointment-0.4.8/edc_appointment/migrations/0045_alter_appointment_appt_reason_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2991 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/migrations/0046_infosources.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8910 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/migrations/0047_alter_appointment_options_and_more.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.818652 edc-appointment-0.4.8/edc_appointment/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      457 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2824 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_fields_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6494 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_methods_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7758 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1783 2022-10-26 02:01:25.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/missed_appointment_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1889 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/next_appointment_crf_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1304 2022-10-25 03:04:52.000000 edc-appointment-0.4.8/edc_appointment/model_mixins/window_period_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.819100 edc-appointment-0.4.8/edc_appointment/modeladmin_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       85 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/modeladmin_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1948 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/modeladmin_mixins/next_appointment_crf_modeladmin_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.819729 edc-appointment-0.4.8/edc_appointment/modelform_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)      158 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/modelform_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6008 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/modelform_mixins/next_appointment_crf_modelform_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1308 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/modelform_mixins/previous_appointment_form_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.820514 edc-appointment-0.4.8/edc_appointment/models/
--rw-r--r--   0 erikvw     (501) staff       (20)      372 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      935 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/models/appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/models/appointment_type.py
--rw-r--r--   0 erikvw     (501) staff       (20)      285 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment/models/list_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6960 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/models/signals.py
--rw-r--r--   0 erikvw     (501) staff       (20)      132 2020-03-04 23:12:12.000000 edc-appointment-0.4.8/edc_appointment/offline_models.py
--rw-r--r--   0 erikvw     (501) staff       (20)    12476 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/skip_appointments.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1306 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment/stubs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      428 2022-08-25 03:20:20.000000 edc-appointment-0.4.8/edc_appointment/system_checks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.820776 edc-appointment-0.4.8/edc_appointment/templates/
--rw-r--r--   0 erikvw     (501) staff       (20)      451 2022-07-18 12:12:49.000000 edc-appointment-0.4.8/edc_appointment/templates/button.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.821098 edc-appointment-0.4.8/edc_appointment/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3780 2023-07-02 20:11:24.000000 edc-appointment-0.4.8/edc_appointment/templatetags/appointment_tags.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.822403 edc-appointment-0.4.8/edc_appointment/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      236 2023-08-01 04:05:04.000000 edc-appointment-0.4.8/edc_appointment/tests/appointment_test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.823613 edc-appointment-0.4.8/edc_appointment/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     3319 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/tests/helper.py
--rw-r--r--   0 erikvw     (501) staff       (20)      524 2020-10-04 12:36:31.000000 edc-appointment-0.4.8/edc_appointment/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)       59 2020-03-04 23:12:11.000000 edc-appointment-0.4.8/edc_appointment/tests/no_holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     2702 2023-10-05 13:40:41.000000 edc-appointment-0.4.8/edc_appointment/tests/test_case_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.827214 edc-appointment-0.4.8/edc_appointment/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:24:07.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5550 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)    29614 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11840 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment_creator.py
--rw-r--r--   0 erikvw     (501) staff       (20)    28857 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment_form_validator.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9322 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_datetimes.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9520 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_sequence.py
--rw-r--r--   0 erikvw     (501) staff       (20)    11916 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_status.py
--rw-r--r--   0 erikvw     (501) staff       (20)      455 2023-08-01 04:05:04.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6702 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_delete_appointment.py
--rw-r--r--   0 erikvw     (501) staff       (20)    10008 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_next_appointment_crf.py
--rw-r--r--   0 erikvw     (501) staff       (20)    25939 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_skipped_appt.py
--rw-r--r--   0 erikvw     (501) staff       (20)    13802 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_unscheduled.py
--rw-r--r--   0 erikvw     (501) staff       (20)    18854 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_window_period.py
--rw-r--r--   0 erikvw     (501) staff       (20)     6328 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment/tests/tests/test_window_period2.py
--rw-r--r--   0 erikvw     (501) staff       (20)      992 2023-10-31 02:29:07.000000 edc-appointment-0.4.8/edc_appointment/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-05-31 16:24:50.000000 edc-appointment-0.4.8/edc_appointment/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)    21958 2023-12-05 02:41:28.000000 edc-appointment-0.4.8/edc_appointment/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.827690 edc-appointment-0.4.8/edc_appointment/view_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       57 2020-03-04 23:12:12.000000 edc-appointment-0.4.8/edc_appointment/view_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5894 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment/view_mixins/appointment_view_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.828302 edc-appointment-0.4.8/edc_appointment/views/
--rw-r--r--   0 erikvw     (501) staff       (20)      101 2020-03-04 23:12:12.000000 edc-appointment-0.4.8/edc_appointment/views/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      286 2023-05-24 16:42:58.000000 edc-appointment-0.4.8/edc_appointment/views/home_view.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2917 2023-11-12 23:19:21.000000 edc-appointment-0.4.8/edc_appointment/views/unscheduled_appointment_view.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.831237 edc-appointment-0.4.8/edc_appointment.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     9365 2024-01-06 03:42:29.000000 edc-appointment-0.4.8/edc_appointment.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     8373 2024-01-06 03:42:29.000000 edc-appointment-0.4.8/edc_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-01-06 03:42:29.000000 edc-appointment-0.4.8/edc_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-01 22:36:23.000000 edc-appointment-0.4.8/edc_appointment.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2024-01-06 03:42:29.000000 edc-appointment-0.4.8/edc_appointment.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       36 2024-01-06 03:42:29.000000 edc-appointment-0.4.8/edc_appointment.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.829274 edc-appointment-0.4.8/edc_appointment_app/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 14:10:52.000000 edc-appointment-0.4.8/edc_appointment_app/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      122 2022-05-25 14:10:52.000000 edc-appointment-0.4.8/edc_appointment_app/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment_app/consents.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1251 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment_app/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)     7832 2024-01-06 03:42:20.000000 edc-appointment-0.4.8/edc_appointment_app/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1438 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/edc_appointment_app/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-06 03:42:29.831031 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/
--rw-r--r--   0 erikvw     (501) staff       (20)      225 2023-10-06 00:11:33.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1954 2023-11-16 03:53:38.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/crfs.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1459 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule1.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1330 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule2.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1687 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule3.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1813 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule4.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1910 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule5.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2152 2023-10-09 15:41:40.000000 edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule6.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1724 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2902 2023-12-13 19:33:50.000000 edc-appointment-0.4.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1171 2024-01-06 03:42:29.832025 edc-appointment-0.4.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.533796 edc-appointment-0.4.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)      243 2023-08-01 04:05:04.000000 edc-appointment-0.4.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-04 14:15:00.000000 edc-appointment-0.4.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.493098 edc-appointment-0.4.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.498833 edc-appointment-0.4.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2091 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      944 2022-05-02 18:44:30.000000 edc-appointment-0.4.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-appointment-0.4.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      362 2020-03-04 23:12:07.000000 edc-appointment-0.4.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)     2435 2023-09-22 02:23:07.000000 edc-appointment-0.4.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    18047 2020-03-04 23:11:42.000000 edc-appointment-0.4.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      156 2023-09-22 02:23:07.000000 edc-appointment-0.4.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     9365 2024-01-24 05:30:45.533680 edc-appointment-0.4.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     8521 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 22:57:31.000000 edc-appointment-0.4.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.504566 edc-appointment-0.4.9/edc_appointment/
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-10-15 23:22:52.000000 edc-appointment-0.4.9/edc_appointment/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.506456 edc-appointment-0.4.9/edc_appointment/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      167 2022-07-18 12:12:49.000000 edc-appointment-0.4.9/edc_appointment/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2514 2022-07-18 12:12:49.000000 edc-appointment-0.4.9/edc_appointment/admin/actions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8929 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/admin/appointment_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      306 2022-11-01 12:53:23.000000 edc-appointment-0.4.9/edc_appointment/admin/list_filters.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      175 2021-05-12 12:28:28.000000 edc-appointment-0.4.9/edc_appointment/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8189 2023-09-22 02:23:07.000000 edc-appointment-0.4.9/edc_appointment/appointment_reason_updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1753 2022-09-25 16:15:58.000000 edc-appointment-0.4.9/edc_appointment/appointment_status_updater.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      561 2022-08-25 03:20:20.000000 edc-appointment-0.4.9/edc_appointment/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      296 2023-08-01 04:05:04.000000 edc-appointment-0.4.9/edc_appointment/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2023-08-01 04:05:04.000000 edc-appointment-0.4.9/edc_appointment/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1114 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1009 2024-01-06 03:42:20.000000 edc-appointment-0.4.9/edc_appointment/constants.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      387 2022-08-25 03:20:20.000000 edc-appointment-0.4.9/edc_appointment/context_processors.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.507321 edc-appointment-0.4.9/edc_appointment/creators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      425 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/creators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9284 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/creators/appointment_creator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3709 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/creators/appointments_creator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10135 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/creators/unscheduled_appointment_creator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2023-10-05 13:40:41.000000 edc-appointment-0.4.9/edc_appointment/creators/utils.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1107 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/exceptions.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      329 2023-11-30 05:10:38.000000 edc-appointment-0.4.9/edc_appointment/form_runners.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.508231 edc-appointment-0.4.9/edc_appointment/form_validator_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      180 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/form_validator_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3181 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/edc_appointment/form_validator_mixins/next_appointment_crf_form_validator_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4256 2024-01-18 02:23:45.000000 edc-appointment-0.4.9/edc_appointment/form_validator_mixins/window_period_form_validator_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.509095 edc-appointment-0.4.9/edc_appointment/form_validators/
+-rw-r--r--   0 erikvw     (501) staff       (20)      195 2024-01-06 03:42:20.000000 edc-appointment-0.4.9/edc_appointment/form_validators/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    24467 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/form_validators/appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      318 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/form_validators/next_appointment_crf_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3138 2023-12-05 02:41:28.000000 edc-appointment-0.4.9/edc_appointment/form_validators/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.509613 edc-appointment-0.4.9/edc_appointment/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)       46 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1328 2024-01-17 05:21:38.000000 edc-appointment-0.4.9/edc_appointment/forms/appointment_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      926 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/list_data.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.509850 edc-appointment-0.4.9/edc_appointment/management/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 01:04:14.000000 edc-appointment-0.4.9/edc_appointment/management/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.510638 edc-appointment-0.4.9/edc_appointment/management/commands/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-11-19 01:04:14.000000 edc-appointment-0.4.9/edc_appointment/management/commands/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1830 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/management/commands/close_appointments.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      567 2023-10-09 15:41:40.000000 edc-appointment-0.4.9/edc_appointment/management/commands/update_appointment_status.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2293 2023-09-27 03:22:15.000000 edc-appointment-0.4.9/edc_appointment/management/commands/update_skipped_appointments.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9288 2023-10-09 15:41:40.000000 edc-appointment-0.4.9/edc_appointment/managers.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.519865 edc-appointment-0.4.9/edc_appointment/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)      844 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    20411 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0002_auto_20161126_1156.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1454 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0003_auto_20161127_2226.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1094 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0004_auto_20161210_1408.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      710 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0005_auto_20161221_2135.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3687 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0006_auto_20170106_2118.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1656 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0007_auto_20170302_2220.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6350 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0008_auto_20171115_1601.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1044 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0009_auto_20171119_1032.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      798 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0010_auto_20171124_1120.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2076 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0011_auto_20171128_1054.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      370 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0012_auto_20171128_2153.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      248 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0013_delete_holiday.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1193 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0014_auto_20180116_1411.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      513 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0015_auto_20180706_1519.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      495 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0016_auto_20181108_0353.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      679 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0017_auto_20190201_0446.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3583 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0018_auto_20190305_0123.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      680 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0019_auto_20190627_2257.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      575 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0020_auto_20190922_0439.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      601 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0021_auto_20191024_1000.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      696 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0022_auto_20200729_2310.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2852 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0023_auto_20200821_2119.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      553 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0024_auto_20200911_0425.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1300 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0025_auto_20210624_0225.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4159 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0026_auto_20220501_1548.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1290 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0027_appointment_document_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0028_appointment_document_status_comments_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      655 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0029_appointment_ignore_window_period_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2881 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0030_alter_appointment_appt_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      818 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0031_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      826 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0032_alter_appointment_unique_together.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2463 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0033_alter_appointment_appt_reason_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4224 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0034_appointmenttype_alter_appointment_appt_type_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      939 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0035_rename_appointment_appt_type.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1235 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0036_auto_20230124_1822.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      472 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/migrations/0037_remove_appointment_appt_type_old_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      770 2023-07-10 03:30:01.000000 edc-appointment-0.4.9/edc_appointment/migrations/0038_alter_appointment_options.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      424 2023-08-03 05:09:25.000000 edc-appointment-0.4.9/edc_appointment/migrations/0039_appointmenttype_extra_value.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1032 2023-08-22 03:04:53.000000 edc-appointment-0.4.9/edc_appointment/migrations/0040_appointment_appt_type_other_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2626 2023-08-22 03:04:53.000000 edc-appointment-0.4.9/edc_appointment/migrations/0041_alter_appointment_appt_reason_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2817 2023-08-23 01:29:06.000000 edc-appointment-0.4.9/edc_appointment/migrations/0042_alter_appointment_device_created_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3217 2023-09-22 02:23:07.000000 edc-appointment-0.4.9/edc_appointment/migrations/0043_alter_appointment_appt_status_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1522 2023-09-25 23:04:21.000000 edc-appointment-0.4.9/edc_appointment/migrations/0044_alter_appointment_appt_reason_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1986 2023-09-27 03:22:15.000000 edc-appointment-0.4.9/edc_appointment/migrations/0045_alter_appointment_appt_reason_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2991 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/migrations/0046_infosources.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8910 2023-12-05 02:41:28.000000 edc-appointment-0.4.9/edc_appointment/migrations/0047_alter_appointment_options_and_more.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.521046 edc-appointment-0.4.9/edc_appointment/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      457 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2824 2023-10-05 13:40:41.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_fields_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6506 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_methods_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7822 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1783 2022-10-26 02:01:25.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/missed_appointment_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1858 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/next_appointment_crf_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1304 2022-10-25 03:04:52.000000 edc-appointment-0.4.9/edc_appointment/model_mixins/window_period_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.521470 edc-appointment-0.4.9/edc_appointment/modeladmin_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       85 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/modeladmin_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1948 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/modeladmin_mixins/next_appointment_crf_modeladmin_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.522105 edc-appointment-0.4.9/edc_appointment/modelform_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)      158 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/modelform_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6008 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/edc_appointment/modelform_mixins/next_appointment_crf_modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1308 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/modelform_mixins/previous_appointment_form_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.522938 edc-appointment-0.4.9/edc_appointment/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)      372 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      935 2024-01-06 03:42:20.000000 edc-appointment-0.4.9/edc_appointment/models/appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      224 2023-12-05 02:41:28.000000 edc-appointment-0.4.9/edc_appointment/models/appointment_type.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      285 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment/models/list_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6960 2023-10-05 13:40:41.000000 edc-appointment-0.4.9/edc_appointment/models/signals.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      132 2020-03-04 23:12:12.000000 edc-appointment-0.4.9/edc_appointment/offline_models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12476 2023-12-05 02:41:28.000000 edc-appointment-0.4.9/edc_appointment/skip_appointments.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1306 2023-10-09 15:41:40.000000 edc-appointment-0.4.9/edc_appointment/stubs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      428 2022-08-25 03:20:20.000000 edc-appointment-0.4.9/edc_appointment/system_checks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.523131 edc-appointment-0.4.9/edc_appointment/templates/
+-rw-r--r--   0 erikvw     (501) staff       (20)      451 2022-07-18 12:12:49.000000 edc-appointment-0.4.9/edc_appointment/templates/button.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.523477 edc-appointment-0.4.9/edc_appointment/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3780 2023-07-02 20:11:24.000000 edc-appointment-0.4.9/edc_appointment/templatetags/appointment_tags.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.524829 edc-appointment-0.4.9/edc_appointment/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      236 2023-08-01 04:05:04.000000 edc-appointment-0.4.9/edc_appointment/tests/appointment_test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.526273 edc-appointment-0.4.9/edc_appointment/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     3400 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/helper.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      524 2020-10-04 12:36:31.000000 edc-appointment-0.4.9/edc_appointment/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)       59 2020-03-04 23:12:11.000000 edc-appointment-0.4.9/edc_appointment/tests/no_holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     2702 2023-10-05 13:40:41.000000 edc-appointment-0.4.9/edc_appointment/tests/test_case_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.529382 edc-appointment-0.4.9/edc_appointment/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-03-01 04:24:07.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5743 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    22425 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8578 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    12042 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment_creator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3250 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment_creator2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    32282 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment_form_validator.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10739 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_datetimes.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9732 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_sequence.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    11897 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_status.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      455 2023-08-01 04:05:04.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6914 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_delete_appointment.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    10032 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_next_appointment_crf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    26902 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_skipped_appt.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    14657 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_unscheduled.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    18990 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_window_period.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     6457 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/tests/tests/test_window_period2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      992 2023-10-31 02:29:07.000000 edc-appointment-0.4.9/edc_appointment/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-05-31 16:24:50.000000 edc-appointment-0.4.9/edc_appointment/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    21958 2023-12-05 02:41:28.000000 edc-appointment-0.4.9/edc_appointment/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.529833 edc-appointment-0.4.9/edc_appointment/view_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       57 2020-03-04 23:12:12.000000 edc-appointment-0.4.9/edc_appointment/view_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4590 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/view_mixins/appointment_view_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.530727 edc-appointment-0.4.9/edc_appointment/views/
+-rw-r--r--   0 erikvw     (501) staff       (20)      101 2020-03-04 23:12:12.000000 edc-appointment-0.4.9/edc_appointment/views/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      286 2023-05-24 16:42:58.000000 edc-appointment-0.4.9/edc_appointment/views/home_view.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2921 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment/views/unscheduled_appointment_view.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.533277 edc-appointment-0.4.9/edc_appointment.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     9365 2024-01-24 05:30:45.000000 edc-appointment-0.4.9/edc_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     8479 2024-01-24 05:30:45.000000 edc-appointment-0.4.9/edc_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2024-01-24 05:30:45.000000 edc-appointment-0.4.9/edc_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-01 22:36:23.000000 edc-appointment-0.4.9/edc_appointment.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2024-01-24 05:30:45.000000 edc-appointment-0.4.9/edc_appointment.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       36 2024-01-24 05:30:45.000000 edc-appointment-0.4.9/edc_appointment.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.531716 edc-appointment-0.4.9/edc_appointment_app/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 14:10:52.000000 edc-appointment-0.4.9/edc_appointment_app/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      122 2022-05-25 14:10:52.000000 edc-appointment-0.4.9/edc_appointment_app/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      488 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/consents.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1251 2023-10-06 00:11:33.000000 edc-appointment-0.4.9/edc_appointment_app/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     7902 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1438 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/edc_appointment_app/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2024-01-24 05:30:45.533064 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/
+-rw-r--r--   0 erikvw     (501) staff       (20)      471 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1954 2023-11-16 03:53:38.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/crfs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1682 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule1.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1545 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule2.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1955 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule3.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2111 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule4.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2248 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule5.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2549 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule6.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1724 2023-12-13 19:33:50.000000 edc-appointment-0.4.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2902 2024-01-24 05:30:35.000000 edc-appointment-0.4.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1171 2024-01-24 05:30:45.534138 edc-appointment-0.4.9/setup.cfg
```

### Comparing `edc-appointment-0.4.8/.github/workflows/build.yml` & `edc-appointment-0.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/.gitignore` & `edc-appointment-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/.pre-commit-config.yaml` & `edc-appointment-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/CHANGES` & `edc-appointment-0.4.9/CHANGES`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/LICENSE` & `edc-appointment-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/PKG-INFO` & `edc-appointment-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-appointment
-Version: 0.4.8
+Version: 0.4.9
 Summary: Appointment module for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django appointments data collection clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-appointment-0.4.8/README.rst` & `edc-appointment-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/admin/actions.py` & `edc-appointment-0.4.9/edc_appointment/admin/actions.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/admin/appointment_admin.py` & `edc-appointment-0.4.9/edc_appointment/admin/appointment_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from django.utils.translation import gettext as _
 from django_audit_fields.admin import audit_fieldset_tuple
 from edc_constants.constants import NOT_APPLICABLE
 from edc_document_status.fieldsets import document_status_fieldset_tuple
 from edc_document_status.modeladmin_mixins import DocumentStatusModelAdminMixin
 from edc_model_admin.dashboard import ModelAdminSubjectDashboardMixin
 from edc_model_admin.history import SimpleHistoryAdmin
-from edc_sites.admin import SiteModelAdminMixin
+from edc_sites.admin import SiteModelAdminMixin, site_fieldset_tuple
 from edc_visit_schedule.exceptions import OnScheduleError
 from edc_visit_schedule.fieldsets import (
     visit_schedule_fields,
     visit_schedule_fieldset_tuple,
 )
 from edc_visit_schedule.utils import off_schedule_or_raise
 
@@ -56,14 +56,15 @@
         "timing",
         "schedule_name",
     )
     list_filter = (
         AppointmentListFilter,
         "appt_status",
         "visit_code",
+        "visit_code_sequence",
         "appt_type",
         "appt_timing",
     )
 
     additional_instructions = format_html(
         "To start or continue to edit FORMS for this subject, change the "
         'appointment status below to "In Progress" and click SAVE. <BR>'
@@ -101,14 +102,15 @@
                         "facility_name",
                     ),
                 }
             ),
         ),
         document_status_fieldset_tuple,
         visit_schedule_fieldset_tuple,
+        site_fieldset_tuple,
         audit_fieldset_tuple,
     )
 
     radio_fields = {
         "appt_type": admin.VERTICAL,
         "appt_status": admin.VERTICAL,
         "appt_reason": admin.VERTICAL,
```

### Comparing `edc-appointment-0.4.8/edc_appointment/appointment_reason_updater.py` & `edc-appointment-0.4.9/edc_appointment/appointment_reason_updater.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/appointment_status_updater.py` & `edc-appointment-0.4.9/edc_appointment/appointment_status_updater.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/apps.py` & `edc-appointment-0.4.9/edc_appointment/apps.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/auths.py` & `edc-appointment-0.4.9/edc_appointment/auths.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/choices.py` & `edc-appointment-0.4.9/edc_appointment/choices.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/constants.py` & `edc-appointment-0.4.9/edc_appointment/constants.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/creators/appointment_creator.py` & `edc-appointment-0.4.9/edc_appointment/creators/appointment_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from django.db.utils import IntegrityError
 from django.utils.timezone import is_naive
 from edc_facility.facility import Facility, FacilityError
 from edc_sites.utils import valid_site_for_subject_or_raise
 from edc_visit_schedule.utils import is_baseline
 
 from ..constants import SCHEDULED_APPT
+from ..exceptions import AppointmentCreatorError
 from ..utils import (
     get_appointment_type_model_cls,
     get_appt_reason_default,
     get_appt_type_default,
 )
 
 if TYPE_CHECKING:
@@ -28,18 +29,14 @@
     pass
 
 
 class CreateAppointmentDateError(Exception):
     pass
 
 
-class AppointmentCreatorError(Exception):
-    pass
-
-
 if TYPE_CHECKING:
     from edc_visit_schedule.visit import Visit
 
 
 class AppointmentCreator:
     def __init__(
         self,
@@ -62,21 +59,21 @@
         ignore_window_period: bool | None = None,
         skip_get_current_site: bool | None = None,
     ):
         self._appointment = None
         self._appointment_model_cls = None
         self._default_appt_type = default_appt_type
         self._default_appt_reason = default_appt_reason
-        self.skip_baseline = skip_baseline
-        self.subject_identifier = subject_identifier
+        self.skip_baseline: bool | None = skip_baseline
+        self.subject_identifier: str = subject_identifier
         self.visit_schedule_name = visit_schedule_name
         self.schedule_name: str = schedule_name
-        self.appt_status = appt_status
-        self.appt_reason = appt_reason
-        self.appointment_model = appointment_model
+        self.appt_status: str = appt_status
+        self.appt_reason: str = appt_reason
+        self.appointment_model: str = appointment_model or "edc_appointment.appointment"
         # already taken appt_datetimes for this subject
         self.taken_datetimes = taken_datetimes or []
         self.visit = visit
         self.visit_code_sequence = visit_code_sequence or 0
         self.timepoint = timepoint or self.visit.timepoint
         self.site = valid_site_for_subject_or_raise(
             self.subject_identifier, skip_get_current_site=skip_get_current_site
@@ -211,15 +208,15 @@
         else:
             return self.suggested_datetime
         return arw.datetime
 
     @property
     def appointment_model_cls(self) -> Appointment:
         """Returns the appointment model class."""
-        return django_apps.get_model("edc_appointment.appointment")
+        return django_apps.get_model(self.appointment_model)
 
     @property
     def default_appt_type(self) -> AppointmentType | None:
         """Returns an AppointmentType instance or None for
         the default appointment type, e.g. 'clinic'.
         """
         if not self._default_appt_type:
```

### Comparing `edc-appointment-0.4.8/edc_appointment/creators/appointments_creator.py` & `edc-appointment-0.4.9/edc_appointment/creators/appointments_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
     def __init__(
         self,
         subject_identifier: str | None = None,
         visit_schedule: VisitSchedule | None = None,
         schedule: Schedule | None = None,
         report_datetime: datetime | None = None,
-        appointment_model: Appointment = None,
+        appointment_model: str = None,
         skip_baseline: bool | None = None,
     ):
-        self.subject_identifier = subject_identifier
-        self.visit_schedule = visit_schedule
-        self.schedule = schedule
-        self.report_datetime = report_datetime
-        self.appointment_model = appointment_model
-        self.skip_baseline = skip_baseline
+        self.subject_identifier: str = subject_identifier
+        self.visit_schedule: VisitSchedule = visit_schedule
+        self.schedule: Schedule = schedule
+        self.report_datetime: datetime = report_datetime
+        self.appointment_model: str = appointment_model
+        self.skip_baseline: bool | None = skip_baseline
 
     def create_appointments(
         self, base_appt_datetime=None, taken_datetimes=None
     ) -> list[Appointment]:
         """Creates appointments when called by post_save signal.
 
         Timepoint datetimes are adjusted according to the available
```

### Comparing `edc-appointment-0.4.8/edc_appointment/creators/unscheduled_appointment_creator.py` & `edc-appointment-0.4.9/edc_appointment/creators/unscheduled_appointment_creator.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,49 +14,32 @@
 from ..constants import (
     COMPLETE_APPT,
     IN_PROGRESS_APPT,
     INCOMPLETE_APPT,
     NEW_APPT,
     UNSCHEDULED_APPT,
 )
-from ..exceptions import AppointmentPermissionsRequired, AppointmentWindowError
+from ..exceptions import (
+    AppointmentInProgressError,
+    AppointmentPermissionsRequired,
+    AppointmentWindowError,
+    InvalidParentAppointmentMissingVisitError,
+    InvalidParentAppointmentStatusError,
+    InvalidVisitCodeSequencesError,
+    UnscheduledAppointmentError,
+    UnscheduledAppointmentNotAllowed,
+)
 from .appointment_creator import AppointmentCreator, CreateAppointmentError
 
 if TYPE_CHECKING:
     from edc_facility import Facility
 
     from ..models import Appointment
 
-
-class UnscheduledAppointmentError(Exception):
-    pass
-
-
-class UnscheduledAppointmentNotAllowed(Exception):
-    pass
-
-
-class InvalidVisitCodeSequencesError(Exception):
-    pass
-
-
-class InvalidTimepointError(Exception):
-    pass
-
-
-class InvalidParentAppointmentStatusError(Exception):
-    pass
-
-
-class InvalidParentAppointmentMissingVisitError(Exception):
-    pass
-
-
-class AppointmentInProgressError(Exception):
-    pass
+__all__ = ["UnscheduledAppointmentCreator"]
 
 
 class UnscheduledAppointmentCreator:
 
     """Attempts to create a new unscheduled appointment where the
     visit code sequence == the given `visit_code_sequence` or raises.
     """
```

### Comparing `edc-appointment-0.4.8/edc_appointment/creators/utils.py` & `edc-appointment-0.4.9/edc_appointment/creators/utils.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/exceptions.py` & `edc-appointment-0.4.9/edc_appointment/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -40,7 +40,35 @@
 
 class AppointmentPermissionsRequired(Exception):
     pass
 
 
 class AppointmentMissingValuesError(Exception):
     pass
+
+
+class UnscheduledAppointmentNotAllowed(Exception):
+    pass
+
+
+class InvalidVisitCodeSequencesError(Exception):
+    pass
+
+
+class InvalidTimepointError(Exception):
+    pass
+
+
+class InvalidParentAppointmentStatusError(Exception):
+    pass
+
+
+class InvalidParentAppointmentMissingVisitError(Exception):
+    pass
+
+
+class AppointmentInProgressError(Exception):
+    pass
+
+
+class AppointmentCreatorError(Exception):
+    pass
```

### Comparing `edc-appointment-0.4.8/edc_appointment/form_validator_mixins/next_appointment_crf_form_validator_mixin.py` & `edc-appointment-0.4.9/edc_appointment/form_validator_mixins/next_appointment_crf_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/form_validator_mixins/window_period_form_validator_mixin.py` & `edc-appointment-0.4.9/edc_appointment/form_validator_mixins/window_period_form_validator_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/form_validators/appointment_form_validator.py` & `edc-appointment-0.4.9/edc_appointment/form_validators/appointment_form_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import TYPE_CHECKING, Any
 
 from django.apps import apps as django_apps
 from django.conf import settings
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
+from edc_consent import ConsentDefinitionDoesNotExist
 from edc_consent.utils import consent_datetime_or_raise
 from edc_facility.utils import get_facilities
 from edc_form_validators import INVALID_ERROR
 from edc_form_validators.form_validator import FormValidator
 from edc_metadata.metadata_helper import MetadataHelperMixin
 from edc_utils import formatted_datetime, get_utcnow, to_utc
 from edc_utils.date import to_local
@@ -207,15 +208,17 @@
                 "Skipping consent_datetime form validation. "
                 "`edc_consent` not in `INSTALLED_APPS`"
             )
         else:
             appt_datetime = self.cleaned_data.get("appt_datetime")
             appt_status = self.cleaned_data.get("appt_status")
             if appt_datetime and appt_status != NEW_APPT:
-                consent_datetime = self.get_consent_datetime_or_raise(to_utc(appt_datetime))
+                consent_datetime = self.get_consent_datetime_or_raise(
+                    appt_datetime=to_utc(appt_datetime)
+                )
                 if to_utc(appt_datetime).date() < consent_datetime.date():
                     formatted_date = formatted_datetime(
                         to_local(consent_datetime), format_as_date=True
                     )
                     self.raise_validation_error(
                         {
                             "appt_datetime": (
@@ -539,19 +542,24 @@
             f"{url}?q={self.instance.subject_identifier}"
             f"&visit_code={self.instance.visit_code}"
             f"&visit_code_sequence={self.instance.visit_code_sequence}"
         )
         return url
 
     def get_consent_datetime_or_raise(self: Any, appt_datetime: datetime) -> datetime:
-        return consent_datetime_or_raise(
-            report_datetime=appt_datetime,
-            model_obj=self.instance,
-            raise_validation_error=self.raise_validation_error,
-        )
+        consent_datetime = None
+        try:
+            consent_datetime = consent_datetime_or_raise(
+                report_datetime=appt_datetime,
+                appointment=self.instance,
+                raise_validation_error=self.raise_validation_error,
+            )
+        except ConsentDefinitionDoesNotExist as e:
+            self.raise_validation_error({"appt_datetime": str(e)}, INVALID_APPT_DATE)
+        return consent_datetime
 
     def validate_subject_on_schedule(self: Any) -> None:
         if self.cleaned_data.get("appt_datetime"):
             appt_datetime = self.cleaned_data.get("appt_datetime")
             subject_identifier = self.instance.subject_identifier
             onschedule_model = site_visit_schedules.get_onschedule_model(
                 visit_schedule_name=self.instance.visit_schedule_name,
```

### Comparing `edc-appointment-0.4.8/edc_appointment/form_validators/utils.py` & `edc-appointment-0.4.9/edc_appointment/form_validators/utils.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/forms/appointment_form.py` & `edc-appointment-0.4.9/edc_appointment/forms/appointment_form.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/list_data.py` & `edc-appointment-0.4.9/edc_appointment/list_data.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/management/commands/close_appointments.py` & `edc-appointment-0.4.9/edc_appointment/management/commands/close_appointments.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/management/commands/update_appointment_status.py` & `edc-appointment-0.4.9/edc_appointment/management/commands/update_appointment_status.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/management/commands/update_skipped_appointments.py` & `edc-appointment-0.4.9/edc_appointment/management/commands/update_skipped_appointments.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/managers.py` & `edc-appointment-0.4.9/edc_appointment/managers.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0001_initial.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0002_auto_20161126_1156.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0002_auto_20161126_1156.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0003_auto_20161127_2226.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0003_auto_20161127_2226.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0004_auto_20161210_1408.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0004_auto_20161210_1408.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0005_auto_20161221_2135.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0005_auto_20161221_2135.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0006_auto_20170106_2118.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0006_auto_20170106_2118.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0007_auto_20170302_2220.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0007_auto_20170302_2220.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0008_auto_20171115_1601.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0008_auto_20171115_1601.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0009_auto_20171119_1032.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0009_auto_20171119_1032.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0010_auto_20171124_1120.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0010_auto_20171124_1120.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0011_auto_20171128_1054.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0011_auto_20171128_1054.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0014_auto_20180116_1411.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0014_auto_20180116_1411.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0015_auto_20180706_1519.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0015_auto_20180706_1519.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0017_auto_20190201_0446.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0017_auto_20190201_0446.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0018_auto_20190305_0123.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0018_auto_20190305_0123.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0019_auto_20190627_2257.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0019_auto_20190627_2257.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0020_auto_20190922_0439.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0020_auto_20190922_0439.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0021_auto_20191024_1000.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0021_auto_20191024_1000.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0022_auto_20200729_2310.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0022_auto_20200729_2310.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0023_auto_20200821_2119.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0023_auto_20200821_2119.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0024_auto_20200911_0425.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0024_auto_20200911_0425.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0025_auto_20210624_0225.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0025_auto_20210624_0225.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0026_auto_20220501_1548.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0026_auto_20220501_1548.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0027_appointment_document_status_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0027_appointment_document_status_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0028_appointment_document_status_comments_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0028_appointment_document_status_comments_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0029_appointment_ignore_window_period_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0029_appointment_ignore_window_period_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0030_alter_appointment_appt_status_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0030_alter_appointment_appt_status_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0031_auto_20220704_1841.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0031_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0032_alter_appointment_unique_together.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0032_alter_appointment_unique_together.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0033_alter_appointment_appt_reason_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0033_alter_appointment_appt_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0034_appointmenttype_alter_appointment_appt_type_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0034_appointmenttype_alter_appointment_appt_type_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0035_rename_appointment_appt_type.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0035_rename_appointment_appt_type.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0036_auto_20230124_1822.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0036_auto_20230124_1822.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0038_alter_appointment_options.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0038_alter_appointment_options.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0040_appointment_appt_type_other_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0040_appointment_appt_type_other_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0041_alter_appointment_appt_reason_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0041_alter_appointment_appt_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0042_alter_appointment_device_created_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0042_alter_appointment_device_created_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0043_alter_appointment_appt_status_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0043_alter_appointment_appt_status_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0044_alter_appointment_appt_reason_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0044_alter_appointment_appt_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0045_alter_appointment_appt_reason_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0045_alter_appointment_appt_reason_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0046_infosources.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0046_infosources.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/migrations/0047_alter_appointment_options_and_more.py` & `edc-appointment-0.4.9/edc_appointment/migrations/0047_alter_appointment_options_and_more.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_fields_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_fields_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_methods_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_methods_model_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING, Type, TypeVar
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from edc_facility.facility import Facility
 from edc_facility.utils import get_facility
 from edc_visit_tracking.model_mixins import get_related_visit_model_attr
 
@@ -44,15 +44,15 @@
 
     @classmethod
     def related_visit_model_attr(cls: Appointment) -> str:
         """Returns the reversed related visit attr"""
         return get_related_visit_model_attr(cls)
 
     @classmethod
-    def related_visit_model_cls(cls: Appointment) -> VisitModel:
+    def related_visit_model_cls(cls: Appointment) -> Type[VisitModel]:
         return getattr(cls, cls.related_visit_model_attr()).related.related_model
 
     @property
     def next_by_timepoint(self: Appointment) -> Appointment | None:
         """Returns the next appointment or None of all appointments
         for this subject for visit_code_sequence=0.
         """
```

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/appointment_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/appointment_model_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from ..utils import raise_on_appt_may_not_be_missed, update_appt_status
 from .appointment_fields_model_mixin import AppointmentFieldsModelMixin
 from .appointment_methods_model_mixin import AppointmentMethodsModelMixin
 from .missed_appointment_model_mixin import MissedAppointmentModelMixin
 from .window_period_model_mixin import WindowPeriodModelMixin
 
 if TYPE_CHECKING:
+    from edc_visit_schedule.schedule import Schedule
+
     from ..models import Appointment
 
 
 class AppointmentModelMixin(
     NonUniqueSubjectIdentifierFieldMixin,
     AppointmentFieldsModelMixin,
     AppointmentMethodsModelMixin,
@@ -66,15 +68,15 @@
 
     def save(self: Appointment, *args, **kwargs):
         if not kwargs.get("update_fields", None):
             if self.id and is_baseline(instance=self):
                 visit_schedule = site_visit_schedules.get_visit_schedule(
                     self.visit_schedule_name
                 )
-                schedule = visit_schedule.schedules.get(self.schedule_name)
+                schedule: Schedule = visit_schedule.schedules.get(self.schedule_name)
                 try:
                     onschedule_obj = django_apps.get_model(
                         schedule.onschedule_model
                     ).objects.get(
                         subject_identifier=self.subject_identifier,
                         onschedule_datetime__lte=to_utc(self.appt_datetime)
                         + relativedelta(seconds=1),
```

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/missed_appointment_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/missed_appointment_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/next_appointment_crf_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/next_appointment_crf_model_mixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 from django.db import models
 from django.db.models import PROTECT
 from django.utils.translation import gettext_lazy as _
 from edc_facility.utils import get_health_facility_model
-from edc_visit_schedule.models import VisitSchedule
 
 
 class NextAppointmentCrfModelMixin(models.Model):
     health_facility = models.ForeignKey(
         get_health_facility_model(),
         on_delete=PROTECT,
         null=True,
@@ -30,15 +29,15 @@
         null=True,
         blank=False,
     )
 
     # named this way to not conflict with property `visit_schedule`
     # see also edc-crf
     visitschedule = models.ForeignKey(
-        VisitSchedule,
+        "edc_visit_schedule.VisitSchedule",
         on_delete=PROTECT,
         verbose_name=_("Which study visit code is closest to this appointment date"),
         max_length=15,
         null=True,
         blank=False,
         help_text=_(
             "Click SAVE to let the EDC suggest. Once selected, interim appointments will "
```

### Comparing `edc-appointment-0.4.8/edc_appointment/model_mixins/window_period_model_mixin.py` & `edc-appointment-0.4.9/edc_appointment/model_mixins/window_period_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/modeladmin_mixins/next_appointment_crf_modeladmin_mixin.py` & `edc-appointment-0.4.9/edc_appointment/modeladmin_mixins/next_appointment_crf_modeladmin_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/modelform_mixins/next_appointment_crf_modelform_mixins.py` & `edc-appointment-0.4.9/edc_appointment/modelform_mixins/next_appointment_crf_modelform_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/modelform_mixins/previous_appointment_form_mixin.py` & `edc-appointment-0.4.9/edc_appointment/modelform_mixins/previous_appointment_form_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/models/appointment.py` & `edc-appointment-0.4.9/edc_appointment/models/appointment.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/models/signals.py` & `edc-appointment-0.4.9/edc_appointment/models/signals.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/skip_appointments.py` & `edc-appointment-0.4.9/edc_appointment/skip_appointments.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/stubs.py` & `edc-appointment-0.4.9/edc_appointment/stubs.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/templatetags/appointment_tags.py` & `edc-appointment-0.4.9/edc_appointment/templatetags/appointment_tags.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-local-private.pem` & `edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/etc/user-rsa-restricted-private.pem` & `edc-appointment-0.4.9/edc_appointment/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/helper.py` & `edc-appointment-0.4.9/edc_appointment/tests/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from datetime import datetime
 from typing import TYPE_CHECKING
 from uuid import uuid4
 
 from dateutil.relativedelta import relativedelta
 from django.apps import apps as django_apps
 from django.conf import settings
-from edc_consent import ConsentDefinitionDoesNotExist, site_consents
+from edc_consent.consent_definition import ConsentDefinition
+from edc_registration.models import RegisteredSubject
+from edc_sites import site_sites
 from edc_utils import get_utcnow
+from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 
 from edc_appointment.creators import UnscheduledAppointmentCreator
 
 if TYPE_CHECKING:
     from edc_appointment.models import Appointment
 
@@ -29,55 +32,47 @@
         Defaults to edc_appointment.subjectscreening
         """
         try:
             return django_apps.get_model(settings.SUBJECT_SCREENING_MODEL)
         except LookupError:
             return django_apps.get_model("edc_appointment_app.subjectscreening")
 
-    @property
-    def consent_model_cls(self):
-        """Returns a consent model class.
-
-        Defaults to edc_appointment.subjectconsent
-        """
-        try:
-            cdef = site_consents.get_consent_definition(model=settings.SUBJECT_CONSENT_MODEL)
-        except ConsentDefinitionDoesNotExist:
-            cdef = site_consents.get_consent_definition(
-                model="edc_appointment_app.subjectconsent"
-            )
-        return cdef.model_cls
-
     def consent_and_put_on_schedule(
         self,
-        subject_identifier=None,
-        visit_schedule_name=None,
-        schedule_name=None,
-        age_in_years=None,
+        visit_schedule_name: str = None,
+        schedule_name: str = None,
+        age_in_years: int | None = None,
         report_datetime: datetime | None = None,
+        onschedule_datetime: datetime | None = None,
+        consent_definition: ConsentDefinition | None = None,
     ):
-        subject_identifier = subject_identifier or self.subject_identifier
-        self.screening_model_cls.objects.create(
-            subject_identifier=subject_identifier,
+        report_datetime = report_datetime or self.now
+        RegisteredSubject.objects.filter(subject_identifier=self.subject_identifier).delete()
+        subject_screening = self.screening_model_cls.objects.create(
+            subject_identifier=self.subject_identifier,
             report_datetime=report_datetime or self.now,
             screening_identifier=uuid4(),
             age_in_years=age_in_years or 25,
         )
-        subject_consent = self.consent_model_cls.objects.create(
-            subject_identifier=subject_identifier,
+        schedule: Schedule = site_visit_schedules.get_visit_schedule(
+            visit_schedule_name
+        ).schedules.get(schedule_name)
+
+        cdef = consent_definition or schedule.get_consent_definition(
+            report_datetime=report_datetime, site=site_sites.get(subject_screening.site.id)
+        )
+        subject_consent = cdef.model_cls.objects.create(
+            subject_identifier=self.subject_identifier,
             consent_datetime=report_datetime or self.now,
             dob=self.now - relativedelta(years=age_in_years or 25),
         )
-        visit_schedule = site_visit_schedules.get_visit_schedule(
-            visit_schedule_name or "visit_schedule1"
-        )
-        schedule = visit_schedule.schedules.get(schedule_name or "schedule1")
+        visit_schedule = site_visit_schedules.get_visit_schedule(visit_schedule_name)
+        schedule = visit_schedule.schedules.get(schedule_name)
         schedule.put_on_schedule(
-            subject_identifier=subject_consent.subject_identifier,
-            onschedule_datetime=subject_consent.consent_datetime,
+            self.subject_identifier, onschedule_datetime or subject_consent.consent_datetime
         )
         return subject_consent
 
     @staticmethod
     def add_unscheduled_appointment(appointment: Appointment | None = None):
         creator = UnscheduledAppointmentCreator(
             subject_identifier=appointment.subject_identifier,
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/holidays.csv` & `edc-appointment-0.4.9/edc_appointment/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/test_case_mixins.py` & `edc-appointment-0.4.9/edc_appointment/tests/test_case_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_admin.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import re
 from unittest.mock import patch
 
 from django.test import override_settings
 from django.urls import reverse
 from django_webtest import WebTest
 from edc_auth.auth_updater.group_updater import GroupUpdater, PermissionsCodenameError
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility import import_holidays
 from edc_protocol import Protocol
 from edc_test_utils.get_user_for_tests import get_user_for_tests
 from edc_test_utils.webtest import login
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 from edc_visit_tracking.utils import get_related_visit_model_cls
 
 from edc_appointment.admin import AppointmentAdmin
 from edc_appointment.auth_objects import codenames
 from edc_appointment.constants import NEW_APPT
 from edc_appointment.tests.helper import Helper
 from edc_appointment.utils import get_appointment_model_cls
-from edc_appointment_app.consents import v1_consent
-from edc_appointment_app.visit_schedule import visit_schedule1
+from edc_appointment_app.consents import consent_v1
+from edc_appointment_app.visit_schedule import get_visit_schedule1
 
 
 def get_url_name():
     return "subject_dashboard_url"
 
 
 @override_settings(SITE_ID=10)
@@ -37,18 +37,19 @@
         import_holidays()
 
     def setUp(self) -> None:
         super().setUp()
         self.user = get_user_for_tests(view_only=True)
 
         self.subject_identifier = "12345"
+        self.visit_schedule1 = get_visit_schedule1()
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule1)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=Protocol().study_open_datetime,
         )
 
     def get_app_form(self, url_name=None, response=None):
         form = None
@@ -71,15 +72,18 @@
 
     @patch.object(
         AppointmentAdmin,
         "get_subject_dashboard_url_name",
         side_effect=get_url_name,
     )
     def test_admin_ok(self, mock_get_subject_dashboard_url_name):
-        subject_consent = self.helper.consent_and_put_on_schedule()
+        schedule_name = "schedule1"
+        subject_consent = self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = (
             get_appointment_model_cls()
             .objects.all()
             .order_by("timepoint", "visit_code_sequence")
         )
         # there are 4 appts
         self.assertEqual(appointments.count(), 4)
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,95 @@
+from __future__ import annotations
+
 from datetime import datetime
-from decimal import Context
+from typing import TYPE_CHECKING
 from zoneinfo import ZoneInfo
 
 import time_machine
-from dateutil.relativedelta import FR, MO, SA, SU, TH, TU, WE, relativedelta
-from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import transaction
 from django.db.models.deletion import ProtectedError
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_constants.constants import INCOMPLETE
 from edc_facility.import_holidays import import_holidays
 from edc_protocol import Protocol
 from edc_utils import get_utcnow
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
-from edc_visit_tracking.constants import MISSED_VISIT, SCHEDULED, UNSCHEDULED
+from edc_visit_tracking.constants import MISSED_VISIT, SCHEDULED
 from edc_visit_tracking.exceptions import RelatedVisitReasonError
 from edc_visit_tracking.utils import get_related_visit_model_cls
 
 from edc_appointment.constants import (
     IN_PROGRESS_APPT,
     INCOMPLETE_APPT,
     MISSED_APPT,
     ONTIME_APPT,
-    SCHEDULED_APPT,
-    UNSCHEDULED_APPT,
-)
-from edc_appointment.exceptions import (
-    AppointmentBaselineError,
-    AppointmentDatetimeError,
 )
+from edc_appointment.exceptions import AppointmentBaselineError
 from edc_appointment.managers import AppointmentDeleteError
-from edc_appointment.utils import get_appointment_model_cls, get_appt_reason_choices
-from edc_appointment_app.consents import v1_consent
+from edc_appointment.utils import get_appointment_model_cls
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import OnScheduleOne, OnScheduleTwo, SubjectConsent
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 
+if TYPE_CHECKING:
+    from edc_visit_schedule.schedule import Schedule
+
+
 utc_tz = ZoneInfo("UTC")
 
 
-@override_settings(SITE_ID=10)
+@override_settings(SITE_ID=10, EDC_SITES_REGISTER_DEFAULT=True)
 @time_machine.travel(datetime(2019, 6, 11, 8, 00, tzinfo=utc_tz))
 class TestAppointment(TestCase):
     helper_cls = Helper
 
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        self.visit_schedule1 = get_visit_schedule1()
+        self.schedule1: Schedule = self.visit_schedule1.schedules.get("schedule1")
+        self.visit_schedule2 = get_visit_schedule2()
+        site_visit_schedules.register(self.visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=Protocol().study_open_datetime,
         )
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
 
     def test_appointments_creation(self):
         """Assert appointment triggering method creates appointments."""
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
 
     def test_appointments_creation2(self):
         """Asserts first appointment correctly selected if
         both visit_schedule_name and schedule_name provided.
         """
-        self.helper.consent_and_put_on_schedule()
         OnScheduleTwo.objects.create(
             subject_identifier=self.subject_identifier, onschedule_datetime=get_utcnow()
         )
         self.assertEqual(get_appointment_model_cls().objects.all().count(), 8)
 
     def test_deletes_appointments(self):
         """Asserts manager method can delete appointments."""
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
 
         get_related_visit_model_cls().objects.create(
             appointment=appointments[0],
@@ -110,15 +113,14 @@
             .objects.filter(subject_identifier=self.subject_identifier)
             .count(),
             1,
         )
 
     def test_deletes_appointments_with_unscheduled(self):
         """Asserts manager method can delete appointments."""
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
 
         appointment = appointments[0]
 
@@ -138,28 +140,24 @@
 
         visit_schedule = site_visit_schedules.get_visit_schedule(
             visit_schedule_name=appointment.visit_schedule_name
         )
         schedule = visit_schedule.schedules.get(appointment.schedule_name)
 
         # this calls the manager method "delete_for_subject_after_date"
-        schedule.take_off_schedule(
-            subject_identifier=self.subject_identifier,
-            offschedule_datetime=appointment.appt_datetime,
-        )
+        schedule.take_off_schedule(self.subject_identifier, appointment.appt_datetime)
 
         self.assertEqual(
             get_appointment_model_cls()
             .objects.filter(subject_identifier=self.subject_identifier)
             .count(),
             1,
         )
 
     def test_delete_single_appointment(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
 
         get_related_visit_model_cls().objects.create(
             appointment=appointments[0],
@@ -189,194 +187,61 @@
         unscheduled_appointment = get_appointment_model_cls().objects.get(
             visit_code="1000", visit_code_sequence=1
         )
 
         unscheduled_appointment.delete()
         self.assertEqual(appointments.count(), 4)
 
-    def test_appointments_dates_mo(self):
-        """Test appointment datetimes are chronological."""
-        for index in range(0, 7):
-            SubjectConsent.objects.create(
-                subject_identifier=f"{self.subject_identifier}-{index}",
-                consent_datetime=get_utcnow(),
-            )
-        for day in [MO, TU, WE, TH, FR, SA, SU]:
-            subject_consent = SubjectConsent.objects.all()[day.weekday]
-            OnScheduleOne.objects.create(
-                subject_identifier=subject_consent.subject_identifier,
-                onschedule_datetime=(
-                    subject_consent.consent_datetime
-                    + relativedelta(weeks=2)
-                    + relativedelta(weekday=day(-1))
-                ),
-            )
-            appt_datetimes = [
-                obj.appt_datetime
-                for obj in get_appointment_model_cls()
-                .objects.filter(subject_identifier=subject_consent.subject_identifier)
-                .order_by("appt_datetime")
-            ]
-            last = None
-            self.assertGreater(len(appt_datetimes), 0)
-            for appt_datetime in appt_datetimes:
-                if not last:
-                    last = appt_datetime
-                else:
-                    self.assertGreater(appt_datetime, last)
-                    last = appt_datetime
-
-    def test_attempt_to_change(self):
-        for index in range(0, 7):
-            SubjectConsent.objects.create(
-                subject_identifier=f"{self.subject_identifier}-{index}",
-                consent_datetime=get_utcnow(),
-            )
-        for day in [MO, TU, WE, TH, FR, SA, SU]:
-            subject_consent = SubjectConsent.objects.all()[day.weekday]
-            OnScheduleOne.objects.create(
-                subject_identifier=subject_consent.subject_identifier,
-                onschedule_datetime=(
-                    subject_consent.consent_datetime
-                    + relativedelta(weeks=2)
-                    + relativedelta(weekday=day(-1))
-                ),
-            )
-        subject_identifier = subject_consent.subject_identifier
-        self.assertEqual(
-            get_appointment_model_cls()
-            .objects.filter(subject_identifier=subject_identifier)
-            .count(),
-            4,
-        )
-
-        # create two unscheduled appts after first
-        appointment0 = (
-            get_appointment_model_cls()
-            .objects.filter(subject_identifier=subject_identifier)
-            .order_by("appt_datetime")[0]
-        )
-        get_related_visit_model_cls().objects.create(
-            appointment=appointment0,
-            report_datetime=appointment0.appt_datetime,
-            reason=SCHEDULED,
-        )
-        appointment0.appt_status = INCOMPLETE_APPT
-        appointment0.save()
-
-        appointment0_1 = self.helper.add_unscheduled_appointment(appointment0)
-        get_related_visit_model_cls().objects.create(
-            appointment=appointment0_1,
-            report_datetime=appointment0.appt_datetime,
-            reason=UNSCHEDULED,
-        )
-        appointment0_1.appt_status = INCOMPLETE_APPT
-        appointment0_1.save()
-
-        appointment0_2 = self.helper.add_unscheduled_appointment(appointment0_1)
-
-        appointment0_1.appt_datetime = appointment0_2.appt_datetime + relativedelta(days=1)
-
-        self.assertRaises(AppointmentDatetimeError, appointment0_1.save)
-
-    def test_timepoint(self):
-        """Assert timepoints are saved from the schedule correctly
-        as Decimals and ordered by appt_datetime.
-        """
-        context = Context(prec=2)
-        self.helper.consent_and_put_on_schedule()
-        self.assertEqual(
-            [
-                obj.timepoint
-                for obj in get_appointment_model_cls().objects.all().order_by("appt_datetime")
-            ],
-            [context.create_decimal(n) for n in range(0, 4)],
-        )
-
     def test_first_appointment_with_visit_schedule_and_schedule(self):
         """Asserts first appointment correctly selected if
         both visit_schedule_name and schedule_name provided.
         """
-        self.helper.consent_and_put_on_schedule()
         subject_consent = SubjectConsent.objects.get(
             subject_identifier=self.subject_identifier
         )
         OnScheduleTwo.objects.create(
             subject_identifier=subject_consent.subject_identifier,
             onschedule_datetime=subject_consent.consent_datetime,
         )
         onschedule_one = OnScheduleOne.objects.get(subject_identifier=self.subject_identifier)
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=onschedule_one.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1,
+            schedule_name=self.schedule1.name,
         )
 
         appointment = (
             get_appointment_model_cls()
             .objects.filter(
                 subject_identifier=onschedule_one.subject_identifier,
-                visit_schedule_name="visit_schedule1",
-                schedule_name="schedule1",
+                visit_schedule_name=self.visit_schedule1.name,
+                schedule_name=self.schedule1.name,
             )
             .order_by("appt_datetime")[0]
         )
 
         self.assertEqual(first_appointment, appointment)
 
-    def test_first_appointment_with_visit_schedule(self):
-        """Asserts first appointment correctly selected if just
-        visit_schedule_name provided.
-        """
-        subject_consent = SubjectConsent.objects.create(
-            subject_identifier=self.subject_identifier, consent_datetime=get_utcnow()
-        )
-        OnScheduleTwo.objects.create(
-            subject_identifier=self.subject_identifier,
-            onschedule_datetime=subject_consent.consent_datetime,
-        )
-        OnScheduleOne.objects.create(
-            subject_identifier=self.subject_identifier,
-            onschedule_datetime=(subject_consent.report_datetime + relativedelta(months=1)),
-        )
-
-        first_appointment = get_appointment_model_cls().objects.first_appointment(
-            subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule2",
-        )
-        self.assertEqual(first_appointment.schedule_name, "schedule2")
-
-        self.assertEqual(
-            get_appointment_model_cls()
-            .objects.filter(
-                subject_identifier=self.subject_identifier,
-                visit_schedule_name="visit_schedule2",
-            )
-            .order_by("appt_datetime")[0],
-            first_appointment,
-        )
-
     def test_first_appointment_with_unscheduled(self):
         """Asserts first appointment correctly selected if
         unscheduled visits have been added.
         """
-        self.helper.consent_and_put_on_schedule()
         subject_consent = SubjectConsent.objects.get(
             subject_identifier=self.subject_identifier
         )
         OnScheduleTwo.objects.create(
             subject_identifier=subject_consent.subject_identifier,
             onschedule_datetime=subject_consent.consent_datetime,
         )
         onschedule_one = OnScheduleOne.objects.get(subject_identifier=self.subject_identifier)
 
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=onschedule_one.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
 
         # add unscheduled
         get_related_visit_model_cls().objects.create(
             appointment=first_appointment,
             report_datetime=first_appointment.appt_datetime,
             reason=SCHEDULED,
@@ -385,34 +250,33 @@
         first_appointment.save()
         self.helper.add_unscheduled_appointment(first_appointment)
 
         appointment = (
             get_appointment_model_cls()
             .objects.filter(
                 subject_identifier=onschedule_one.subject_identifier,
-                visit_schedule_name="visit_schedule1",
-                schedule_name="schedule1",
+                visit_schedule_name=self.visit_schedule1.name,
+                schedule_name=self.schedule1.name,
             )
             .order_by("appt_datetime")[0]
         )
         self.assertEqual(first_appointment, appointment)
 
     def test_next_appointment(self):
-        self.helper.consent_and_put_on_schedule()
         onschedule = OnScheduleOne.objects.get(subject_identifier=self.subject_identifier)
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=onschedule.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         next_appointment = get_appointment_model_cls().objects.next_appointment(
             visit_code=first_appointment.visit_code,
             subject_identifier=onschedule.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(
             get_appointment_model_cls()
             .objects.filter(subject_identifier=onschedule.subject_identifier)
             .order_by("appt_datetime")[1],
             next_appointment,
         )
@@ -424,20 +288,19 @@
             get_appointment_model_cls()
             .objects.filter(subject_identifier=onschedule.subject_identifier)
             .order_by("appt_datetime")[1],
             next_appointment,
         )
 
     def test_next_appointment_with_unscheduled(self):
-        self.helper.consent_and_put_on_schedule()
         onschedule = OnScheduleOne.objects.get(subject_identifier=self.subject_identifier)
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=onschedule.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
 
         # add unscheduled
         get_related_visit_model_cls().objects.create(
             appointment=first_appointment,
             report_datetime=first_appointment.appt_datetime,
             reason=SCHEDULED,
@@ -446,16 +309,16 @@
         first_appointment.save()
         first_appointment.refresh_from_db()
         self.helper.add_unscheduled_appointment(first_appointment)
 
         next_appointment = get_appointment_model_cls().objects.next_appointment(
             visit_code=first_appointment.visit_code,
             subject_identifier=onschedule.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(
             get_appointment_model_cls()
             .objects.filter(
                 subject_identifier=onschedule.subject_identifier, visit_code_sequence=0
             )
             .order_by("timepoint")[1],
@@ -472,34 +335,32 @@
             )
             .order_by("timepoint")[1],
             next_appointment,
         )
 
     def test_next_appointment_after_last_returns_none(self):
         """Assert returns None if next after last appointment."""
-        self.helper.consent_and_put_on_schedule()
 
         last_appointment = get_appointment_model_cls().objects.last_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(
             get_appointment_model_cls().objects.next_appointment(appointment=last_appointment),
             None,
         )
 
     def test_next_appointment_after_last_returns_none_with_unscheduled(self):
         """Assert returns None if next after last appointment."""
-        self.helper.consent_and_put_on_schedule()
 
         last_appointment = get_appointment_model_cls().objects.last_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
 
         # add unscheduled
         for appointment in (
             get_appointment_model_cls()
             .objects.all()
             .order_by("timepoint", "visit_code_sequence")
@@ -518,19 +379,18 @@
         self.assertEqual(
             get_appointment_model_cls().objects.next_appointment(appointment=last_appointment),
             None,
         )
 
     def test_next_appointment_until_none(self):
         """Assert can walk from first to last appointment."""
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         first = get_appointment_model_cls().objects.first_appointment(
             appointment=appointments[0]
         )
         appts = [first]
         for appointment in appointments:
             appts.append(
@@ -538,58 +398,55 @@
             )
         self.assertIsNotNone(appts[0])
         self.assertEqual(appts[0], first)
         self.assertEqual(appts[-1], None)
 
     def test_previous_appointment1(self):
         """Assert returns None if relative to first appointment."""
-        self.helper.consent_and_put_on_schedule()
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(
             get_appointment_model_cls().objects.previous_appointment(
                 appointment=first_appointment
             ),
             None,
         )
 
     def test_previous_appointment2(self):
         """Assert returns previous appointment."""
-        self.helper.consent_and_put_on_schedule()
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         next_appointment = get_appointment_model_cls().objects.next_appointment(
             appointment=first_appointment
         )
         self.assertEqual(
             get_appointment_model_cls().objects.previous_appointment(
                 appointment=next_appointment
             ),
             first_appointment,
         )
 
     def test_next_and_previous_appointment3(self):
         """Assert accepts appointment or indiviual attrs."""
-        self.helper.consent_and_put_on_schedule()
         first_appointment = get_appointment_model_cls().objects.first_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         next_appointment = get_appointment_model_cls().objects.next_appointment(
             visit_code=first_appointment.visit_code,
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(
             get_appointment_model_cls()
             .objects.filter(subject_identifier=self.subject_identifier)
             .order_by("appt_datetime")[1],
             next_appointment,
         )
@@ -599,75 +456,27 @@
         self.assertEqual(
             get_appointment_model_cls()
             .objects.filter(subject_identifier=self.subject_identifier)
             .order_by("appt_datetime")[1],
             appointment,
         )
 
-    @override_settings(
-        EDC_APPOINTMENT_APPT_REASON_CHOICES=((UNSCHEDULED_APPT, "Unscheduled"),)
-    )
-    def test_setting_reason_choices_invalid(self):
-        self.assertRaises(ImproperlyConfigured, get_appt_reason_choices)
-
-    @override_settings(
-        EDC_APPOINTMENT_APPT_REASON_CHOICES=(
-            (SCHEDULED_APPT, "Routine / Scheduled"),
-            (UNSCHEDULED_APPT, "Unscheduled"),
-        )
-    )
-    def test_setting_reason_choices_valid(self):
-        try:
-            choices = get_appt_reason_choices()
-        except ImproperlyConfigured:
-            self.fail("ImproperlyConfigured unexpectedly raised")
-        self.assertEqual(
-            choices,
-            (
-                (SCHEDULED_APPT, "Routine / Scheduled"),
-                (UNSCHEDULED_APPT, "Unscheduled"),
-            ),
-        )
-
-    @override_settings(
-        EDC_APPOINTMENT_APPT_REASON_CHOICES=(
-            (SCHEDULED_APPT, "Routine / Scheduled"),
-            (UNSCHEDULED_APPT, "Unscheduled"),
-            ("blah", "Blah"),
-        )
-    )
-    def test_setting_reason_choices_valid2(self):
-        try:
-            choices = get_appt_reason_choices()
-        except ImproperlyConfigured:
-            self.fail("ImproperlyConfigured unexpectedly raised")
-        self.assertEqual(
-            choices,
-            (
-                (SCHEDULED_APPT, "Routine / Scheduled"),
-                (UNSCHEDULED_APPT, "Unscheduled"),
-                ("blah", "Blah"),
-            ),
-        )
-
     def test_raises_appt_timing_missed_at_baseline(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = (
             get_appointment_model_cls()
             .objects.filter(subject_identifier=self.subject_identifier)
             .order_by("timepoint")
         )
         self.assertEqual(appointments.count(), 4)
         appointment = appointments.first()
         appointment.appt_status = IN_PROGRESS_APPT
         appointment.appt_timing = MISSED_APPT
         self.assertRaises(AppointmentBaselineError, appointment.save)
 
     def test_appt_timing(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = (
             get_appointment_model_cls()
             .objects.filter(subject_identifier=self.subject_identifier)
             .order_by("timepoint")
         )
         self.assertEqual(appointments.count(), 4)
         # create report for baseline visit
@@ -684,15 +493,14 @@
         appointment = appointment.next
         appointment.appt_timing = MISSED_APPT
         appointment.save()
         appointment.refresh_from_db()
         self.assertEqual(appointment.appt_timing, MISSED_APPT)
 
     def test_appointment_creates_subject_visit_if_missed(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
         # create report for baseline visit
         get_related_visit_model_cls().objects.create(
             appointment=appointments[0],
@@ -713,15 +521,14 @@
         self.assertIn("auto-created", subject_visit.comments)
         self.assertEqual(subject_visit.document_status, INCOMPLETE)
 
         # resave does not cause error
         appointment.save()
 
     def test_raises_if_subject_visit_reason_out_of_sync_with_appt(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = get_appointment_model_cls().objects.filter(
             subject_identifier=self.subject_identifier
         )
         self.assertEqual(appointments.count(), 4)
         # create report for baseline visit
         get_related_visit_model_cls().objects.create(
             appointment=appointments[0],
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment_creator.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from __future__ import annotations
+
 import os
 from datetime import datetime
 from unittest import skip
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil.relativedelta import relativedelta
 from django.conf import settings
 from django.test import TestCase
 from django.test.utils import override_settings
-from edc_consent import site_consents
 from edc_consent.consent_definition import ConsentDefinition
+from edc_consent.site_consents import site_consents
 from edc_constants.constants import FEMALE, MALE
 from edc_facility.import_holidays import import_holidays
 from edc_facility.utils import get_facility
 from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_schedule.visit import Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
 from edc_appointment.creators import AppointmentCreator
 from edc_appointment.models import Appointment
 from edc_appointment.tests.helper import Helper
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 
 utc_tz = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
 @time_machine.travel(datetime(2019, 6, 11, 8, 00, tzinfo=utc_tz))
 class AppointmentCreatorTestCase(TestCase):
@@ -42,15 +44,15 @@
         )
 
         self.schedule = Schedule(
             name="schedule",
             onschedule_model="edc_appointment_app.onschedule",
             offschedule_model="edc_appointment_app.offschedule",
             appointment_model="edc_appointment.appointment",
-            consent_model="edc_appointment_app.subjectconsent",
+            consent_definitions=[consent_v1],
         )
 
         self.visit1000 = Visit(
             code="1000",
             timepoint=0,
             rbase=relativedelta(days=0),
             rlower=relativedelta(days=0),
@@ -76,34 +78,37 @@
             facility_name="7-day-clinic",
         )
         self.schedule.add_visit(self.visit1000)
         self.schedule.add_visit(self.visit1001)
         self.schedule.add_visit(self.visit1010)
         self.visit_schedule.add_schedule(self.schedule)
 
-        site_visit_schedules.register(visit_schedule=self.visit_schedule)
+        site_visit_schedules.register(self.visit_schedule)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
 
         class Meta:
             label_lower = ""
 
         class DummyAppointmentObj:
             subject_identifier = self.subject_identifier
             visit_schedule = self.visit_schedule
             schedule = self.schedule
             facility = get_facility(name="7-day-clinic")
             _meta = Meta()
 
         self.model_obj = DummyAppointmentObj()
 
-    def put_on_schedule(self, dt):
+    def put_on_schedule(self, dt, consent_definition: ConsentDefinition | None = None):
         self.helper = self.helper_cls(subject_identifier=self.subject_identifier, now=dt)
         self.helper.consent_and_put_on_schedule(
-            visit_schedule_name="visit_schedule", schedule_name="schedule"
+            visit_schedule_name=self.visit_schedule.name,
+            schedule_name=self.schedule.name,
+            report_datetime=dt,
+            consent_definition=consent_definition,
         )
 
 
 class TestAppointmentCreator(AppointmentCreatorTestCase):
     @classmethod
     def setUpClass(cls):
         import_holidays()
@@ -271,15 +276,15 @@
             end=datetime(1901, 10, 2, 0, 0, 0, tzinfo=utc_tz),
             age_min=18,
             age_is_adult=18,
             age_max=64,
             gender=[MALE, FEMALE],
         )
         site_consents.register(consent_definition)
-        self.put_on_schedule(appt_datetime)
+        self.put_on_schedule(appt_datetime, consent_definition)
 
         expected_appt_datetime = datetime(1900, 1, 2, tzinfo=ZoneInfo("UTC"))
         creator = AppointmentCreator(
             subject_identifier=self.subject_identifier,
             visit_schedule_name=self.visit_schedule.name,
             schedule_name=self.schedule.name,
             visit=self.visit1000,
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appointment_form_validator.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appointment_form_validator.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil.relativedelta import relativedelta
 from django.core.exceptions import ObjectDoesNotExist
 from django.forms import ValidationError
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_constants.constants import NOT_APPLICABLE
 from edc_facility.import_holidays import import_holidays
 from edc_form_validators import ModelFormFieldValidatorError
 from edc_metadata import KEYED, REQUIRED
 from edc_metadata.models import CrfMetadata, RequisitionMetadata
 from edc_visit_schedule.constants import DAY01
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
@@ -36,17 +36,17 @@
     INVALID_APPT_STATUS,
     INVALID_APPT_STATUS_AT_BASELINE,
     INVALID_MISSED_APPT_NOT_ALLOWED,
     INVALID_PREVIOUS_APPOINTMENT_NOT_UPDATED,
 )
 from edc_appointment.models import Appointment
 from edc_appointment.utils import get_previous_appointment
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 from ..test_case_mixins import AppointmentTestCaseMixin
 
 utc_tz = ZoneInfo("UTC")
 
 
@@ -58,25 +58,30 @@
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        self.visit_schedule1 = get_visit_schedule1()
+        self.visit_schedule2 = get_visit_schedule2()
+        site_visit_schedules.register(visit_schedule=self.visit_schedule1)
+        site_visit_schedules.register(visit_schedule=self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=datetime(2017, 1, 7, tzinfo=ZoneInfo("UTC")),
         )
 
     def test_get_previous(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         for i in [0, 1]:
             Appointment.objects.create(
                 subject_identifier=appointments[0].subject_identifier,
                 appt_datetime=appointments[0].appt_datetime + relativedelta(hours=i + 1),
                 timepoint=appointments[0].timepoint,
                 visit_code=appointments[0].visit_code,
@@ -113,15 +118,18 @@
         except ModelFormFieldValidatorError as e:
             self.fail(f"ModelFormFieldValidatorError unexpectedly raised. Got {e}")
 
     def test_appointment_sequence(self):
         """Asserts a sequence error is raised if previous appointment
         is still NEW_APPT.
         """
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(appt_status=IN_PROGRESS_APPT), instance=appointments[1]
         )
         with self.assertRaises(ValidationError) as cm:
             form_validator.validate()
         self.assertIn(INVALID_PREVIOUS_APPOINTMENT_NOT_UPDATED, form_validator._error_codes)
@@ -135,15 +143,18 @@
         self.assertIn(INVALID_PREVIOUS_APPOINTMENT_NOT_UPDATED, form_validator._error_codes)
         self.assertIn("1000.0", str(cm.exception))
 
     def test_visit_report_sequence(self):
         """Asserts a sequence error is raised if previous visit
         not complete for an in progress appointment.
         """
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
 
         # try to add second appt before the first
         # should fail
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(appt_status=IN_PROGRESS_APPT), instance=appointments[1]
         )
@@ -180,15 +191,18 @@
 
     def test_visit_report_sequence2(self):
         """Asserts a sequence error is raised if previous visit
         not complete for an in progress appointment.
 
         Validate the visit_code_sequence
         """
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
 
         # add continuation appt (visit_code_sequence=1)
         for i in [0, 1]:
             Appointment.objects.create(
                 subject_identifier=appointments[i].subject_identifier,
                 appt_datetime=appointments[i].appt_datetime + relativedelta(hours=i + 1),
@@ -247,43 +261,52 @@
         )
         try:
             form_validator.validate_visit_report_sequence()
         except ValidationError:
             self.fail("ValidationError unexpectedly raised.")
 
     def test_interim_sequence(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
 
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(
                 subject_identifier=self.subject_identifier,
                 appt_status=IN_PROGRESS_APPT,
                 visit_code="1000",
                 visit_code_sequence=1,
                 timepoint=Decimal("0.1"),
             )
         )
         form_validator.validate_visit_report_sequence()
 
     def test_confirm_appt_field_attrs(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].visit_code, DAY01)
         self.assertEqual(appointments[0].visit_code_sequence, 0)
         self.assertEqual(appointments[0].visit_schedule_name, "visit_schedule1")
         self.assertEqual(appointments[0].schedule_name, "schedule1")
         visit_schedule = site_visit_schedules.get_visit_schedule(
             appointments[0].visit_schedule_name
         )
         schedule = visit_schedule.schedules.get(appointments[0].schedule_name)
         self.assertEqual(schedule.visits.first.timepoint, Decimal("0.0"))
         self.assertEqual(appointments[0].timepoint, Decimal("0.0"))
 
     def test_baseline_appt_ontime_ok(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(
                 subject_identifier=self.subject_identifier,
                 appt_timing=ONTIME_APPT,
                 appt_reason=SCHEDULED_APPT,
             ),
@@ -291,15 +314,18 @@
         )
         try:
             form_validator.validate_appointment_timing()
         except ValidationError:
             self.fail("ValidationError unexpectedly raised")
 
     def test_baseline_appt_cannot_be_missed(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(
                 subject_identifier=self.subject_identifier,
                 appt_timing=MISSED_APPT,
                 appt_reason=SCHEDULED_APPT,
             ),
@@ -307,15 +333,18 @@
         )
         with self.assertRaises(ValidationError) as cm:
             form_validator.validate_appointment_timing()
         self.assertIsNotNone(cm.exception)
         self.assertIn(INVALID_APPT_STATUS_AT_BASELINE, form_validator._error_codes)
 
     def test_can_miss_scheduled_appt_if_not_baseline(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -335,15 +364,18 @@
 
         try:
             form_validator.validate_appointment_timing()
         except ValidationError:
             self.fail("ValidationError unexpectedly raised")
 
     def test_cannot_miss_unscheduled_appt(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -367,15 +399,18 @@
         with self.assertRaises(ValidationError) as cm:
             form_validator.validate_appointment_timing()
         self.assertIsNotNone(cm.exception)
         self.assertIn(INVALID_MISSED_APPT_NOT_ALLOWED, form_validator._error_codes)
 
     @override_settings(EDC_VISIT_TRACKING_ALLOW_MISSED_UNSCHEDULED=True)
     def test_can_miss_unscheduled_appt_if_allowed_in_settings(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -402,15 +437,18 @@
             self.fail(f"ValidationError unexpectedly raised. Got {e}")
 
     @override_settings(
         SUBJECT_VISIT_MISSED_MODEL="edc_appointment_app.subjectvisitmissed",
         SUBJECT_VISIT_MISSED_REASONS_MODEL="edc_visit_tracking.subjectvisitmissedreasons",
     )
     def test_change_from_missed_removes_missed_visit_report(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -455,15 +493,18 @@
             self.fail("ObjectDoesNotExist not raised")
 
     @override_settings(
         SUBJECT_VISIT_MISSED_MODEL="edc_appointment_app.subjectvisitmissed",
         SUBJECT_VISIT_MISSED_REASONS_MODEL="edc_viist_tracking.subjectvisitmissedreasons",
     )
     def test_change_to_missed_not_allowed_if_crfs_exist(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -517,15 +558,18 @@
             self.fail("ValidationError raised")
 
     @override_settings(
         SUBJECT_VISIT_MISSED_MODEL="edc_appointment_app.subjectvisitmissed",
         SUBJECT_VISIT_MISSED_REASONS_MODEL="edc_visit_tracking.subjectvisitmissedreasons",
     )
     def test_change_to_missed_not_allowed_if_requisitions_exist(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -579,15 +623,18 @@
         except ValidationError:
             self.fail("ValidationError raised")
 
     def test_baseline_visit_report_datetime_must_match_appt_datetime(self):
         """Baseline appt date resets starting appointment, so visit
         report must match.
         """
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         # create report for baseline visit
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -595,15 +642,18 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfone": ("next_appt_date", "next_visit_code")
         }
     )
     def test_skipped_never_allowed_at_baseline(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         self.assertEqual(appointments[0].appt_timing, ONTIME_APPT)
         form_validator = AppointmentFormValidator(
             cleaned_data=dict(
                 subject_identifier=self.subject_identifier,
                 appt_status=SKIPPED_APPT,
                 appt_timing=NOT_APPLICABLE,
@@ -618,15 +668,18 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfone": ("next_appt_date", "next_visit_code")
         }
     )
     def test_skipped_allowed_after_baseline_and_settings_attr_is_set(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
         )
         appointments[0].appt_status = INCOMPLETE_APPT
@@ -644,15 +697,18 @@
         try:
             form_validator.validate()
         except ValidationError as e:
             self.fail(f"ValidationError unexpectedly raised. Got {e}")
 
     @override_settings(EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={})
     def test_skipped_not_allowed_if_settings_attr_not_set(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
         )
         appointments[0].appt_status = INCOMPLETE_APPT
@@ -674,15 +730,18 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfone": ("next_appt_date", "next_visit_code")
         }
     )
     def test_skip_appointments(self):
-        self.helper.consent_and_put_on_schedule()
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_datetimes.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_datetimes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from copy import deepcopy
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil._common import weekday
 from dateutil.relativedelta import FR, MO, SA, SU, TH, TU, WE, relativedelta
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
 from edc_visit_schedule.schedule.visit_collection import VisitCollection
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 
 from edc_appointment.models import Appointment
-from edc_appointment_app.consents import v1_consent
-from edc_appointment_app.visit_schedule import visit_schedule1
+from edc_appointment_app.consents import consent_v1
+from edc_appointment_app.visit_schedule import get_visit_schedule1
 
 from ..helper import Helper
 
 utc_tz = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
@@ -28,25 +27,22 @@
     """Note: visit schedule has appointments on days 0, 1, 2, 3, etc.
     Default facility accepts appointments any day of the week.
     """
 
     @classmethod
     def setUpTestData(cls):
         import_holidays()
-
-    def setUp(self):
-        site_visit_schedules._registry = {}
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
 
     def register_visit_schedule(self, facility_name=None):
         """Overwrite facility name on each visit and register
         the modified visit_schedule.
         """
-        visit_schedule = deepcopy(visit_schedule1)
+        visit_schedule = get_visit_schedule1()
         for schedule_name, schedule in visit_schedule.schedules.items():
             visit_collection = VisitCollection()
             for k, v in schedule.visits.items():
                 v.facility_name = facility_name
                 visit_collection.update({k: v})
             schedule.visits = visit_collection
             visit_schedule.schedules[schedule_name] = schedule
@@ -57,31 +53,36 @@
             for k, v in schedule.visits.items():
                 self.assertEqual(v.facility_name, facility_name)
 
     def get_appt_datetimes(self, base_appt_datetime=None, subject_identifier=None):
         self.assertIsNotNone(base_appt_datetime)
         now = base_appt_datetime.astimezone(ZoneInfo("UTC"))
         self.helper = self.helper_cls(subject_identifier=subject_identifier, now=now)
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.filter(subject_identifier=subject_identifier)
         return [obj.appt_datetime for obj in appointments]
 
     def test_appointments_creation_dates(self):
         """Assert does not skip any days regardless of
         base appointment day.
 
-        default facility (in tests) accepts appointments any day of the week.
+        default facility (in tests) accepts appointments any day
+        of the week.
         """
         self.register_visit_schedule(facility_name="7-day-clinic")
         for i in range(0, 7, 7):
             subject_identifier = f"12345{i}"
             dte = datetime(2017, 1, 7) + relativedelta(days=i)
             now = dte.astimezone(ZoneInfo("UTC"))
             self.helper = self.helper_cls(subject_identifier=subject_identifier, now=now)
-            self.helper.consent_and_put_on_schedule()
+            self.helper.consent_and_put_on_schedule(
+                visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+            )
             appointments = Appointment.objects.filter(subject_identifier=subject_identifier)
             appt_datetimes = [obj.appt_datetime for obj in appointments]
             base_appt_datetime = appt_datetimes[0]
             for index, appt_datetime in enumerate(appt_datetimes):
                 self.assertEqual(
                     base_appt_datetime + relativedelta(days=index * 7), appt_datetime
                 )
@@ -95,97 +96,121 @@
             base_appt_datetime=base_appt_datetime, subject_identifier="123456"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), MO)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TH)
 
+    def test_appointments_creation_dates3(self):
+        """Assert skips SA, SU."""
+        self.register_visit_schedule(facility_name="5-day-clinic")
         base_appt_datetime = datetime(2017, 1, 8)
         self.assertTrue(weekday(base_appt_datetime.weekday()), SU)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="1234567"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), MO)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TH)
 
+    def test_appointments_creation_dates4(self):
+        """Assert skips SA, SU."""
+        self.register_visit_schedule(facility_name="5-day-clinic")
         base_appt_datetime = datetime(2017, 1, 9)
         self.assertTrue(weekday(base_appt_datetime.weekday()), MO)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="12345678"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), MO)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TH)
 
+    def test_appointments_creation_dates5(self):
+        """Assert skips SA, SU."""
+        self.register_visit_schedule(facility_name="5-day-clinic")
         base_appt_datetime = datetime(2017, 1, 10)
         self.assertTrue(weekday(base_appt_datetime.weekday()), TU)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="123456789"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), FR)
 
+    def test_appointments_creation_dates6(self):
+        """Assert skips SA, SU."""
+        self.register_visit_schedule(facility_name="5-day-clinic")
         base_appt_datetime = datetime(2017, 1, 11)
         self.assertTrue(weekday(base_appt_datetime.weekday()), WE)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="1234567890"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), FR)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), MO)
 
-    def test_appointments_creation_dates3(self):
-        """Assert skips FR, SA, SU, MO."""
+    def test_appointments_creation_dates7(self):
+        """Assert 3-day-clinic skips FR, SA, SU, MO."""
         self.register_visit_schedule(facility_name="3-day-clinic")
         base_appt_datetime = datetime(2017, 1, 7)  # noqa
         self.assertTrue(weekday(base_appt_datetime.weekday()), SA)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="123456"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TU)
 
+    def test_appointments_creation_dates8(self):
+        """Assert 3-day-clinic skips FR, SA, SU, MO."""
+        self.register_visit_schedule(facility_name="3-day-clinic")
         base_appt_datetime = datetime(2017, 1, 8)
         self.assertTrue(weekday(base_appt_datetime.weekday()), SU)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="1234567"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TU)
 
+    def test_appointments_creation_dates9(self):
+        """Assert 3-day-clinic skips FR, SA, SU, MO."""
+        self.register_visit_schedule(facility_name="3-day-clinic")
         base_appt_datetime = datetime(2017, 1, 9)
         self.assertTrue(weekday(base_appt_datetime.weekday()), MO)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="12345678"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TU)
 
+    def test_appointments_creation_dates10(self):
+        """Assert 3-day-clinic skips FR, SA, SU, MO."""
+        self.register_visit_schedule(facility_name="3-day-clinic")
         base_appt_datetime = datetime(2017, 1, 10)
         self.assertTrue(weekday(base_appt_datetime.weekday()), TU)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="123456789"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), TU)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[2].weekday()), TH)
         self.assertTrue(weekday(appt_datetimes[3].weekday()), TU)
 
+    def test_appointments_creation_dates11(self):
+        """Assert 3-day-clinic skips FR, SA, SU, MO."""
+        self.register_visit_schedule(facility_name="3-day-clinic")
         base_appt_datetime = datetime(2017, 1, 11)
         self.assertTrue(weekday(base_appt_datetime.weekday()), WE)
         appt_datetimes = self.get_appt_datetimes(
             base_appt_datetime=base_appt_datetime, subject_identifier="1234567890"
         )
         self.assertTrue(weekday(appt_datetimes[0].weekday()), WE)
         self.assertTrue(weekday(appt_datetimes[1].weekday()), TH)
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_sequence.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import datetime as dt
 from zoneinfo import ZoneInfo
 
 import time_machine
 from django.db.models import ProtectedError
 from django.db.models.signals import post_save
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
 from edc_protocol import Protocol
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 
 from edc_appointment.constants import INCOMPLETE_APPT
 from edc_appointment.creators import UnscheduledAppointmentCreator
 from edc_appointment.managers import AppointmentDeleteError
 from edc_appointment.models import Appointment
 from edc_appointment.utils import delete_appointment_in_sequence, get_next_appointment
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 
 utc_tz = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
@@ -33,44 +33,48 @@
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        self.visit_schedule1 = get_visit_schedule1()
+        self.visit_schedule2 = get_visit_schedule2()
+        site_visit_schedules.register(self.visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=Protocol().study_open_datetime,
         )
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name="schedule1"
+        )
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         self.assertEqual(appointments.count(), 4)
 
         appointment = Appointment.objects.get(timepoint=0.0)
         SubjectVisit.objects.create(
             appointment=appointment,
             subject_identifier=appointment.subject_identifier,
             report_datetime=appointment.appt_datetime,
-            visit_schedule_name=visit_schedule1.name,
+            visit_schedule_name=self.visit_schedule1.name,
             schedule_name="schedule1",
             visit_code="1000",
             reason=SCHEDULED,
         )
         appointment.appt_status = INCOMPLETE_APPT
         appointment.save_base(update_fields=["appt_status"])
         appointment.refresh_from_db()
 
         for i in range(0, 3):
             creator = UnscheduledAppointmentCreator(
                 subject_identifier=self.subject_identifier,
-                visit_schedule_name=visit_schedule1.name,
+                visit_schedule_name=self.visit_schedule1.name,
                 schedule_name="schedule1",
                 visit_code="1000",
                 suggested_visit_code_sequence=appointment.visit_code_sequence + 1,
             )
             appointment = creator.appointment
             appointment.appt_status = INCOMPLETE_APPT
             appointment.save_base(update_fields=["appt_status"])
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_appt_status.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_appt_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import datetime as dt
 from zoneinfo import ZoneInfo
 
 import time_machine
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
 from edc_metadata.utils import get_crf_metadata_model_cls
 from edc_protocol import Protocol
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 
 from edc_appointment.appointment_status_updater import AppointmentStatusUpdater
 from edc_appointment.constants import IN_PROGRESS_APPT, INCOMPLETE_APPT, NEW_APPT
 from edc_appointment.models import Appointment
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 
 utc_tz = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
@@ -30,25 +30,30 @@
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        self.visit_schedule1 = get_visit_schedule1()
+        self.visit_schedule2 = get_visit_schedule2()
+        site_visit_schedules.register(self.visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=Protocol().study_open_datetime,
         )
+        schedule_name = self.visit_schedule1.schedules.get("schedule1").name
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=schedule_name
+        )
 
     def test_appointment_status(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         self.assertEqual(appointments.count(), 4)
 
         SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -64,15 +69,14 @@
         self.assertEqual(appointment.appt_status, INCOMPLETE_APPT)
         appointment.appt_status = IN_PROGRESS_APPT
         appointment.save()
         appointment.refresh_from_db()
         self.assertEqual(appointment.appt_status, IN_PROGRESS_APPT)
 
     def test_appointment_status2(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         self.assertEqual(appointments.count(), 4)
 
         # complete baseline appt/visit
         appointment_baseline = appointments[0]
         appointment_baseline.appt_status = IN_PROGRESS_APPT
         appointment_baseline.save()
@@ -92,24 +96,22 @@
         appointment.save()
         appointment.refresh_from_db()
         appointment_baseline.refresh_from_db()
         self.assertEqual(appointment_baseline.appt_status, INCOMPLETE_APPT)
         self.assertEqual(appointment.appt_status, IN_PROGRESS_APPT)
 
     def test_appt_status_updater_init(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         self.assertEqual(appointments.count(), 4)
 
         # complete baseline appt/visit
         appointment_baseline = appointments[0]
         AppointmentStatusUpdater(appointment=appointment_baseline)
 
     def test_appt_status_updater_init2(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         appointment_baseline = appointments[0]
         appointment_1 = appointments[1]
         appointment_2 = appointments[2]
         appointment_3 = appointments[3]
 
         self.assertEqual(appointments.count(), 4)
@@ -142,15 +144,14 @@
         appointment_baseline.refresh_from_db()
         self.assertEqual(appointment_baseline.appt_status, IN_PROGRESS_APPT)
         self.assertEqual(appointment_1.appt_status, NEW_APPT)
         self.assertEqual(appointment_2.appt_status, NEW_APPT)
         self.assertEqual(appointment_3.appt_status, NEW_APPT)
 
     def test_appt_status_updater_appt_1(self):
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         appointment_baseline = appointments[0]
         appointment_1 = appointments[1]
         appointment_2 = appointments[2]
         appointment_3 = appointments[3]
 
         self.assertEqual(appointments.count(), 4)
@@ -198,15 +199,14 @@
         self.assertEqual(appointment_2.appt_status, IN_PROGRESS_APPT)
         self.assertEqual(appointment_3.appt_status, NEW_APPT)
 
     def test_appt_status_updater_appt_1_save_base(self):
         """Using save base and update_fields skips
         AppointmentStatusUpdater in the signal
         """
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         appointment_baseline = appointments[0]
         appointment_1 = appointments[1]
         appointment_2 = appointments[2]
         appointment_3 = appointments[3]
 
         self.assertEqual(appointments.count(), 4)
@@ -240,15 +240,14 @@
         self.assertEqual(appointment_2.appt_status, NEW_APPT)
         self.assertEqual(appointment_3.appt_status, NEW_APPT)
 
     def test_appt_status_updater_appt_1_save_base2(self):
         """Using save base and update_fields skips
         AppointmentStatusUpdater in the signal
         """
-        self.helper.consent_and_put_on_schedule()
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         appointment_baseline = appointments[0]
         appointment_1 = appointments[1]
         appointment_2 = appointments[2]
         appointment_3 = appointments[3]
 
         self.assertEqual(appointments.count(), 4)
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_delete_appointment.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_delete_appointment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import datetime as dt
 from zoneinfo import ZoneInfo
 
 import time_machine
 from django.db.models import ProtectedError
 from django.db.models.signals import post_save
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
 from edc_protocol import Protocol
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 
 from edc_appointment.constants import INCOMPLETE_APPT
 from edc_appointment.creators import UnscheduledAppointmentCreator
 from edc_appointment.managers import AppointmentDeleteError
 from edc_appointment.models import Appointment, appointments_on_post_delete
 from edc_appointment.utils import delete_appointment_in_sequence
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 
 utc = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
@@ -40,44 +40,48 @@
             appointments_on_post_delete, dispatch_uid="appointments_on_post_delete"
         )
 
     def setUp(self):
         post_save.disconnect(dispatch_uid="appointments_on_post_delete")
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        self.visit_schedule1 = get_visit_schedule1()
+        self.visit_schedule2 = get_visit_schedule2()
+        site_visit_schedules.register(self.visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=Protocol().study_open_datetime,
         )
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name="schedule1"
+        )
         appointments = Appointment.objects.filter(subject_identifier=self.subject_identifier)
         self.assertEqual(appointments.count(), 4)
 
         appointment = Appointment.objects.get(timepoint=0.0)
         SubjectVisit.objects.create(
             appointment=appointment,
             subject_identifier=appointment.subject_identifier,
             report_datetime=appointment.appt_datetime,
-            visit_schedule_name=visit_schedule1.name,
+            visit_schedule_name=self.visit_schedule1.name,
             schedule_name="schedule1",
             visit_code="1000",
             reason=SCHEDULED,
         )
         appointment.appt_status = INCOMPLETE_APPT
         appointment.save_base(update_fields=["appt_status"])
         appointment.refresh_from_db()
 
         for i in range(1, 4):
             creator = UnscheduledAppointmentCreator(
                 subject_identifier=self.subject_identifier,
-                visit_schedule_name=visit_schedule1.name,
+                visit_schedule_name=self.visit_schedule1.name,
                 schedule_name="schedule1",
                 visit_code="1000",
                 suggested_visit_code_sequence=appointment.visit_code_sequence + 1,
             )
             creator.appointment.appt_status = INCOMPLETE_APPT
             creator.appointment.save_base(update_fields=["appt_status"])
             appointment = creator.appointment
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_next_appointment_crf.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_next_appointment_crf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import datetime as dt
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil.relativedelta import relativedelta
 from django.contrib.auth.models import User
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_constants.constants import NOT_APPLICABLE, PATIENT
 from edc_facility import import_holidays
 from edc_facility.models import HealthFacility, HealthFacilityTypes
 from edc_utils import get_utcnow
 from edc_visit_schedule.apps import populate_visit_schedule
 from edc_visit_schedule.models import VisitSchedule
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 from edc_visit_tracking.utils import get_related_visit_model_cls
 
 from edc_appointment.constants import SKIPPED_APPT
 from edc_appointment.models import Appointment, InfoSources
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.forms import NextAppointmentCrfForm
 from edc_appointment_app.models import NextAppointmentCrf, SubjectConsent
-from edc_appointment_app.visit_schedule import visit_schedule6
+from edc_appointment_app.visit_schedule import get_visit_schedule6
 
 utc = ZoneInfo("UTC")
 tz = ZoneInfo("Africa/Dar_es_Salaam")
 
 
 @override_settings(SITE_ID=10)
 class TestNextAppointmentCrf(TestCase):
@@ -34,17 +34,17 @@
         import_holidays()
 
     @time_machine.travel(dt.datetime(2019, 6, 11, 8, 00, tzinfo=utc))
     def setUp(self):
         self.user = User.objects.create_superuser("user_login", "u@example.com", "pass")
         site_visit_schedules._registry = {}
         site_visit_schedules.loaded = False
-        site_visit_schedules.register(visit_schedule6)
+        site_visit_schedules.register(get_visit_schedule6())
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         populate_visit_schedule()
 
         self.subject_identifier = "101-40990029-4"
         identity = "123456789"
         subject_consent = SubjectConsent.objects.create(
             subject_identifier=self.subject_identifier,
             consent_datetime=get_utcnow() - relativedelta(days=10),
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_skipped_appt.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_skipped_appt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil.relativedelta import relativedelta
+from django.conf import settings
+from django.contrib.sites.models import Site
 from django.core.exceptions import ImproperlyConfigured
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility import import_holidays
 from edc_visit_schedule.apps import populate_visit_schedule
 from edc_visit_schedule.models import VisitSchedule
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED
 
 from edc_appointment.constants import (
@@ -23,28 +25,28 @@
 from edc_appointment.skip_appointments import (
     SkipAppointmentsFieldError,
     SkipAppointmentsValueError,
 )
 from edc_appointment.tests.helper import Helper
 from edc_appointment.tests.test_case_mixins import AppointmentTestCaseMixin
 from edc_appointment.utils import get_allow_skipped_appt_using
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.forms import CrfThreeForm
 from edc_appointment_app.models import (
     CrfFive,
     CrfFour,
     CrfOne,
     CrfThree,
     CrfTwo,
     SubjectVisit,
 )
 from edc_appointment_app.visit_schedule import (
-    visit_schedule1,
-    visit_schedule2,
-    visit_schedule5,
+    get_visit_schedule1,
+    get_visit_schedule2,
+    get_visit_schedule5,
 )
 
 utc = ZoneInfo("UTC")
 
 
 @override_settings(SITE_ID=10)
 @time_machine.travel(datetime(2019, 6, 11, 8, 00, tzinfo=utc))
@@ -54,32 +56,34 @@
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
-        site_visit_schedules.register(visit_schedule=visit_schedule5)
+        site_visit_schedules.register(get_visit_schedule1())
+        site_visit_schedules.register(get_visit_schedule2())
+        site_visit_schedules.register(get_visit_schedule5())
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=datetime(2017, 6, 5, 8, 0, 0, tzinfo=utc),
         )
         populate_visit_schedule()
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfone": ("next_appt_date", "next_visit_code")
         }
     )
     def test_skip_appointments_using_crf_date(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -119,15 +123,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crftwo": ("report_datetime", "next_visit_code_blah"),
         }
     )
     def test_skip_appointments_using_bad_settings_for_crf(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -145,15 +151,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crftwo": ("report_datetime_blah", "f1"),
         }
     )
     def test_skip_appointments_using_bad_settings_for_crf2(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -172,15 +180,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfthree": ("report_datetime", "f1"),
         }
     )
     def test_skip_appointments_using_crf_ok(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -200,15 +210,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfthree": ("report_datetime", "f1"),
         }
     )
     def test_skip_multiple_appointments_using_good_crf(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -227,15 +239,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfthree": ("appt_date", "f1"),
         }
     )
     def test_skip_multiple_appointments_using_last_crf(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -273,15 +287,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crftwo": ("report_datetime", "visitschedule"),
         }
     )
     def test_visit_code_as_visit_schedule_fk_ok(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -304,15 +320,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfthree": ("appt_date", "f1"),
         }
     )
     def test_last_crf_with_absurd_date_relative_to_visit_code(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -327,15 +345,17 @@
 
     @override_settings(
         EDC_APPOINTMENT_ALLOW_SKIPPED_APPT_USING={
             "edc_appointment_app.crfthree": ("appt_date", "f1"),
         }
     )
     def test_delete(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name="visit_schedule1", schedule_name="schedule1"
+        )
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
         appointments[0].appt_status = IN_PROGRESS_APPT
         appointments[0].save()
         subject_visit = SubjectVisit.objects.create(
             appointment=appointments[0],
             report_datetime=appointments[0].appt_datetime,
             reason=SCHEDULED,
@@ -545,14 +565,15 @@
                 report_datetime=appointments[0].appt_datetime,
                 f1="blah",
             )
         data = dict(
             report_datetime=appointments[0].appt_datetime,
             appt_date=appointments[0].appt_datetime + relativedelta(days=3),
             f1=appointments[1].visit_code,
+            site=Site.objects.get(id=settings.SITE_ID),
         )
         form = CrfThreeForm(data=data, instance=CrfThree(subject_visit=subject_visit))
         form.is_valid()
         self.assertEqual({}, {k: v for k, v in form._errors.items() if k != "subject_visit"})
 
         CrfThree.objects.create(subject_visit=subject_visit, **data)
 
@@ -579,14 +600,15 @@
                 f1="blah",
             )
         data = dict(
             report_datetime=appointments[1].appt_datetime,
             appt_date=appointments[1].appt_datetime + relativedelta(days=5),
             f1=appointments[1].visit_code,
             allow_create_interim=True,
+            site=Site.objects.get(id=settings.SITE_ID),
         )
         form = CrfThreeForm(data=data, instance=CrfThree(subject_visit=subject_visit))
         form.is_valid()
         self.assertEqual({}, {k: v for k, v in form._errors.items() if k != "subject_visit"})
         CrfThree.objects.create(subject_visit=subject_visit, **data)
 
         appointments = Appointment.objects.all().order_by("timepoint", "visit_code_sequence")
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_unscheduled.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_unscheduled.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 from datetime import datetime
 from decimal import Decimal
 from zoneinfo import ZoneInfo
 
 from dateutil.relativedelta import relativedelta
 from django.test import TestCase, override_settings
-from edc_consent import site_consents
+from edc_consent.site_consents import site_consents
 from edc_facility.import_holidays import import_holidays
 from edc_sites.tests import SiteTestCaseMixin
 from edc_utils import get_utcnow
 from edc_visit_schedule.exceptions import ScheduleError
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import SCHEDULED, UNSCHEDULED
 
 from edc_appointment.constants import (
     CANCELLED_APPT,
     IN_PROGRESS_APPT,
     INCOMPLETE_APPT,
     NEW_APPT,
 )
-from edc_appointment.creators import (
+from edc_appointment.creators import UnscheduledAppointmentCreator
+from edc_appointment.exceptions import (
     InvalidParentAppointmentMissingVisitError,
     InvalidParentAppointmentStatusError,
-    UnscheduledAppointmentCreator,
     UnscheduledAppointmentNotAllowed,
 )
 from edc_appointment.models import Appointment
-from edc_appointment_app.consents import v1_consent
+from edc_appointment_app.consents import consent_v1
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule1, visit_schedule2
+from edc_appointment_app.visit_schedule import get_visit_schedule1, get_visit_schedule2
 
 from ..helper import Helper
 
 
 @override_settings(SITE_ID=10)
 class TestUnscheduledAppointmentCreator(SiteTestCaseMixin, TestCase):
     helper_cls = Helper
 
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
+        self.visit_schedule1 = get_visit_schedule1()
+        self.schedule1 = self.visit_schedule1.schedules.get("schedule1")
+        self.visit_schedule2 = get_visit_schedule2()
+        self.schedule2 = self.visit_schedule2.schedules.get("schedule2")
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule1)
-        site_visit_schedules.register(visit_schedule=visit_schedule2)
+        site_visit_schedules.register(self.visit_schedule1)
+        site_visit_schedules.register(self.visit_schedule2)
         site_consents.registry = {}
-        site_consents.register(v1_consent)
+        site_consents.register(consent_v1)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=datetime(2017, 1, 7, tzinfo=ZoneInfo("UTC")),
         )
 
     def test_unscheduled_allowed_but_raises_on_appt_status(self):
-        self.helper.consent_and_put_on_schedule()
-        schedule_name = "schedule1"
-        visit = visit_schedule1.schedules.get(schedule_name).visits.first
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
+        visit = self.visit_schedule1.schedules.get(self.schedule1.name).visits.first
         appointment = Appointment.objects.get(
             subject_identifier=self.subject_identifier,
             visit_code=visit.code,
             visit_code_sequence=0,
         )
         # subject_visit not created so expect exception because of
         # the missing subject_visit
@@ -68,16 +73,16 @@
                 appointment.appt_status = appt_status
                 appointment.save()
                 self.assertEqual(appointment.appt_status, appt_status)
                 self.assertRaises(
                     InvalidParentAppointmentMissingVisitError,
                     UnscheduledAppointmentCreator,
                     subject_identifier=self.subject_identifier,
-                    visit_schedule_name=visit_schedule1.name,
-                    schedule_name=schedule_name,
+                    visit_schedule_name=self.visit_schedule1.name,
+                    schedule_name=self.schedule1.name,
                     visit_code=visit.code,
                     suggested_visit_code_sequence=appointment.visit_code_sequence + 1,
                 )
         # add a subject_visit and expect exception to be raises because
         # of appt_status
         subject_visit = SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
@@ -91,75 +96,76 @@
                 if appointment.appt_status == INCOMPLETE_APPT:
                     continue
                 self.assertEqual(appointment.appt_status, appt_status)
                 self.assertRaises(
                     InvalidParentAppointmentStatusError,
                     UnscheduledAppointmentCreator,
                     subject_identifier=self.subject_identifier,
-                    visit_schedule_name=visit_schedule1.name,
-                    schedule_name=schedule_name,
+                    visit_schedule_name=self.visit_schedule1.name,
+                    schedule_name=self.schedule1.name,
                     visit_code=visit.code,
                     suggested_visit_code_sequence=appointment.visit_code_sequence + 1,
                 )
 
     def test_unscheduled_not_allowed(self):
         self.assertRaises(
             UnscheduledAppointmentNotAllowed,
             UnscheduledAppointmentCreator,
             subject_identifier=self.subject_identifier,
-            visit_schedule_name=visit_schedule2.name,
-            schedule_name="schedule2",
+            visit_schedule_name=self.visit_schedule2.name,
+            schedule_name=self.schedule2.name,
             visit_code="5000",
             suggested_visit_code_sequence=1,
         )
 
     def test_add_subject_visits(self):
-        self.helper.consent_and_put_on_schedule()
-        schedule_name = "schedule1"
-        for visit in visit_schedule1.schedules.get(schedule_name).visits.values():
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
+        for visit in self.visit_schedule1.schedules.get(self.schedule1.name).visits.values():
             with self.subTest(visit=visit):
                 # get parent appointment
                 appointment = Appointment.objects.get(
                     subject_identifier=self.subject_identifier,
                     visit_code=visit.code,
                     visit_code_sequence=0,
                     timepoint=visit.timepoint,
-                    visit_schedule_name=visit_schedule1.name,
-                    schedule_name=schedule_name,
+                    visit_schedule_name=self.visit_schedule1.name,
+                    schedule_name=self.schedule1.name,
                 )
                 appointment.appt_status = IN_PROGRESS_APPT
                 appointment.save()
                 appointment.refresh_from_db()
 
                 # fill in subject visit report for this appointment
                 subject_visit = SubjectVisit.objects.create(
                     appointment=appointment,
                     subject_identifier=self.subject_identifier,
                     report_datetime=appointment.appt_datetime,
                     reason=SCHEDULED,
                     visit_code=visit.code,
                     visit_code_sequence=0,
-                    visit_schedule_name=visit_schedule1.name,
-                    schedule_name=schedule_name,
+                    visit_schedule_name=self.visit_schedule1.name,
+                    schedule_name=self.schedule1.name,
                 )
                 appointment.refresh_from_db()
                 self.assertTrue(appointment.related_visit, subject_visit)
                 self.assertEqual(0, appointment.related_visit.visit_code_sequence)
                 self.assertEqual(1, appointment.next_visit_code_sequence)
 
                 # close appt (set to INCOMPLETE_APPT)
                 appointment.appt_status = INCOMPLETE_APPT
                 appointment.save()
                 appointment.refresh_from_db()
 
                 # create unscheduled off of this appt
                 creator = UnscheduledAppointmentCreator(
                     subject_identifier=self.subject_identifier,
-                    visit_schedule_name=visit_schedule1.name,
-                    schedule_name=schedule_name,
+                    visit_schedule_name=self.visit_schedule1.name,
+                    schedule_name=self.schedule1.name,
                     visit_code=visit.code,
                     facility=appointment.facility,
                     suggested_visit_code_sequence=1,
                     suggested_appt_datetime=appointment.appt_datetime + relativedelta(days=1),
                 )
                 new_appointment = creator.appointment
                 new_appointment.appt_status = IN_PROGRESS_APPT
@@ -183,17 +189,18 @@
                 # close the unscheduled appt (set to INCOMPLETE_APPT)
                 new_appointment.appt_status = INCOMPLETE_APPT
                 new_appointment.save()
                 self.assertEqual(new_appointment.appt_status, INCOMPLETE_APPT)
                 self.assertEqual(visit.timepoint, int(new_appointment.timepoint))
 
     def test_unscheduled_timepoint_not_incremented(self):
-        self.helper.consent_and_put_on_schedule()
-        schedule_name = "schedule1"
-        visit = visit_schedule1.schedules.get(schedule_name).visits.first
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
+        visit = self.visit_schedule1.schedules.get(self.schedule1.name).visits.first
         appointment = Appointment.objects.get(
             subject_identifier=self.subject_identifier, visit_code=visit.code
         )
         self.assertEqual(appointment.timepoint, Decimal("0.0"))
         SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
@@ -224,19 +231,21 @@
                     reason=UNSCHEDULED,
                 )
                 creator.appointment.appt_status = INCOMPLETE_APPT
                 creator.appointment.save()
                 appointment = creator.appointment
 
     def test_appointment_title(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
         appointment = Appointment.objects.first_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(appointment.title, "Day 1")
 
         SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         appointment.appt_status = INCOMPLETE_APPT
@@ -257,16 +266,16 @@
         )
         creator.appointment.appt_status = INCOMPLETE_APPT
         creator.appointment.save()
 
         next_appointment = Appointment.objects.next_appointment(
             visit_code=appointment.visit_code,
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
 
         SubjectVisit.objects.create(
             appointment=next_appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         next_appointment.appt_status = INCOMPLETE_APPT
         next_appointment.save()
@@ -279,33 +288,35 @@
             facility=next_appointment.facility,
             suggested_visit_code_sequence=next_appointment.visit_code_sequence + 1,
         )
 
         self.assertEqual(creator.appointment.title, "Day 2.1")
 
     def test_appointment_title_if_visit_schedule_changes(self):
-        self.helper.consent_and_put_on_schedule()
+        self.helper.consent_and_put_on_schedule(
+            visit_schedule_name=self.visit_schedule1.name, schedule_name=self.schedule1.name
+        )
         appointment = Appointment.objects.first_appointment(
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
         self.assertEqual(appointment.title, "Day 1")
 
         SubjectVisit.objects.create(
             appointment=appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         appointment.appt_status = INCOMPLETE_APPT
         appointment.save()
 
         next_appointment = Appointment.objects.next_appointment(
             visit_code=appointment.visit_code,
             subject_identifier=self.subject_identifier,
-            visit_schedule_name="visit_schedule1",
-            schedule_name="schedule1",
+            visit_schedule_name=self.visit_schedule1.name,
+            schedule_name=self.schedule1.name,
         )
 
         SubjectVisit.objects.create(
             appointment=next_appointment, report_datetime=get_utcnow(), reason=SCHEDULED
         )
         next_appointment.appt_status = INCOMPLETE_APPT
         next_appointment.visit_code = "1111"
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_window_period.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_window_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import datetime as dt
 from unittest.mock import patch
 from zoneinfo import ZoneInfo
 
 import time_machine
 from dateutil.relativedelta import relativedelta
+from django.conf import settings
+from django.contrib.sites.models import Site
 from django.test import TestCase, override_settings
 from edc_facility.import_holidays import import_holidays
 from edc_sites.tests import SiteTestCaseMixin
 from edc_utils import get_utcnow
 from edc_visit_schedule.site_visit_schedules import site_visit_schedules
 from edc_visit_tracking.constants import MISSED_VISIT, SCHEDULED, UNSCHEDULED
 from tqdm import tqdm
 
 from edc_appointment.constants import (
     COMPLETE_APPT,
     INCOMPLETE_APPT,
     MISSED_APPT,
     ONTIME_APPT,
 )
-from edc_appointment.creators import (
-    UnscheduledAppointmentCreator,
+from edc_appointment.creators import UnscheduledAppointmentCreator
+from edc_appointment.exceptions import (
+    AppointmentWindowError,
     UnscheduledAppointmentError,
 )
-from edc_appointment.exceptions import AppointmentWindowError
 from edc_appointment.forms import AppointmentForm
 from edc_appointment.models import Appointment
 from edc_appointment_app.models import SubjectVisit
-from edc_appointment_app.visit_schedule import visit_schedule3
+from edc_appointment_app.visit_schedule import get_visit_schedule3
 
 from ...utils import AppointmentDateWindowPeriodGapError, get_appointment_by_datetime
 from ..helper import Helper
 
 utc = ZoneInfo("UTC")
 
 
@@ -42,15 +44,15 @@
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule3)
+        site_visit_schedules.register(get_visit_schedule3())
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=get_utcnow() - relativedelta(years=2),  # Protocol().study_open_datetime,
         )
 
     @staticmethod
     def create_unscheduled(appointment):
@@ -75,14 +77,15 @@
                 "timepoint_datetime": appointment.timepoint_datetime,
                 "appt_close_datetime": appointment.timepoint_datetime,
                 "facility_name": appointment.facility_name,
                 "appt_type": appointment.appt_type,
                 "appt_status": appointment.appt_status,
                 "appt_reason": appointment.appt_reason,
                 "document_status": appointment.document_status,
+                "site": Site.objects.get(id=settings.SITE_ID),
             },
             instance=appointment,
         )
 
     @staticmethod
     def update_appt_as_incomplete(appointment):
         appointment.refresh_from_db()
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/tests/test_window_period2.py` & `edc-appointment-0.4.9/edc_appointment/tests/tests/test_window_period2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from edc_appointment.models import Appointment
 from edc_appointment.tests.helper import Helper
 from edc_appointment.utils import (
     AppointmentDateWindowPeriodGapError,
     get_appointment_by_datetime,
     get_window_gap_days,
 )
-from edc_appointment_app.visit_schedule.visit_schedule4 import visit_schedule4
+from edc_appointment_app.visit_schedule import get_visit_schedule4
 
 utc = ZoneInfo("UTC")
 
 
 @time_machine.travel(dt.datetime(2019, 7, 11, 8, 00, tzinfo=utc))
 @override_settings(SITE_ID=10)
 class TestAppointmentWindowPeriod2(SiteTestCaseMixin, TestCase):
@@ -28,26 +28,28 @@
 
     @classmethod
     def setUpTestData(cls):
         import_holidays()
 
     def setUp(self):
         self.subject_identifier = "12345"
+        self.visit_schedule4 = get_visit_schedule4()
+        self.schedule4 = self.visit_schedule4.schedules.get("three_monthly_schedule")
         site_visit_schedules._registry = {}
-        site_visit_schedules.register(visit_schedule=visit_schedule4)
+        site_visit_schedules.register(self.visit_schedule4)
         self.helper = self.helper_cls(
             subject_identifier=self.subject_identifier,
             now=get_utcnow() - relativedelta(years=2),
         )
 
     @override_settings(EDC_VISIT_SCHEDULE_DEFAULT_MAX_VISIT_GAP_ALLOWED=0)
     def test_suggested_date_in_window_period_gap_raises(self):
         self.helper.consent_and_put_on_schedule(
-            visit_schedule_name="visit_schedule4",
-            schedule_name="three_monthly_schedule",
+            visit_schedule_name=self.visit_schedule4.name,
+            schedule_name=self.schedule4.name,
         )
         appointments = Appointment.objects.filter(
             subject_identifier=self.subject_identifier
         ).order_by("appt_datetime")
         self.assertEqual(appointments.count(), 5)
         appointment_1000 = appointments[0]
         appointment_1060 = appointments[2]
@@ -72,16 +74,16 @@
         self.assertIn(
             "Date falls in a `window period gap` between 1030 and 1060", str(cm.exception)
         )
 
     @override_settings(EDC_VISIT_SCHEDULE_DEFAULT_MAX_VISIT_GAP_ALLOWED=7)
     def test_match_window_period_gap_adjusted(self):
         self.helper.consent_and_put_on_schedule(
-            visit_schedule_name="visit_schedule4",
-            schedule_name="three_monthly_schedule",
+            visit_schedule_name=self.visit_schedule4.name,
+            schedule_name=self.schedule4.name,
         )
         appointments = Appointment.objects.filter(
             subject_identifier=self.subject_identifier
         ).order_by("appt_datetime")
         self.assertEqual(appointments.count(), 5)
         appointment_1000 = appointments[0]
         appointment_1060 = appointments[2]
@@ -117,16 +119,16 @@
                 if not in_adjusted_window:
                     self.assertIsNone(appointment)
                 else:
                     self.assertEqual("1060", appointment.visit_code)
 
     def test_past_last_visit(self):
         self.helper.consent_and_put_on_schedule(
-            visit_schedule_name="visit_schedule4",
-            schedule_name="three_monthly_schedule",
+            visit_schedule_name=self.visit_schedule4.name,
+            schedule_name=self.schedule4.name,
         )
         appointments = Appointment.objects.filter(
             subject_identifier=self.subject_identifier
         ).order_by("appt_datetime")
         self.assertEqual(appointments.count(), 5)
         appointment_1000 = appointments[0]
         appointment_1120 = appointments[4]
@@ -150,16 +152,16 @@
             )
         except AppointmentDateWindowPeriodGapError as e:
             self.fail(f"AppointmentDateWindowPeriodGapError unexpectedly raised. Got {e}")
         self.assertIsNone(appointment)
 
     def test_window_gap_days(self):
         self.helper.consent_and_put_on_schedule(
-            visit_schedule_name="visit_schedule4",
-            schedule_name="three_monthly_schedule",
+            visit_schedule_name=self.visit_schedule4.name,
+            schedule_name=self.schedule4.name,
         )
         appointments = Appointment.objects.filter(
             subject_identifier=self.subject_identifier
         ).order_by("appt_datetime")
         appointment_1030 = appointments[1]
         gap_days = get_window_gap_days(appointment_1030)
         self.assertEqual(gap_days, 62)
```

### Comparing `edc-appointment-0.4.8/edc_appointment/tests/urls.py` & `edc-appointment-0.4.9/edc_appointment/tests/urls.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/urls.py` & `edc-appointment-0.4.9/edc_appointment/urls.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/utils.py` & `edc-appointment-0.4.9/edc_appointment/utils.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment/view_mixins/appointment_view_mixin.py` & `edc-appointment-0.4.9/edc_appointment/view_mixins/appointment_view_mixin.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from typing import TYPE_CHECKING, Any
 
 from django.apps import apps as django_apps
 from django.contrib import messages
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.translation import gettext as _
 from edc_sites.site import sites
-from edc_subject_model_wrappers import AppointmentModelWrapper
 
 from ..constants import (
     CANCELLED_APPT,
     COMPLETE_APPT,
     IN_PROGRESS_APPT,
     INCOMPLETE_APPT,
     NEW_APPT,
@@ -25,20 +24,17 @@
     from ..models import Appointment
 
 
 class AppointmentViewMixin:
 
     """A view mixin to handle appointments on the dashboard."""
 
-    appointment_model_wrapper_cls = AppointmentModelWrapper
-
     def __init__(self, **kwargs):
         self._appointment = None
         self._appointments = None
-        self._wrapped_appointments = None
         self.appointment_model: str = "edc_appointment.appointment"
         self.appointment_id: str | None = None
         super().__init__(**kwargs)
 
     def get(self, request, *args, **kwargs):
         self.appointment_id = kwargs.get("appointment")
         return super().get(request, *args, **kwargs)
@@ -56,27 +52,31 @@
             kwargs.update(report_datetime=report_datetime)
 
         update_unscheduled_appointment_sequence(
             subject_identifier=self.subject_identifier,
         )
         has_call_manager = True if django_apps.app_configs.get("edc_call_manager") else False
         kwargs.update(
-            appointment=self.appointment_wrapped,
-            appointments=self.appointments_wrapped,
+            appointment=self.appointment,
+            appointments=self.appointments,
             CANCELLED_APPT=CANCELLED_APPT,
             COMPLETE_APPT=COMPLETE_APPT,
             INCOMPLETE_APPT=INCOMPLETE_APPT,
             IN_PROGRESS_APPT=IN_PROGRESS_APPT,
             NEW_APPT=NEW_APPT,
             SKIPPED_APPT=SKIPPED_APPT,
             has_call_manager=has_call_manager,
         )
         return super().get_context_data(**kwargs)
 
     @property
+    def appointment_model_cls(self) -> Appointment:
+        return django_apps.get_model(self.appointment_model)
+
+    @property
     def appointment_options(self) -> dict[str, Any]:
         opts = {}
         if self.kwargs.get("appointment"):
             opts = dict(id=self.kwargs.get("appointment"))
         elif (
             self.kwargs.get("subject_identifier")
             and self.kwargs.get("visit_schedule_name")
@@ -107,47 +107,16 @@
                         try:
                             self._appointment = self.appointment_model_cls.objects.get(**opts)
                         except ObjectDoesNotExist:
                             pass
         return self._appointment
 
     @property
-    def appointment_wrapped(self) -> AppointmentModelWrapper | None:
-        if self.appointment:
-            return self.appointment_model_wrapper_cls(model_obj=self.appointment)
-        return None
-
-    @property
     def appointments(self) -> QuerySet[Appointment]:
         """Returns a Queryset of all appointments for this subject."""
         if not self._appointments:
             self._appointments = self.appointment_model_cls.objects.filter(
                 subject_identifier=self.subject_identifier,
                 site_id__in=sites.get_site_ids_for_user(request=self.request),
             ).order_by("timepoint", "visit_code_sequence")
 
         return self._appointments
-
-    @property
-    def appointments_wrapped(self) -> list[AppointmentModelWrapper]:
-        """Returns a list of wrapped appointments."""
-        if not self._wrapped_appointments:
-            if self.appointments:
-                wrapped = [
-                    self.appointment_model_wrapper_cls(model_obj=obj)
-                    for obj in self.appointments
-                ]
-                for i in range(0, len(wrapped)):
-                    if wrapped[i].appt_status == IN_PROGRESS_APPT:
-                        wrapped[i].disabled = False
-                        for j in range(0, len(wrapped)):
-                            if j != i:
-                                wrapped[j].disabled = True
-                self._wrapped_appointments = wrapped
-        return self._wrapped_appointments or []
-
-    @property
-    def appointment_model_cls(self) -> Appointment:
-        return django_apps.get_model(self.appointment_model)
-
-    def empty_appointment(self, **kwargs) -> Appointment:
-        return self.appointment_model_cls()
```

### Comparing `edc-appointment-0.4.8/edc_appointment/views/unscheduled_appointment_view.py` & `edc-appointment-0.4.9/edc_appointment/views/unscheduled_appointment_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.http.response import HttpResponseRedirect
 from django.urls.base import reverse
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from django.views.generic.base import View
 
-from ..creators import (
+from ..creators import UnscheduledAppointmentCreator
+from ..exceptions import (
     AppointmentInProgressError,
+    AppointmentPermissionsRequired,
+    AppointmentWindowError,
     InvalidParentAppointmentMissingVisitError,
     InvalidParentAppointmentStatusError,
-    UnscheduledAppointmentCreator,
     UnscheduledAppointmentError,
     UnscheduledAppointmentNotAllowed,
 )
-from ..exceptions import AppointmentPermissionsRequired, AppointmentWindowError
 
 
 class UnscheduledAppointmentView(View):
 
     """A view that creates an unscheduled appointment and redirects to
     the subject dashboard.
```

### Comparing `edc-appointment-0.4.8/edc_appointment.egg-info/PKG-INFO` & `edc-appointment-0.4.9/edc_appointment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-appointment
-Version: 0.4.8
+Version: 0.4.9
 Summary: Appointment module for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-appointment
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django appointments data collection clinicedc clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-appointment-0.4.8/edc_appointment.egg-info/SOURCES.txt` & `edc-appointment-0.4.9/edc_appointment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,17 @@
 edc_appointment/tests/etc/user-rsa-restricted-private.pem
 edc_appointment/tests/etc/user-rsa-restricted-public.pem
 edc_appointment/tests/etc/user-salt-local.key
 edc_appointment/tests/etc/user-salt-restricted.key
 edc_appointment/tests/tests/__init__.py
 edc_appointment/tests/tests/test_admin.py
 edc_appointment/tests/tests/test_appointment.py
+edc_appointment/tests/tests/test_appointment2.py
 edc_appointment/tests/tests/test_appointment_creator.py
+edc_appointment/tests/tests/test_appointment_creator2.py
 edc_appointment/tests/tests/test_appointment_form_validator.py
 edc_appointment/tests/tests/test_appt_datetimes.py
 edc_appointment/tests/tests/test_appt_sequence.py
 edc_appointment/tests/tests/test_appt_status.py
 edc_appointment/tests/tests/test_auths.py
 edc_appointment/tests/tests/test_delete_appointment.py
 edc_appointment/tests/tests/test_next_appointment_crf.py
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/forms.py` & `edc-appointment-0.4.9/edc_appointment_app/forms.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment_app/models.py` & `edc-appointment-0.4.9/edc_appointment_app/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from edc_visit_tracking.models import SubjectVisitMissedReasons
 
 from edc_appointment.model_mixins.next_appointment_crf_model_mixin import (
     NextAppointmentCrfModelMixin,
 )
 from edc_appointment.utils import get_appointment_model_name
 
+from .consents import consent_v1
+
 
 class Panel(ListModelMixin):
     class Meta:
         pass
 
 
 #
@@ -117,14 +119,15 @@
 
     confirm_identity = models.CharField(max_length=25)
 
     dob = models.DateField(default=date(1995, 1, 1))
 
 
 class SubjectScreening(ScreeningModelMixin, BaseUuidModel):
+    consent_definition = consent_v1
     objects = SubjectIdentifierManager()
 
 
 class SubjectOffstudy(SiteModelMixin, OffstudyModelMixin, BaseUuidModel):
     objects = SubjectIdentifierManager()
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/sites.py` & `edc-appointment-0.4.9/edc_appointment_app/sites.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/crfs.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/crfs.py`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule1.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from dateutil.relativedelta import relativedelta
 from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.visit import Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
+from ..consents import consent_v1
 from .crfs import crfs, crfs_missed, crfs_unscheduled, requisitions
 
-visit_schedule1 = VisitSchedule(
-    name="visit_schedule1",
-    offstudy_model="edc_appointment_app.subjectoffstudy",
-    death_report_model="edc_appointment_app.deathreport",
-)
 
-schedule1 = Schedule(
-    name="schedule1",
-    onschedule_model="edc_appointment_app.onscheduleone",
-    offschedule_model="edc_appointment_app.offscheduleone",
-    appointment_model="edc_appointment.appointment",
-    consent_model="edc_appointment_app.subjectconsent",
-)
+def get_visit_schedule1() -> VisitSchedule:
+    visit_schedule1 = VisitSchedule(
+        name="visit_schedule1",
+        offstudy_model="edc_appointment_app.subjectoffstudy",
+        death_report_model="edc_appointment_app.deathreport",
+    )
 
+    schedule1 = Schedule(
+        name="schedule1",
+        onschedule_model="edc_appointment_app.onscheduleone",
+        offschedule_model="edc_appointment_app.offscheduleone",
+        appointment_model="edc_appointment.appointment",
+        consent_definitions=[consent_v1],
+    )
 
-visits = []
-for index in range(0, 4):
-    visits.append(
-        Visit(
-            code=f"{1 if index == 0 else index + 1}000",
-            title=f"Day {1 if index == 0 else index + 1}",
-            timepoint=index,
-            rbase=relativedelta(days=7 * index),
-            rlower=relativedelta(days=0),
-            rupper=relativedelta(days=6),
-            requisitions=requisitions,
-            crfs=crfs,
-            crfs_missed=crfs_missed,
-            requisitions_unscheduled=requisitions,
-            crfs_unscheduled=crfs_unscheduled,
-            allow_unscheduled=True,
-            facility_name="5-day-clinic",
+    visits = []
+    for index in range(0, 4):
+        visits.append(
+            Visit(
+                code=f"{1 if index == 0 else index + 1}000",
+                title=f"Day {1 if index == 0 else index + 1}",
+                timepoint=index,
+                rbase=relativedelta(days=7 * index),
+                rlower=relativedelta(days=0),
+                rupper=relativedelta(days=6),
+                requisitions=requisitions,
+                crfs=crfs,
+                crfs_missed=crfs_missed,
+                requisitions_unscheduled=requisitions,
+                crfs_unscheduled=crfs_unscheduled,
+                allow_unscheduled=True,
+                facility_name="5-day-clinic",
+            )
         )
-    )
-for visit in visits:
-    schedule1.add_visit(visit)
-visit_schedule1.add_schedule(schedule1)
+    for visit in visits:
+        schedule1.add_visit(visit)
+    visit_schedule1.add_schedule(schedule1)
+    return visit_schedule1
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule2.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from dateutil.relativedelta import relativedelta
 from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.visit import Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
+from ..consents import consent_v1
 from .crfs import crfs, crfs_missed, requisitions
 
-visit_schedule2 = VisitSchedule(
-    name="visit_schedule2",
-    offstudy_model="edc_appointment_app.subjectoffstudy",
-    death_report_model="edc_appointment_app.deathreport",
-)
-
-schedule2 = Schedule(
-    name="schedule2",
-    onschedule_model="edc_appointment_app.onscheduletwo",
-    offschedule_model="edc_appointment_app.offscheduletwo",
-    appointment_model="edc_appointment.appointment",
-    consent_model="edc_appointment_app.subjectconsent",
-    base_timepoint=4,
-)
-
-
-visits = []
-for index in range(4, 8):
-    visits.append(
-        Visit(
-            code=f"{1 if index == 0 else index + 1}000",
-            title=f"Day {1 if index == 0 else index + 1}",
-            timepoint=index,
-            rbase=relativedelta(days=7 * index),
-            rlower=relativedelta(days=0),
-            rupper=relativedelta(days=6),
-            requisitions=requisitions,
-            crfs=crfs,
-            crfs_missed=crfs_missed,
-            facility_name="7-day-clinic",
-        )
+
+def get_visit_schedule2() -> VisitSchedule:
+    visit_schedule2 = VisitSchedule(
+        name="visit_schedule2",
+        offstudy_model="edc_appointment_app.subjectoffstudy",
+        death_report_model="edc_appointment_app.deathreport",
+    )
+
+    schedule2 = Schedule(
+        name="schedule2",
+        onschedule_model="edc_appointment_app.onscheduletwo",
+        offschedule_model="edc_appointment_app.offscheduletwo",
+        appointment_model="edc_appointment.appointment",
+        consent_definitions=[consent_v1],
+        base_timepoint=4,
     )
-for visit in visits:
-    schedule2.add_visit(visit)
 
-visit_schedule2.add_schedule(schedule2)
+    visits = []
+    for index in range(4, 8):
+        visits.append(
+            Visit(
+                code=f"{1 if index == 0 else index + 1}000",
+                title=f"Day {1 if index == 0 else index + 1}",
+                timepoint=index,
+                rbase=relativedelta(days=7 * index),
+                rlower=relativedelta(days=0),
+                rupper=relativedelta(days=6),
+                requisitions=requisitions,
+                crfs=crfs,
+                crfs_missed=crfs_missed,
+                facility_name="7-day-clinic",
+            )
+        )
+    for visit in visits:
+        schedule2.add_visit(visit)
+
+    visit_schedule2.add_schedule(schedule2)
+    return visit_schedule2
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule3.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule5.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,72 @@
 from dateutil.relativedelta import relativedelta
 from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.visit import Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
-from .crfs import crfs, crfs_missed, requisitions
+from edc_appointment_app.consents import consent_v1
+from edc_appointment_app.visit_schedule.crfs import crfs, crfs_missed
 
-visit_schedule3 = VisitSchedule(
-    name="visit_schedule3",
-    offstudy_model="edc_appointment_app.subjectoffstudy",
-    death_report_model="edc_appointment_app.deathreport",
-)
-
-schedule3 = Schedule(
-    name="three_monthly_schedule",
-    onschedule_model="edc_appointment_app.onschedulethree",
-    offschedule_model="edc_appointment_app.offschedulethree",
-    appointment_model="edc_appointment.appointment",
-    consent_model="edc_appointment_app.subjectconsent",
-)
-
-visits = [
-    Visit(
-        code="1000",
-        title="Baseline",
-        timepoint=0,
-        rbase=relativedelta(days=0),
-        rlower=relativedelta(days=0),
-        rupper=relativedelta(days=0),
-        requisitions=requisitions,
-        crfs=crfs,
-        crfs_missed=crfs_missed,
-        facility_name="7-day-clinic",
+
+def get_visit_schedule5() -> VisitSchedule:
+    visit_schedule5 = VisitSchedule(
+        name="visit_schedule5",
+        offstudy_model="edc_appointment_app.subjectoffstudy",
+        death_report_model="edc_appointment_app.deathreport",
+    )
+
+    schedule5 = Schedule(
+        name="monthly_schedule",
+        onschedule_model="edc_appointment_app.onschedulethree",
+        offschedule_model="edc_appointment_app.offschedulethree",
+        appointment_model="edc_appointment.appointment",
+        consent_definitions=[consent_v1],
     )
-]
-for index, visit_code in [(3, "1030"), (6, "1060"), (9, "1090"), (12, "1120")]:
-    visits.append(
+
+    visits = [
         Visit(
-            code=visit_code,
-            title=f"Month {index}",
-            timepoint=index,
-            rbase=relativedelta(months=index),
-            rlower=relativedelta(days=14),
-            rupper=relativedelta(days=45),
-            requisitions=requisitions,
+            code="1000",
+            title="Baseline",
+            timepoint=0,
+            rbase=relativedelta(days=0),
+            rlower=relativedelta(days=0),
+            rupper=relativedelta(days=0),
+            add_window_gap_to_lower=True,
+            requisitions=None,
             crfs=crfs,
             crfs_missed=crfs_missed,
             facility_name="7-day-clinic",
-            allow_unscheduled=True,
         )
-    )
-for visit in visits:
-    schedule3.add_visit(visit)
+    ]
+    for index, visit_code in [
+        (1, "1010"),
+        (2, "1020"),
+        (3, "1030"),
+        (4, "1040"),
+        (5, "1050"),
+        (6, "1060"),
+        (7, "1070"),
+        (8, "1080"),
+        (9, "1090"),
+    ]:
+        visits.append(
+            Visit(
+                code=visit_code,
+                title=f"Month {index}",
+                timepoint=index,
+                rbase=relativedelta(months=index),
+                rlower=relativedelta(days=15),
+                rupper=relativedelta(days=15),
+                add_window_gap_to_lower=True,
+                max_window_gap_to_lower=None,
+                requisitions=None,
+                crfs=crfs,
+                crfs_missed=crfs_missed,
+                facility_name="7-day-clinic",
+                allow_unscheduled=True,
+            )
+        )
+    for visit in visits:
+        schedule5.add_visit(visit)
 
-visit_schedule3.add_schedule(schedule3)
+    visit_schedule5.add_schedule(schedule5)
+    return visit_schedule5
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule4.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule3.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 from dateutil.relativedelta import relativedelta
 from edc_visit_schedule.schedule import Schedule
 from edc_visit_schedule.visit import Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
-from edc_appointment_app.visit_schedule.crfs import crfs, crfs_missed
+from ..consents import consent_v1
+from .crfs import crfs, crfs_missed, requisitions
 
-visit_schedule4 = VisitSchedule(
-    name="visit_schedule4",
-    offstudy_model="edc_appointment_app.subjectoffstudy",
-    death_report_model="edc_appointment_app.deathreport",
-)
-
-schedule4 = Schedule(
-    name="three_monthly_schedule",
-    onschedule_model="edc_appointment_app.onschedulethree",
-    offschedule_model="edc_appointment_app.offschedulethree",
-    appointment_model="edc_appointment.appointment",
-    consent_model="edc_appointment_app.subjectconsent",
-)
-
-visits = [
-    Visit(
-        code="1000",
-        title="Baseline",
-        timepoint=0,
-        rbase=relativedelta(days=0),
-        rlower=relativedelta(days=0),
-        rupper=relativedelta(days=0),
-        add_window_gap_to_lower=True,
-        requisitions=None,
-        crfs=crfs,
-        crfs_missed=crfs_missed,
-        facility_name="7-day-clinic",
+
+def get_visit_schedule3() -> VisitSchedule:
+    visit_schedule3 = VisitSchedule(
+        name="visit_schedule3",
+        offstudy_model="edc_appointment_app.subjectoffstudy",
+        death_report_model="edc_appointment_app.deathreport",
+    )
+
+    schedule3 = Schedule(
+        name="three_monthly_schedule",
+        onschedule_model="edc_appointment_app.onschedulethree",
+        offschedule_model="edc_appointment_app.offschedulethree",
+        appointment_model="edc_appointment.appointment",
+        consent_definitions=[consent_v1],
     )
-]
-for index, visit_code in [(3, "1030"), (6, "1060"), (9, "1090"), (12, "1120")]:
-    visits.append(
+
+    visits = [
         Visit(
-            code=visit_code,
-            title=f"Month {index}",
-            timepoint=index,
-            rbase=relativedelta(months=index),
-            rlower=relativedelta(days=15),
-            rupper=relativedelta(days=15),
-            add_window_gap_to_lower=True,
-            max_window_gap_to_lower=None,
-            requisitions=None,
+            code="1000",
+            title="Baseline",
+            timepoint=0,
+            rbase=relativedelta(days=0),
+            rlower=relativedelta(days=0),
+            rupper=relativedelta(days=0),
+            requisitions=requisitions,
             crfs=crfs,
             crfs_missed=crfs_missed,
             facility_name="7-day-clinic",
-            allow_unscheduled=True,
         )
-    )
-for visit in visits:
-    schedule4.add_visit(visit)
+    ]
+    for index, visit_code in [(3, "1030"), (6, "1060"), (9, "1090"), (12, "1120")]:
+        visits.append(
+            Visit(
+                code=visit_code,
+                title=f"Month {index}",
+                timepoint=index,
+                rbase=relativedelta(months=index),
+                rlower=relativedelta(days=14),
+                rupper=relativedelta(days=45),
+                requisitions=requisitions,
+                crfs=crfs,
+                crfs_missed=crfs_missed,
+                facility_name="7-day-clinic",
+                allow_unscheduled=True,
+            )
+        )
+    for visit in visits:
+        schedule3.add_visit(visit)
 
-visit_schedule4.add_schedule(schedule4)
+    visit_schedule3.add_schedule(schedule3)
+    return visit_schedule3
```

### Comparing `edc-appointment-0.4.8/edc_appointment_app/visit_schedule/visit_schedule5.py` & `edc-appointment-0.4.9/edc_appointment_app/visit_schedule/visit_schedule6.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,93 @@
 from dateutil.relativedelta import relativedelta
+from edc_visit_schedule.constants import MONTH0, MONTH1, MONTH2, MONTH3, MONTH4
 from edc_visit_schedule.schedule import Schedule
-from edc_visit_schedule.visit import Visit
+from edc_visit_schedule.visit import Crf, CrfCollection, Visit
 from edc_visit_schedule.visit_schedule import VisitSchedule
 
-from edc_appointment_app.visit_schedule.crfs import crfs, crfs_missed
+from edc_appointment_app.consents import consent_v1
 
-visit_schedule5 = VisitSchedule(
-    name="visit_schedule5",
-    offstudy_model="edc_appointment_app.subjectoffstudy",
-    death_report_model="edc_appointment_app.deathreport",
-)
-
-schedule5 = Schedule(
-    name="monthly_schedule",
-    onschedule_model="edc_appointment_app.onschedulethree",
-    offschedule_model="edc_appointment_app.offschedulethree",
-    appointment_model="edc_appointment.appointment",
-    consent_model="edc_appointment_app.subjectconsent",
-)
-
-visits = [
-    Visit(
-        code="1000",
-        title="Baseline",
+
+def get_visit_schedule6() -> VisitSchedule:
+    app_label = "edc_appointment_app"
+
+    crfs = CrfCollection(
+        Crf(show_order=1, model=f"{app_label}.nextappointmentcrf", required=True),
+    )
+
+    visit0 = Visit(
+        code=MONTH0,
+        title=MONTH0,
         timepoint=0,
         rbase=relativedelta(days=0),
         rlower=relativedelta(days=0),
-        rupper=relativedelta(days=0),
-        add_window_gap_to_lower=True,
-        requisitions=None,
+        rupper=relativedelta(days=6),
+        crfs=crfs,
+        facility_name="5-day-clinic",
+    )
+
+    visit1 = Visit(
+        code=MONTH1,
+        title=MONTH1,
+        timepoint=1,
+        rbase=relativedelta(months=1),
+        rlower=relativedelta(days=0),
+        rupper=relativedelta(days=6),
+        crfs=crfs,
+        facility_name="5-day-clinic",
+    )
+
+    visit2 = Visit(
+        code=MONTH2,
+        title=MONTH2,
+        timepoint=2,
+        rbase=relativedelta(months=2),
+        rlower=relativedelta(days=0),
+        rupper=relativedelta(days=6),
         crfs=crfs,
-        crfs_missed=crfs_missed,
-        facility_name="7-day-clinic",
+        facility_name="5-day-clinic",
     )
-]
-for index, visit_code in [
-    (1, "1010"),
-    (2, "1020"),
-    (3, "1030"),
-    (4, "1040"),
-    (5, "1050"),
-    (6, "1060"),
-    (7, "1070"),
-    (8, "1080"),
-    (9, "1090"),
-]:
-    visits.append(
-        Visit(
-            code=visit_code,
-            title=f"Month {index}",
-            timepoint=index,
-            rbase=relativedelta(months=index),
-            rlower=relativedelta(days=15),
-            rupper=relativedelta(days=15),
-            add_window_gap_to_lower=True,
-            max_window_gap_to_lower=None,
-            requisitions=None,
-            crfs=crfs,
-            crfs_missed=crfs_missed,
-            facility_name="7-day-clinic",
-            allow_unscheduled=True,
-        )
+
+    visit3 = Visit(
+        code=MONTH3,
+        title=MONTH3,
+        timepoint=3,
+        rbase=relativedelta(months=3),
+        rlower=relativedelta(days=0),
+        rupper=relativedelta(days=6),
+        crfs=crfs,
+        facility_name="5-day-clinic",
+    )
+
+    visit4 = Visit(
+        code=MONTH4,
+        title=MONTH4,
+        timepoint=4,
+        rbase=relativedelta(months=4),
+        rlower=relativedelta(days=0),
+        rupper=relativedelta(days=6),
+        crfs=crfs,
+        facility_name="5-day-clinic",
+    )
+
+    schedule = Schedule(
+        name="schedule6",
+        onschedule_model=f"{app_label}.onschedulesix",
+        offschedule_model=f"{app_label}.offschedulesix",
+        consent_definitions=[consent_v1],
+        appointment_model="edc_appointment.appointment",
+    )
+
+    schedule.add_visit(visit0)
+    schedule.add_visit(visit1)
+    schedule.add_visit(visit2)
+    schedule.add_visit(visit3)
+    schedule.add_visit(visit4)
+
+    visit_schedule6 = VisitSchedule(
+        name="visit_schedule6",
+        offstudy_model=f"{app_label}.subjectoffstudy",
+        death_report_model=f"{app_label}.deathreport",
     )
-for visit in visits:
-    schedule5.add_visit(visit)
 
-visit_schedule5.add_schedule(schedule5)
+    visit_schedule6.add_schedule(schedule)
+    return visit_schedule6
```

### Comparing `edc-appointment-0.4.8/pyproject.toml` & `edc-appointment-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-appointment-0.4.8/runtests.py` & `edc-appointment-0.4.9/runtests.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         "django.contrib.sessions",
         "django.contrib.messages",
         "django.contrib.staticfiles",
         "django.contrib.sites",
         "django_crypto_fields.apps.AppConfig",
         "django_revision.apps.AppConfig",
         "multisite",
+        "edc_sites.apps.AppConfig",
         "edc_auth.apps.AppConfig",
         "edc_action_item.apps.AppConfig",
         "edc_offstudy.apps.AppConfig",
         "edc_consent.apps.AppConfig",
         "edc_crf.apps.AppConfig",
         "edc_dashboard.apps.AppConfig",
         "edc_data_manager.apps.AppConfig",
@@ -58,15 +59,14 @@
         "edc_model_admin.apps.AppConfig",
         "edc_navbar.apps.AppConfig",
         "edc_protocol.apps.AppConfig",
         "edc_randomization.apps.AppConfig",
         "edc_registration.apps.AppConfig",
         "edc_notification.apps.AppConfig",
         "edc_review_dashboard.apps.AppConfig",
-        "edc_sites.apps.AppConfig",
         "edc_timepoint.apps.AppConfig",
         "edc_visit_schedule.apps.AppConfig",
         "edc_visit_tracking.apps.AppConfig",
         "edc_appointment.apps.AppConfig",
         "edc_appointment_app.apps.AppConfig",
     ],
     add_dashboard_middleware=True,
```

### Comparing `edc-appointment-0.4.8/setup.cfg` & `edc-appointment-0.4.9/setup.cfg`

 * *Files identical despite different names*

