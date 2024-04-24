# Comparing `tmp/fastlifeweb-0.4.1.tar.gz` & `tmp/fastlifeweb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastlifeweb-0.4.1.tar", max compression
+gzip compressed data, was "fastlifeweb-0.5.0.tar", max compression
```

## Comparing `fastlifeweb-0.4.1.tar` & `fastlifeweb-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.4.1/LICENSE
--rw-r--r--   0        0        0      510 2024-04-13 13:57:35.096106 fastlifeweb-0.4.1/README.md
--rw-r--r--   0        0        0     2090 2024-04-20 17:20:30.931598 fastlifeweb-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      312 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/__init__.py
--rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.4.1/src/fastlife/configurator/__init__.py
--rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.4.1/src/fastlife/configurator/base.py
--rw-r--r--   0        0        0     5740 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/configurator/configurator.py
--rw-r--r--   0        0        0     1463 2024-04-13 13:57:35.099439 fastlifeweb-0.4.1/src/fastlife/configurator/registry.py
--rw-r--r--   0        0        0     1489 2024-04-13 13:57:35.099439 fastlifeweb-0.4.1/src/fastlife/configurator/settings.py
--rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.4.1/src/fastlife/py.typed
--rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.4.1/src/fastlife/request/__init__.py
--rw-r--r--   0        0        0     3642 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/request/form_data.py
--rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.4.1/src/fastlife/security/__init__.py
--rw-r--r--   0        0        0     1025 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/security/csrf.py
--rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.4.1/src/fastlife/security/policy.py
--rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.4.1/src/fastlife/session/__init__.py
--rw-r--r--   0        0        0     3049 2024-04-19 06:48:48.276132 fastlifeweb-0.4.1/src/fastlife/session/middleware.py
--rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.4.1/src/fastlife/session/serializer.py
--rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/shared_utils/__init__.py
--rw-r--r--   0        0        0      466 2023-11-25 15:57:32.200572 fastlifeweb-0.4.1/src/fastlife/shared_utils/infer.py
--rw-r--r--   0        0        0     1410 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/shared_utils/resolver.py
--rw-r--r--   0        0        0      677 2024-04-13 13:57:35.099439 fastlifeweb-0.4.1/src/fastlife/templates/A.jinja
--rw-r--r--   0        0        0     1137 2024-04-13 13:57:35.099439 fastlifeweb-0.4.1/src/fastlife/templates/Button.jinja
--rw-r--r--   0        0        0      366 2024-04-15 06:41:03.874701 fastlifeweb-0.4.1/src/fastlife/templates/Checkbox.jinja
--rw-r--r--   0        0        0       59 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/CsrfToken.jinja
--rw-r--r--   0        0        0      367 2024-04-20 12:30:01.651834 fastlifeweb-0.4.1/src/fastlife/templates/Form.jinja
--rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H1.jinja
--rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H2.jinja
--rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H3.jinja
--rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H4.jinja
--rw-r--r--   0        0        0      193 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H5.jinja
--rw-r--r--   0        0        0      191 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/H6.jinja
--rw-r--r--   0        0        0      120 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/templates/Hidden.jinja
--rw-r--r--   0        0        0      638 2024-04-14 21:06:08.222497 fastlifeweb-0.4.1/src/fastlife/templates/Input.jinja
--rw-r--r--   0        0        0      170 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/Label.jinja
--rw-r--r--   0        0        0      121 2024-04-15 06:29:06.881534 fastlifeweb-0.4.1/src/fastlife/templates/Option.jinja
--rw-r--r--   0        0        0      164 2024-04-13 13:57:35.102773 fastlifeweb-0.4.1/src/fastlife/templates/P.jinja
--rw-r--r--   0        0        0      723 2024-04-13 13:57:35.106106 fastlifeweb-0.4.1/src/fastlife/templates/Radio.jinja
--rw-r--r--   0        0        0      480 2024-04-20 16:07:29.325194 fastlifeweb-0.4.1/src/fastlife/templates/Select.jinja
--rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/templates/__init__.py
--rw-r--r--   0        0        0      298 2024-04-15 06:38:03.760573 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Boolean.jinja
--rw-r--r--   0        0        0      500 2024-04-15 06:29:02.724849 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Dropdown.jinja
--rw-r--r--   0        0        0       83 2024-03-30 15:07:08.088027 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Hidden.jinja
--rw-r--r--   0        0        0      123 2024-04-13 13:57:35.106106 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Hint.jinja
--rw-r--r--   0        0        0      449 2024-04-13 13:57:35.106106 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Model.jinja
--rw-r--r--   0        0        0     1380 2024-04-14 07:07:58.770652 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Sequence.jinja
--rw-r--r--   0        0        0      402 2024-04-13 13:57:35.106106 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Text.jinja
--rw-r--r--   0        0        0      950 2024-04-15 05:32:37.810352 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Union.jinja
--rw-r--r--   0        0        0      287 2024-03-30 15:07:08.091360 fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Widget.jinja
--rw-r--r--   0        0        0      234 2024-04-13 13:57:35.106106 fastlifeweb-0.4.1/src/fastlife/templating/__init__.py
--rw-r--r--   0        0        0     1378 2024-04-13 13:57:35.109439 fastlifeweb-0.4.1/src/fastlife/templating/binding.py
--rw-r--r--   0        0        0      181 2024-04-13 13:57:35.109439 fastlifeweb-0.4.1/src/fastlife/templating/renderer/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-20 17:17:37.757534 fastlifeweb-0.4.1/src/fastlife/templating/renderer/abstract.py
--rw-r--r--   0        0        0     3458 2024-04-20 17:17:57.137615 fastlifeweb-0.4.1/src/fastlife/templating/renderer/jinjax.py
--rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/__init__.py
--rw-r--r--   0        0        0     2769 2024-04-20 17:11:26.562688 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/base.py
--rw-r--r--   0        0        0      468 2024-04-14 07:07:58.773985 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/boolean.py
--rw-r--r--   0        0        0      901 2024-04-14 07:07:58.773985 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/dropdown.py
--rw-r--r--   0        0        0    10335 2024-04-15 06:46:25.562707 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/factory.py
--rw-r--r--   0        0        0      308 2024-04-14 07:07:58.773985 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/hidden.py
--rw-r--r--   0        0        0      986 2024-04-20 17:18:08.717664 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/model.py
--rw-r--r--   0        0        0     1347 2024-04-14 07:07:58.773985 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/sequence.py
--rw-r--r--   0        0        0      819 2024-04-14 07:07:58.773985 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/text.py
--rw-r--r--   0        0        0     1689 2024-04-14 07:07:58.777319 fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/union.py
--rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.4.1/src/fastlife/testing/__init__.py
--rw-r--r--   0        0        0    16404 2024-04-20 07:26:17.322149 fastlifeweb-0.4.1/src/fastlife/testing/testclient.py
--rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.4.1/src/fastlife/views/__init__.py
--rw-r--r--   0        0        0     1092 2024-04-13 13:57:35.112773 fastlifeweb-0.4.1/src/fastlife/views/pydantic_form.py
--rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 fastlifeweb-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-01-05 08:56:46.068218 fastlifeweb-0.5.0/LICENSE
+-rw-r--r--   0        0        0      510 2024-04-13 13:57:35.096106 fastlifeweb-0.5.0/README.md
+-rw-r--r--   0        0        0     2090 2024-04-24 07:06:46.703181 fastlifeweb-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      312 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/__init__.py
+-rw-r--r--   0        0        0       91 2024-01-14 12:49:19.832886 fastlifeweb-0.5.0/src/fastlife/configurator/__init__.py
+-rw-r--r--   0        0        0      216 2024-03-29 07:03:39.778516 fastlifeweb-0.5.0/src/fastlife/configurator/base.py
+-rw-r--r--   0        0        0     5740 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/configurator/configurator.py
+-rw-r--r--   0        0        0     1463 2024-04-13 13:57:35.099439 fastlifeweb-0.5.0/src/fastlife/configurator/registry.py
+-rw-r--r--   0        0        0     1489 2024-04-13 13:57:35.099439 fastlifeweb-0.5.0/src/fastlife/configurator/settings.py
+-rw-r--r--   0        0        0        0 2023-09-22 06:52:58.847518 fastlifeweb-0.5.0/src/fastlife/py.typed
+-rw-r--r--   0        0        0        0 2023-09-18 06:50:01.267211 fastlifeweb-0.5.0/src/fastlife/request/__init__.py
+-rw-r--r--   0        0        0     4049 2024-04-23 21:07:54.516620 fastlifeweb-0.5.0/src/fastlife/request/form_data.py
+-rw-r--r--   0        0        0        0 2024-01-14 12:49:19.832886 fastlifeweb-0.5.0/src/fastlife/security/__init__.py
+-rw-r--r--   0        0        0     1025 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/security/csrf.py
+-rw-r--r--   0        0        0      509 2024-03-29 07:03:39.778516 fastlifeweb-0.5.0/src/fastlife/security/policy.py
+-rw-r--r--   0        0        0      838 2024-03-29 07:03:39.778516 fastlifeweb-0.5.0/src/fastlife/session/__init__.py
+-rw-r--r--   0        0        0     3049 2024-04-19 06:48:48.276132 fastlifeweb-0.5.0/src/fastlife/session/middleware.py
+-rw-r--r--   0        0        0     1458 2024-03-29 07:03:39.778516 fastlifeweb-0.5.0/src/fastlife/session/serializer.py
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/shared_utils/__init__.py
+-rw-r--r--   0        0        0      466 2023-11-25 15:57:32.200572 fastlifeweb-0.5.0/src/fastlife/shared_utils/infer.py
+-rw-r--r--   0        0        0     1410 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/shared_utils/resolver.py
+-rw-r--r--   0        0        0      677 2024-04-13 13:57:35.099439 fastlifeweb-0.5.0/src/fastlife/templates/A.jinja
+-rw-r--r--   0        0        0     1137 2024-04-13 13:57:35.099439 fastlifeweb-0.5.0/src/fastlife/templates/Button.jinja
+-rw-r--r--   0        0        0      447 2024-04-21 09:51:45.697435 fastlifeweb-0.5.0/src/fastlife/templates/Checkbox.jinja
+-rw-r--r--   0        0        0       59 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/CsrfToken.jinja
+-rw-r--r--   0        0        0      367 2024-04-20 12:30:01.651834 fastlifeweb-0.5.0/src/fastlife/templates/Form.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H1.jinja
+-rw-r--r--   0        0        0      196 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H2.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H3.jinja
+-rw-r--r--   0        0        0      195 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H4.jinja
+-rw-r--r--   0        0        0      193 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H5.jinja
+-rw-r--r--   0        0        0      191 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/H6.jinja
+-rw-r--r--   0        0        0      120 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/templates/Hidden.jinja
+-rw-r--r--   0        0        0      638 2024-04-14 21:06:08.222497 fastlifeweb-0.5.0/src/fastlife/templates/Input.jinja
+-rw-r--r--   0        0        0      170 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/Label.jinja
+-rw-r--r--   0        0        0      121 2024-04-15 06:29:06.881534 fastlifeweb-0.5.0/src/fastlife/templates/Option.jinja
+-rw-r--r--   0        0        0      164 2024-04-13 13:57:35.102773 fastlifeweb-0.5.0/src/fastlife/templates/P.jinja
+-rw-r--r--   0        0        0      723 2024-04-13 13:57:35.106106 fastlifeweb-0.5.0/src/fastlife/templates/Radio.jinja
+-rw-r--r--   0        0        0      480 2024-04-20 16:07:29.325194 fastlifeweb-0.5.0/src/fastlife/templates/Select.jinja
+-rw-r--r--   0        0        0        0 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/templates/__init__.py
+-rw-r--r--   0        0        0      281 2024-04-21 07:55:52.000197 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Boolean.jinja
+-rw-r--r--   0        0        0      665 2024-04-24 07:03:20.679414 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Checklist.jinja
+-rw-r--r--   0        0        0      500 2024-04-15 06:29:02.724849 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Dropdown.jinja
+-rw-r--r--   0        0        0       83 2024-03-30 15:07:08.088027 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Hidden.jinja
+-rw-r--r--   0        0        0      123 2024-04-13 13:57:35.106106 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Hint.jinja
+-rw-r--r--   0        0        0      449 2024-04-13 13:57:35.106106 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Model.jinja
+-rw-r--r--   0        0        0     1380 2024-04-14 07:07:58.770652 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Sequence.jinja
+-rw-r--r--   0        0        0      402 2024-04-13 13:57:35.106106 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Text.jinja
+-rw-r--r--   0        0        0      950 2024-04-15 05:32:37.810352 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Union.jinja
+-rw-r--r--   0        0        0      287 2024-04-24 06:47:08.537681 fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Widget.jinja
+-rw-r--r--   0        0        0      234 2024-04-13 13:57:35.106106 fastlifeweb-0.5.0/src/fastlife/templating/__init__.py
+-rw-r--r--   0        0        0     1378 2024-04-13 13:57:35.109439 fastlifeweb-0.5.0/src/fastlife/templating/binding.py
+-rw-r--r--   0        0        0      181 2024-04-13 13:57:35.109439 fastlifeweb-0.5.0/src/fastlife/templating/renderer/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-20 17:17:37.757534 fastlifeweb-0.5.0/src/fastlife/templating/renderer/abstract.py
+-rw-r--r--   0        0        0     3458 2024-04-20 17:17:57.137615 fastlifeweb-0.5.0/src/fastlife/templating/renderer/jinjax.py
+-rw-r--r--   0        0        0        0 2023-12-02 23:16:17.801084 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-20 17:11:26.562688 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/base.py
+-rw-r--r--   0        0        0      436 2024-04-24 05:54:40.214145 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/boolean.py
+-rw-r--r--   0        0        0      770 2024-04-24 07:05:59.163085 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/checklist.py
+-rw-r--r--   0        0        0      901 2024-04-14 07:07:58.773985 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/dropdown.py
+-rw-r--r--   0        0        0    12850 2024-04-24 06:47:47.057723 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/factory.py
+-rw-r--r--   0        0        0      308 2024-04-14 07:07:58.773985 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/hidden.py
+-rw-r--r--   0        0        0      986 2024-04-20 17:18:08.717664 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/model.py
+-rw-r--r--   0        0        0     1347 2024-04-14 07:07:58.773985 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/sequence.py
+-rw-r--r--   0        0        0      819 2024-04-14 07:07:58.773985 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/text.py
+-rw-r--r--   0        0        0     1689 2024-04-14 07:07:58.777319 fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/union.py
+-rw-r--r--   0        0        0       67 2023-09-16 21:42:04.218390 fastlifeweb-0.5.0/src/fastlife/testing/__init__.py
+-rw-r--r--   0        0        0    16404 2024-04-20 07:26:17.322149 fastlifeweb-0.5.0/src/fastlife/testing/testclient.py
+-rw-r--r--   0        0        0      154 2024-01-14 12:49:19.836219 fastlifeweb-0.5.0/src/fastlife/views/__init__.py
+-rw-r--r--   0        0        0     1092 2024-04-13 13:57:35.112773 fastlifeweb-0.5.0/src/fastlife/views/pydantic_form.py
+-rw-r--r--   0        0        0     1833 1970-01-01 00:00:00.000000 fastlifeweb-0.5.0/PKG-INFO
```

### Comparing `fastlifeweb-0.4.1/LICENSE` & `fastlifeweb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/pyproject.toml` & `fastlifeweb-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   "Development Status :: 4 - Beta",
   "Framework :: AsyncIO",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet :: WWW/HTTP",
 ]
-version = "0.4.1"
+version = "0.5.0"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 beautifulsoup4 = {version = "^4.12.2", extras = ["testing"]}
 fastapi = "^0.110.0"
 jinjax = "^0.32"
 pydantic = "^2.3.0"
```

### Comparing `fastlifeweb-0.4.1/src/fastlife/configurator/configurator.py` & `fastlifeweb-0.5.0/src/fastlife/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/configurator/registry.py` & `fastlifeweb-0.5.0/src/fastlife/configurator/registry.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/configurator/settings.py` & `fastlifeweb-0.5.0/src/fastlife/configurator/settings.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/request/form_data.py` & `fastlifeweb-0.5.0/src/fastlife/request/form_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     flatten_input: Mapping[str, Any],
     unflattened_output: MutableMapping[str, Any] | MutableSequence[Any],
     level: int = 0,
     *,
     csrf_token_name: Optional[str] = None,
 ) -> Mapping[str, Any] | Sequence[Any]:
     # we sort to ensure that list index are ordered
-    formkeys = sorted(flatten_input.keys())
-    for key in formkeys:
+    # formkeys = sorted(flatten_input.keys())
+    for key in flatten_input:
         if csrf_token_name is not None and key == csrf_token_name:
             continue
         lkey, sep, rest = key.partition(".")
 
         if not sep:
             # this is a leaf
             if isinstance(unflattened_output, list):
@@ -74,16 +74,25 @@
     return unflattened_output
 
 
 async def unflatten_mapping_form_data(
     request: Request, reg: Registry
 ) -> Mapping[str, Any]:
     form_data = await request.form()
+    form_data_decode_list: MutableMapping[str, Any] = {}
+    for key, val in form_data.multi_items():
+        if key in form_data_decode_list:
+            if not isinstance(form_data_decode_list, list):
+                form_data_decode_list[key] = [form_data_decode_list[key]]
+            form_data_decode_list[key].append(val)
+        else:
+            form_data_decode_list[key] = val
+
     ret = unflatten_struct(
-        form_data, {}, csrf_token_name=reg.settings.csrf_token_name
+        form_data_decode_list, {}, csrf_token_name=reg.settings.csrf_token_name
     )  # type: ignore
     return ret  # type: ignore
 
 
 async def unflatten_sequence_form_data(
     request: Request, reg: Registry
 ) -> Sequence[str]:
```

### Comparing `fastlifeweb-0.4.1/src/fastlife/security/csrf.py` & `fastlifeweb-0.5.0/src/fastlife/security/csrf.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/session/__init__.py` & `fastlifeweb-0.5.0/src/fastlife/session/__init__.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/session/middleware.py` & `fastlifeweb-0.5.0/src/fastlife/session/middleware.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/session/serializer.py` & `fastlifeweb-0.5.0/src/fastlife/session/serializer.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/shared_utils/resolver.py` & `fastlifeweb-0.5.0/src/fastlife/shared_utils/resolver.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/A.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/A.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/Button.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/Button.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/Input.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/Input.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/Radio.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/Radio.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Sequence.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Sequence.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templates/pydantic_form/Union.jinja` & `fastlifeweb-0.5.0/src/fastlife/templates/pydantic_form/Union.jinja`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/binding.py` & `fastlifeweb-0.5.0/src/fastlife/templating/binding.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/abstract.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/abstract.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/jinjax.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/jinjax.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/base.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/base.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/dropdown.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/dropdown.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/factory.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import secrets
 from collections.abc import MutableSequence, Sequence
 from decimal import Decimal
+from enum import Enum
 from types import NoneType
 from typing import Any, Literal, Mapping, Optional, Type, cast, get_origin
 from uuid import UUID
 
 from markupsafe import Markup
 from pydantic import BaseModel, EmailStr, SecretStr, ValidationError
 from pydantic.fields import FieldInfo
 
 from fastlife.shared_utils.infer import is_complex_type, is_union
 from fastlife.templating.renderer.abstract import AbstractTemplateRenderer
 from fastlife.templating.renderer.widgets.boolean import BooleanWidget
+from fastlife.templating.renderer.widgets.checklist import Checkable, ChecklistWidget
 from fastlife.templating.renderer.widgets.dropdown import DropDownWidget
 from fastlife.templating.renderer.widgets.hidden import HiddenWidget
 from fastlife.templating.renderer.widgets.sequence import SequenceWidget
 
 from .base import Widget, get_title
 from .model import ModelWidget
 from .text import TextWidget
@@ -92,14 +94,20 @@
                 or type_origin is list
             ):
                 return self.build_sequence(name, typ, field, value, removable)
 
             if type_origin is Literal:
                 return self.build_literal(name, typ, field, value, removable)
 
+            if type_origin is set:
+                return self.build_set(name, typ, field, value, removable)
+
+        if issubclass(typ, Enum):  # if it raises here, the type_origin is unknown
+            return self.build_enum(name, typ, field, value, removable)
+
         if issubclass(typ, BaseModel):  # if it raises here, the type_origin is unknown
             return self.build_model(name, typ, field, value or {}, removable)
 
         if issubclass(typ, bool):
             return self.build_boolean(name, typ, field, value or False, removable)
 
         if issubclass(typ, EmailStr):  # type: ignore
@@ -224,14 +232,63 @@
             title=field.title if field else "",
             value=items,
             item_type=typ,  # type: ignore
             token=self.token,
             removable=removable,
         )
 
+    def build_set(
+        self,
+        field_name: str,
+        field_type: Type[Any],
+        field: Optional[FieldInfo],
+        value: Optional[Sequence[Any]],
+        removable: bool,
+    ) -> Widget[Any]:
+        choice_wrapper = field_type.__args__[0]
+        choices = []
+        choice_wrapper_origin = get_origin(choice_wrapper)
+        if choice_wrapper_origin:
+            if choice_wrapper_origin is Literal:
+                litchoice: list[str] = choice_wrapper.__args__  # type: ignore
+                choices = [
+                    Checkable(
+                        label=c,
+                        value=c,
+                        checked=c in value if value else False,  # type: ignore
+                        name=field_name,
+                        token=self.token,
+                    )
+                    for c in litchoice
+                ]
+
+            else:
+                raise NotImplementedError
+        elif issubclass(choice_wrapper, Enum):
+            choices = [
+                Checkable(
+                    label=e.value,
+                    value=e.name,
+                    checked=e.name in value if value else False,  # type: ignore
+                    name=field_name,
+                    token=self.token,
+                )
+                for e in choice_wrapper
+            ]
+        else:
+            raise NotImplementedError
+
+        return ChecklistWidget(
+            field_name,
+            title=field.title if field else "",
+            token=self.token,
+            value=choices,
+            removable=removable,
+        )
+
     def build_boolean(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: bool,
         removable: bool,
@@ -302,14 +359,32 @@
             options=choices,
             removable=removable,
             title=field.title if field else "",
             token=self.token,
             value=str(value),
         )
 
+    def build_enum(
+        self,
+        field_name: str,
+        field_type: Type[Any],  # an enum subclass
+        field: FieldInfo | None,
+        value: str | int | float,
+        removable: bool,
+    ) -> Widget[Any]:
+        options = [(item.name, item.value) for item in field_type]  # type: ignore
+        return DropDownWidget(
+            field_name,
+            options=options,  # type: ignore
+            removable=removable,
+            title=field.title if field else "",
+            token=self.token,
+            value=str(value),
+        )
+
     def build_simpletype(
         self,
         field_name: str,
         field_type: Type[Any],
         field: FieldInfo | None,
         value: str | int | float,
         removable: bool,
```

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/model.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/model.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/sequence.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/sequence.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/text.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/text.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/templating/renderer/widgets/union.py` & `fastlifeweb-0.5.0/src/fastlife/templating/renderer/widgets/union.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/testing/testclient.py` & `fastlifeweb-0.5.0/src/fastlife/testing/testclient.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/src/fastlife/views/pydantic_form.py` & `fastlifeweb-0.5.0/src/fastlife/views/pydantic_form.py`

 * *Files identical despite different names*

### Comparing `fastlifeweb-0.4.1/PKG-INFO` & `fastlifeweb-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastlifeweb
-Version: 0.4.1
+Version: 0.5.0
 Summary: High-level web framework
 Home-page: https://github.com/mardiros/fastlife
 License: BSD-derived
 Author: Guillaume Gauvrit
 Author-email: guillaume@gauvr.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

