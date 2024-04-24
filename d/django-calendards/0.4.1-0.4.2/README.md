# Comparing `tmp/django_calendards-0.4.1.tar.gz` & `tmp/django_calendards-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_calendards-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_calendards-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_calendards-0.4.1.tar` & `django_calendards-0.4.2.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0     6148 2024-03-21 00:01:30.234485 django_calendards-0.4.1/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-19 23:57:37.500103 django_calendards-0.4.1/.gitattributes
--rw-r--r--   0        0        0       52 2024-03-19 23:59:27.327559 django_calendards-0.4.1/.idea/.gitignore
--rw-r--r--   0        0        0      407 2024-03-19 23:59:27.160455 django_calendards-0.4.1/.idea/django-calendards.iml
--rw-r--r--   0        0        0      174 2024-03-19 23:59:27.191851 django_calendards-0.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      425 2024-03-20 00:29:01.638630 django_calendards-0.4.1/.idea/misc.xml
--rw-r--r--   0        0        0      286 2024-03-19 23:59:27.173072 django_calendards-0.4.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-19 23:59:27.197111 django_calendards-0.4.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_calendards-0.4.1/LICENSE
--rw-r--r--   0        0        0      987 2024-03-20 03:11:20.036924 django_calendards-0.4.1/README.md
--rw-r--r--   0        0        0        0 2024-03-12 06:31:16.606654 django_calendards-0.4.1/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 00:02:36.853233 django_calendards-0.4.1/django_calendards/__init__.py
--rw-r--r--   0        0        0      338 2024-03-20 00:29:14.195262 django_calendards-0.4.1/django_calendards/admin.py
--rw-r--r--   0        0        0      165 2024-03-20 00:02:36.854696 django_calendards-0.4.1/django_calendards/apps.py
--rw-r--r--   0        0        0     1250 2024-03-20 01:00:38.697855 django_calendards-0.4.1/django_calendards/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-20 00:02:36.855167 django_calendards-0.4.1/django_calendards/migrations/__init__.py
--rw-r--r--   0        0        0      681 2024-03-20 00:29:31.895640 django_calendards-0.4.1/django_calendards/models.py
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/LICENSE.txt
--rw-r--r--   0        0        0      256 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/README.md
--rw-r--r--   0        0        0      813 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.css
--rw-r--r--   0        0        0      351 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.d.ts
--rw-r--r--   0        0        0     3042 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.esm.js
--rw-r--r--   0        0        0     3755 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.js
--rw-r--r--   0        0        0      416 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.css
--rw-r--r--   0        0        0     1650 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.js
--rw-r--r--   0        0        0      876 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/LICENSE.txt
--rw-r--r--   0        0        0      271 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/README.md
--rw-r--r--   0        0        0    38672 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.js
--rw-r--r--   0        0        0    18513 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.min.js
--rw-r--r--   0        0        0      950 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/af.js
--rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-dz.js
--rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-kw.js
--rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ly.js
--rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ma.js
--rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-sa.js
--rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-tn.js
--rw-r--r--   0        0        0     1000 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar.js
--rw-r--r--   0        0        0     1009 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/az.js
--rw-r--r--   0        0        0     1020 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bg.js
--rw-r--r--   0        0        0      998 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bs.js
--rw-r--r--   0        0        0      944 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ca.js
--rw-r--r--   0        0        0      994 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/cs.js
--rw-r--r--   0        0        0      935 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/da.js
--rw-r--r--   0        0        0     1022 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/de.js
--rw-r--r--   0        0        0     1066 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/el.js
--rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-au.js
--rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-gb.js
--rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-nz.js
--rw-r--r--   0        0        0      941 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es-us.js
--rw-r--r--   0        0        0      931 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es.js
--rw-r--r--   0        0        0      997 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/et.js
--rw-r--r--   0        0        0      941 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/eu.js
--rw-r--r--   0        0        0     1050 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fa.js
--rw-r--r--   0        0        0      960 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fi.js
--rw-r--r--   0        0        0      878 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ca.js
--rw-r--r--   0        0        0     1006 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ch.js
--rw-r--r--   0        0        0      995 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr.js
--rw-r--r--   0        0        0      932 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/gl.js
--rw-r--r--   0        0        0      861 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/he.js
--rw-r--r--   0        0        0     1146 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hi.js
--rw-r--r--   0        0        0      994 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hr.js
--rw-r--r--   0        0        0      940 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hu.js
--rw-r--r--   0        0        0      949 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/id.js
--rw-r--r--   0        0        0      953 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/is.js
--rw-r--r--   0        0        0     1002 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/it.js
--rw-r--r--   0        0        0      866 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ja.js
--rw-r--r--   0        0        0     1055 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ka.js
--rw-r--r--   0        0        0     1057 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/kk.js
--rw-r--r--   0        0        0      802 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ko.js
--rw-r--r--   0        0        0      946 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lb.js
--rw-r--r--   0        0        0      948 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lt.js
--rw-r--r--   0        0        0      989 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lv.js
--rw-r--r--   0        0        0      936 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/mk.js
--rw-r--r--   0        0        0     1015 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ms.js
--rw-r--r--   0        0        0      928 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nb.js
--rw-r--r--   0        0        0      945 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nl.js
--rw-r--r--   0        0        0      930 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nn.js
--rw-r--r--   0        0        0      962 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pl.js
--rw-r--r--   0        0        0      871 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt-br.js
--rw-r--r--   0        0        0      939 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt.js
--rw-r--r--   0        0        0     1008 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ro.js
--rw-r--r--   0        0        0     1069 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ru.js
--rw-r--r--   0        0        0     1010 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sk.js
--rw-r--r--   0        0        0      940 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sl.js
--rw-r--r--   0        0        0     1002 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sq.js
--rw-r--r--   0        0        0     1077 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr-cyrl.js
--rw-r--r--   0        0        0      995 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr.js
--rw-r--r--   0        0        0      927 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sv.js
--rw-r--r--   0        0        0     1243 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/th.js
--rw-r--r--   0        0        0      933 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/tr.js
--rw-r--r--   0        0        0      633 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ug.js
--rw-r--r--   0        0        0     1100 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uk.js
--rw-r--r--   0        0        0      749 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uz.js
--rw-r--r--   0        0        0     1017 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/vi.js
--rw-r--r--   0        0        0     1114 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-cn.js
--rw-r--r--   0        0        0      814 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-tw.js
--rw-r--r--   0        0        0    27363 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.css
--rw-r--r--   0        0        0   119971 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.d.ts
--rw-r--r--   0        0        0   334647 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.esm.js
--rw-r--r--   0        0        0   373420 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.js
--rw-r--r--   0        0        0    14357 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.css
--rw-r--r--   0        0        0   127416 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.js
--rw-r--r--   0        0        0      822 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/LICENSE.txt
--rw-r--r--   0        0        0      257 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/README.md
--rw-r--r--   0        0        0     1807 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.css
--rw-r--r--   0        0        0    12587 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.d.ts
--rw-r--r--   0        0        0    75216 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.esm.js
--rw-r--r--   0        0        0    82087 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.js
--rw-r--r--   0        0        0     1004 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.css
--rw-r--r--   0        0        0    28238 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.js
--rw-r--r--   0        0        0      875 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/LICENSE.txt
--rw-r--r--   0        0        0      272 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/README.md
--rw-r--r--   0        0        0      599 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.d.ts
--rw-r--r--   0        0        0     6336 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.esm.js
--rw-r--r--   0        0        0     7367 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.js
--rw-r--r--   0        0        0     2600 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.min.js
--rw-r--r--   0        0        0      898 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/LICENSE.txt
--rw-r--r--   0        0        0      303 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/README.md
--rw-r--r--   0        0        0    13764 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.d.ts
--rw-r--r--   0        0        0    94523 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.esm.js
--rw-r--r--   0        0        0   103154 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.js
--rw-r--r--   0        0        0    36208 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.min.js
--rw-r--r--   0        0        0      925 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/LICENSE.txt
--rw-r--r--   0        0        0      248 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/README.md
--rw-r--r--   0        0        0     1938 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.css
--rw-r--r--   0        0        0     1635 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.d.ts
--rw-r--r--   0        0        0    14938 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.esm.js
--rw-r--r--   0        0        0    16587 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.js
--rw-r--r--   0        0        0     1102 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.css
--rw-r--r--   0        0        0     6551 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.js
--rw-r--r--   0        0        0      863 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/LICENSE.txt
--rw-r--r--   0        0        0      249 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/README.md
--rw-r--r--   0        0        0      580 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.d.ts
--rw-r--r--   0        0        0     5618 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.esm.js
--rw-r--r--   0        0        0     6672 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.js
--rw-r--r--   0        0        0     2603 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.min.js
--rw-r--r--   0        0        0      889 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/LICENSE.txt
--rw-r--r--   0        0        0      282 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/README.md
--rw-r--r--   0        0        0      387 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.d.ts
--rw-r--r--   0        0        0     2319 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.esm.js
--rw-r--r--   0        0        0     3014 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.js
--rw-r--r--   0        0        0     1255 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.min.js
--rw-r--r--   0        0        0      967 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/LICENSE.txt
--rw-r--r--   0        0        0      255 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/README.md
--rw-r--r--   0        0        0      526 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.d.ts
--rw-r--r--   0        0        0     3417 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.esm.js
--rw-r--r--   0        0        0     4253 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.js
--rw-r--r--   0        0        0     1634 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.min.js
--rw-r--r--   0        0        0      897 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/LICENSE.txt
--rw-r--r--   0        0        0      266 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/README.md
--rw-r--r--   0        0        0      245 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.d.ts
--rw-r--r--   0        0        0     4304 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.esm.js
--rw-r--r--   0        0        0     5169 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.js
--rw-r--r--   0        0        0     1681 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.min.js
--rw-r--r--   0        0        0      905 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/package.json
--rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/LICENSE.txt
--rw-r--r--   0        0        0      260 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/README.md
--rw-r--r--   0        0        0     7304 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.css
--rw-r--r--   0        0        0     9492 2020-05-28 07:18:24.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.d.ts
--rw-r--r--   0        0        0    65257 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.esm.js
--rw-r--r--   0        0        0    71134 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.js
--rw-r--r--   0        0        0     3377 2020-05-28 07:18:20.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.css
--rw-r--r--   0        0        0    25180 2020-05-28 07:18:28.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.js
--rw-r--r--   0        0        0      942 2020-05-28 07:18:18.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/package.json
--rw-r--r--   0        0        0   137525 2019-12-18 03:54:50.000000 django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/vendor/rrule.js
--rw-r--r--   0        0        0     1800 2024-04-12 07:02:53.713306 django_calendards-0.4.1/django_calendards/templates/django_calendards/calendards.html
--rw-r--r--   0        0        0     2183 2024-04-12 05:47:21.387698 django_calendards-0.4.1/django_calendards/templates/django_calendards/modalds.html
--rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_calendards-0.4.1/django_calendards/templatetags/__init__.py
--rw-r--r--   0        0        0     1293 2024-03-20 02:03:05.123543 django_calendards-0.4.1/django_calendards/templatetags/django_calendards_tags.py
--rw-r--r--   0        0        0       60 2024-03-20 00:02:36.855013 django_calendards-0.4.1/django_calendards/tests.py
--rw-r--r--   0        0        0       63 2024-03-20 00:02:36.853580 django_calendards-0.4.1/django_calendards/views.py
--rw-r--r--   0        0        0      637 2024-04-12 07:05:42.401070 django_calendards-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1303 1970-01-01 00:00:00.000000 django_calendards-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-03-21 00:01:30.234485 django_calendards-0.4.2/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-19 23:57:37.500103 django_calendards-0.4.2/.gitattributes
+-rw-r--r--   0        0        0       52 2024-03-19 23:59:27.327559 django_calendards-0.4.2/.idea/.gitignore
+-rw-r--r--   0        0        0      407 2024-03-19 23:59:27.160455 django_calendards-0.4.2/.idea/django-calendards.iml
+-rw-r--r--   0        0        0      174 2024-03-19 23:59:27.191851 django_calendards-0.4.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      425 2024-03-20 00:29:01.638630 django_calendards-0.4.2/.idea/misc.xml
+-rw-r--r--   0        0        0      286 2024-03-19 23:59:27.173072 django_calendards-0.4.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-19 23:59:27.197111 django_calendards-0.4.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_calendards-0.4.2/LICENSE
+-rw-r--r--   0        0        0      987 2024-03-20 03:11:20.036924 django_calendards-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-12 06:31:16.606654 django_calendards-0.4.2/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 00:02:36.853233 django_calendards-0.4.2/django_calendards/__init__.py
+-rw-r--r--   0        0        0      338 2024-03-20 00:29:14.195262 django_calendards-0.4.2/django_calendards/admin.py
+-rw-r--r--   0        0        0      165 2024-03-20 00:02:36.854696 django_calendards-0.4.2/django_calendards/apps.py
+-rw-r--r--   0        0        0     1250 2024-03-20 01:00:38.697855 django_calendards-0.4.2/django_calendards/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-20 00:02:36.855167 django_calendards-0.4.2/django_calendards/migrations/__init__.py
+-rw-r--r--   0        0        0      681 2024-03-20 00:29:31.895640 django_calendards-0.4.2/django_calendards/models.py
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/LICENSE.txt
+-rw-r--r--   0        0        0      256 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/README.md
+-rw-r--r--   0        0        0      813 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.css
+-rw-r--r--   0        0        0      351 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.d.ts
+-rw-r--r--   0        0        0     3042 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.esm.js
+-rw-r--r--   0        0        0     3755 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.js
+-rw-r--r--   0        0        0      416 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.css
+-rw-r--r--   0        0        0     1650 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.js
+-rw-r--r--   0        0        0      876 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/LICENSE.txt
+-rw-r--r--   0        0        0      271 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/README.md
+-rw-r--r--   0        0        0    38672 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.js
+-rw-r--r--   0        0        0    18513 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.min.js
+-rw-r--r--   0        0        0      950 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/af.js
+-rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-dz.js
+-rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-kw.js
+-rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ly.js
+-rw-r--r--   0        0        0     1013 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ma.js
+-rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-sa.js
+-rw-r--r--   0        0        0     1012 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-tn.js
+-rw-r--r--   0        0        0     1000 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar.js
+-rw-r--r--   0        0        0     1009 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/az.js
+-rw-r--r--   0        0        0     1020 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bg.js
+-rw-r--r--   0        0        0      998 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bs.js
+-rw-r--r--   0        0        0      944 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ca.js
+-rw-r--r--   0        0        0      994 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/cs.js
+-rw-r--r--   0        0        0      935 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/da.js
+-rw-r--r--   0        0        0     1022 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/de.js
+-rw-r--r--   0        0        0     1066 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/el.js
+-rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-au.js
+-rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-gb.js
+-rw-r--r--   0        0        0      576 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-nz.js
+-rw-r--r--   0        0        0      941 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es-us.js
+-rw-r--r--   0        0        0      931 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es.js
+-rw-r--r--   0        0        0      997 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/et.js
+-rw-r--r--   0        0        0      941 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/eu.js
+-rw-r--r--   0        0        0     1050 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fa.js
+-rw-r--r--   0        0        0      960 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fi.js
+-rw-r--r--   0        0        0      878 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ca.js
+-rw-r--r--   0        0        0     1006 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ch.js
+-rw-r--r--   0        0        0      995 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr.js
+-rw-r--r--   0        0        0      932 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/gl.js
+-rw-r--r--   0        0        0      861 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/he.js
+-rw-r--r--   0        0        0     1146 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hi.js
+-rw-r--r--   0        0        0      994 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hr.js
+-rw-r--r--   0        0        0      940 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hu.js
+-rw-r--r--   0        0        0      949 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/id.js
+-rw-r--r--   0        0        0      953 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/is.js
+-rw-r--r--   0        0        0     1002 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/it.js
+-rw-r--r--   0        0        0      866 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ja.js
+-rw-r--r--   0        0        0     1055 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ka.js
+-rw-r--r--   0        0        0     1057 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/kk.js
+-rw-r--r--   0        0        0      802 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ko.js
+-rw-r--r--   0        0        0      946 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lb.js
+-rw-r--r--   0        0        0      948 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lt.js
+-rw-r--r--   0        0        0      989 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lv.js
+-rw-r--r--   0        0        0      936 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/mk.js
+-rw-r--r--   0        0        0     1015 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ms.js
+-rw-r--r--   0        0        0      928 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nb.js
+-rw-r--r--   0        0        0      945 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nl.js
+-rw-r--r--   0        0        0      930 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nn.js
+-rw-r--r--   0        0        0      962 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pl.js
+-rw-r--r--   0        0        0      871 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt-br.js
+-rw-r--r--   0        0        0      939 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt.js
+-rw-r--r--   0        0        0     1008 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ro.js
+-rw-r--r--   0        0        0     1069 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ru.js
+-rw-r--r--   0        0        0     1010 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sk.js
+-rw-r--r--   0        0        0      940 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sl.js
+-rw-r--r--   0        0        0     1002 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sq.js
+-rw-r--r--   0        0        0     1077 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr-cyrl.js
+-rw-r--r--   0        0        0      995 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr.js
+-rw-r--r--   0        0        0      927 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sv.js
+-rw-r--r--   0        0        0     1243 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/th.js
+-rw-r--r--   0        0        0      933 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/tr.js
+-rw-r--r--   0        0        0      633 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ug.js
+-rw-r--r--   0        0        0     1100 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uk.js
+-rw-r--r--   0        0        0      749 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uz.js
+-rw-r--r--   0        0        0     1017 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/vi.js
+-rw-r--r--   0        0        0     1114 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-cn.js
+-rw-r--r--   0        0        0      814 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-tw.js
+-rw-r--r--   0        0        0    27363 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.css
+-rw-r--r--   0        0        0   119971 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.d.ts
+-rw-r--r--   0        0        0   334647 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.esm.js
+-rw-r--r--   0        0        0   373420 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.js
+-rw-r--r--   0        0        0    14357 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.css
+-rw-r--r--   0        0        0   127416 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.js
+-rw-r--r--   0        0        0      822 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/LICENSE.txt
+-rw-r--r--   0        0        0      257 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/README.md
+-rw-r--r--   0        0        0     1807 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.css
+-rw-r--r--   0        0        0    12587 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.d.ts
+-rw-r--r--   0        0        0    75216 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.esm.js
+-rw-r--r--   0        0        0    82087 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.js
+-rw-r--r--   0        0        0     1004 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.css
+-rw-r--r--   0        0        0    28238 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.js
+-rw-r--r--   0        0        0      875 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/LICENSE.txt
+-rw-r--r--   0        0        0      272 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/README.md
+-rw-r--r--   0        0        0      599 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.d.ts
+-rw-r--r--   0        0        0     6336 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.esm.js
+-rw-r--r--   0        0        0     7367 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.js
+-rw-r--r--   0        0        0     2600 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.min.js
+-rw-r--r--   0        0        0      898 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/LICENSE.txt
+-rw-r--r--   0        0        0      303 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/README.md
+-rw-r--r--   0        0        0    13764 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.d.ts
+-rw-r--r--   0        0        0    94523 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.esm.js
+-rw-r--r--   0        0        0   103154 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.js
+-rw-r--r--   0        0        0    36208 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.min.js
+-rw-r--r--   0        0        0      925 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/LICENSE.txt
+-rw-r--r--   0        0        0      248 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/README.md
+-rw-r--r--   0        0        0     1938 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.css
+-rw-r--r--   0        0        0     1635 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.d.ts
+-rw-r--r--   0        0        0    14938 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.esm.js
+-rw-r--r--   0        0        0    16587 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.js
+-rw-r--r--   0        0        0     1102 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.css
+-rw-r--r--   0        0        0     6551 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.js
+-rw-r--r--   0        0        0      863 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/LICENSE.txt
+-rw-r--r--   0        0        0      249 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/README.md
+-rw-r--r--   0        0        0      580 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.d.ts
+-rw-r--r--   0        0        0     5618 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.esm.js
+-rw-r--r--   0        0        0     6672 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.js
+-rw-r--r--   0        0        0     2603 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.min.js
+-rw-r--r--   0        0        0      889 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/LICENSE.txt
+-rw-r--r--   0        0        0      282 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/README.md
+-rw-r--r--   0        0        0      387 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.d.ts
+-rw-r--r--   0        0        0     2319 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.esm.js
+-rw-r--r--   0        0        0     3014 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.js
+-rw-r--r--   0        0        0     1255 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.min.js
+-rw-r--r--   0        0        0      967 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/LICENSE.txt
+-rw-r--r--   0        0        0      255 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/README.md
+-rw-r--r--   0        0        0      526 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.d.ts
+-rw-r--r--   0        0        0     3417 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.esm.js
+-rw-r--r--   0        0        0     4253 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.js
+-rw-r--r--   0        0        0     1634 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.min.js
+-rw-r--r--   0        0        0      897 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/LICENSE.txt
+-rw-r--r--   0        0        0      266 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/README.md
+-rw-r--r--   0        0        0      245 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.d.ts
+-rw-r--r--   0        0        0     4304 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.esm.js
+-rw-r--r--   0        0        0     5169 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.js
+-rw-r--r--   0        0        0     1681 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.min.js
+-rw-r--r--   0        0        0      905 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/package.json
+-rw-r--r--   0        0        0     1053 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/LICENSE.txt
+-rw-r--r--   0        0        0      260 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/README.md
+-rw-r--r--   0        0        0     7304 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.css
+-rw-r--r--   0        0        0     9492 2020-05-28 07:18:24.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.d.ts
+-rw-r--r--   0        0        0    65257 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.esm.js
+-rw-r--r--   0        0        0    71134 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.js
+-rw-r--r--   0        0        0     3377 2020-05-28 07:18:20.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.css
+-rw-r--r--   0        0        0    25180 2020-05-28 07:18:28.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.js
+-rw-r--r--   0        0        0      942 2020-05-28 07:18:18.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/package.json
+-rw-r--r--   0        0        0   137525 2019-12-18 03:54:50.000000 django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/vendor/rrule.js
+-rw-r--r--   0        0        0     1800 2024-04-12 07:02:53.713306 django_calendards-0.4.2/django_calendards/templates/django_calendards/calendards.html
+-rw-r--r--   0        0        0     2183 2024-04-12 05:47:21.387698 django_calendards-0.4.2/django_calendards/templates/django_calendards/modalds.html
+-rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_calendards-0.4.2/django_calendards/templatetags/__init__.py
+-rw-r--r--   0        0        0     1293 2024-03-20 02:03:05.123543 django_calendards-0.4.2/django_calendards/templatetags/django_calendards_tags.py
+-rw-r--r--   0        0        0       60 2024-03-20 00:02:36.855013 django_calendards-0.4.2/django_calendards/tests.py
+-rw-r--r--   0        0        0       63 2024-03-20 00:02:36.853580 django_calendards-0.4.2/django_calendards/views.py
+-rw-r--r--   0        0        0      638 2024-04-24 02:15:25.109954 django_calendards-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1304 1970-01-01 00:00:00.000000 django_calendards-0.4.2/PKG-INFO
```

### Comparing `django_calendards-0.4.1/.DS_Store` & `django_calendards-0.4.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/LICENSE` & `django_calendards-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/README.md` & `django_calendards-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/migrations/0001_initial.py` & `django_calendards-0.4.2/django_calendards/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/models.py` & `django_calendards-0.4.2/django_calendards/models.py`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales-all.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/af.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/af.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-dz.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-dz.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-kw.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-kw.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ly.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ly.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ma.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-ma.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-sa.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-sa.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-tn.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar-tn.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ar.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/az.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/az.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bg.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bg.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bs.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/bs.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ca.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ca.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/cs.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/cs.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/da.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/da.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/de.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/de.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/el.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/el.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-au.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-au.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-gb.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-gb.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-nz.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/en-nz.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es-us.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es-us.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/es.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/et.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/et.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/eu.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/eu.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fa.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fa.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fi.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fi.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ca.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ca.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ch.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr-ch.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/fr.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/gl.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/gl.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/he.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/he.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hi.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hi.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hr.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hr.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hu.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/hu.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/id.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/id.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/is.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/is.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/it.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/it.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ja.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ja.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ka.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ka.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/kk.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/kk.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ko.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ko.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lb.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lb.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lt.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lt.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lv.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/lv.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/mk.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/mk.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ms.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ms.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nb.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nb.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nl.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nl.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nn.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/nn.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pl.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pl.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt-br.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt-br.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/pt.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ro.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ro.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ru.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ru.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sk.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sk.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sl.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sl.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sq.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sq.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr-cyrl.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sr.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sv.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/sv.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/th.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/th.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/tr.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/tr.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ug.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/ug.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uk.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uk.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uz.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/uz.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/vi.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/vi.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-cn.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-cn.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-tw.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/locales/zh-tw.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/core/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/core/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/daygrid/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/daygrid/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/google-calendar/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/interaction/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/interaction/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/list/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/list/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/luxon/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/luxon/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment-timezone/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/moment/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/moment/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/rrule/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/rrule/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/LICENSE.txt` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.d.ts` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.d.ts`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.esm.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.esm.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.css` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.css`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/main.min.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/packages/timegrid/package.json` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/packages/timegrid/package.json`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/static/calendards/fullcalendar4/vendor/rrule.js` & `django_calendards-0.4.2/django_calendards/static/calendards/fullcalendar4/vendor/rrule.js`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/templates/django_calendards/calendards.html` & `django_calendards-0.4.2/django_calendards/templates/django_calendards/calendards.html`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/templates/django_calendards/modalds.html` & `django_calendards-0.4.2/django_calendards/templates/django_calendards/modalds.html`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/django_calendards/templatetags/django_calendards_tags.py` & `django_calendards-0.4.2/django_calendards/templatetags/django_calendards_tags.py`

 * *Files identical despite different names*

### Comparing `django_calendards-0.4.1/pyproject.toml` & `django_calendards-0.4.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-calendards"
-version = "0.4.1"
+version = "0.4.2"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
-    "Django >= 5.0.3",
+    "Django >= 4.2.11",
 ]
 
 [project.urls]
 Home = "https://www.demiansoft.com"
 
 [tool.flit.sdist]
 # include = ["analyticsds/","calendards/","popupds/"]
```

### Comparing `django_calendards-0.4.1/PKG-INFO` & `django_calendards-0.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-calendards
-Version: 0.4.1
+Version: 0.4.2
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: Django >= 5.0.3
+Requires-Dist: Django >= 4.2.11
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-calendards  
   
 #### Introduction  
   
 demiansoft 에서 사용하는 장고앱 모음 django-calendards
```

