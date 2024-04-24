# Comparing `tmp/django_analyticsds-0.3.2.tar.gz` & `tmp/django_analyticsds-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_analyticsds-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_analyticsds-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_analyticsds-0.3.2.tar` & `django_analyticsds-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     6148 2024-03-21 00:31:38.763461 django_analyticsds-0.3.2/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-19 11:29:26.020500 django_analyticsds-0.3.2/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-19 12:37:53.981351 django_analyticsds-0.3.2/.gitignore
--rw-r--r--   0        0        0       52 2024-03-19 11:44:29.802980 django_analyticsds-0.3.2/.idea/.gitignore
--rw-r--r--   0        0        0      408 2024-03-19 11:39:49.813842 django_analyticsds-0.3.2/.idea/django-analyticsds.iml
--rw-r--r--   0        0        0      174 2024-03-19 11:39:49.823834 django_analyticsds-0.3.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      427 2024-03-19 11:39:49.820046 django_analyticsds-0.3.2/.idea/misc.xml
--rw-r--r--   0        0        0      288 2024-03-19 11:39:49.816703 django_analyticsds-0.3.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-19 11:39:49.825823 django_analyticsds-0.3.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_analyticsds-0.3.2/LICENSE
--rw-r--r--   0        0        0     2085 2024-03-20 03:11:59.390131 django_analyticsds-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-03-19 11:30:50.526044 django_analyticsds-0.3.2/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-19 11:41:20.813701 django_analyticsds-0.3.2/django_analyticsds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-19 11:32:15.236554 django_analyticsds-0.3.2/django_analyticsds/__init__.py
--rw-r--r--   0        0        0       63 2024-03-19 11:32:15.237150 django_analyticsds-0.3.2/django_analyticsds/admin.py
--rw-r--r--   0        0        0      194 2024-03-19 11:57:47.349805 django_analyticsds-0.3.2/django_analyticsds/apps.py
--rw-r--r--   0        0        0        0 2024-03-19 11:32:15.238697 django_analyticsds-0.3.2/django_analyticsds/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-03-19 11:32:15.238405 django_analyticsds-0.3.2/django_analyticsds/models.py
--rw-r--r--   0        0        0     1571 2024-03-17 11:25:17.304081 django_analyticsds-0.3.2/django_analyticsds/templates/django_analyticsds/analyticsds.html
--rw-r--r--   0        0        0        0 2023-03-21 07:33:49.694261 django_analyticsds-0.3.2/django_analyticsds/templatetags/__init__.py
--rw-r--r--   0        0        0      413 2024-03-20 03:17:27.877161 django_analyticsds-0.3.2/django_analyticsds/templatetags/django_analyticsds_tags.py
--rw-r--r--   0        0        0       60 2024-03-19 11:32:15.238550 django_analyticsds-0.3.2/django_analyticsds/tests.py
--rw-r--r--   0        0        0       63 2024-03-19 11:32:15.236889 django_analyticsds-0.3.2/django_analyticsds/views.py
--rw-r--r--   0        0        0      584 2024-03-21 00:33:33.762114 django_analyticsds-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 django_analyticsds-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-03-24 09:10:56.258187 django_analyticsds-0.3.3/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-19 11:29:26.020500 django_analyticsds-0.3.3/.gitattributes
+-rw-r--r--   0        0        0       30 2024-03-27 23:56:50.660397 django_analyticsds-0.3.3/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-19 11:44:29.802980 django_analyticsds-0.3.3/.idea/.gitignore
+-rw-r--r--   0        0        0      408 2024-03-19 11:39:49.813842 django_analyticsds-0.3.3/.idea/django-analyticsds.iml
+-rw-r--r--   0        0        0      174 2024-03-19 11:39:49.823834 django_analyticsds-0.3.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      427 2024-03-19 11:39:49.820046 django_analyticsds-0.3.3/.idea/misc.xml
+-rw-r--r--   0        0        0      288 2024-03-19 11:39:49.816703 django_analyticsds-0.3.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-19 11:39:49.825823 django_analyticsds-0.3.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_analyticsds-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2085 2024-03-20 03:11:59.390131 django_analyticsds-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 11:30:50.526044 django_analyticsds-0.3.3/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-22 02:21:13.647126 django_analyticsds-0.3.3/django_analyticsds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-19 11:32:15.236554 django_analyticsds-0.3.3/django_analyticsds/__init__.py
+-rw-r--r--   0        0        0       63 2024-03-19 11:32:15.237150 django_analyticsds-0.3.3/django_analyticsds/admin.py
+-rw-r--r--   0        0        0      194 2024-03-19 11:57:47.349805 django_analyticsds-0.3.3/django_analyticsds/apps.py
+-rw-r--r--   0        0        0        0 2024-03-19 11:32:15.238697 django_analyticsds-0.3.3/django_analyticsds/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-03-19 11:32:15.238405 django_analyticsds-0.3.3/django_analyticsds/models.py
+-rw-r--r--   0        0        0     1571 2024-03-17 11:25:17.304081 django_analyticsds-0.3.3/django_analyticsds/templates/django_analyticsds/analyticsds.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:33:49.694261 django_analyticsds-0.3.3/django_analyticsds/templatetags/__init__.py
+-rw-r--r--   0        0        0      413 2024-03-20 03:17:27.877161 django_analyticsds-0.3.3/django_analyticsds/templatetags/django_analyticsds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-19 11:32:15.238550 django_analyticsds-0.3.3/django_analyticsds/tests.py
+-rw-r--r--   0        0        0       63 2024-03-19 11:32:15.236889 django_analyticsds-0.3.3/django_analyticsds/views.py
+-rw-r--r--   0        0        0      585 2024-04-24 01:47:43.053912 django_analyticsds-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2403 1970-01-01 00:00:00.000000 django_analyticsds-0.3.3/PKG-INFO
```

### Comparing `django_analyticsds-0.3.2/.DS_Store` & `django_analyticsds-0.3.3/.DS_Store`

 * *Files 9% similar despite different names*

```diff
@@ -67,69 +67,69 @@
 00000420: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 00000430: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 00000440: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000450: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000460: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000470: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000480: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000490: 7208 0908 095f 1018 7b7b 3331 332c 2031  r...._..{{313, 1
-000004a0: 3637 7d2c 207b 3932 302c 2034 3336 7d7d  67}, {920, 436}}
+00000490: 7208 0908 095f 1018 7b7b 3330 392c 2033  r...._..{{309, 3
+000004a0: 3632 7d2c 207b 3932 302c 2034 3336 7d7d  62}, {920, 436}}
 000004b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 000004c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 000004d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 000004e0: 0005 005f 0064 0061 0074 0061 7653 726e  ..._.d.a.t.avSrn
 000004f0: 6c6f 6e67 0000 0001 0000 0009 005f 006d  long........._.m
 00000500: 0079 0074 0065 0073 0074 0065 0072 6277  .y.t.e.s.t.e.rbw
-00000510: 7370 626c 6f62 0000 00b7 6270 6c69 7374  spblob....bplist
+00000510: 7370 626c 6f62 0000 00b9 6270 6c69 7374  spblob....bplist
 00000520: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
 00000530: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00000540: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
 00000550: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
 00000560: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
 00000570: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00000580: 6465 6261 7208 0908 095f 1017 7b7b 3634  debar...._..{{64
-00000590: 2c20 3432 307d 2c20 7b39 3230 2c20 3433  , 420}, {920, 43
-000005a0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
-000005b0: 8900 0000 0000 0001 0100 0000 0000 0000  ................
-000005c0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 8a00 0000 0900 5f00 6d00 7900 7400 6500  ......_.m.y.t.e.
-000005e0: 7300 7400 6500 7276 5372 6e6c 6f6e 6700  s.t.e.rvSrnlong.
-000005f0: 0000 0100 0000 0400 6400 6900 7300 7462  ........d.i.s.tb
-00000600: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
-00000610: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
-00000620: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00000630: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-00000640: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-00000650: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-00000660: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00000670: 6964 6562 6172 0809 0809 5f10 187b 7b32  idebar...._..{{2
-00000680: 3730 2c20 3634 387d 2c20 7b39 3230 2c20  70, 648}, {920, 
-00000690: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
-000006a0: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
-000006b0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-000006c0: 0000 8b00 0000 0400 6400 6900 7300 7476  ........d.i.s.tv
-000006d0: 5372 6e6c 6f6e 6700 0000 0100 0000 1200  Srnlong.........
-000006e0: 6400 6a00 6100 6e00 6700 6f00 5f00 6100  d.j.a.n.g.o._.a.
-000006f0: 6e00 6100 6c00 7900 7400 6900 6300 7300  n.a.l.y.t.i.c.s.
-00000700: 6400 7362 7773 7062 6c6f 6200 0000 b862  d.sbwspblob....b
-00000710: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
-00000720: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-00000730: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-00000740: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-00000750: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-00000760: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-00000770: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00000780: 187b 7b35 3530 2c20 3438 337d 2c20 7b39  .{{550, 483}, {9
-00000790: 3230 2c20 3433 367d 7d09 0815 232f 3b52  20, 436}}...#/;R
-000007a0: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
-000007b0: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-000007c0: 0000 0000 0000 8b00 0000 1200 6400 6a00  ............d.j.
-000007d0: 6100 6e00 6700 6f00 5f00 6100 6e00 6100  a.n.g.o._.a.n.a.
-000007e0: 6c00 7900 7400 6900 6300 7300 6400 7376  l.y.t.i.c.s.d.sv
-000007f0: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
+00000580: 6465 6261 7208 0908 095f 1019 7b7b 3139  debar...._..{{19
+00000590: 3335 2c20 3436 357d 2c20 7b39 3230 2c20  35, 465}, {920, 
+000005a0: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
+000005b0: 6e6f 8b00 0000 0000 0001 0100 0000 0000  no..............
+000005c0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 8c00 0000 0900 5f00 6d00 7900 7400  ........_.m.y.t.
+000005e0: 6500 7300 7400 6500 7276 5372 6e6c 6f6e  e.s.t.e.rvSrnlon
+000005f0: 6700 0000 0100 0000 0400 6400 6900 7300  g.........d.i.s.
+00000600: 7462 7773 7062 6c6f 6200 0000 b862 706c  tbwspblob....bpl
+00000610: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+00000620: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00000630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00000640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00000650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00000660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00000670: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
+00000680: 7b32 3730 2c20 3634 387d 2c20 7b39 3230  {270, 648}, {920
+00000690: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
+000006a0: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
+000006b0: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
+000006c0: 0000 0000 8b00 0000 0400 6400 6900 7300  ..........d.i.s.
+000006d0: 7476 5372 6e6c 6f6e 6700 0000 0100 0000  tvSrnlong.......
+000006e0: 1200 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
+000006f0: 6100 6e00 6100 6c00 7900 7400 6900 6300  a.n.a.l.y.t.i.c.
+00000700: 7300 6400 7362 7773 7062 6c6f 6200 0000  s.d.sbwspblob...
+00000710: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00000720: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00000730: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00000740: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00000750: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00000760: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00000770: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+00000780: 5f10 187b 7b39 3432 2c20 3639 317d 2c20  _..{{942, 691}, 
+00000790: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
+000007a0: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+000007b0: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+000007c0: 0000 0000 0000 0000 8b00 0000 1200 6400  ..............d.
+000007d0: 6a00 6100 6e00 6700 6f00 5f00 6100 6e00  j.a.n.g.o._.a.n.
+000007e0: 6100 6c00 7900 7400 6900 6300 7300 6400  a.l.y.t.i.c.s.d.
+000007f0: 7376 5372 6e6c 6f6e 6700 0000 0100 0000  svSrnlong.......
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `django_analyticsds-0.3.2/LICENSE` & `django_analyticsds-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_analyticsds-0.3.2/README.md` & `django_analyticsds-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `django_analyticsds-0.3.2/django_analyticsds/templates/django_analyticsds/analyticsds.html` & `django_analyticsds-0.3.3/django_analyticsds/templates/django_analyticsds/analyticsds.html`

 * *Files identical despite different names*

### Comparing `django_analyticsds-0.3.2/pyproject.toml` & `django_analyticsds-0.3.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-analyticsds"
-version = "0.3.2"
+version = "0.3.3"
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
 exclude = [
```

### Comparing `django_analyticsds-0.3.2/PKG-INFO` & `django_analyticsds-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: django-analyticsds
-Version: 0.3.2
+Version: 0.3.3
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: Django >= 5.0.3
+Requires-Dist: Django >= 4.2.11
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-analyticsds
 
 #### Introduction
 
 demiansoft 에서 사용하는 장고앱 django_analyticsds
```

