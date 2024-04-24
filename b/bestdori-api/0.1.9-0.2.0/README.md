# Comparing `tmp/bestdori_api-0.1.9.tar.gz` & `tmp/bestdori-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bestdori_api-0.1.9.tar", last modified: Tue Mar  5 15:23:05 2024, max compression
+gzip compressed data, was "bestdori-api-0.2.0.tar", last modified: Wed Apr 24 14:38:04 2024, max compression
```

## Comparing `bestdori_api-0.1.9.tar` & `bestdori-api-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/ayachan/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/ayachan/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/ayachan/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/charts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/comics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/costumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/eventarchives.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/gacha.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/logincampaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/miracleticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/missions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/post.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/songmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7228 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/songs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/content.py
--rw-r--r--   0 runner    (1001) docker     (127)    10570 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/bestdori/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/bestdori_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-05 15:23:05.000000 bestdori_api-0.1.9/bestdori_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 15:23:05.478447 bestdori_api-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-05 15:22:56.000000 bestdori_api-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/ayachan/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/ayachan/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/ayachan/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11256 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/charts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/comics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/costumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/eventarchives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/gacha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/logincampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/miracleticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/missions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/songmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/songs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/bestdori/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:38:04.476966 bestdori-api-0.2.0/bestdori_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:38:04.000000 bestdori-api-0.2.0/bestdori_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:38:04.480966 bestdori-api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 14:37:54.000000 bestdori-api-0.2.0/setup.py
```

### Comparing `bestdori_api-0.1.9/LICENSE` & `bestdori-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.9/PKG-INFO` & `bestdori-api-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,296 +1,275 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6265 7374  : 2.1.Name: best
-00000020: 646f 7269 5f61 7069 0a56 6572 7369 6f6e  dori_api.Version
-00000030: 3a20 302e 312e 390a 5375 6d6d 6172 793a  : 0.1.9.Summary:
-00000040: 2042 6573 7464 6f72 6920 e79a 84e5 9084   Bestdori ......
-00000050: e7a7 8d20 4150 4920 e8b0 83e7 94a8 e695  ... API ........
-00000060: b4e5 9088 efbc 8ce5 8fa6 e5a4 96e9 9984  ................
-00000070: e5b8 a6e9 83a8 e588 86e5 8a9f e883 bd0a  ................
-00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
-00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 5769  ://github.com/Wi
-000000a0: 6e64 6f77 7353 6f76 3866 6f72 5573 2f62  ndowsSov8forUs/b
-000000b0: 6573 7464 6f72 695f 6170 690a 4175 7468  estdori_api.Auth
-000000c0: 6f72 3a20 5769 6e64 6f77 7353 6f76 380a  or: WindowsSov8.
-000000d0: 4175 7468 6f72 2d65 6d61 696c 3a20 7177  Author-email: qw
-000000e0: 6572 7479 7569 6f70 3233 3333 4068 6f74  ertyuiop2333@hot
-000000f0: 6d61 696c 2e63 6f6d 0a4c 6963 656e 7365  mail.com.License
-00000100: 3a20 554e 4b4e 4f57 4e0a 4465 7363 7269  : UNKNOWN.Descri
-00000110: 7074 696f 6e3a 2021 5b62 6573 7464 6f72  ption: ![bestdor
-00000120: 695f 6170 6920 6c6f 676f 5d28 6874 7470  i_api logo](http
-00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f57  s://github.com/W
-00000140: 696e 646f 7773 536f 7638 666f 7255 732f  indowsSov8forUs/
-00000150: 6265 7374 646f 7269 5f61 7069 2f62 6c6f  bestdori_api/blo
-00000160: 622f 6d61 696e 2f6c 6f67 6f2e 706e 6729  b/main/logo.png)
-00000170: 0a20 2020 2020 2020 203c 6469 7620 616c  .        <div al
-00000180: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000190: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000001a0: 2042 6573 7464 6f72 695f 6170 690a 2020   Bestdori_api.  
-000001b0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000001c0: 2a3a 7761 726e 696e 673a 20e8 afa5 e9a1  *:warning: .....
-000001d0: b9e7 9bae e4bb 8de7 84b6 e680 a5e9 9c80  ................
-000001e0: e69b b4e6 96b0 e4b8 8e20 4465 6275 6720  ......... Debug 
-000001f0: efbc 8ce4 bdbf e794 a8e6 97b6 e88b a5e9  ................
-00000200: 8187 e588 b020 4275 6720 e688 96e5 85b6  ..... Bug ......
-00000210: e4bb 96e9 9c80 e8a6 81e7 9a84 e68e a5e5  ................
-00000220: 8fa3 e8af b7e5 8f8a e697 b6e6 8f90 e587  ................
-00000230: ba2a 2a0a 2020 2020 2020 2020 0a20 2020  .**.        .   
-00000240: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000250: 2020 2020 0a20 2020 2020 2020 2023 20e7      .        # .
-00000260: ae80 e4bb 8b0a 2020 2020 2020 2020 0a20  ......        . 
-00000270: 2020 2020 2020 20e8 bf99 e698 afe4 b880         .........
-00000280: e4b8 aae7 94a8 2050 7974 686f 6e20 e7bc  ...... Python ..
-00000290: 96e5 8699 e79a 84e8 b083 e794 a820 5b42  ............. [B
-000002a0: 6573 7464 6f72 695d 2868 7474 7073 3a2f  estdori](https:/
-000002b0: 2f62 6573 7464 6f72 692e 636f 6d2f 2920  /bestdori.com/) 
-000002c0: e590 84e7 a78d 2041 5049 20e4 b88e e8b5  ...... API .....
-000002d0: 84e6 ba90 e4b8 8be8 bdbd e79a 84e5 ba93  ................
-000002e0: efbc 8ce5 a4a7 e887 b4e5 8c85 e68b ace4  ................
-000002f0: ba86 e7a4 bee5 8cba e5b8 96e5 ad90 e79a  ................
-00000300: 84e5 a484 e790 86e4 bba5 e58f 8ae5 9084  ................
-00000310: e7a7 8d20 5b42 616e 4720 4472 6561 6def  ... [BanG Dream.
-00000320: bc81 e5b0 91e5 a5b3 e4b9 90e5 9ba2 e6b4  ................
-00000330: bee5 afb9 5d28 6874 7470 733a 2f2f 7a68  ....](https://zh
-00000340: 2e6d 6f65 6769 726c 2e6f 7267 2e63 6e2f  .moegirl.org.cn/
-00000350: 4261 6e47 5f44 7265 616d 215f 2545 3525  BanG_Dream!_%E5%
-00000360: 4230 2539 3125 4535 2541 3525 4233 2545  B0%91%E5%A5%B3%E
-00000370: 3425 4239 2539 3025 4535 2539 4225 4132  4%B9%90%E5%9B%A2
-00000380: 2545 3625 4234 2542 4525 4535 2541 4625  %E6%B4%BE%E5%AF%
-00000390: 4239 2545 4625 4243 2538 3129 20e6 b8b8  B9%EF%BC%81) ...
-000003a0: e688 8fe5 8685 e8b5 84e6 ba90 e79a 84e8  ................
-000003b0: 8eb7 e58f 96e3 8082 0a20 2020 2020 2020  .........       
-000003c0: 202a 2ae8 ada6 e591 8aef bc9a e6ad a4e6   **.............
-000003d0: a8a1 e59d 97e7 9bae e589 8de4 bb8d e784  ................
-000003e0: b6e4 ba9f e5be 85e5 ae8c e596 84e4 b88e  ................
-000003f0: e6b5 8be8 af95 efbc 8ce8 afb7 e4b8 8de8  ................
-00000400: a681 e5b0 86e5 85b6 e5bd 93e5 819a e4b8  ................
-00000410: 80e4 b8aa e7a8 b3e5 ae9a e79a 84e5 ba93  ................
-00000420: e4bd bfe7 94a8 e380 822a 2a0a 2020 2020  .........**.    
-00000430: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00000440: e79b aee5 898d e5b7 b2e6 9c89 e79a 8420  ............... 
-00000450: 4150 4920 e4b8 8ee5 8a9f e883 bd0a 2020  API ..........  
-00000460: 2020 2020 2020 0a20 2020 2020 2020 207c        .        |
-00000470: 4150 4920 e7b1 bbe5 88ab 7ce6 98af e590  API ......|.....
-00000480: a6e5 ae8c e596 847c e694 afe6 8c81 e79a  .......|........
-00000490: 84e5 8685 e5ae b97c 0a20 2020 2020 2020  .......|.       
-000004a0: 207c 3a2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d   |:-------|:----
-000004b0: 2d3a 7c3a 2d2d 2d2d 2d2d 7c0a 2020 2020  -:|:------|.    
-000004c0: 2020 2020 7ce7 94a8 e688 b77c f09f 918d      |......|....
-000004d0: 7ce7 99bb e5bd 95e3 8081 e69f a5e8 afa2  |...............
-000004e0: e380 81e5 b896 e5ad 90e8 8eb7 e58f 96e3  ................
-000004f0: 8081 e4bf a1e6 81af e88e b7e5 8f96 7c0a  ..............|.
-00000500: 2020 2020 2020 2020 7ce5 b896 e5ad 907c          |......|
-00000510: f09f 918d 7ce6 909c e7b4 a2e3 8081 e88e  ....|...........
-00000520: b7e5 8f96 e380 81e5 8f91 e8a1 a8e3 8081  ................
-00000530: e8af 84e8 aeba e380 81e5 969c e6ac a27c  ...............|
-00000540: 0a20 2020 2020 2020 207c e8b0 b1e9 9da2  .        |......
-00000550: 7cf0 9f91 8d7c e7a4 bee5 8cba e8b0 b1e9  |....|..........
-00000560: 9da2 e88e b7e5 8f96 e380 81e9 9fb3 e6ba  ................
-00000570: 90e4 b88e e5b0 81e9 9da2 e88e b7e5 8f96  ................
-00000580: e380 81e8 a784 e695 b4e5 8c96 e380 81e6  ................
-00000590: 95b0 e68d aee7 bb9f e8ae a1e3 8081 e6a0  ................
-000005a0: bce5 bc8f e4ba 92e8 bdac 7c0a 2020 2020  ..........|.    
-000005b0: 2020 2020 7ce6 9585 e4ba 8b7c f09f 918e      |......|....
-000005c0: f09f 918e 7ce7 a4be e58c bae6 9585 e4ba  ....|...........
-000005d0: 8be8 8eb7 e58f 967c 0a20 2020 2020 2020  .......|.       
-000005e0: 207c e8a7 92e8 89b2 7cf0 9fa4 947c e4bf   |......|....|..
-000005f0: a1e6 81af e88e b7e5 8f96 e380 81e8 b584  ................
-00000600: e6ba 90e8 8eb7 e58f 967c 0a20 2020 2020  .........|.     
-00000610: 2020 207c e58d a1e7 898c 7cf0 9f91 8e7c     |......|....|
-00000620: e4bf a1e6 81af e88e b7e5 8f96 e380 81e8  ................
-00000630: b584 e6ba 90e8 8eb7 e58f 967c 0a20 2020  ...........|.   
-00000640: 2020 2020 207c e69c 8de8 a385 7cf0 9f91       |......|...
-00000650: 8ef0 9f91 8e7c e4bf a1e6 81af e88e b7e5  .....|..........
-00000660: 8f96 7c0a 2020 2020 2020 2020 7ce6 b4bb  ..|.        |...
-00000670: e58a a87c f09f a494 7ce4 bfa1 e681 afe8  ...|....|.......
-00000680: 8eb7 e58f 96e3 8081 e8b5 84e6 ba90 e88e  ................
-00000690: b7e5 8f96 7c0a 2020 2020 2020 2020 7ce6  ....|.        |.
-000006a0: b4bb e58a a8e6 95b0 e68d ae7c f09f 918e  ...........|....
-000006b0: 7ce6 95b0 e68d aee8 8eb7 e58f 967c 0a20  |............|. 
-000006c0: 2020 2020 2020 207c e68b 9be5 8b9f 7cf0         |......|.
-000006d0: 9fa4 947c e695 b0e6 8dae e88e b7e5 8f96  ...|............
-000006e0: e380 81e8 b584 e6ba 90e8 8eb7 e58f 967c  ...............|
-000006f0: 0a20 2020 2020 2020 207c e6ad 8ce6 9bb2  .        |......
-00000700: 7cf0 9fa4 947c e4bf a1e6 81af e88e b7e5  |....|..........
-00000710: 8f96 e380 81e8 b584 e6ba 90e8 8eb7 e58f  ................
-00000720: 967c 0a20 2020 2020 2020 207c e6ad 8ce6  .|.        |....
-00000730: 9bb2 204d 6574 617c f09f 918e f09f 918e  .. Meta|........
-00000740: 7ce6 95b0 e68d aee8 8eb7 e58f 967c 0a20  |............|. 
-00000750: 2020 2020 2020 207c e799 bbe5 bd95 e5a5         |........
-00000760: 96e5 8ab1 7cf0 9fa4 947c e4bf a1e6 81af  ....|....|......
-00000770: e88e b7e5 8f96 e380 81e8 b584 e6ba 90e8  ................
-00000780: 8eb7 e58f 967c 0a20 2020 2020 2020 207c  .....|.        |
-00000790: e887 aae9 8089 e588 b87c f09f a494 7ce4  .........|....|.
-000007a0: bfa1 e681 afe8 8eb7 e58f 967c 0a20 2020  ...........|.   
-000007b0: 2020 2020 207c e6bc abe7 94bb 7cf0 9fa4       |......|...
-000007c0: 947c e4bf a1e6 81af e88e b7e5 8f96 e380  .|..............
-000007d0: 81e5 9bbe e789 87e8 8eb7 e58f 967c 0a20  .............|. 
-000007e0: 2020 2020 2020 207c e4bb bbe5 8aa1 7cf0         |......|.
-000007f0: 9fa4 947c e4bf a1e6 81af e88e b7e5 8f96  ...|............
-00000800: 7c0a 2020 2020 2020 2020 7c61 7961 6368  |.        |ayach
-00000810: 616e 7cf0 9fa4 947c e8b0 b1e9 9da2 e588  an|....|........
-00000820: 86e6 9e90 e380 81e6 b58b e8af 95e6 9c8d  ................
-00000830: e4b8 8ae4 bca0 e380 81e9 9abe e5ba a6e5  ................
-00000840: 8886 e69e 907c 0a20 2020 2020 2020 207c  .....|.        |
-00000850: e585 b6e4 bb96 e8b5 84e6 ba90 7cf0 9f91  ............|...
-00000860: 8ef0 9f91 8e7c e4bb 85e5 b08f e983 a8e5  .....|..........
-00000870: 8886 e8b5 84e6 ba90 e69c 89e5 8d95 e78b  ................
-00000880: ace8 8eb7 e58f 967c 0a20 2020 2020 2020  .......|.       
-00000890: 200a 2020 2020 2020 2020 2320 e5bf abe9   .        # ....
-000008a0: 809f e4bd bfe7 94a8 0a20 2020 2020 2020  .........       
-000008b0: 200a 2020 2020 2020 2020 e4bb a5e4 b88b   .        ......
-000008c0: e5b0 86e4 bba5 e88e b7e5 8f96 e7a4 bee5  ................
-000008d0: 8cba e887 aae5 88b6 e8b0 b1e9 9da2 205b  .............. [
-000008e0: 5b46 554c 4c5d 20e5 8589 e381 aee4 b8ad  [FULL] .........
-000008f0: e381 b85d 2868 7474 7073 3a2f 2f62 6573  ...](https://bes
-00000900: 7464 6f72 692e 636f 6d2f 636f 6d6d 756e  tdori.com/commun
-00000910: 6974 792f 6368 6172 7473 2f31 3131 3533  ity/charts/11153
-00000920: 332f 5769 6e64 6f77 7353 6f76 382d 4655  3/WindowsSov8-FU
-00000930: 4c4c 2920 e79a 84e4 bfa1 e681 afe4 b8ba  LL) ............
-00000940: e4be 8be3 8082 0a20 2020 2020 2020 200a  .......        .
-00000950: 2020 2020 2020 2020 e9a6 96e5 8588 efbc          ........
-00000960: 8ce4 bdbf e794 a8e4 bba5 e4b8 8be6 8c87  ................
-00000970: e4bb a4e5 ae89 e8a3 85e6 9cac e6a8 a1e5  ................
-00000980: 9d97 efbc 9a0a 2020 2020 2020 2020 6060  ......        ``
-00000990: 6062 6173 680a 2020 2020 2020 2020 2420  `bash.        $ 
-000009a0: 7069 7033 2069 6e73 7461 6c6c 2062 6573  pip3 install bes
-000009b0: 7464 6f72 695f 6170 690a 2020 2020 2020  tdori_api.      
-000009c0: 2020 6060 600a 2020 2020 2020 2020 e68e    ```.        ..
-000009d0: a5e4 b88b e69d a5e5 9ca8 e4b8 80e4 b8aa  ................
-000009e0: 2050 7974 686f 6e20 e884 9ae6 9cac e696   Python ........
-000009f0: 87e4 bbb6 e4b8 adef bc8c e4bd bfe7 94a8  ................
-00000a00: e5a6 82e4 b88b e4bb a3e7 a081 e88e b7e5  ................
-00000a10: 8f96 e68c 87e5 ae9a e5b8 96e5 ad90 e79a  ................
-00000a20: 84e5 85a8 e983 a8e4 bfa1 e681 afef bc88  ................
-00000a30: e8bf 99e9 878c e688 91e4 bbac e5b7 b2e7  ................
-00000a40: 9fa5 e8af a5e5 b896 e5ad 90e7 9a84 2049  .............. I
-00000a50: 4420 e4b8 ba20 6031 3131 3533 3360 efbc  D ... `111533`..
-00000a60: 89ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-00000a70: 7079 7468 6f6e 0a20 2020 2020 2020 2066  python.        f
-00000a80: 726f 6d20 6265 7374 646f 7269 2e70 6f73  rom bestdori.pos
-00000a90: 7420 696d 706f 7274 2050 6f73 740a 2020  t import Post.  
-00000aa0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
-00000ab0: 6566 206d 6169 6e28 2920 2d3e 204e 6f6e  ef main() -> Non
-00000ac0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-00000ad0: 20e5 ae9e e4be 8be5 8c96 2050 6f73 7420   ......... Post 
-00000ae0: e7b1 bb0a 2020 2020 2020 2020 2020 2020  ....            
-00000af0: 7020 3d20 506f 7374 2869 643d 2731 3131  p = Post(id='111
-00000b00: 3533 3327 290a 2020 2020 2020 2020 2020  533').          
-00000b10: 2020 2320 e8b0 83e7 94a8 e696 b9e6 b395    # ............
-00000b20: e88e b7e5 8f96 e4bf a1e6 81af 0a20 2020  .............   
-00000b30: 2020 2020 2020 2020 2069 6e66 6f20 3d20           info = 
-00000b40: 702e 6765 745f 6465 7461 696c 7328 290a  p.get_details().
-00000b50: 2020 2020 2020 2020 2020 2020 2320 e689              # ..
-00000b60: 93e5 8db0 e4bf a1e6 81af 0a20 2020 2020  ...........     
-00000b70: 2020 2020 2020 2070 7269 6e74 2869 6e66         print(inf
-00000b80: 6f29 0a20 2020 2020 2020 200a 2020 2020  o).        .    
-00000b90: 2020 2020 6d61 696e 2829 0a20 2020 2020      main().     
-00000ba0: 2020 2060 6060 0a20 2020 2020 2020 20e5     ```.        .
-00000bb0: be97 e588 b0e7 9a84 e8be 93e5 87ba e586  ................
-00000bc0: 85e5 aeb9 e5a6 82e4 b88b efbc 9a0a 2020  ..............  
-00000bd0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00000be0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000bf0: 2020 2020 2020 2763 6174 6567 6f72 794e        'categoryN
-00000c00: 616d 6527 3a20 2753 454c 465f 504f 5354  ame': 'SELF_POST
-00000c10: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00000c20: 6361 7465 676f 7279 4964 273a 2027 6368  categoryId': 'ch
-00000c30: 6172 7427 2c0a 2020 2020 2020 2020 2020  art',.          
-00000c40: 2020 2774 6974 6c65 273a 2027 5b46 554c    'title': '[FUL
-00000c50: 4c5d 20e5 8589 e381 aee4 b8ad e381 b827  L] ............'
-00000c60: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00000c70: 6f6e 6727 3a20 7b0a 2020 2020 2020 2020  ong': {.        
-00000c80: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
-00000c90: 2763 7573 746f 6d27 2c0a 2020 2020 2020  'custom',.      
-00000ca0: 2020 2020 2020 2020 2020 2761 7564 696f            'audio
-00000cb0: 273a 2027 6874 7470 733a 2f2f 6265 7374  ': 'https://best
-00000cc0: 646f 7269 2e63 6f6d 2f61 7069 2f75 706c  dori.com/api/upl
-00000cd0: 6f61 642f 6669 6c65 2f65 3461 3038 3066  oad/file/e4a080f
-00000ce0: 3834 6266 6132 6361 3437 6232 3362 3339  84bfa2ca47b23b39
-00000cf0: 3061 3436 3463 3831 3965 6331 3765 3730  0a464c819ec17e70
-00000d00: 6227 2c0a 2020 2020 2020 2020 2020 2020  b',.            
-00000d10: 2020 2020 2763 6f76 6572 273a 2027 6874      'cover': 'ht
-00000d20: 7470 733a 2f2f 6265 7374 646f 7269 2e63  tps://bestdori.c
-00000d30: 6f6d 2f61 7069 2f75 706c 6f61 642f 6669  om/api/upload/fi
-00000d40: 6c65 2f65 3335 3335 6562 6234 6337 3430  le/e3535ebb4c740
-00000d50: 6334 3735 3733 3731 3032 3661 3164 6639  c4757371026a1df9
-00000d60: 6666 6230 3830 3130 3330 3727 0a20 2020  ffb08010307'.   
-00000d70: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000d80: 2020 2020 2020 2020 2761 7274 6973 7473          'artists
-00000d90: 273a 2027 e7b5 90e6 9d9f e383 90e3 83b3  ': '............
-00000da0: e383 8927 2c0a 2020 2020 2020 2020 2020  ...',.          
-00000db0: 2020 2764 6966 6627 3a20 342c 0a20 2020    'diff': 4,.   
-00000dc0: 2020 2020 2020 2020 2027 6c65 7665 6c27           'level'
-00000dd0: 3a20 3330 2c0a 2020 2020 2020 2020 2020  : 30,.          
-00000de0: 2020 2763 6861 7274 273a 205b 0a20 2020    'chart': [.   
-00000df0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2027 6270 6d27 3a20 3139 312c 0a20     'bpm': 191,. 
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2027 6265 6174 273a 2030 2c0a 2020     'beat': 0,.  
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 2774 7970 6527 3a20 2742 504d 270a    'type': 'BPM'.
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00000e80: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000e90: 2020 2020 2020 2020 2027 6265 6174 273a           'beat':
-00000ea0: 2031 3932 2c0a 2020 2020 2020 2020 2020   192,.          
-00000eb0: 2020 2020 2020 2020 2020 276c 616e 6527            'lane'
-00000ec0: 3a20 332e 0a20 2020 2020 2020 2020 2020  : 3..           
-00000ed0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-00000ee0: 2027 5369 6e67 6c65 270a 2020 2020 2020   'Single'.      
-00000ef0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000f00: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-00000f10: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00000f20: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00000f30: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000f40: 2020 6060 600a 2020 2020 2020 2020 e5a6    ```.        ..
-00000f50: 82e6 9e9c e683 b3e8 a681 e88e b7e5 8f96  ................
-00000f60: e8bf 99e4 b8aa e887 aae5 88b6 e8b0 b1e9  ................
-00000f70: 9da2 e79a 84e8 b0b1 e99d a2ef bc8c e688  ................
-00000f80: 96e8 8085 e683 b3e8 a681 e88e b7e5 8f96  ................
-00000f90: e5ae 83e7 9a84 e99f b3e6 ba90 e4b8 8ee5  ................
-00000fa0: b081 e99d a2ef bc8c e4bb a5e4 b88b e4bb  ................
-00000fb0: a3e7 a081 e5b0 86e4 bc9a e8bf 9be8 a18c  ................
-00000fc0: e88e b7e5 8f96 efbc 9a0a 2020 2020 2020  ..........      
-00000fd0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00000fe0: 2020 2020 6672 6f6d 2062 6573 7464 6f72      from bestdor
-00000ff0: 692e 706f 7374 2069 6d70 6f72 7420 506f  i.post import Po
-00001000: 7374 0a20 2020 2020 2020 200a 2020 2020  st.        .    
-00001010: 2020 2020 6465 6620 6d61 696e 2829 202d      def main() -
-00001020: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00001030: 2020 2020 2320 e5ae 9ee4 be8b e58c 9620      # ......... 
-00001040: 506f 7374 20e7 b1bb 0a20 2020 2020 2020  Post ....       
-00001050: 2020 2020 2070 203d 2050 6f73 7428 6964       p = Post(id
-00001060: 3d27 3131 3135 3333 2729 0a20 2020 2020  ='111533').     
-00001070: 2020 2020 2020 2023 20e8 b083 e794 a8e6         # .......
-00001080: 96b9 e6b3 95e8 8eb7 e58f 96e8 b0b1 e99d  ................
-00001090: a20a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-000010a0: 6172 7420 3d20 702e 6765 745f 6368 6172  art = p.get_char
-000010b0: 7428 2920 2320 e88e b7e5 8f96 e79a 84e5  t() # ..........
-000010c0: b086 e698 afe4 b880 e4b8 aae8 b0b1 e99d  ................
-000010d0: a2e5 ae9e e4be 8b0a 2020 2020 2020 2020  ........        
-000010e0: 2020 2020 2320 e8b0 83e7 94a8 e696 b9e6      # ..........
-000010f0: b395 e88e b7e5 8f96 e99f b3e6 ba90 e4b8  ................
-00001100: 8ee5 b081 e99d a20a 2020 2020 2020 2020  ........        
-00001110: 2020 2020 696e 666f 203d 2070 2e67 6574      info = p.get
-00001120: 5f73 6f6e 6728 2920 2320 e88e b7e5 8f96  _song() # ......
-00001130: e79a 84e5 b086 e698 afe4 b880 e4b8 aae5  ................
-00001140: 8c85 e590 abe4 ba86 e99f b3e6 ba90 e4b8  ................
-00001150: 8ee5 b081 e99d a2e7 9a84 2062 7974 6573  .......... bytes
-00001160: 20e5 ad97 e585 b80a 2020 2020 2020 2020   .......        
-00001170: 0a20 2020 2020 2020 206d 6169 6e28 290a  .        main().
-00001180: 2020 2020 2020 2020 6060 600a 506c 6174          ```.Plat
-00001190: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
-000011a0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000011b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000011c0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000011d0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-000011e0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000011f0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00001200: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
-00001210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00001220: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00001230: 740a 5265 7175 6972 6573 2d50 7974 686f  t.Requires-Pytho
-00001240: 6e3a 203e 3d33 2e38 0a44 6573 6372 6970  n: >=3.8.Descrip
-00001250: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00001260: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00001270: 0a                                       .
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a0a 215b 6265 7374 646f 7269  er">..![bestdori
+00000020: 2d61 7069 206c 6f67 6f5d 2868 7474 7073  -api logo](https
+00000030: 3a2f 2f67 6974 6875 622e 636f 6d2f 5769  ://github.com/Wi
+00000040: 6e64 6f77 7353 6f76 3866 6f72 5573 2f62  ndowsSov8forUs/b
+00000050: 6573 7464 6f72 692d 6170 692f 626c 6f62  estdori-api/blob
+00000060: 2f6d 6169 6e2f 6c6f 676f 2e70 6e67 290a  /main/logo.png).
+00000070: 0a23 2042 6573 7464 6f72 692d 6170 690a  .# Bestdori-api.
+00000080: 0a5f e29c a820 5b42 6573 7464 6f72 695d  ._... [Bestdori]
+00000090: 2868 7474 7073 3a2f 2f62 6573 7464 6f72  (https://bestdor
+000000a0: 692e 636f 6d2f 2920 e79a 84e5 9084 e7a7  i.com/) ........
+000000b0: 8d20 4150 4920 e8b0 83e7 94a8 e695 b4e5  . API ..........
+000000c0: 9088 efbc 8ce5 8fa6 e5a4 96e9 9984 e5b8  ................
+000000d0: a6e9 83a8 e588 86e5 8a9f e883 bd20 e29c  ............. ..
+000000e0: a85f 0a0a 2a2a 3a77 6172 6e69 6e67 3a20  ._..**:warning: 
+000000f0: e8af a5e9 a1b9 e79b aee4 bb8d e784 b6e6  ................
+00000100: 80a5 e99c 80e6 9bb4 e696 b0e4 b88e 2044  .............. D
+00000110: 6562 7567 20ef bc8c e4bd bfe7 94a8 e697  ebug ...........
+00000120: b6e8 8ba5 e981 87e5 88b0 2042 7567 20e6  .......... Bug .
+00000130: 8896 e585 b6e4 bb96 e99c 80e8 a681 e79a  ................
+00000140: 84e6 8ea5 e58f a3e8 afb7 e58f 8ae6 97b6  ................
+00000150: e68f 90e5 87ba 2a2a 0a0a 3c2f 6469 763e  ......**..</div>
+00000160: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000170: 6572 223e 0a0a 3c61 2068 7265 663d 2268  er">..<a href="h
+00000180: 7474 7073 3a2f 2f62 6573 7464 6f72 692e  ttps://bestdori.
+00000190: 636f 6d2f 223e 0a20 203c 696d 6720 7372  com/">.  <img sr
+000001a0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001b0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000001c0: 6265 7374 646f 7269 2d61 7069 2d31 3937  bestdori-api-197
+000001d0: 3644 3322 2061 6c74 3d22 6c69 6365 6e73  6D3" alt="licens
+000001e0: 6522 3e0a 3c2f 613e 0a0a 3c61 2068 7265  e">.</a>..<a hre
+000001f0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+00000200: 622e 636f 6d2f 5769 6e64 6f77 7353 6f76  b.com/WindowsSov
+00000210: 3866 6f72 5573 2f62 6573 7464 6f72 692d  8forUs/bestdori-
+00000220: 6170 6922 3e0a 2020 3c69 6d67 2073 7263  api">.  <img src
+00000230: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000240: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00000250: 762f 7265 6c65 6173 652f 5769 6e64 6f77  v/release/Window
+00000260: 7353 6f76 3866 6f72 5573 2f62 6573 7464  sSov8forUs/bestd
+00000270: 6f72 692d 6170 6922 2061 6c74 3d22 4c61  ori-api" alt="La
+00000280: 7465 7374 2052 656c 6561 7365 2056 6572  test Release Ver
+00000290: 7369 6f6e 223e 0a3c 2f61 3e0a 0a3c 6120  sion">.</a>..<a 
+000002a0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000002b0: 7468 7562 2e63 6f6d 2f57 696e 646f 7773  thub.com/Windows
+000002c0: 536f 7638 666f 7255 732f 6265 7374 646f  Sov8forUs/bestdo
+000002d0: 7269 2d61 7069 2f62 6c6f 622f 6d61 696e  ri-api/blob/main
+000002e0: 2f4c 4943 454e 5345 223e 0a20 203c 696d  /LICENSE">.  <im
+000002f0: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
+00000300: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00000310: 7468 7562 2f6c 6963 656e 7365 2f57 696e  thub/license/Win
+00000320: 646f 7773 536f 7638 666f 7255 732f 6265  dowsSov8forUs/be
+00000330: 7374 646f 7269 2d61 7069 2220 616c 743d  stdori-api" alt=
+00000340: 224c 6963 656e 7365 223e 0a3c 2f61 3e0a  "License">.</a>.
+00000350: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000360: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+00000370: 2f64 6f77 6e6c 6f61 6473 2f22 3e0a 2020  /downloads/">.  
+00000380: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000390: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000003a0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+000003b0: 2f62 6573 7464 6f72 692d 6170 6922 2061  /bestdori-api" a
+000003c0: 6c74 3d22 5079 7468 6f6e 2056 6572 7369  lt="Python Versi
+000003d0: 6f6e 223e 0a3c 2f61 3e0a 0a3c 2f70 3e0a  on">.</a>..</p>.
+000003e0: 0a3e 2062 6573 7464 6f72 695f 6170 6920  .> bestdori_api 
+000003f0: e5b7 b2e6 9bb4 e590 8de4 b8ba 2062 6573  ............ bes
+00000400: 7464 6f72 692d 6170 690a 3e20 e88b a5e5  tdori-api.> ....
+00000410: ae89 e8a3 85e8 bf87 e4b9 8be5 898d e79a  ................
+00000420: 8420 6062 6573 7464 6f72 695f 6170 6960  . `bestdori_api`
+00000430: 20e5 8c85 efbc 8ce8 afb7 e4bd bfe7 94a8   ...............
+00000440: e68c 87e4 bba4 0a3e 2060 6060 6261 7368  .......> ```bash
+00000450: 0a3e 2070 6970 2075 6e69 6e73 7461 6c6c  .> pip uninstall
+00000460: 2062 6573 7464 6f72 695f 6170 690a 3e20   bestdori_api.> 
+00000470: 6060 600a 3e20 0a3e 20e5 8db8 e8bd bde5  ```.> .> .......
+00000480: 8e9f 2060 6265 7374 646f 7269 5f61 7069  .. `bestdori_api
+00000490: 6020 e58c 85e5 908e efbc 8ce9 878d e696  ` ..............
+000004a0: b0e5 ae89 e8a3 8520 6062 6573 7464 6f72  ....... `bestdor
+000004b0: 692d 6170 6960 20e5 8c85 0a3e 20e5 90a6  i-api` ....> ...
+000004c0: e588 99e5 8faf e883 bde5 afbc e887 b4e6  ................
+000004d0: 9caa e79f a5e7 9a84 e586 b2e7 aa81 e997  ................
+000004e0: aee9 a298 0a0a 2323 20e7 ae80 e4bb 8b0a  ......## .......
+000004f0: 0ae8 bf99 e698 afe4 b880 e4b8 aae7 94a8  ................
+00000500: 2050 7974 686f 6e20 e7bc 96e5 8699 e79a   Python ........
+00000510: 84e8 b083 e794 a820 5b42 6573 7464 6f72  ....... [Bestdor
+00000520: 695d 2868 7474 7073 3a2f 2f62 6573 7464  i](https://bestd
+00000530: 6f72 692e 636f 6d2f 2920 e590 84e7 a78d  ori.com/) ......
+00000540: 2041 5049 20e4 b88e e8b5 84e6 ba90 e4b8   API ...........
+00000550: 8be8 bdbd e79a 84e5 ba93 efbc 8ce5 a4a7  ................
+00000560: e887 b4e5 8c85 e68b ace4 ba86 e7a4 bee5  ................
+00000570: 8cba e5b8 96e5 ad90 e79a 84e5 a484 e790  ................
+00000580: 86e4 bba5 e58f 8ae5 9084 e7a7 8d20 5b42  ............. [B
+00000590: 616e 4720 4472 6561 6def bc81 e5b0 91e5  anG Dream.......
+000005a0: a5b3 e4b9 90e5 9ba2 e6b4 bee5 afb9 5d28  ..............](
+000005b0: 6874 7470 733a 2f2f 7a68 2e6d 6f65 6769  https://zh.moegi
+000005c0: 726c 2e6f 7267 2e63 6e2f 4261 6e47 5f44  rl.org.cn/BanG_D
+000005d0: 7265 616d 215f 2545 3525 4230 2539 3125  ream!_%E5%B0%91%
+000005e0: 4535 2541 3525 4233 2545 3425 4239 2539  E5%A5%B3%E4%B9%9
+000005f0: 3025 4535 2539 4225 4132 2545 3625 4234  0%E5%9B%A2%E6%B4
+00000600: 2542 4525 4535 2541 4625 4239 2545 4625  %BE%E5%AF%B9%EF%
+00000610: 4243 2538 3129 20e6 b8b8 e688 8fe5 8685  BC%81) .........
+00000620: e8b5 84e6 ba90 e79a 84e8 8eb7 e58f 96e3  ................
+00000630: 8082 0a2a 2ae8 ada6 e591 8aef bc9a e6ad  ...**...........
+00000640: a4e6 a8a1 e59d 97e7 9bae e589 8de4 bb8d  ................
+00000650: e784 b6e4 ba9f e5be 85e5 ae8c e596 84e4  ................
+00000660: b88e e6b5 8be8 af95 efbc 8ce8 afb7 e4b8  ................
+00000670: 8de8 a681 e5b0 86e5 85b6 e5bd 93e5 819a  ................
+00000680: e4b8 80e4 b8aa e7a8 b3e5 ae9a e79a 84e5  ................
+00000690: ba93 e4bd bfe7 94a8 e380 822a 2a0a 0a23  ...........**..#
+000006a0: 2323 20e7 9bae e589 8de5 b7b2 e69c 89e7  ## .............
+000006b0: 9a84 2041 5049 20e4 b88e e58a 9fe8 83bd  .. API .........
+000006c0: 0a0a 7c41 5049 20e7 b1bb e588 ab7c e698  ..|API ......|..
+000006d0: afe5 90a6 e5ae 8ce5 9684 7ce6 94af e68c  ..........|.....
+000006e0: 81e7 9a84 e586 85e5 aeb9 7c0a 7c3a 2d2d  ..........|.|:--
+000006f0: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 3a7c 3a2d  -----|:-----:|:-
+00000700: 2d2d 2d2d 2d7c 0a7c e794 a8e6 88b7 7cf0  -----|.|......|.
+00000710: 9f91 8d7c e799 bbe5 bd95 e380 81e6 9fa5  ...|............
+00000720: e8af a2e3 8081 e5b8 96e5 ad90 e88e b7e5  ................
+00000730: 8f96 e380 81e4 bfa1 e681 afe8 8eb7 e58f  ................
+00000740: 967c 0a7c e5b8 96e5 ad90 7cf0 9f91 8d7c  .|.|......|....|
+00000750: e690 9ce7 b4a2 e380 81e8 8eb7 e58f 96e3  ................
+00000760: 8081 e58f 91e8 a1a8 e380 81e8 af84 e8ae  ................
+00000770: bae3 8081 e596 9ce6 aca2 7c0a 7ce8 b0b1  ..........|.|...
+00000780: e99d a27c f09f 918d 7ce7 a4be e58c bae8  ...|....|.......
+00000790: b0b1 e99d a2e8 8eb7 e58f 96e3 8081 e99f  ................
+000007a0: b3e6 ba90 e4b8 8ee5 b081 e99d a2e8 8eb7  ................
+000007b0: e58f 96e3 8081 e8a7 84e6 95b4 e58c 96e3  ................
+000007c0: 8081 e695 b0e6 8dae e7bb 9fe8 aea1 e380  ................
+000007d0: 81e6 a0bc e5bc 8fe4 ba92 e8bd ac7c 0a7c  .............|.|
+000007e0: e695 85e4 ba8b 7cf0 9f91 8ef0 9f91 8e7c  ......|........|
+000007f0: e7a4 bee5 8cba e695 85e4 ba8b e88e b7e5  ................
+00000800: 8f96 7c0a 7ce8 a792 e889 b27c f09f a494  ..|.|......|....
+00000810: 7ce4 bfa1 e681 afe8 8eb7 e58f 96e3 8081  |...............
+00000820: e8b5 84e6 ba90 e88e b7e5 8f96 7c0a 7ce5  ............|.|.
+00000830: 8da1 e789 8c7c f09f 918e 7ce4 bfa1 e681  .....|....|.....
+00000840: afe8 8eb7 e58f 96e3 8081 e8b5 84e6 ba90  ................
+00000850: e88e b7e5 8f96 7c0a 7ce6 9c8d e8a3 857c  ......|.|......|
+00000860: f09f 918e f09f 918e 7ce4 bfa1 e681 afe8  ........|.......
+00000870: 8eb7 e58f 967c 0a7c e6b4 bbe5 8aa8 7cf0  .....|.|......|.
+00000880: 9fa4 947c e4bf a1e6 81af e88e b7e5 8f96  ...|............
+00000890: e380 81e8 b584 e6ba 90e8 8eb7 e58f 967c  ...............|
+000008a0: 0a7c e6b4 bbe5 8aa8 e695 b0e6 8dae 7cf0  .|............|.
+000008b0: 9f91 8e7c e695 b0e6 8dae e88e b7e5 8f96  ...|............
+000008c0: 7c0a 7ce6 8b9b e58b 9f7c f09f a494 7ce6  |.|......|....|.
+000008d0: 95b0 e68d aee8 8eb7 e58f 96e3 8081 e8b5  ................
+000008e0: 84e6 ba90 e88e b7e5 8f96 7c0a 7ce6 ad8c  ..........|.|...
+000008f0: e69b b27c f09f a494 7ce4 bfa1 e681 afe8  ...|....|.......
+00000900: 8eb7 e58f 96e3 8081 e8b5 84e6 ba90 e88e  ................
+00000910: b7e5 8f96 7c0a 7ce6 ad8c e69b b220 4d65  ....|.|...... Me
+00000920: 7461 7cf0 9f91 8ef0 9f91 8e7c e695 b0e6  ta|........|....
+00000930: 8dae e88e b7e5 8f96 7c0a 7ce7 99bb e5bd  ........|.|.....
+00000940: 95e5 a596 e58a b17c f09f a494 7ce4 bfa1  .......|....|...
+00000950: e681 afe8 8eb7 e58f 96e3 8081 e8b5 84e6  ................
+00000960: ba90 e88e b7e5 8f96 7c0a 7ce8 87aa e980  ........|.|.....
+00000970: 89e5 88b8 7cf0 9fa4 947c e4bf a1e6 81af  ....|....|......
+00000980: e88e b7e5 8f96 7c0a 7ce6 bcab e794 bb7c  ......|.|......|
+00000990: f09f a494 7ce4 bfa1 e681 afe8 8eb7 e58f  ....|...........
+000009a0: 96e3 8081 e59b bee7 8987 e88e b7e5 8f96  ................
+000009b0: 7c0a 7ce4 bbbb e58a a17c f09f a494 7ce4  |.|......|....|.
+000009c0: bfa1 e681 afe8 8eb7 e58f 967c 0a7c 6179  ...........|.|ay
+000009d0: 6163 6861 6e7c f09f a494 7ce8 b0b1 e99d  achan|....|.....
+000009e0: a2e5 8886 e69e 90e3 8081 e6b5 8be8 af95  ................
+000009f0: e69c 8de4 b88a e4bc a0e3 8081 e99a bee5  ................
+00000a00: baa6 e588 86e6 9e90 7c0a 7ce5 85b6 e4bb  ........|.|.....
+00000a10: 96e8 b584 e6ba 907c f09f 918e f09f 918e  .......|........
+00000a20: 7ce4 bb85 e5b0 8fe9 83a8 e588 86e8 b584  |...............
+00000a30: e6ba 90e6 9c89 e58d 95e7 8bac e88e b7e5  ................
+00000a40: 8f96 7c0a 0a23 2320 e5bf abe9 809f e4bd  ..|..## ........
+00000a50: bfe7 94a8 0a0a e4bb a5e4 b88b e5b0 86e4  ................
+00000a60: bba5 e88e b7e5 8f96 e7a4 bee5 8cba e887  ................
+00000a70: aae5 88b6 e8b0 b1e9 9da2 205b 5b46 554c  .......... [[FUL
+00000a80: 4c5d 20e5 8589 e381 aee4 b8ad e381 b85d  L] ............]
+00000a90: 2868 7474 7073 3a2f 2f62 6573 7464 6f72  (https://bestdor
+00000aa0: 692e 636f 6d2f 636f 6d6d 756e 6974 792f  i.com/community/
+00000ab0: 6368 6172 7473 2f31 3131 3533 332f 5769  charts/111533/Wi
+00000ac0: 6e64 6f77 7353 6f76 382d 4655 4c4c 2920  ndowsSov8-FULL) 
+00000ad0: e79a 84e4 bfa1 e681 afe4 b8ba e4be 8be3  ................
+00000ae0: 8082 0a0a e9a6 96e5 8588 efbc 8ce4 bdbf  ................
+00000af0: e794 a8e4 bba5 e4b8 8be6 8c87 e4bb a4e5  ................
+00000b00: ae89 e8a3 85e6 9cac e6a8 a1e5 9d97 efbc  ................
+00000b10: 9a0a 6060 6062 6173 680a 2420 7069 7033  ..```bash.$ pip3
+00000b20: 2069 6e73 7461 6c6c 2062 6573 7464 6f72   install bestdor
+00000b30: 692d 6170 690a 6060 600a e68e a5e4 b88b  i-api.```.......
+00000b40: e69d a5e5 9ca8 e4b8 80e4 b8aa 2050 7974  ............ Pyt
+00000b50: 686f 6e20 e884 9ae6 9cac e696 87e4 bbb6  hon ............
+00000b60: e4b8 adef bc8c e4bd bfe7 94a8 e5a6 82e4  ................
+00000b70: b88b e4bb a3e7 a081 e88e b7e5 8f96 e68c  ................
+00000b80: 87e5 ae9a e5b8 96e5 ad90 e79a 84e5 85a8  ................
+00000b90: e983 a8e4 bfa1 e681 afef bc88 e8bf 99e9  ................
+00000ba0: 878c e688 91e4 bbac e5b7 b2e7 9fa5 e8af  ................
+00000bb0: a5e5 b896 e5ad 90e7 9a84 2049 4420 e4b8  .......... ID ..
+00000bc0: ba20 6031 3131 3533 3360 efbc 89ef bc9a  . `111533`......
+00000bd0: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00000be0: 6265 7374 646f 7269 2e70 6f73 7420 696d  bestdori.post im
+00000bf0: 706f 7274 2050 6f73 740a 0a64 6566 206d  port Post..def m
+00000c00: 6169 6e28 2920 2d3e 204e 6f6e 653a 0a20  ain() -> None:. 
+00000c10: 2020 2023 20e5 ae9e e4be 8be5 8c96 2050     # ......... P
+00000c20: 6f73 7420 e7b1 bb0a 2020 2020 7020 3d20  ost ....    p = 
+00000c30: 506f 7374 2869 643d 2731 3131 3533 3327  Post(id='111533'
+00000c40: 290a 2020 2020 2320 e8b0 83e7 94a8 e696  ).    # ........
+00000c50: b9e6 b395 e88e b7e5 8f96 e4bf a1e6 81af  ................
+00000c60: 0a20 2020 2069 6e66 6f20 3d20 702e 6765  .    info = p.ge
+00000c70: 745f 6465 7461 696c 7328 290a 2020 2020  t_details().    
+00000c80: 2320 e689 93e5 8db0 e4bf a1e6 81af 0a20  # ............. 
+00000c90: 2020 2070 7269 6e74 2869 6e66 6f29 0a0a     print(info)..
+00000ca0: 6d61 696e 2829 0a60 6060 0ae5 be97 e588  main().```......
+00000cb0: b0e7 9a84 e8be 93e5 87ba e586 85e5 aeb9  ................
+00000cc0: e5a6 82e4 b88b efbc 9a0a 6060 6070 7974  ..........```pyt
+00000cd0: 686f 6e0a 7b0a 2020 2020 2763 6174 6567  hon.{.    'categ
+00000ce0: 6f72 794e 616d 6527 3a20 2753 454c 465f  oryName': 'SELF_
+00000cf0: 504f 5354 272c 0a20 2020 2027 6361 7465  POST',.    'cate
+00000d00: 676f 7279 4964 273a 2027 6368 6172 7427  goryId': 'chart'
+00000d10: 2c0a 2020 2020 2774 6974 6c65 273a 2027  ,.    'title': '
+00000d20: 5b46 554c 4c5d 20e5 8589 e381 aee4 b8ad  [FULL] .........
+00000d30: e381 b827 2c0a 2020 2020 2773 6f6e 6727  ...',.    'song'
+00000d40: 3a20 7b0a 2020 2020 2020 2020 2774 7970  : {.        'typ
+00000d50: 6527 3a20 2763 7573 746f 6d27 2c0a 2020  e': 'custom',.  
+00000d60: 2020 2020 2020 2761 7564 696f 273a 2027        'audio': '
+00000d70: 6874 7470 733a 2f2f 6265 7374 646f 7269  https://bestdori
+00000d80: 2e63 6f6d 2f61 7069 2f75 706c 6f61 642f  .com/api/upload/
+00000d90: 6669 6c65 2f65 3461 3038 3066 3834 6266  file/e4a080f84bf
+00000da0: 6132 6361 3437 6232 3362 3339 3061 3436  a2ca47b23b390a46
+00000db0: 3463 3831 3965 6331 3765 3730 6227 2c0a  4c819ec17e70b',.
+00000dc0: 2020 2020 2020 2020 2763 6f76 6572 273a          'cover':
+00000dd0: 2027 6874 7470 733a 2f2f 6265 7374 646f   'https://bestdo
+00000de0: 7269 2e63 6f6d 2f61 7069 2f75 706c 6f61  ri.com/api/uploa
+00000df0: 642f 6669 6c65 2f65 3335 3335 6562 6234  d/file/e3535ebb4
+00000e00: 6337 3430 6334 3735 3733 3731 3032 3661  c740c4757371026a
+00000e10: 3164 6639 6666 6230 3830 3130 3330 3727  1df9ffb08010307'
+00000e20: 0a20 2020 207d 2c0a 2020 2020 2761 7274  .    },.    'art
+00000e30: 6973 7473 273a 2027 e7b5 90e6 9d9f e383  ists': '........
+00000e40: 90e3 83b3 e383 8927 2c0a 2020 2020 2764  .......',.    'd
+00000e50: 6966 6627 3a20 342c 0a20 2020 2027 6c65  iff': 4,.    'le
+00000e60: 7665 6c27 3a20 3330 2c0a 2020 2020 2763  vel': 30,.    'c
+00000e70: 6861 7274 273a 205b 0a20 2020 2020 2020  hart': [.       
+00000e80: 207b 0a20 2020 2020 2020 2020 2020 2027   {.            '
+00000e90: 6270 6d27 3a20 3139 312c 0a20 2020 2020  bpm': 191,.     
+00000ea0: 2020 2020 2020 2027 6265 6174 273a 2030         'beat': 0
+00000eb0: 2c0a 2020 2020 2020 2020 2020 2020 2774  ,.            't
+00000ec0: 7970 6527 3a20 2742 504d 270a 2020 2020  ype': 'BPM'.    
+00000ed0: 2020 2020 7d2c 0a20 2020 2020 2020 207b      },.        {
+00000ee0: 0a20 2020 2020 2020 2020 2020 2027 6265  .            'be
+00000ef0: 6174 273a 2031 3932 2c0a 2020 2020 2020  at': 192,.      
+00000f00: 2020 2020 2020 276c 616e 6527 3a20 332e        'lane': 3.
+00000f10: 0a20 2020 2020 2020 2020 2020 2027 7479  .            'ty
+00000f20: 7065 273a 2027 5369 6e67 6c65 270a 2020  pe': 'Single'.  
+00000f30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000f40: 202e 2e2e 0a20 2020 205d 2c0a 2020 2020   ....    ],.    
+00000f50: 2e2e 2e0a 7d0a 6060 600a e5a6 82e6 9e9c  ....}.```.......
+00000f60: e683 b3e8 a681 e88e b7e5 8f96 e8bf 99e4  ................
+00000f70: b8aa e887 aae5 88b6 e8b0 b1e9 9da2 e79a  ................
+00000f80: 84e8 b0b1 e99d a2ef bc8c e688 96e8 8085  ................
+00000f90: e683 b3e8 a681 e88e b7e5 8f96 e5ae 83e7  ................
+00000fa0: 9a84 e99f b3e6 ba90 e4b8 8ee5 b081 e99d  ................
+00000fb0: a2ef bc8c e4bb a5e4 b88b e4bb a3e7 a081  ................
+00000fc0: e5b0 86e4 bc9a e8bf 9be8 a18c e88e b7e5  ................
+00000fd0: 8f96 efbc 9a0a 6060 6070 7974 686f 6e0a  ......```python.
+00000fe0: 6672 6f6d 2062 6573 7464 6f72 692e 706f  from bestdori.po
+00000ff0: 7374 2069 6d70 6f72 7420 506f 7374 0a0a  st import Post..
+00001000: 6465 6620 6d61 696e 2829 202d 3e20 4e6f  def main() -> No
+00001010: 6e65 3a0a 2020 2020 2320 e5ae 9ee4 be8b  ne:.    # ......
+00001020: e58c 9620 506f 7374 20e7 b1bb 0a20 2020  ... Post ....   
+00001030: 2070 203d 2050 6f73 7428 6964 3d27 3131   p = Post(id='11
+00001040: 3135 3333 2729 0a20 2020 2023 20e8 b083  1533').    # ...
+00001050: e794 a8e6 96b9 e6b3 95e8 8eb7 e58f 96e8  ................
+00001060: b0b1 e99d a20a 2020 2020 6368 6172 7420  ......    chart 
+00001070: 3d20 702e 6765 745f 6368 6172 7428 2920  = p.get_chart() 
+00001080: 2320 e88e b7e5 8f96 e79a 84e5 b086 e698  # ..............
+00001090: afe4 b880 e4b8 aae8 b0b1 e99d a2e5 ae9e  ................
+000010a0: e4be 8b0a 2020 2020 2320 e8b0 83e7 94a8  ....    # ......
+000010b0: e696 b9e6 b395 e88e b7e5 8f96 e99f b3e6  ................
+000010c0: ba90 e4b8 8ee5 b081 e99d a20a 2020 2020  ............    
+000010d0: 696e 666f 203d 2070 2e67 6574 5f73 6f6e  info = p.get_son
+000010e0: 6728 2920 2320 e88e b7e5 8f96 e79a 84e5  g() # ..........
+000010f0: b086 e698 afe4 b880 e4b8 aae5 8c85 e590  ................
+00001100: abe4 ba86 e99f b3e6 ba90 e4b8 8ee5 b081  ................
+00001110: e99d a2e7 9a84 2062 7974 6573 20e5 ad97  ...... bytes ...
+00001120: e585 b80a 0a6d 6169 6e28 290a 6060 60    .....main().```
```

### Comparing `bestdori_api-0.1.9/bestdori/__init__.py` & `bestdori-api-0.2.0/bestdori/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,19 @@
     eventarchives,
     gacha,
     songs,
     songmeta,
     logincampaigns,
     miracleticket,
     comics,
-    missions
+    missions,
+    models
 )
 
-from ._settings import settings
+from .utils._settings import settings
 
 __all__ = [
     'User',
     'Me',
     'Post',
     'Chart',
     'Character',
@@ -127,9 +128,10 @@
     'gacha',
     'songs',
     'songmeta',
     'logincampaigns',
     'miracleticket',
     'comics',
     'missions',
+    'models',
     'settings'
 ]
```

### Comparing `bestdori_api-0.1.9/bestdori/cards.py` & `bestdori-api-0.2.0/bestdori/cards.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''`bestdori.cards`
 
 BanG Dream! 卡牌相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, RES, ASSETS
 from .utils.network import Api, Res, Assets
 from .exceptions import (
+    NoDataException,
     CardNotExistError
 )
 
 # 获取总卡牌信息
 def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
     '''获取总卡牌信息
 
@@ -19,15 +19,15 @@
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有卡牌 ID `all.0.json`
             `5`: 获取所有已有卡牌的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总卡牌信息
     '''
-    return Api(API['cards']['all'].format(index), proxy=settings.proxy).request('get').json()
+    return Api(API['cards']['all'].format(index=index)).request('get').json()
 
 # 获取属性图标
 def get_attribute_icon(attribute: Literal['powerful', 'pure', 'cool', 'happy']) -> bytes:
     '''获取属性图标
 
     参数:
         attribute (Literal[&#39;powerful&#39;, &#39;pure&#39;, &#39;cool&#39;, &#39;happy&#39;]): 属性名称
@@ -35,89 +35,89 @@
             `pure`: PURE
             `cool`: COOL
             `happy`: HAPPY
 
     返回:
         bytes: 属性图标字节数据
     '''
-    return Res(RES['icon']['svg'].format(name=f'{attribute}'), settings.proxy).get()
+    return Res(RES['icon']['svg'].format(name=f'{attribute}')).get()
 
 # 获取星星图标
 def get_star_icon(star: Literal['star', 'star_trained']) -> bytes:
     '''获取星星图标
 
     参数:
         star (Literal[&#39;star&#39;, &#39;star_trained&#39;]): 星标种类
             `star`: 普通星标
             `star_trained`: 训练后星标
 
     返回:
         bytes: 星星图标字节数据
     '''
-    return Res(RES['icon']['png'].format(name=f'{star}'), settings.proxy).get()
+    return Res(RES['icon']['png'].format(name=f'{star}')).get()
 
 # 获取卡牌完整边框
 def get_frame(level: Literal[1, 2, 3, 4, 5]) -> bytes:
     '''获取卡牌完整边框
 
     参数:
         level (Literal[1, 2, 3, 4, 5]): 边框星级
 
     返回:
         bytes: 卡牌完整边框字节数据
     '''
-    return Res(RES['image']['png'].format(f'frame-{level}'), settings.proxy).get()
+    return Res(RES['image']['png'].format(name=f'frame-{level}')).get()
 
 # 获取卡牌缩略图边框
 def get_card_frame(level: Literal[1, 2, 3, 4, 5]) -> bytes:
     '''获取卡牌缩略图边框
 
     参数:
         level (Literal[1, 2, 3, 4, 5]): 边框星级
 
     返回:
         bytes: 卡牌缩略图边框字节数据
     '''
-    return Res(RES['image']['png'].format(f'card-{level}'), settings.proxy).get()
+    return Res(RES['image']['png'].format(name=f'card-{level}')).get()
 
 # 卡牌类
 class Card:
     '''卡牌类
 
     参数:
-        id_ (int): 卡牌 ID
+        id (int): 卡牌 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''卡牌类
 
         参数:
-            id_ (int): 卡牌 ID
+            id (int): 卡牌 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''卡牌 ID'''
         self._info: dict[str, Any] = {}
         '''卡牌信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not str(id_) in all_id.keys():
-            raise CardNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise CardNotExistError(id)
         return
     
     # 获取卡牌信息
     def get_info(self) -> dict[str, Any]:
         '''获取卡牌信息
 
         返回:
             dict[str, Any]: 卡牌详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有卡牌信息存储
             response = Api(
-                API['cards']['info'].format(self.id), proxy=settings.proxy
+                API['cards']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取卡牌评论
     def get_comment(
         self,
@@ -155,100 +155,100 @@
 
         返回:
             str: 卡牌标题
         '''
         info = self.get_info()
         # 获取 prefix 数据
         if (prefix := info.get('prefix', None)) is None:
-            raise Exception('无法获取卡牌标题。')
+            raise NoDataException('卡牌标题')
         # 获取第一个非 None 卡牌标题
         try:
             return next(filter(lambda x: x is not None, prefix))
         except StopIteration:
-            raise Exception('无法获取卡牌标题。')
+            raise NoDataException('卡牌标题')
     
     # 获取卡牌所在服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取卡牌所在服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 releasedAt 数据
         if (released_at := info.get('releasedAt', None)) is None:
-            raise Exception('无法获取卡牌发布时间。')
+            raise NoDataException('卡牌发布时间')
         # 根据 releasedAt 数据判断服务器
         if released_at[0] is not None: return 'jp'
         elif released_at[1] is not None: return 'en'
         elif released_at[2] is not None: return 'tw'
         elif released_at[3] is not None: return 'cn'
         elif released_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取卡牌所在服务器。')
+            raise NoDataException('卡牌所在服务器')
     
     # 获取卡牌完整图片
-    def get_card(self, type_: Literal['normal', 'after_training']) -> bytes:
+    def get_card(self, type: Literal['normal', 'after_training']) -> bytes:
         '''获取卡牌完整图片
 
         参数:
-            type_ (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
+            type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
 
         返回:
             bytes: 卡牌完整图片字节数据 `bytes`
         '''
         # 获取卡牌数据包名称
         info = self.get_info()
         if (resource_set_name := info.get('resourceSetName', None)) is None:
             raise ValueError('无法获取卡牌数据包名称。')
         return Assets(
             ASSETS['characters']['resourceset'].format(
-                resource_set_name=resource_set_name, name='card', type=type_
-            ), self.server, settings.proxy
+                resource_set_name=resource_set_name, name='card', type=type
+            ), self.server
         ).get()
     
     # 获取卡牌无背景图片
-    def get_trim(self, type_: Literal['normal', 'after_training']) -> bytes:
+    def get_trim(self, type: Literal['normal', 'after_training']) -> bytes:
         '''获取卡牌无背景图片
 
         参数:
-            type_ (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
+            type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
 
         返回:
             bytes: 卡牌无背景图片字节数据 `bytes`
         '''
         # 获取卡牌数据包名称
         info = self.get_info()
         if (resource_set_name := info.get('resourceSetName', None)) is None:
             raise ValueError('无法获取卡牌数据包名称。')
         return Assets(
             ASSETS['characters']['resourceset'].format(
-                resource_set_name=resource_set_name, name='trim', type=type_
-            ), self.server, settings.proxy
+                resource_set_name=resource_set_name, name='trim', type=type
+            ), self.server
         ).get()
     
     # 获取卡牌缩略图图片
-    def get_thumb(self, type_: Literal['normal', 'after_training']) -> bytes:
+    def get_thumb(self, type: Literal['normal', 'after_training']) -> bytes:
         '''获取卡牌缩略图图片
 
         参数:
             type (Literal[&#39;normal&#39;, &#39;after_training&#39;]): 指定特训前或特训后
 
         返回:
             bytes: 卡牌缩略图图片字节数据 `bytes`
         '''
         # 获取卡牌数据包名称
         info = self.get_info()
         if (resource_set_name := info.get('resourceSetName', None)) is None:
             raise ValueError('无法获取卡牌数据包名称。')
         return Assets(
             ASSETS['thumb']['chara'].format(
-                id=str(int(self.id) // 50), resource_set_name=resource_set_name, type=type_
-            ), self.server, settings.proxy
+                id=str(int(self.id) // 50), resource_set_name=resource_set_name, type=type
+            ), self.server
         ).get()
     
     # 获取 LIVE 服装图片
     def get_livesd(self) -> bytes:
         '''获取 LIVE 服装图片
 
         返回:
@@ -257,9 +257,9 @@
         # 获取卡牌 livesd 数据包名称
         info = self.get_info()
         if (sd_resource_name := info.get('sdResourceName', None)) is None:
             raise ValueError('无法获取卡牌 livesd 数据包名称。')
         return Assets(
             ASSETS['characters']['livesd'].format(
                 sd_resource_name=sd_resource_name
-            ), self.server, settings.proxy
+            ), self.server
         ).get()
```

### Comparing `bestdori_api-0.1.9/bestdori/characters.py` & `bestdori-api-0.2.0/bestdori/characters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 '''`bestdori.characters`
 
 BanG Dream! 角色相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from .utils import hex_to_rgb
-from ._settings import settings
+from .utils import hexto_rgb
 from .utils.utils import API, RES, ASSETS
 from .utils.network import Api, Res, Assets
 from .exceptions import (
+    NoDataException,
     CharacterNotExistError
 )
 
 # 获取总角色信息
 def get_all(index: Literal[2]=2) -> dict[str, dict[str, Any]]:
     '''获取总角色信息
 
     参数:
         index (Literal[2], optional): 指定获取哪种 `all.json`
             `2`: 获取所有已有角色信息 `all.2.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总角色信息
     '''
-    return Api(API['characters']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['characters']['all'].format(index=index)).request('get').json()
 
 # 获取主要角色信息
 def get_main(index: Literal[3]=3) -> dict[str, dict[str, Any]]:
     '''获取主要角色信息
 
     参数:
         index (Literal[3], optional): 指定获取哪种 `all.json`
             `3`: 获取所有已有主要角色信息 `all.3.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的主要角色信息
     '''
-    return Api(API['characters']['main'].format(index), settings.proxy).request('get').json()
+    return Api(API['characters']['main'].format(index=index)).request('get').json()
 
 # 角色类
 class Character:
     '''角色类
 
     参数:
-        id_ (int): 角色 ID
+        id (int): 角色 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''角色类
 
         参数:
-            id_ (int): 角色 ID
+            id (int): 角色 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''角色 ID'''
         self._info: dict[str, Any] = {}
         '''角色信息'''
         # 检测 ID 是否存在
         all_id = get_all(2)
-        if not str(id_) in all_id.keys():
-            raise CharacterNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise CharacterNotExistError(id)
         return
     
     # 获取角色信息
     def get_info(self) -> dict[str, Any]:
         '''获取角色信息
 
         返回:
             dict[str, Any]: 角色详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有角色信息存储
             response = Api(
-                API['characters']['info'].format(self.id), proxy=settings.proxy
+                API['characters']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取角色评论
     def get_comment(
         self,
@@ -114,20 +114,20 @@
 
         返回:
             str: 角色名称
         '''
         info = self.get_info()
         # 获取 characterName 数据
         if (character_name := info.get('characterName', None)) is None:
-            raise Exception('无法获取角色名称。')
+            raise NoDataException('角色名称')
         # 获取第一个非 None 角色名称
         try:
             return next(filter(lambda x: x is not None, character_name))
         except StopIteration:
-            raise Exception('无法获取角色名称。')
+            raise NoDataException('角色名称')
     
     # 获取角色图标
     @property
     def icon(self) -> bytes:
         '''获取角色图标
 
         返回:
@@ -142,24 +142,24 @@
 
         返回:
             tuple[int, int, int]: 角色颜色元组
         '''
         info = self.get_info()
         # 获取 colorCode 数据
         if (color_code := info.get('colorCode', None)) is None:
-            raise Exception('无法获取角色颜色。')
+            raise NoDataException('角色颜色')
         # 将 colorCode 转换为颜色元组
         try:
-            return hex_to_rgb(color_code)
+            return hexto_rgb(color_code)
         except ValueError:
-            raise Exception('无法获取角色颜色。')
+            raise NoDataException('角色颜色')
     
     # 获取角色主视觉图
     def get_kv_image(self) -> bytes:
         '''获取角色主视觉图
 
         返回:
             bytes: 主视觉图资源字节 `bytes`
         '''
         return Assets(
-            ASSETS['characters']['character_kv_image'].format(id=self.id), 'jp', settings.proxy
+            ASSETS['characters']['character_kv_image'].format(id=self.id), 'jp'
         ).get()
```

### Comparing `bestdori_api-0.1.9/bestdori/charts.py` & `bestdori-api-0.2.0/bestdori/charts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 '''`bestdori.charts`
 
 谱面相关操作'''
 from json import dumps, loads
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .utils.note import *
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
 
 # 谱面数据类
 class Statistics:
     '''谱面数据类
 
     参数:
         time (float): 谱面时长
@@ -269,21 +268,21 @@
         '''
         return cls(loads(data))
     
     # 获取官方谱面
     @classmethod
     def get_chart(
         cls,
-        id_: int,
+        id: int,
         diff: Literal['easy', 'normal', 'hard', 'expert', 'special']='expert'
     ) -> 'Chart':
         '''获取官方谱面
 
         参数:
-            id_ (int): 谱面 ID
+            id (int): 谱面 ID
             diff (Literal[&#39;easy&#39;, &#39;normal&#39;, &#39;hard&#39;, &#39;expert&#39;, &#39;special&#39;], optional): 难度名称
 
         返回:
             Chart: 获取到的谱面对象 `bestdori.chart.Chart`
         '''
-        response = Api(API['charts']['info'].format(id=id_, diff=diff), settings.proxy).request('get')
+        response = Api(API['charts']['info'].format(id=id, diff=diff)).request('get')
         return cls.normalize(response.json())
```

### Comparing `bestdori_api-0.1.9/bestdori/comics.py` & `bestdori-api-0.2.0/bestdori/comics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 '''`bestdori.comics`
 
 BanG Dream! 漫画相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .exceptions import (
-    ServerNotAvailableError,
-    ComicNotExistError
+    NoDataException,
+    ComicNotExistError,
+    ServerNotAvailableError
 )
 
 # 获取总漫画信息
 def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
     '''获取总漫画信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有漫画信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总漫画信息
     '''
-    return Api(API['all']['comics'].format(index), settings.proxy).request('get').json()
+    return Api(API['all']['comics'].format(index=index)).request('get').json()
 
 # 漫画类
 class Comic:
     '''漫画类
 
     参数:
-        id_ (int): 漫画 ID
+        id (int): 漫画 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''漫画类
 
         参数:
-            id_ (int): 漫画 ID
+            id (int): 漫画 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''漫画 ID'''
         self._info: dict[str, Any] = {}
         '''漫画信息'''
         # 检测 ID 是否存在
         all_ = get_all(5)
-        if not str(id_) in all_.keys():
-            raise ComicNotExistError(id_)
-        self._info = all_[str(id_)]
+        if not str(id) in all_.keys():
+            raise ComicNotExistError(id)
+        self._info = all_[str(id)]
         return
     
     # 获取漫画信息
     def get_info(self) -> dict[str, Any]:
         '''获取漫画信息
 
         返回:
@@ -96,59 +96,59 @@
 
         返回:
             str: 漫画标题
         '''
         info = self.get_info()
         # 获取 title 数据
         if (title := info.get('title', None)) is None:
-            raise Exception('无法获取漫画标题。')
+            raise NoDataException('漫画标题')
         # 获取第一个非 None 漫画标题
         try:
             return next(filter(lambda x: x is not None, title))
         except StopIteration:
-            raise Exception('无法获取漫画标题。')
+            raise NoDataException('漫画标题')
     
     # 获取漫画副标题
     @property
     def sub_title(self) -> str:
         '''获取漫画副标题
 
         返回:
             str: 漫画副标题
         '''
         info = self.get_info()
         # 获取 subTitle 数据
         if (sub_title := info.get('subTitle', None)) is None:
-            raise Exception('无法获取漫画副标题。')
+            raise NoDataException('漫画副标题')
         # 获取第一个非 None 漫画副标题
         try:
             return next(filter(lambda x: x is not None, sub_title))
         except StopIteration:
-            raise Exception('无法获取漫画副标题。')
+            raise NoDataException('漫画副标题')
     
     # 获取漫画默认服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取漫画默认服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 publicStartAt 数据
         if (public_start_at := info.get('publicStartAt', None)) is None:
-            raise Exception('无法获取漫画 ID 列表。')
+            raise NoDataException('漫画 ID 列表')
         # 根据 publicStartAt 数据判断服务器
         if public_start_at[0] is not None: return 'jp'
         elif public_start_at[1] is not None: return 'en'
         elif public_start_at[2] is not None: return 'tw'
         elif public_start_at[3] is not None: return 'cn'
         elif public_start_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取漫画所在服务器。')
+            raise NoDataException('漫画所在服务器')
 
     # 获取漫画类型
     @property
     def type(self) -> Literal['singleframe', 'fourframe']:
         '''获取漫画类型
 
         返回:
@@ -184,15 +184,15 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if public_start_at[index] is None:
             raise ServerNotAvailableError(f'漫画 {self.title}', server)
         return Assets(
             ASSETS['comic']['thumbnail'].format(
                 type=self.type, asset_bundle_name=asset_bundle_name
-            ), server, settings.proxy
+            ), server
         ).get()
     
     # 获取漫画图像
     def get(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取漫画图像
 
         参数:
@@ -211,9 +211,9 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if public_start_at[index] is None:
             raise ServerNotAvailableError(f'漫画 {self.title}', server)
         return Assets(
             ASSETS['comic']['comic'].format(
                 type=self.type, asset_bundle_name=asset_bundle_name
-            ), server, settings.proxy
+            ), server
         ).get()
```

### Comparing `bestdori_api-0.1.9/bestdori/costumes.py` & `bestdori-api-0.2.0/bestdori/costumes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 '''`bestdori.costumes`
 
 BanG Dream! 服装相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .exceptions import (
-    CostumeNotExistError,
-    AssetsNotExistError
+    NoDataException,
+    AssetsNotExistError,
+    CostumeNotExistError
 )
 
 # 获取总服装信息
 def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
     '''获取总服装信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有服装 ID `all.0.json`
             `5`: 获取所有已有服装的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总服装信息
     '''
-    return Api(API['costumes']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['costumes']['all'].format(index=index)).request('get').json()
 
 # 服装类
 class Costume:
     '''服装类
 
     参数:
-        id_ (int): 服装 ID
+        id (int): 服装 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''服装类
 
         参数:
-            id_ (int): 服装 ID
+            id (int): 服装 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''服装 ID'''
         self._info: dict[str, Any] = {}
         '''服装信息'''
         # 检测 ID 是否存在
         all_ = get_all(0)
-        if not str(id_) in all_.keys():
-            raise CostumeNotExistError(id_)
+        if not str(id) in all_.keys():
+            raise CostumeNotExistError(id)
         return
     
     # 获取服装信息
     def get_info(self) -> dict[str, Any]:
         '''获取服装信息
 
         返回:
             dict[str, Any]: 服装详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有服装信息存储
             response = Api(
-                API['costumes']['info'].format(self.id), settings.proxy
+                API['costumes']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取服装评论
     def get_comment(
         self,
@@ -91,32 +91,49 @@
             category_name='COSTUME_COMMENT',
             category_id=str(self.id),
             order=order,
             limit=limit,
             offset=offset
         )
     
+    # 获取 LIVE 服装图片
+    def get_sdchara(self) -> bytes:
+        '''获取 LIVE 服装图片
+
+        返回:
+            bytes: 服装 LIVE 图片字节数据 `bytes`
+        '''
+        # 获取服装 sdchara 数据包名称
+        info = self.get_info()
+        if (sd_resource_name := info.get('sdResourceName', None)) is None:
+            raise ValueError('无法获取服装数据包名称。')
+        return Assets(
+            ASSETS['characters']['livesd'].format(
+                sd_resource_name=sd_resource_name
+            ), self.server
+        ).get()
+    
     # 获取角色 ID
     @property
     def character_id(self) -> int:
         '''获取角色 ID'''
         info = self.get_info()
         # 获取 characterId 数据
         if (character_id := info.get('characterId', None)) is None:
-            raise Exception('无法获取角色 ID。')
+            raise NoDataException('角色 ID')
         return character_id
     
     # 获取卡牌 ID
     @property
     def card_id(self) -> int:
         '''获取角色 ID'''
         info = self.get_info()
         # 获取 cards 数据
         if (cards := info.get('cards', None)) is None:
-            raise Exception('无法获取卡牌 ID。')
+            raise NoDataException('卡牌 ID')
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(self.server)
         return cards[index]
     
     # 获取服装标题
     @property
     def description(self) -> str:
@@ -124,41 +141,41 @@
 
         返回:
             str: 服装标题
         '''
         info = self.get_info()
         # 获取 description 数据
         if (description := info.get('description', None)) is None:
-            raise Exception('无法获取服装标题。')
+            raise NoDataException('服装标题')
         # 获取第一个非 None 服装标题
         try:
             return next(filter(lambda x: x is not None, description))
         except StopIteration:
-            raise Exception('无法获取服装标题。')
+            raise NoDataException('服装标题')
     
     # 获取服装所在服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取服装所在服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 publishedAt 数据
         if (published_at := info.get('publishedAt', None)) is None:
-            raise Exception('无法获取服装发布时间。')
+            raise NoDataException('服装发布时间')
         # 根据 publishedAt 数据判断服务器
         if published_at[0] is not None: return 'jp'
         elif published_at[1] is not None: return 'en'
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取服装所在服务器。')
+            raise NoDataException('服装所在服务器')
     
     # 获取服装模型数据
     @property
     def build_data(self) -> bytes:
         '''获取服装模型数据
 
         返回:
@@ -168,15 +185,15 @@
         info = self.get_info()
         if (asset_bundle_name := info.get('assetBundleName', None)) is None:
             raise ValueError('无法获取服装数据包名称。')
         try:
             return Assets(
                 ASSETS['live2d']['buildData'].format(
                     asset_bundle_name=asset_bundle_name
-                ), self.server, settings.proxy
+                ), self.server
             ).get()
         except AssetsNotExistError:
             raise AssetsNotExistError(f'服装模型 {asset_bundle_name}-{self.server}')
     
     # 获取服装图标
     @property
     def icon(self) -> bytes:
@@ -188,12 +205,12 @@
         # 获取服装数据包名称
         info = self.get_info()
         if (asset_bundle_name := info.get('assetBundleName', None)) is None:
             raise ValueError('无法获取服装数据包名称。')
         try:
             return Assets(
                 ASSETS['thumb']['costume'].format(
-                    id=str(int(self.id) // 50), asset_bundle_name=asset_bundle_name
-                ), self.server, settings.proxy
+                    id=str(self.id // 50), asset_bundle_name=asset_bundle_name
+                ), self.server
             ).get()
         except AssetsNotExistError:
             raise AssetsNotExistError(f'服装图标 {asset_bundle_name}-{self.server}')
```

### Comparing `bestdori_api-0.1.9/bestdori/eventarchives.py` & `bestdori-api-0.2.0/bestdori/eventarchives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 '''`bestdori.eventarchives`
 
 BanG Dream! 活动数据相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
 from .exceptions import (
     EventNotExistError
 )
 
 # 获取总活动数据信息
 def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
     '''获取总活动信息
@@ -18,38 +17,38 @@
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有活动数据的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总活动信息
     '''
-    return Api(API['all']['archives'].format(index), settings.proxy).request('get').json()
+    return Api(API['all']['archives'].format(index=index)).request('get').json()
 
 # 活动数据类
 class EventArchive():
     '''活动数据类
 
     参数:
-        id_ (int): 活动 ID
+        id (int): 活动 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''活动数据类
 
         参数:
-            id_ (int): 活动 ID
+            id (int): 活动 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''活动 ID'''
         self._info: dict[str, Any] = {}
         '''活动信息'''
         # 检测 ID 是否存在
         all_id = get_all(5)
-        if not str(id_) in all_id.keys():
-            raise EventNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise EventNotExistError(id)
         return
     
     # 获取排名分数线
     def get_top(
         self,
         server: Literal[0, 1, 2, 3, 4],
         mid: Literal['0']='0',
@@ -66,15 +65,15 @@
                 `4`: 韩服
             mid (Literal[&#39;0&#39;], optional): 指定是否为中间分数线，默认为 `0`
             latest (Literal[&#39;1&#39;], optional): 指定是否为最终分数线，默认为 `1`
 
         返回:
             dict[str, list[dict[str, Any]]]: 排名分数线数据
         '''
-        return Api(API['events']['top'], settings.proxy).request(
+        return Api(API['events']['top']).request(
             'get', params={
                 'server': server,
                 'event': self.id,
                 'mid': mid,
                 'latest': latest
             }
         ).json()
```

### Comparing `bestdori_api-0.1.9/bestdori/events.py` & `bestdori-api-0.2.0/bestdori/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 '''`bestdori.events`
 
 BanG Dream! 活动相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal, Optional
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .eventarchives import EventArchive
 from .exceptions import (
-    ServerNotAvailableError,
-    EventHasNoStampError,
+    NoDataException,
+    EventNotExistError,
     AssetsNotExistError,
-    EventNotExistError
+    EventHasNoStampError,
+    ServerNotAvailableError
 )
 
 # 获取总活动信息
 def get_all(index: Literal[0, 5, 6]=5) -> dict[str, dict[str, Any]]:
     '''获取总活动信息
 
     参数:
@@ -24,53 +24,53 @@
             `0`: 仅获取所有已有活动 ID `all.0.json`
             `5`: 获取所有已有活动的简洁信息 `all.5.json`
             `6`: 获取所有已有活动的简洁信息 `all.6.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总活动信息
     '''
-    return Api(API['events']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['events']['all'].format(index=index)).request('get').json()
 
 # 活动类
 class Event:
     '''活动类
 
     参数:
-        id_ (int): 活动 ID
+        id (int): 活动 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''活动类
 
         参数:
-            id_ (int): 活动 ID
+            id (int): 活动 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''活动 ID'''
         self.archive: EventArchive = EventArchive(self.id)
         '''活动数据'''
         self._info: dict[str, Any] = {}
         '''活动信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not str(id_) in all_id.keys():
-            raise EventNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise EventNotExistError(id)
         return
     
     # 获取活动信息
     def get_info(self) -> dict[str, Any]:
         '''获取活动信息
 
         返回:
             dict[str, Any]: 活动详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有活动信息存储
             response = Api(
-                API['events']['info'].format(self.id), settings.proxy
+                API['events']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取活动评论
     def get_comment(
         self,
@@ -108,41 +108,41 @@
 
         返回:
             str: 活动标题
         '''
         info = self.get_info()
         # 获取 eventName 数据
         if (event_name := info.get('eventName', None)) is None:
-            raise Exception('无法获取活动标题。')
+            raise NoDataException('活动标题')
         # 获取第一个非 None 活动标题
         try:
             return next(filter(lambda x: x is not None, event_name))
         except StopIteration:
-            raise Exception('无法获取活动标题。')
+            raise NoDataException('活动标题')
     
     # 获取活动默认服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取活动默认服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 startAt 数据
         if (start_at := info.get('startAt', None)) is None:
-            raise Exception('无法获取活动起始时间。')
+            raise NoDataException('活动起始时间')
         # 根据 startAt 数据判断服务器
         if start_at[0] is not None: return 'jp'
         elif start_at[1] is not None: return 'en'
         elif start_at[2] is not None: return 'tw'
         elif start_at[3] is not None: return 'cn'
         elif start_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取活动所在服务器。')
+            raise NoDataException('活动所在服务器')
     
     # 获取活动缩略图图像
     def get_banner(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取活动缩略图图像
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
@@ -160,15 +160,15 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if start_at[index] is None:
             raise ServerNotAvailableError(f'活动 {self.name}', server)
         return Assets(
             ASSETS['event']['banner'].format(
                 asset_bundle_name=asset_bundle_name
-            ), server, settings.proxy
+            ), server
         ).get()
     
     # 获取活动 logo 图像
     def get_logo(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取活动 logo 图像
 
         参数:
@@ -187,29 +187,29 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if start_at[index] is None:
             raise ServerNotAvailableError(f'活动 {self.name}', server)
         return Assets(
             ASSETS['event']['logo'].format(
                 asset_bundle_name=asset_bundle_name
-            ), server, settings.proxy
+            ), server
         ).get()
 
     # 获取活动主界面图像
     def get_topscreen(
         self,
         server: Literal['jp', 'en', 'tw', 'cn', 'kr'],
-        type_: Literal['bg', 'trim']
+        type: Literal['bg', 'trim']
     ) -> bytes:
         '''获取活动主界面图像
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
             
-            type_ (Literal[&#39;bg&#39;, &#39;trim&#39;]): 图像类型
+            type (Literal[&#39;bg&#39;, &#39;trim&#39;]): 图像类型
                 `bg`: 背景图像
                 `trim`: 角色图像
 
         返回:
             bytes: 活动主界面图像字节数据 `bytes`
         '''
         # 获取活动数据包名称
@@ -221,50 +221,50 @@
             raise ValueError('无法获取活动起始时间。')
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if start_at[index] is None:
             raise ServerNotAvailableError(f'活动 {self.name}', server)
         return Assets(
             ASSETS['event']['topscreen'].format(
-                asset_bundle_name=asset_bundle_name, type=type_
-            ), server, settings.proxy
+                asset_bundle_name=asset_bundle_name, type=type
+            ), server
         ).get()
     
     # 获取活动奖励稀有表情
     def get_stamp(self) -> bytes:
         '''获取活动奖励稀有表情
 
         返回:
             bytes: 活动奖励稀有表情字节数据 `bytes`
         '''
         info = self.get_info()
         # 获取活动点数奖励列表
         if (point_rewards := info.get('pointRewards', None)) is None:
-            raise Exception('获取活动奖励失败。')
+            raise NoDataException('活动奖励')
         # 获取第一个非 None 奖励列表
         try:
             point_reward = next(filter(lambda x: x is not None, point_rewards))
         except StopIteration:
-            raise Exception('获取活动奖励失败。')
+            raise NoDataException('活动奖励')
         # 获取 rewardType 为 stamp 的活动奖励
         try:
             reward = next(filter(lambda x: x['rewardType'] == 'stamp', point_reward))
         except StopIteration:
             raise EventHasNoStampError(self.id)
         stamp_id = reward['rewardId']
         # 获取全部贴纸资源
         stamps = Api(
-            API['all']['stamps'].format(index='2'), settings.proxy
+            API['all']['stamps'].format(index=2)
         ).request('get').json()
         if (stamp := stamps.get(stamp_id, None)) is None:
             raise AssetsNotExistError(f'贴纸 {stamp_id}')
         # 获取贴纸资源
         image_name = stamp['imageName']
         return Assets(
-            ASSETS['stamp']['get'].format(image_name=image_name), self.server, settings.proxy
+            ASSETS['stamp']['get'].format(image_name=image_name), self.server
         ).get()
 
     # 获取排名分数线
     def get_top(
         self,
         server: Optional[Literal[0, 1, 2, 3, 4]]=None,
         mid: Literal['0']='0',
@@ -287,9 +287,9 @@
         '''
         if server is None:
             if self.server == 'jp': server = 0
             elif self.server == 'en': server = 1
             elif self.server == 'tw': server = 2
             elif self.server == 'cn': server = 3
             elif self.server == 'kr': server = 4
-            else: raise Exception('无法获取活动服务器。')
+            else: raise NoDataException('活动服务器')
         return self.archive.get_top(server, mid, latest)
```

### Comparing `bestdori_api-0.1.9/bestdori/exceptions.py` & `bestdori-api-0.2.0/bestdori/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''`bestdori.exceptions`
 
 API 错误信息相关操作'''
 from typing import Any
 
+from httpx._models import Response
+from httpx._exceptions import RequestError
+
 # 错误基类
 class BaseException(Exception):
     '''错误基类'''
     # 初始化
     def __init__(self, msg: str) -> None:
         self.message = msg
         '''错误信息'''
@@ -16,15 +19,15 @@
         '''输出字符串'''
         return self.message
 
 # 请求发送错误
 class RequestException(BaseException):
     '''请求发送错误'''
     # 初始化
-    def __init__(self, api: str, msg: str='无错误代码获取。', **kwargs: Any) -> None:
+    def __init__(self, api: str, msg: str='无错误代码获取', **kwargs: Any) -> None:
         if len(kwargs) > 0:
             msg += f': {kwargs}'
         else:
             msg += '。'
         super().__init__(msg)
         self.api = api
         '''请求所使用的 API'''
@@ -46,58 +49,70 @@
         super().__init__(msg)
     
     # 字符串化
     def __str__(self) -> str:
         '''输出字符串'''
         return f'获取资源时出错。{self.message}'
 
+# 帖子错误
+class PostException(BaseException):
+    '''帖子错误'''
+    # 初始化
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+        self.message = msg
+        '''错误信息'''
+        return
+
 # 帖子不是社区谱面
-class PostHasNoChartError(BaseException):
+class PostHasNoChartError(PostException):
     '''帖子不是社区谱面'''
     # 初始化
     def __init__(self, post: dict[str, Any]) -> None:
         name = post.get('categoryName', 'DEFAULT_POST')
         msg = f'该帖子类型 {name} 不是社区谱面。'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 帖子没有音乐字段
-class PostHasNoSongError(BaseException):
+class PostHasNoSongError(PostException):
     '''帖子没有音乐字段'''
     # 初始化
     def __init__(self, post: dict[str, Any]) -> None:
         name = post.get('categoryName', 'DEFAULT_POST')
         msg = f'该帖子类型 {name} 不存在歌曲资源。'
         super().__init__(msg)
+        return
+
+# 某 id 指定的资源不存在
+class NotExistException(BaseException):
+    '''资源不存在'''
+    # 初始化
+    def __init__(self, src: str) -> None:
+        msg = f'{src} 不存在。'
+        super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
 # 歌曲不存在
-class SongNotExistError(BaseException):
+class SongNotExistError(NotExistException):
     '''歌曲不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'歌曲 ID {id_} 不存在。'
-        super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
+    def __init__(self, id: int) -> None:
+        super().__init__(f'歌曲 ID {id}')
         return
 
 # 歌曲难度不存在
-class DiffNotExistError(BaseException):
+class DiffNotExistError(NotExistException):
     '''歌曲难度不存在'''
     # 初始化
     def __init__(self, diff: str) -> None:
-        msg = f'歌曲不存在难度 {diff}。'
+        msg = f'歌曲难度 {diff}'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 请求无效
 class RequestInvalidError(RequestException):
     '''请求无效'''
     # 初始化
     def __init__(self, api: str, **kwargs: Any) -> None:
@@ -155,110 +170,101 @@
     '''资源不存在'''
     # 初始化
     def __init__(self, asset_name: str) -> None:
         msg = f'资源 {asset_name} 可能不存在。'
         super().__init__(msg)
 
 # 角色不存在
-class CharacterNotExistError(BaseException):
+class CharacterNotExistError(NotExistException):
     '''角色不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'角色 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'角色 ID {id}'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 卡牌不存在
-class CardNotExistError(BaseException):
+class CardNotExistError(NotExistException):
     '''卡牌不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'卡牌 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'卡牌 ID {id}'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 服装不存在
-class CostumeNotExistError(BaseException):
+class CostumeNotExistError(NotExistException):
     '''服装不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'服装 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'服装 ID {id}'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 活动不存在
-class EventNotExistError(BaseException):
+class EventNotExistError(NotExistException):
     '''活动不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'活动 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'活动 ID {id}'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 招募不存在
-class GachaNotExistError(BaseException):
+class GachaNotExistError(NotExistException):
     '''招募不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'招募 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'招募 ID {id}NotExistException'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 登录奖励不存在
-class LoginCampaignNotExistError(BaseException):
+class LoginCampaignNotExistError(NotExistException):
     '''登录奖励不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'登录奖励 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'登录奖励 ID {id} 不存在。'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 自选券不存在
-class MiracleTicketExchangeNotExistError(BaseException):
+class MiracleTicketExchangeNotExistError(NotExistException):
     '''自选券不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'自选券 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'自选券 ID {id} 不存在。'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 漫画不存在
-class ComicNotExistError(BaseException):
+class ComicNotExistError(NotExistException):
     '''漫画不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'漫画 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'漫画 ID {id} 不存在。'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 任务不存在
-class MissionNotExistError(BaseException):
+class MissionNotExistError(NotExistException):
     '''任务不存在'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'任务 ID {id_} 不存在。'
+    def __init__(self, id: int) -> None:
+        msg = f'任务 ID {id} 不存在。'
+        super().__init__(msg)
+        return
+
+# 玩家不存在
+class PlayerNotExistError(NotExistException):
+    '''玩家不存在'''
+    # 初始化
+    def __init__(self, server: str, id: int) -> None:
+        msg = f'服务器 {server} 上的玩家 ID {id} 不存在。'
         super().__init__(msg)
-        self.message = msg
-        '''错误信息'''
         return
 
 # 服务器指定错误
 class ServerNotAvailableError(BaseException):
     '''服务器指定错误'''
     # 初始化
     def __init__(self, name: str, server: str) -> None:
@@ -268,21 +274,60 @@
         '''错误信息'''
         return
 
 # 活动没有奖励贴纸错误
 class EventHasNoStampError(BaseException):
     '''活动没有奖励贴纸错误'''
     # 初始化
-    def __init__(self, id_: int) -> None:
-        msg = f'活动 ID {id_} 没有奖励贴纸。'
+    def __init__(self, id: int) -> None:
+        msg = f'活动 ID {id} 没有奖励贴纸。'
+        super().__init__(msg)
+        self.message = msg
+        '''错误信息'''
+        return
+
+# 无法获取到信息错误
+class NoDataException(BaseException):
+    '''无法获取到信息错误'''
+    # 初始化
+    def __init__(self, src: str) -> None:
+        msg = f'无法获取 {src} 。'
         super().__init__(msg)
         self.message = msg
         '''错误信息'''
         return
 
+# 设置出错
+class SettingsException(BaseException):
+    '''设置出错'''
+    # 初始化
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+        self.message = msg
+        '''错误信息'''
+        return
+
+# 没有设置 Cookies
+class NoCookiesError(SettingsException):
+    '''没有设置 Cookies'''
+    # 初始化
+    def __init__(self) -> None:
+        msg = '没有设置 Cookies'
+        super().__init__(msg)
+        return
+
+# 没有获取到 ContentType
+class NoContentTypeError(RequestError):
+    '''没有获取到 ContentType'''
+    # 初始化
+    def __init__(self, response: Response) -> None:
+        msg = f'没有获取到 {response.url} 的 ContentType'
+        super().__init__(msg)
+        return
+
 # 请求错误集合
 REQUEST_EXCEPTION: dict[str, type[RequestException]] = {
     'REQUEST_INVALID': RequestInvalidError,
     'LOGIN_REQUIRED': LoginRequiredError,
     'CREDENTIALS_INVALID': CredentialsInvalidError,
     'USER_INVALID': UserInvalidError,
     'ALREADY_UPLOADED': AlreadyUploadedError,
```

### Comparing `bestdori_api-0.1.9/bestdori/gacha.py` & `bestdori-api-0.2.0/bestdori/gacha.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 '''`bestdori.gacha`
 
 BanG Dream! 招募相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .exceptions import (
-    ServerNotAvailableError,
+    NoDataException,
+    GachaNotExistError,
     AssetsNotExistError,
-    GachaNotExistError
+    ServerNotAvailableError
 )
 
 # 获取总招募信息
 def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
     '''获取总招募信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有招募 ID `all.0.json`
             `5`: 获取所有已有招募的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总招募信息
     '''
-    return Api(API['gacha']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['gacha']['all'].format(index=index)).request('get').json()
 
 # 招募类
 class Gacha:
     '''招募类
 
     参数:
-        id_ (int): 招募 ID
+        id (int): 招募 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''招募类
 
         参数:
-            id_ (int): 招募 ID
+            id (int): 招募 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''招募 ID'''
         self._info: dict[str, Any] = {}
         '''招募信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not id_ in all_id.keys():
-            raise GachaNotExistError(id_)
+        if not id in all_id.keys():
+            raise GachaNotExistError(id)
         return
     
     # 获取招募信息
     def get_info(self) -> dict[str, Any]:
         '''获取招募信息
 
         返回:
             dict[str, Any]: 招募详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有招募信息存储
             response = Api(
-                API['gacha']['info'].format(self.id), settings.proxy
+                API['gacha']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取招募评论
     def get_comment(
         self,
@@ -103,41 +103,41 @@
 
         返回:
             str: 招募标题
         '''
         info = self.get_info()
         # 获取 eventName 数据
         if (gacha_name := info.get('gachaName', None)) is None:
-            raise Exception('无法获取招募标题。')
+            raise NoDataException('招募标题')
         # 获取第一个非 None 招募标题
         try:
             return next(filter(lambda x: x is not None, gacha_name))
         except StopIteration:
-            raise Exception('无法获取招募标题。')
+            raise NoDataException('招募标题')
     
     # 获取招募默认服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取招募默认服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 publishedAt 数据
         if (published_at := info.get('publishedAt', None)) is None:
-            raise Exception('无法获取招募起始时间。')
+            raise NoDataException('招募起始时间')
         # 根据 publishedAt 数据判断服务器
         if published_at[0] is not None: return 'jp'
         elif published_at[1] is not None: return 'en'
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取招募所在服务器。')
+            raise NoDataException('招募所在服务器')
     
     # 获取招募缩略图图片
     def get_banner(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取招募缩略图图片
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
@@ -155,57 +155,57 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if start_at[index] is None:
             raise ServerNotAvailableError(f'招募 {self.name}', server)
         return Assets(
             ASSETS['homebanner']['get'].format(
                 banner_asset_bundle_name=banner_asset_bundle_name
-            ), server, settings.proxy
+            ), server
         ).get()
     
     # 获取招募 pickup 图像
     def get_pickups(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[bytes]:
         '''获取招募 pickup 图像
 
         参数:
-            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): _description_
+            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器
 
         返回:
             list[bytes]: pickup 图像字节数据 `bytes` 列表
         '''
         PICKUPS = ['pickup1', 'pickup2', 'pickup']
         # 遍历尝试获取
         pickup_list: list[bytes] = []
         for pickup in PICKUPS:
             try:
                 pickup_list.append(
                     Assets(
                         ASSETS['gacha']['screen'].format(
                             id=self.id, asset_name=pickup
-                        ), server, settings.proxy
+                        ), server
                     ).get()
                 )
             except:
                 continue
         if len(pickup_list) <= 0:
             # 没有获取到任何 pickup 图像
             raise AssetsNotExistError('招募 pickup 图像')
         return pickup_list
     
     # 获取招募 logo 图像
     def get_logo(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取招募 logo 图像
 
         参数:
-            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): _description_
+            server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器
 
         返回:
             bytes: logo 图像字节数据 `bytes`
         '''
         try:
             return Assets(
                 ASSETS['gacha']['screen'].format(
                     id=self.id, asset_name='logo'
-                ), server, settings.proxy
+                ), server
             ).get()
         except:
             raise AssetsNotExistError('招募 logo 图像')
```

### Comparing `bestdori_api-0.1.9/bestdori/logincampaigns.py` & `bestdori-api-0.2.0/bestdori/logincampaigns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 '''`bestdori.logincampaigns`
 
 BanG Dream! 登录奖励相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
-from ._settings import settings
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .exceptions import (
-    LoginCampaignNotExistError,
-    ServerNotAvailableError
+    NoDataException,
+    ServerNotAvailableError,
+    LoginCampaignNotExistError
 )
 
 # 获取总登录奖励信息
 def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
     '''获取总登录奖励信息
 
     参数:
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有登录奖励 ID `all.0.json`
             `5`: 获取所有已有登录奖励的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总登录奖励信息
     '''
-    return Api(API['loginCampaigns']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['loginCampaigns']['all'].format(index=index)).request('get').json()
 
 # 登录奖励类
 class LoginCampaign:
     '''登录奖励类
 
     参数:
-        id_ (int): 登录奖励 ID
+        id (int): 登录奖励 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''登录奖励类
 
         参数:
-            id_ (int): 登录奖励 ID
+            id (int): 登录奖励 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''登录奖励 ID'''
         self._info: dict[str, Any] = {}
         '''登录奖励信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not str(id_) in all_id.keys():
-            raise LoginCampaignNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise LoginCampaignNotExistError(id)
         return
     
     # 获取登录奖励信息
     def get_info(self) -> dict[str, Any]:
         '''获取登录奖励信息
 
         返回:
             dict[str, Any]: 登录奖励详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有登录奖励信息存储
             response = Api(
-                API['loginCampaigns']['info'].format(self.id), settings.proxy
+                API['loginCampaigns']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取登录奖励评论
     def get_comment(
         self,
@@ -102,41 +102,41 @@
 
         返回:
             str: 登录奖励标题
         '''
         info = self.get_info()
         # 获取 eventName 数据
         if (caption := info.get('caption', None)) is None:
-            raise Exception('无法获取登录奖励标题。')
+            raise NoDataException('登录奖励标题')
         # 获取第一个非 None 登录奖励标题
         try:
             return next(filter(lambda x: x is not None, caption))
         except StopIteration:
-            raise Exception('无法获取登录奖励标题。')
+            raise NoDataException('登录奖励标题')
     
     # 获取登录奖励默认服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取登录奖励默认服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 startAt 数据
         if (published_at := info.get('publishedAt', None)) is None:
-            raise Exception('无法获取登录奖励起始时间。')
+            raise NoDataException('登录奖励起始时间')
         # 根据 startAt 数据判断服务器
         if published_at[0] is not None: return 'jp'
         elif published_at[1] is not None: return 'en'
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取登录奖励所在服务器。')
+            raise NoDataException('登录奖励所在服务器')
     
     # 获取登录奖励背景图图像
     def get_background(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
         '''获取登录奖励背景图图像
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
@@ -152,9 +152,9 @@
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if asset_bundle_name[index] is None:
             raise ServerNotAvailableError(f'登录奖励 {self.name}', server)
         return Assets(
             ASSETS['event']['loginbouns'].format(
                 asset_bundle_name=asset_bundle_name[index]
-            ), server, settings.proxy
+            ), server
         ).get()
```

### Comparing `bestdori_api-0.1.9/bestdori/miracleticket.py` & `bestdori-api-0.2.0/bestdori/miracleticket.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 '''`bestdori.miracleticket`
 
 BanG Dream! 自选券相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
 from .exceptions import (
-    MiracleTicketExchangeNotExistError,
-    ServerNotAvailableError
+    NoDataException,
+    ServerNotAvailableError,
+    MiracleTicketExchangeNotExistError
 )
 
 # 获取总自选券信息
 def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
     '''获取总自选券信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有自选券信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总自选券信息
     '''
     return Api(
-        API['all']['miracleTicketExchanges'].format(index), settings.proxy
+        API['all']['miracleTicketExchanges'].format(index=index)
     ).request('get').json()
 
 # 自选券类
 class MiracleTicketExchange:
     '''自选券类
 
     参数:
-        id_ (int): 自选券 ID
+        id (int): 自选券 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''自选券类
 
         参数:
-            id_ (int): 自选券 ID
+            id (int): 自选券 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''自选券 ID'''
         self._info: dict[str, Any] = {}
         '''自选券信息'''
         # 检测 ID 是否存在
         all_ = get_all(5)
-        if not str(id_) in all_.keys():
-            raise MiracleTicketExchangeNotExistError(id_)
-        self._info = all_[str(id_)]
+        if not str(id) in all_.keys():
+            raise MiracleTicketExchangeNotExistError(id)
+        self._info = all_[str(id)]
         return
     
     # 获取自选券信息
     def get_info(self) -> dict[str, Any]:
         '''获取自选券信息
 
         返回:
@@ -67,55 +67,55 @@
 
         返回:
             str: 自选券标题
         '''
         info = self.get_info()
         # 获取 eventName 数据
         if (name := info.get('name', None)) is None:
-            raise Exception('无法获取自选券标题。')
+            raise NoDataException('自选券标题')
         # 获取第一个非 None 自选券标题
         try:
             return next(filter(lambda x: x is not None, name))
         except StopIteration:
-            raise Exception('无法获取自选券标题。')
+            raise NoDataException('自选券标题')
     
     # 获取自选券默认服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取自选券默认服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 ids 数据
         if (ids := info.get('ids', None)) is None:
-            raise Exception('无法获取自选券 ID 列表。')
+            raise NoDataException('自选券 ID 列表')
         # 根据 ids 数据判断服务器
         if ids[0] is not None: return 'jp'
         elif ids[1] is not None: return 'en'
         elif ids[2] is not None: return 'tw'
         elif ids[3] is not None: return 'cn'
         elif ids[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取自选券所在服务器。')
+            raise NoDataException('自选券所在服务器')
     
     # 获取自选券 ID 列表
     def get_ids(self, server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> list[int]:
         '''获取自选券 ID 列表
 
         参数:
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
 
         返回:
             list[int]: 自选券 ID 列表
         '''
         info = self.get_info()
         # 获取 ids 数据
         if (ids := info.get('ids', None)) is None:
-            raise Exception('无法获取自选券 ID 列表。')
+            raise NoDataException('自选券 ID 列表')
         # 判断服务器
         SERVERS = ['jp', 'en', 'tw', 'cn', 'kr']
         index = SERVERS.index(server)
         if ids[index] is None:
             raise ServerNotAvailableError(f'活动 {self.name}', server)
         return ids[index]
```

### Comparing `bestdori_api-0.1.9/bestdori/missions.py` & `bestdori-api-0.2.0/bestdori/missions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 '''`bestdori.missions`
 
 BanG Dream! 任务相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .post import get_list
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
 from .exceptions import (
+    NoDataException,
     MissionNotExistError
 )
 
 # 获取总任务信息
 def get_all(index: Literal[0, 5]=5) -> dict[str, dict[str, Any]]:
     '''获取总任务信息
 
@@ -19,51 +19,51 @@
         index (Literal[0, 5], optional): 指定获取哪种 `all.json`
             `0`: 仅获取所有已有任务 ID `all.0.json`
             `5`: 获取所有已有任务的简洁信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总任务信息
     '''
-    return Api(API['missions']['all'].format(index), settings.proxy).request('get').json()
+    return Api(API['missions']['all'].format(index=index)).request('get').json()
 
 # 任务类
 class Mission:
     '''任务类
 
     参数:
-        id_ (int): 任务 ID
+        id (int): 任务 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''任务类
 
         参数:
-            id_ (int): 任务 ID
+            id (int): 任务 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''任务 ID'''
         self._info: dict[str, Any] = {}
         '''任务信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not str(id_) in all_id.keys():
-            raise MissionNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise MissionNotExistError(id)
         return
     
     # 获取任务信息
     def get_info(self) -> dict[str, Any]:
         '''获取任务信息
 
         返回:
             dict[str, Any]: 任务详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有任务信息存储
             response = Api(
-                API['missions']['info'].format(self.id), settings.proxy
+                API['missions']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取任务评论
     def get_comment(
         self,
@@ -101,35 +101,35 @@
 
         返回:
             str: 任务标题
         '''
         info = self.get_info()
         # 获取 title 数据
         if (title := info.get('title', None)) is None:
-            raise Exception('无法获取任务标题。')
+            raise NoDataException('任务标题')
         # 获取第一个非 None 任务标题
         try:
             return next(filter(lambda x: x is not None, title))
         except StopIteration:
-            raise Exception('无法获取任务标题。')
+            raise NoDataException('任务标题')
     
     # 获取任务所在服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
         '''获取任务所在服务器
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 startAt 数据
         if (start_at := info.get('startAt', None)) is None:
-            raise Exception('无法获取任务起始时间。')
+            raise NoDataException('任务起始时间')
         # 根据 startAt 数据判断服务器
         if start_at[0] is not None: return 'jp'
         elif start_at[1] is not None: return 'en'
         elif start_at[2] is not None: return 'tw'
         elif start_at[3] is not None: return 'cn'
         elif start_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取任务所在服务器。')
+            raise NoDataException('任务所在服务器')
```

### Comparing `bestdori_api-0.1.9/bestdori/post.py` & `bestdori-api-0.2.0/bestdori/post.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 '''`bestdori.post`
 
 社区帖子相关操作'''
 from typing_extensions import overload
-from typing import TypedDict, Optional, Literal, Union, TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Union, Literal, Optional, TypedDict
 
 from .charts import Chart
-from ._settings import settings
 from .utils.content import Content
 from .utils.utils import API, ASSETS
 from .utils.network import Api, Assets
 from .exceptions import (
+    NoDataException,
+    RequestException,
+    PostHasNoSongError,
     AssetsNotExistError,
-    PostHasNoChartError,
-    PostHasNoSongError
+    PostHasNoChartError
 )
 
 if TYPE_CHECKING:
     from .user import Me
 
 # 标签类
 class Tag(TypedDict):
@@ -154,45 +155,45 @@
     kwargs = {key: value for key, value in kwargs.items() if value is not None}
     # 将下划线字段名转换为小驼峰字段名
     kwargs = {
         (
             "".join(x.capitalize() if i > 0 else x for i, x in enumerate(key.split("_")))
         ): value for key, value in kwargs.items() if value is not None
     }
-    response = Api(API['post']['list'], settings.proxy).request('post', data=kwargs)
+    response = Api(API['post']['list']).request('post', data=kwargs)
     return response.json()
 
 # 搜索标签
 def search_tags(
-    type_: str,
+    type: str,
     data: str='',
     fuzzy: bool=True
 ) -> list[Tag]:
     '''搜索已有标签
 
     参数:
         type (str): 标签类型
         data (str, optional): 搜索标签数据关键词
         fuzzy (bool, optional): 是否使用模糊搜索
 
     返回:
         list[Tag]: 标签类 `Tag` 列表
     '''
-    response = Api(API['post']['tag'], settings.proxy).request(
+    response = Api(API['post']['tag']).request(
         'get',
         params={
-            'type': type_,
+            'type': type,
             'data': data,
             'fuzzy': fuzzy
         }
     )
     if (tags := response.json().get('tags', None)) is not None:
         return [Tag(tag) for tag in tags]
     else:
-        raise Exception('搜索标签时出现未知错误。')
+        raise RequestException(API['post']['tag'], '搜索标签时出现未知错误')
 
 # 发表谱面
 @overload
 def post(
     me: 'Me',
     *,
     artists: str,
@@ -304,89 +305,89 @@
     kwargs = {key: value for key, value in kwargs.items() if value is not None}
     # 将下划线字段名转换为小驼峰字段名
     kwargs = {
         (
             "".join(x.capitalize() if i > 0 else x for i, x in enumerate(key.split("_")))
         ): value for key, value in kwargs.items() if value is not None
     }
-    response = Api(API['post']['post'], settings.proxy).request(
+    response = Api(API['post']['post']).request(
         'post',
         cookies=me.cookies,
         data=kwargs
     )
-    if (id_ := response.json().get('id', None)) is None:
+    if (id := response.json().get('id', None)) is None:
         raise ValueError('发表帖子时出现未知错误。')
-    return id_
+    return id
 
 # 查询帖子顺序
-def find_post(category_name: str, category_id: str, id_: int) -> int:
+def find_post(category_name: str, category_id: str, id: int) -> int:
     '''查询帖子顺序
 
     参数:
         category_name (str): 画廊名称
         category_id (str): 画廊 ID
         id (int): 查询的帖子 ID
 
     返回:
         int: 帖子在该画廊的时间顺序
     '''
     params = {
         'categoryName': category_name,
         'categoryId': category_id,
-        'id': id_
+        'id': id
     }
-    response = Api(API['post']['find'], settings.proxy).request('get', params=params)
+    response = Api(API['post']['find']).request('get', params=params)
     if (position := response.json().get('position', None)) is None:
         raise ValueError('查询帖子顺序时出现未知错误。')
     return position
 
 # 社区帖子类
 class Post:
     '''社区帖子类
 
     参数:
-        id_ (str): 社区帖子 ID
+        id (str): 社区帖子 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''社区帖子类
 
         参数:
-            id_ (int): 社区帖子 ID
+            id (int): 社区帖子 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''社区帖子 ID'''
         self._post: dict[str, Any] = {}
         '''社区帖子内容'''
         return
     
     # 获取帖子基础信息
     def get_basic(self) -> dict[str, Any]:
         '''获取帖子基础信息
 
         返回:
             dict[str, Any]: 基础信息
         '''
-        response = Api(API['post']['basic'], settings.proxy).request('get', params={'id': self.id,})
+        response = Api(API['post']['basic']).request('get', params={'id': self.id,})
         return response.json()
     
     # 获取帖子信息
     def get_details(self) -> dict[str, Any]:
         '''获取帖子信息
 
         返回:
             dict[str, Any]: 帖子详细信息
         '''
         if len(self._post) <= 0:
             # 如果没有帖子内容存储
-            response = Api(API['post']['details'], settings.proxy).request('get', params={'id': self.id,})
+            response = Api(API['post']['details']).request('get', params={'id': self.id,})
             if (post := response.json().get('post', None)) is not None:
                 self._post = dict(post)
             else:
-                raise Exception('无帖子信息获取。')
+                raise NoDataException('帖子信息')
         return self._post
     
     # 获取谱面对象
     def get_chart(self) -> Chart:
         '''获取谱面对象
 
         返回:
@@ -435,114 +436,84 @@
         返回:
             SongInfo: 歌曲音频与封面字节
         '''
         post = self.get_details()
         if (song := post.get('song', None)) is None:
             raise PostHasNoSongError(post)
         
-        if (type_ := song.get('type', None)) is None:
+        if (type := song.get('type', None)) is None:
             raise TypeError('该帖子没有歌曲类型。')
         
         result: dict[str, Union[bytes, None]] = {}
-        if type_ == 'custom': # 自定义歌曲
+        if type == 'custom': # 自定义歌曲
             # 获取歌曲音频
             if (audio := song.get('audio', None)) is None:
                 result['audio'] = None
             else:
-                try:
-                    response = Api(audio, settings.proxy).request('get')
-                    response.raise_for_status()
-                    result['audio'] = response.content
-                except Exception as exception:
-                    if settings.print:
-                        print(f'获取自定义歌曲音频时失败：{type(exception).__name__}: {exception}')
-                    result['audio'] = None
+                response = Api(audio).request('get')
+                response.raise_for_status()
+                result['audio'] = response.content
             # 获取歌曲封面
             if (cover := song.get('cover', None)) is None:
                 result['cover'] = None
             else:
-                try:
-                    response = Api(cover, settings.proxy).request('get')
-                    response.raise_for_status()
-                    result['cover'] = response.content
-                except Exception as exception:
-                    if settings.print:
-                        print(f'获取自定义歌曲封面时失败：{type(exception).__name__}: {exception}')
-                    result['cover'] = None
-        elif type_ == 'bandori': # BanG Dream! 歌曲
+                response = Api(cover).request('get')
+                response.raise_for_status()
+                result['cover'] = response.content
+        elif type == 'bandori': # BanG Dream! 歌曲
             # 获取歌曲 ID
-            if (id_ := song.get('id', None)) is None:
+            if (id := song.get('id', None)) is None:
                 raise ValueError('未能获取歌曲 ID。')
             # 获取歌曲信息
-            info = Api(API['songs']['info'].format(id=id_), settings.proxy).request('get').json()
+            info = Api(API['songs']['info'].format(id=id)).request('get').json()
             # 获取歌曲所在服务器
             if (published_at := info.get('publishedAt', None)) is None:
-                raise Exception('无法获取歌曲发布时间。')
+                raise NoDataException('歌曲发布时间')
             # 根据 publishedAt 数据判断服务器
             if published_at[0] is not None: server = 'jp'
             elif published_at[1] is not None: server = 'en'
             elif published_at[2] is not None: server = 'tw'
             elif published_at[3] is not None: server = 'cn'
             elif published_at[4] is not None: server = 'kr'
             else:
-                raise Exception('无法获取歌曲服务器。')
+                raise NoDataException('歌曲服务器')
             # 获取歌曲音频
-            try:
-                result['audio'] = Assets(
-                    ASSETS['songs']['sound'].format(id=str(id_)), server, settings.proxy
-                ).get()
-            except Exception as exception:
-                if settings.print:
-                    print(f'获取 BanG Dream! 歌曲音频时失败：{type(exception).__name__}: {exception}')
-                result['audio'] = None
+            result['audio'] = Assets(
+                ASSETS['songs']['sound'].format(id=id), server
+            ).get()
             # 获取歌曲封面
-            try:
-                # 获取数据包序列号
-                quotient, remainder = divmod(id_, 10)
-                if remainder == 0:
-                    index = str(id_)
-                else:
-                    index = str((quotient + 1) * 10)
-                
-                if (jacket_image := info.get('jacketImage', None)) is None:
-                    raise Exception('歌曲封面资源未找到。')
-                result['cover'] = Assets(
-                    ASSETS['songs']['musicjacket'].format(
-                        index=index, jacket_image=jacket_image[-1]
-                    ), server, settings.proxy
-                ).get()
-            except Exception as exception:
-                if settings.print:
-                    print(f'获取 BanG Dream! 歌曲封面时失败：{type(exception).__name__}: {exception}')
-                result['cover'] = None
-        elif type_ == 'llsif': # LoveLive! 歌曲
+            # 获取数据包序列号
+            quotient, remainder = divmod(id, 10)
+            if remainder == 0:
+                index = id
+            else:
+                index = (quotient + 1) * 10
+            
+            if (jacket_image := info.get('jacketImage', None)) is None:
+                raise NoDataException('歌曲封面资源')
+            result['cover'] = Assets(
+                ASSETS['songs']['musicjacket'].format(
+                    index=index, jacket_image=jacket_image[-1]
+                ), server
+            ).get()
+        elif type == 'llsif': # LoveLive! 歌曲
             # 获取歌曲 ID
-            if (id_ := song.get('id', None)) is None:
+            if (id := song.get('id', None)) is None:
                 raise ValueError('未能获取歌曲 ID。')
             # 获取歌曲信息
-            info = Api(API['misc']['llsif'].format(index=10), settings.proxy).request('get').json()[str(id_)]
+            info = Api(API['misc']['llsif'].format(index=10)).request('get').json()[str(id)]
             # 获取歌曲资源库
             live_icon_asset = info.get('live_icon_asset', None)
             sound_asset = info.get('sound_asset', None)
             # 获取歌曲音频
-            try:
-                result['audio'] = Assets(sound_asset, 'llsif', settings.proxy).get()
-            except Exception as exception:
-                if settings.print:
-                    print(f'获取 LoveLive! 歌曲音频时失败：{type(exception).__name__}: {exception}')
-                result['audio'] = None
+            result['audio'] = Assets(sound_asset, 'llsif').get()
             # 获取歌曲封面
-            try:
-                result['cover'] = Assets(live_icon_asset, 'llsif', settings.proxy).get()
-            except Exception as exception:
-                if settings.print:
-                    print(f'获取 LoveLive! 歌曲封面时失败：{type(exception).__name__}: {exception}')
-                result['cover'] = None
+            result['cover'] = Assets(live_icon_asset, 'llsif').get()
         else:
-            raise AssetsNotExistError(f'{type_} 歌曲')
+            raise AssetsNotExistError(f'{type} 歌曲')
         
         return SongRes(**result)
     
     # 获取帖子评论
     def get_comment(
         self,
         limit: int=20,
@@ -594,13 +565,13 @@
     def like(self, me: 'Me', value: bool=True) -> None:
         '''喜欢 / 取消喜欢帖子
 
         参数:
             me (Me): 自身用户对象
             value (bool, optional): 值 `True`: 喜欢帖子 `False`: 取消喜欢帖子
         '''
-        Api(API['post']['like'], settings.proxy).request(
+        Api(API['post']['like']).request(
             'post',
             data={'id': self.id, 'value': value},
             cookies=me.cookies
         )
         return
```

### Comparing `bestdori_api-0.1.9/bestdori/songmeta.py` & `bestdori-api-0.2.0/bestdori/songmeta.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 '''`bestdori.songmeta`
 
 BanG Dream! 歌曲 Meta 相关操作'''
-from typing import Optional, Literal, Any
+from typing import Any, Literal
 
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
 
 # 获取总歌曲 Meta 信息
 def get_all(index: Literal[5]=5) -> dict[str, dict[str, Any]]:
     '''获取总歌曲 Meta 信息
 
     参数:
         index (Literal[5], optional): 指定获取哪种 `all.json`
             `5`: 获取所有已有歌曲 Meta 信息 `all.5.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总歌曲 Meta 信息
     '''
-    return Api(API['all']['meta'].format(index=index), settings.proxy).request('get').json()
+    return Api(API['all']['meta'].format(index=index)).request('get').json()
```

### Comparing `bestdori_api-0.1.9/bestdori/songs.py` & `bestdori-api-0.2.0/bestdori/songs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 '''`bestdori.songs`
 
 BanG Dream! 歌曲相关操作'''
-from typing import Optional, Literal, Any
-from requests.exceptions import HTTPError
+from typing import Any, Literal
+
+from httpx._exceptions import HTTPStatusError
 
 from .charts import Chart
 from .post import get_list
-from ._settings import settings
 from .utils.utils import ASSETS, API
 from .utils.network import Assets, Api
 from .exceptions import (
+    NoDataException,
     DiffNotExistError,
     SongNotExistError
 )
 
 # 获取总歌曲信息
 def get_all(index: Literal[0, 5, 7]=5) -> dict[str, dict[str, Any]]:
     '''获取总歌曲信息
@@ -23,15 +24,15 @@
             `0`: 仅获取所有已有歌曲 ID `all.0.json`
             `5`: 获取所有已有歌曲的简洁信息 `all.5.json`，默认为该项
             `7`: 获取所有已有歌曲的较为详细信息 `all.7.json`
 
     返回:
         dict[str, dict[str, Any]]: 获取到的总歌曲信息
     '''
-    return Api(API['songs']['all'].format(index=index), settings.proxy).request('get').json()
+    return Api(API['songs']['all'].format(index=index)).request('get').json()
 
 # 歌曲封面内部类
 class Jacket:
     '''歌曲封面类
 
     参数:
         url (str): 封面链接
@@ -56,62 +57,62 @@
     # 获取封面 url
     @property
     def url(self) -> str:
         '''获取封面 url'''
         return Assets(
             ASSETS['songs']['musicjacket'].format(
                 index=self._index, jacket_image=self._jacket_image
-            ), self._server, settings.proxy
+            ), self._server
         ).get_url()
     
     # 获取封面字节数据
     @property
     def bytes(self) -> bytes:
         '''获取封面字节数据'''
         return Assets(
             ASSETS['songs']['musicjacket'].format(
                 index=self._index, jacket_image=self._jacket_image
-            ), self._server, settings.proxy
+            ), self._server
         ).get()
 
 # 歌曲类
 class Song:
     '''歌曲类
 
     参数:
-        id_ (int): 歌曲 ID
+        id (int): 歌曲 ID
     '''
     # 初始化
-    def __init__(self, id_: int) -> None:
+    def __init__(self, id: int) -> None:
         '''歌曲类
 
         参数:
-            id_ (int): 歌曲 ID
+            id (int): 歌曲 ID
         '''
-        self.id: int = id_
+        self.id: int = id
         '''歌曲 ID'''
         self._info: dict[str, Any] = {}
         '''歌曲信息'''
         # 检测 ID 是否存在
         all_id = get_all(0)
-        if not str(id_) in all_id.keys():
-            raise SongNotExistError(id_)
+        if not str(id) in all_id.keys():
+            raise SongNotExistError(id)
         return
     
     # 获取歌曲信息
     def get_info(self) -> dict[str, Any]:
         '''获取歌曲信息
 
         返回:
             dict[str, Any]: 歌曲详细信息
         '''
         if len(self._info) <= 0:
             # 如果没有歌曲信息存储
             response = Api(
-                API['songs']['info'].format(id=self.id), settings.proxy
+                API['songs']['info'].format(id=self.id)
             ).request('get')
             self._info = dict(response.json())
         return self._info
     
     # 获取歌曲所在服务器
     @property
     def server(self) -> Literal['jp', 'en', 'tw', 'cn', 'kr']:
@@ -119,41 +120,41 @@
 
         返回:
             Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]: 歌曲所在服务器
         '''
         info = self.get_info()
         # 获取 publishedAt 数据
         if (published_at := info.get('publishedAt', None)) is None:
-            raise Exception('无法获取歌曲发布时间。')
+            raise NoDataException('歌曲发布时间')
         # 根据 publishedAt 数据判断服务器
         if published_at[0] is not None: return 'jp'
         elif published_at[1] is not None: return 'en'
         elif published_at[2] is not None: return 'tw'
         elif published_at[3] is not None: return 'cn'
         elif published_at[4] is not None: return 'kr'
         else:
-            raise Exception('无法获取歌曲服务器。')
+            raise NoDataException('歌曲服务器')
     
     # 获取歌曲名称
     @property
     def name(self) -> str:
         '''获取歌曲名称
 
         返回:
             str: 歌曲名称
         '''
         info = self.get_info()
         # 获取 musicTitle 数据
         if (music_title := info.get('musicTitle', None)) is None:
-            raise Exception('无法获取歌曲名称。')
+            raise NoDataException('歌曲名称')
         # 获取第一个非 None 歌曲名称
         try:
             return next(filter(lambda x: x is not None, music_title))
         except StopIteration:
-            raise Exception('无法获取歌曲名称。')
+            raise NoDataException('歌曲名称')
     
     # 获取歌曲谱面
     def get_chart(
         self,
         diff: Literal['easy', 'normal', 'hard', 'expert', 'special']='expert'
     ) -> Chart:
         '''获取歌曲谱面
@@ -163,17 +164,20 @@
 
         返回:
             Chart: 获取到的谱面对象
         '''
         try:
             chart = Chart.get_chart(self.id, diff)
             return chart
-        except HTTPError:
-            # 难度不存在
-            raise DiffNotExistError(diff)
+        except HTTPStatusError as e:
+            if e.response.status_code == 404:
+                # 难度不存在
+                raise DiffNotExistError(diff)
+            else:
+                raise e
     
     # 获取歌曲封面
     def get_jacket(self) -> list[Jacket]:
         '''获取歌曲封面
 
         返回:
             Jacket: 歌曲封面对象 `Jacket`
@@ -183,30 +187,30 @@
         if remainder == 0:
             index = self.id
         else:
             index = (quotient + 1) * 10
         
         info = self.get_info()
         if (jacket_image := info.get('jacketImage', None)) is None:
-            raise Exception('歌曲封面资源未找到。')
+            raise NoDataException('歌曲封面资源')
         jacket: list[Jacket] = []
         
         for image in jacket_image:
             jacket.append(Jacket(index, image, self.server))
         
         return jacket
     
     # 获取歌曲音频
     def get_bgm(self) -> bytes:
         '''获取歌曲音频
 
         返回:
             bytes: 歌曲音频字节数据 `bytes`
         '''
-        return Assets(ASSETS['songs']['sound'].format(id=self.id), self.server, settings.proxy).get()
+        return Assets(ASSETS['songs']['sound'].format(id=self.id), self.server).get()
     
     # 获取歌曲评论
     def get_comment(
         self,
         limit: int=20,
         offset: int=0,
         order: Literal['TIME_DESC', 'TIME_ASC']='TIME_ASC'
```

### Comparing `bestdori_api-0.1.9/bestdori/upload.py` & `bestdori-api-0.2.0/bestdori/upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 '''`bestdori.upload`
 
 Bestdori 文件相关操作'''
 from pathlib import Path
 from hashlib import sha1
 from io import BufferedReader
-from typing import Optional, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
+from .user import Me
 from .utils.utils import API
 from .utils.network import Api
-from ._settings import settings
+from .utils._settings import settings
 from .exceptions import AlreadyUploadedError
 
 if TYPE_CHECKING:
     from .user import Me
 
 # 从 Bestdori 获取指定哈希文件字节
-def download(hash_: str) -> bytes:
+def download(hash: str) -> bytes:
     '''从 Bestdori 获取指定哈希文件字节
 
     参数:
-        hash_ (str): 文件哈希值
+        hash (str): 文件哈希值
 
     返回:
         bytes: 文件字节 `bytes`
     '''
-    return Api(API['upload']['file'].format(hash=hash_), settings.proxy).request('get').content
+    return Api(API['upload']['file'].format(hash=hash)).request('get').content
 
 # 通过哈希值构建 Bestdori 文件 URL
-def hash_to_url(hash_: str) -> str:
+def hash_to_url(hash: str) -> str:
     '''通过哈希值构建 Bestdori 文件 URL
 
     参数:
-        hash_ (str): 文件哈希值
+        hash (str): 文件哈希值
 
     返回:
         str: 文件 URL
     '''
-    return f'https://bestdori.com/api/upload/file/{hash_}'
+    return f'https://bestdori.com/api/upload/file/{hash}'
 
 # 上传文件类
 class Upload:
     '''上传文件类
 
     参数:
         file_bytes (bytes): 文件字节
         name (str): 文件名
         reader (BufferedReader): 文件字节流
     '''
     # 初始化
     def __init__(self, file_bytes: bytes, name: str, reader: BufferedReader) -> None:
         # 处理文件字节
-        hash_ = sha1(file_bytes).hexdigest() # 计算 SHA-1 哈希
+        hash = sha1(file_bytes).hexdigest() # 计算 SHA-1 哈希
         size = len(file_bytes) # 计算文件大小
         # 赋值对象属性
         self._ver: int = 3
         '''文件版本'''
-        self._hash: str = hash_
+        self._hash: str = hash
         '''文件哈希'''
         self._size: int = size
         '''文件大小'''
         self._name: str = name
         '''文件名'''
         self._reader: BufferedReader = reader
         '''文件字节流'''
@@ -88,47 +89,53 @@
     # 上传文件
     def upload(self) -> str:
         '''上传文件
 
         返回:
             str: 上传文件的哈希值
         '''
-        if not settings.cookies:
-            raise ValueError('未设置用户 Cookies。')
+        try:
+            cookies = settings._cookies()
+        except:
+            if settings._username is None or settings._password is None:
+                raise ValueError('未添加用户信息。')
+            else:
+                settings._me = Me(settings._username, settings._password)
+                cookies = settings._cookies()
         
         if self._reader.closed:
             raise ValueError('文件流已关闭。')
         
         # 构建上传负载
         payload = {
             'ver': self._ver,
             'hash': self._hash,
             'size': self._size
         }
         # 发送预上传请求
         try:
-            Api(API['upload']['prepare'], settings.proxy).request('post', cookies=settings.cookies, data=payload)
+            Api(API['upload']['prepare']).request('post', cookies=cookies, data=payload)
         except AlreadyUploadedError:
             self._reader.close()
             return self._hash
         # 发送上传请求
         with self._reader:
-            response = Api(API['upload']['upload'], settings.proxy).request(
+            response = Api(API['upload']['upload']).request(
                 'post',
                 files={
                     'file': (self._name, self._reader)
                 },
-                cookies=settings.cookies
+                cookies=cookies
             )
         # 获取文件的哈希值
         hash_get = response.json()['hash']
         #重复查询至多 5 次上传状态
         for _ in range(5):
             # 发送上传状态查询请求
-            response = Api(API['upload']['status'].format(hash=hash_get), settings.proxy).request('get')
+            response = Api(API['upload']['status'].format(hash=hash_get)).request('get')
             # 获取上传状态
             status = response.json()['status']
             # 若上传成功则返回
             if status == 'available':
                 return hash_get
         
         raise TimeoutError(f'上传文件 {self._name} 超时。')
```

### Comparing `bestdori_api-0.1.9/bestdori/user.py` & `bestdori-api-0.2.0/bestdori/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''`bestdori.user`
 
 BanG Dream! 歌曲相关操作'''
 from httpx._models import Cookies
-from typing import Optional, Literal, Any
+from typing import Any, Literal, Optional
 
-from ._settings import settings
 from .post import get_list
 from .utils.utils import API
 from .utils.network import Api
 
 # 用户类
 class User:
     '''用户类
@@ -35,15 +34,15 @@
 
         返回:
             dict[str, Any]: 用户详细信息
         '''
         if len(self._info) <= 0:
             # 若无用户信息存储
             response = Api(
-                API['user']['info'], settings.proxy
+                API['user']['info']
             ).request('get', params={'username': self.username})
             self._info = dict(response.json())
         return self._info
     
     # 获取用户帖子
     def get_posts(
         self,
@@ -198,35 +197,35 @@
             password (str): 密码
 
         返回:
             Me: 自身用户对象
         '''
         me = cls(username, password)
         response = Api(
-            API['user']['login'], settings.proxy
+            API['user']['login']
         ).request('post', data={'username': me.username, 'password': me.password})
         me._cookies = response.cookies
         me.me()
         return me
     
     # 获取用户 Cookies
     @property
     def cookies(self) -> Cookies:
         '''获取用户 Cookies'''
         if self._cookies is None:
             response = Api(
-                API['user']['login'], settings.proxy
+                API['user']['login']
             ).request('post', data={'username': self.username, 'password': self.password})
             self._cookies = response.cookies
         return self._cookies
     
     # 获取用户自我信息
     def me(self) -> dict[str, Any]:
         '''获取用户自我信息
 
         返回:
             dict[str, Any]: 自我信息
         '''
         if len(self._me) == 0:
-            response = Api(API['user']['me'], settings.proxy).request('get', cookies=self.cookies)
+            response = Api(API['user']['me']).request('get', cookies=self.cookies)
             self._me = dict(response.json())
         return self._me
```

### Comparing `bestdori_api-0.1.9/bestdori/utils/__init__.py` & `bestdori-api-0.2.0/bestdori/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 from .utils import API, RES,ASSETS
 from .network import Api, Res, Assets
 from ..exceptions import (
     AssetsNotExistError
 )
 
 # 将十六进制颜色代码转换为 RGB 元组
-def hex_to_rgb(hex_: str) -> tuple[int, int, int]:
+def hexto_rgb(hex: str) -> tuple[int, int, int]:
     '''将十六进制颜色代码转换为 RGB 元组
 
     参数:
-        hex_ (str): 十六进制颜色代码
+        hex (str): 十六进制颜色代码
 
     返回:
         tuple[int, int, int]: RGB 元组
     '''
-    if hex_[0] == '#':
-        hex_ = hex_[1:]
-    if len(hex_) == 3:
-        hex_ = hex_[0] * 2 + hex_[1] * 2 + hex_[2] * 2
-    rgb = tuple(int(hex_[i:i+2], 16) for i in (0, 2, 4))
+    if hex[0] == '#':
+        hex = hex[1:]
+    if len(hex) == 3:
+        hex = hex[0] * 2 + hex[1] * 2 + hex[2] * 2
+    rgb = tuple(int(hex[i:i+2], 16) for i in (0, 2, 4))
     if len(rgb) != 3:
         raise ValueError('十六进制颜色代码')
     return rgb
 
 # 获取称号资源
 def get_degree(
     degree_name: str,
@@ -91,46 +91,46 @@
     返回:
         dict[str, dict[str, Any]]: 获取到的主要乐队信息
     '''
     return Api(API['bands']['main'].format(index=index), proxy=proxy).request('get').json()
 
 # 获取乐队 logo
 def get_band_logo(
-    id_: int,
-    type_: Literal['logoS', 'logoL', 'logoL_Mask'],
+    id: int,
+    type: Literal['logoS', 'logoL', 'logoL_Mask'],
     server: Literal['jp', 'en', 'tw', 'cn', 'kr']
 ) -> bytes:
     '''获取乐队 logo
 
     参数:
-        id_ (int): 乐队 ID
+        id (int): 乐队 ID
         
-        type_ (Literal[&#39;logoS&#39;, &#39;logoL&#39;, &#39;logoL_Mask&#39;]): logo 类型
+        type (Literal[&#39;logoS&#39;, &#39;logoL&#39;, &#39;logoL_Mask&#39;]): logo 类型
             `logoS`: 小 logo
             `logoL`: 大 logo
             `logoL_Mask`: 大 logo 遮罩
         
         server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 指定服务器
 
     返回:
         bytes: 乐队 logo 字节数据 `bytes`
     '''
-    return Assets(ASSETS['band']['logo'].format(id=id_, type=type_), server).get()
+    return Assets(ASSETS['band']['logo'].format(id=id, type=type), server).get()
 
 # 获取乐队图标
-def get_band_icon(id_: str) -> bytes:
+def get_band_icon(id: str) -> bytes:
     '''获取乐队图标
 
     参数:
-        id_ (str): 乐队 ID
+        id (str): 乐队 ID
 
     返回:
         bytes: 乐队图标字节数据
     '''
-    return Res(RES['icon']['svg'].format(name=f'band_{id_}')).get()
+    return Res(RES['icon']['svg'].format(name=f'band_{id}')).get()
 
 # 获取服务器图标
 def get_server_icon(server: Literal['jp', 'en', 'tw', 'cn', 'kr']) -> bytes:
     '''获取服务器图标
 
     参数:
         server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 服务器名称
```

### Comparing `bestdori_api-0.1.9/bestdori/utils/content.py` & `bestdori-api-0.2.0/bestdori/utils/content.py`

 * *Files identical despite different names*

### Comparing `bestdori_api-0.1.9/bestdori/utils/network.py` & `bestdori-api-0.2.0/bestdori/utils/network.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 '''`bestdori.utils.network`
 
 向 Bestdori 发送请求相关模块'''
 from json import dumps
 from io import BufferedReader
+from typing import Any, Union, Literal, Optional, cast
+
+from httpx import HTTPStatusError
 from httpx._models import Cookies
 from httpx import Response, Request, Client
-from typing import Optional, Literal, cast, Any
 
+from ._settings import settings
 from ..exceptions import (
-    AssetsNotExistError,
+    REQUEST_EXCEPTION,
     RequestException,
-    REQUEST_EXCEPTION
+    NoContentTypeError,
+    AssetsNotExistError
 )
 
 # 向 Bestdori 发送 API 请求类
 class Api:
     '''向 Bestdori 发送 API 请求类
 
     参数:
         api (str): 请求的 API 地址
-        
-        proxy (Optional[str]): 代理服务器'''
+        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+    '''
     api: str
     '''请求的 API 地址'''
-    proxy: Optional[str]=None
+    proxy: Optional[Union[dict[str, str], str]]=None
     '''代理服务器'''
     headers: dict[str, str]
     '''请求头'''
     # 初始化
     def __init__(
         self,
         api: str,
-        proxy: Optional[str]=None
+        proxy: Optional[Union[dict[str, str], str]]=None
     ) -> None:
         '''初始化'''
         self.api = api
-        self.proxy = proxy
+        self.proxy = proxy or settings.proxy
         self.headers = {'Content-Type': 'application/json;charset=UTF-8'}
         return
     
     # 请求发送
     def request(
         self,
         method: Literal['get', 'post'],
@@ -49,21 +53,17 @@
         data: Optional[dict[str, Any]]=None,
         files: Optional[dict[str, tuple[str, BufferedReader]]]=None
     ) -> Response:
         '''请求发送
 
         参数:
             method (Literal[&#39;get&#39;, &#39;post&#39;]): API 调用方法
-            
             cookies (Optional[Cookies], optional): Cookies
-            
             params (Optional[dict[str, Any]], optional): 调用参数
-            
             data (Optional[dict[str, Any]], optional): 调用参数，将以 `json` 字符串形式发送
-            
             files (Optional[dict[str, tuple[str, BufferedReader]]], optional): 发送文件参数
 
         返回:
             Response: 收到的响应
         '''
         # 处理接收到的 API
         if self.api.startswith('http://') or self.api.startswith('https://'):
@@ -77,32 +77,33 @@
             cookies=cookies,
             params=params,
             data=cast(dict, dumps(data)) if data is not None else data,
             files=files,
             headers=self.headers if not self.api.endswith('/upload') else None
         )
         # 构建代理服务器字典
-        if self.proxy is not None:
+        if isinstance(self.proxy, str):
             proxies = {'http://': self.proxy, 'https://': self.proxy}
+        elif isinstance(self.proxy, dict):
+            proxies = self.proxy
         else:
             proxies = None
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies)) as client:
+        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
-            client.close()
         
         # 处理接收到的响应
         response.raise_for_status()
         # 判断接收到的响应是否为 json 格式
         if 'application/json' not in (content_type := response.headers.get('content-type', None)):
             if content_type is not None:
                 return response
             else:
-                raise Exception('接收到的响应没有 content-type。')
+                raise NoContentTypeError(response)
         
         if isinstance((response_data := response.json()), dict):
             if (result := response_data.get('result', None)) is not None:
                 if result is False:
                     if (code := response_data.get('code', None)) is not None:
                         if code in REQUEST_EXCEPTION.keys(): # 若错误码已被记录
                             exception_class = REQUEST_EXCEPTION[code]
@@ -120,43 +121,40 @@
 
 # 获取 Bestdori 资源数据
 class Assets:
     '''获取 Bestdori 资源数据
 
     参数:
         url (str): 请求的资源地址
-        
         server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;]): 资源所在服务器
-        
-        proxy (Optional[str]): 代理服务器'''
+        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+    '''
     url: str
     '''请求的资源地址'''
     server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif']
     '''资源所在服务器'''
-    proxy: Optional[str]=None
+    proxy: Optional[Union[dict[str, str], str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         url: str,
         server: Literal['jp', 'en', 'tw', 'cn', 'kr', 'llsif'],
-        proxy: Optional[str]=None
+        proxy: Optional[Union[dict[str, str], str]]=None
     ) -> None:
         '''获取 Bestdori 资源数据
 
         参数:
             url (str): 请求的资源地址
-            
             server (Literal[&#39;jp&#39;, &#39;en&#39;, &#39;tw&#39;, &#39;cn&#39;, &#39;kr&#39;, &#39;llsif&#39;]): 资源所在服务器
-            
-            proxy (Optional[str]): 代理服务器
+            proxy (Optional[Union[dict[str, str], str]]): 代理服务器
         '''
         self.url = url
         self.server = server
-        self.proxy = proxy
+        self.proxy = proxy or settings.proxy
         return
     
     # 获取资源连接
     def get_url(self) -> str:
         '''获取资源连接
 
         返回:
@@ -202,25 +200,33 @@
         if self.url.startswith('http://') or self.url.startswith('https://'):
             self.url = self.url
         else:
             self.url = f'https://bestdori.com/assets/{self.server}/' + self.url
         # 构建一个请求体
         request = Request('get', self.url)
         # 构建代理服务器字典
-        if self.proxy is not None:
+        if isinstance(self.proxy, str):
             proxies = {'http://': self.proxy, 'https://': self.proxy}
+        elif isinstance(self.proxy, dict):
+            proxies = self.proxy
         else:
             proxies = None
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies)) as client:
+        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
-            client.close()
         
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise AssetsNotExistError(self.url)
+            else:
+                raise exception
+        
         # 检测响应资源是否存在
         content_type = response.headers.get('content-type', None)
         if content_type is None or content_type == 'text/html':
             raise AssetsNotExistError(self.url)
         return response.content
     
     # 从 card.niconi.co.ni 获取资源
@@ -240,52 +246,56 @@
         # 构建代理服务器字典
         if self.proxy is not None:
             proxies = {'http://': self.proxy, 'https://': self.proxy}
         else:
             proxies = None
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies)) as client:
+        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
-            client.close()
         
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise AssetsNotExistError(self.url)
+            else:
+                raise exception
         # 检测响应资源是否存在
         content_type = response.headers.get('content-type', None)
         if content_type is None or content_type == 'text/html':
             raise AssetsNotExistError(self.url)
         return response.content
 
 # 获取 Bestdori res 资源数据
 class Res:
     '''获取 Bestdori res 资源数据
 
     参数:
         url (str): 请求的 res 资源地址
-        
-        proxy (Optional[str]): 代理服务器'''
+        proxy (Optional[Union[dict[str, str], str]]): 代理服务器
+    '''
     url: str
     '''请求的资源地址'''
-    proxy: Optional[str]=None
+    proxy: Optional[Union[dict[str, str], str]]=None
     '''代理服务器'''
     # 初始化
     def __init__(
         self,
         url: str,
-        proxy: Optional[str]=None
+        proxy: Optional[Union[dict[str, str], str]]=None
     ) -> None:
         '''获取 Bestdori 资源数据
 
         参数:
             url (str): 请求的资源地址
-            
             proxy (Optional[str]): 代理服务器
         '''
         self.url = url
-        self.proxy = proxy
+        self.proxy = proxy or settings.proxy
         return
     
     # 获取资源
     def get(self) -> bytes:
         '''获取资源
 
         返回:
@@ -298,23 +308,30 @@
             self.url = f'https://bestdori.com/res/' + self.url
         # 构建一个请求体
         request = Request(
             'get',
             self.url
         )
         # 构建代理服务器字典
-        if self.proxy is not None:
+        if isinstance(self.proxy, str):
             proxies = {'http://': self.proxy, 'https://': self.proxy}
+        elif isinstance(self.proxy, dict):
+            proxies = self.proxy
         else:
             proxies = None
         
         # 发送请求并获取响应
-        with Client(proxies=cast(dict, proxies)) as client:
+        with Client(proxies=cast(dict, proxies), timeout=settings.timeout, trust_env=False) as client:
             response = client.send(request)
-            client.close()
         
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except HTTPStatusError as exception:
+            if exception.response.status_code == 404:
+                raise AssetsNotExistError(self.url)
+            else:
+                raise exception
         # 检测响应资源是否存在
         content_type = response.headers.get('content-type', None)
         if content_type is None or content_type == 'text/html':
             raise AssetsNotExistError(self.url)
         return response.content
```

### Comparing `bestdori_api-0.1.9/bestdori/utils/note.py` & `bestdori-api-0.2.0/bestdori/utils/note.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 谱面音符相关模块'''
 from typing import Literal, Any
 from typing_extensions import override
 
 # 谱面音符类
 class NoteType:
     '''谱面音符类'''
-    type_: str
+    type: str
     '''音符类型'''
     beat: float
     '''节拍数'''
     # 初始化
     def __init__(self, **values) -> None:
         '''初始化'''
         for key, value in values.items():
             if key == 'type':
                 continue
             setattr(self, key, value)
         return
     
+    def __getitem__(self, key: str) -> Any:
+        '''获取属性'''
+        return getattr(self, key)
+    
     # 节拍数增减
     def beat_move(self, beat: float) -> None:
         '''节拍数增减
 
         参数:
             beat (float): 移动的节拍数
         '''
@@ -73,56 +77,56 @@
 class BPM(NoteType):
     '''BPM
 
     参数:
         bpm (float): BPM 值
         
         beat (float): 节拍数'''
-    type_: str = 'BPM'
+    type: str = 'BPM'
     '''音符类型'''
     bpm: float
     '''BPM 值'''
     # 字典化
     @property
     def __dict__(self) -> dict:
         '''字典化'''
         return {
             'bpm': self.bpm,
             'beat': self.beat,
-            'type': self.type_
+            'type': self.type
         }
 
 # 单键
 class Single(NoteType):
     '''单键
 
     参数:
         beat (float): 节拍数
         
         lane (int): 轨道数
         
         flick (bool, optional): 是否为滑键
         
         skill (bool, optional): 是否为技能键'''
-    type_: str = 'Single'
+    type: str = 'Single'
     '''音符类型'''
     lane: int
     '''轨道数'''
     flick: bool = False
     '''是否为滑键'''
     skill: bool = False
     '''是否为技能键'''
     # 字典化
     @property
     def __dict__(self) -> dict:
         '''字典化'''
         note = {
             'beat': self.beat,
             'lane': self.lane,
-            'type': self.type_
+            'type': self.type
         }
         if self.flick:
             note['flick'] = self.flick
         if self.skill:
             note['skill'] = self.skill
         return note
 
@@ -134,42 +138,42 @@
         beat (float): 节拍数
         
         lane (int): 轨道数
         
         width (int): 滑键宽度
         
         direction (Literal[&#39;Left&#39;, &#39;Right&#39;]): 滑键方向'''
-    type_: str = 'Directional'
+    type: str = 'Directional'
     '''音符类型'''
     lane: int
     '''轨道数'''
     width: int
     '''滑键宽度'''
     direction: Literal['Left', 'Right']
     '''滑键方向'''
     # 字典化
     @property
     def __dict__(self) -> dict:
         '''字典化'''
         note = {
             'beat': self.beat,
             'lane': self.lane,
-            'type': self.type_,
+            'type': self.type,
             'width': self.width,
             'direction': self.direction
         }
         return note
 
 # 滑条
 class Slide(NoteType):
     '''滑条
 
     参数:
         connections (list[Connection]): 滑键节点'''
-    type_: str = 'Slide'
+    type: str = 'Slide'
     '''音符类型'''
     connections: list[Connection]
     '''滑键节点'''
     # 初始化
     def __init__(self, **values) -> None:
         '''初始化'''
         for key, value in values.items():
@@ -187,15 +191,15 @@
         return
     
     # 字典化
     @property
     def __dict__(self) -> dict:
         '''字典化'''
         note: dict[str, Any] = {
-            'type': self.type_
+            'type': self.type
         }
         if self.connections:
             note['connections'] = [connection.__dict__ for connection in self.connections]
         return note
     
     # 节拍数增减
     @override
@@ -203,12 +207,13 @@
         for connection in self.connections:
             connection.beat += beat
         self.beat = self.connections[0].beat
         return
 
 __all__ = [
     'NoteType',
+    'Connection',
     'BPM',
     'Single',
     'Directional',
     'Slide'
 ]
```

### Comparing `bestdori_api-0.1.9/bestdori/utils/utils.py` & `bestdori-api-0.2.0/bestdori/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,17 @@
         'prepare': 'upload/prepare',
         'upload': 'upload',
         'status': 'upload/status/{hash}'
     },
     'misc': {
         'llsif': 'misc/llsif.{index}.json'
     },
+    'player': {
+        'get': 'player/{server}/{id}'
+    },
     'all': {
         'skills': 'skills/all.{index}.json',
         'stamps': 'stamps/all.{index}.json',
         'degrees': 'degrees/all.{index}.json',
         'meta': 'songs/meta/all.{index}.json',
         'archives': 'archives/all.{index}.json',
         'miracleTicketExchanges': 'miracleTicketExchanges/all.{index}.json',
```

### Comparing `bestdori_api-0.1.9/bestdori_api.egg-info/PKG-INFO` & `bestdori-api-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,296 +1,374 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6265 7374  : 2.1.Name: best
 00000020: 646f 7269 2d61 7069 0a56 6572 7369 6f6e  dori-api.Version
-00000030: 3a20 302e 312e 390a 5375 6d6d 6172 793a  : 0.1.9.Summary:
+00000030: 3a20 302e 322e 300a 5375 6d6d 6172 793a  : 0.2.0.Summary:
 00000040: 2042 6573 7464 6f72 6920 e79a 84e5 9084   Bestdori ......
 00000050: e7a7 8d20 4150 4920 e8b0 83e7 94a8 e695  ... API ........
 00000060: b4e5 9088 efbc 8ce5 8fa6 e5a4 96e9 9984  ................
 00000070: e5b8 a6e9 83a8 e588 86e5 8a9f e883 bd0a  ................
 00000080: 486f 6d65 2d70 6167 653a 2068 7474 7073  Home-page: https
 00000090: 3a2f 2f67 6974 6875 622e 636f 6d2f 5769  ://github.com/Wi
 000000a0: 6e64 6f77 7353 6f76 3866 6f72 5573 2f62  ndowsSov8forUs/b
-000000b0: 6573 7464 6f72 695f 6170 690a 4175 7468  estdori_api.Auth
+000000b0: 6573 7464 6f72 692d 6170 690a 4175 7468  estdori-api.Auth
 000000c0: 6f72 3a20 5769 6e64 6f77 7353 6f76 380a  or: WindowsSov8.
 000000d0: 4175 7468 6f72 2d65 6d61 696c 3a20 7177  Author-email: qw
 000000e0: 6572 7479 7569 6f70 3233 3333 4068 6f74  ertyuiop2333@hot
 000000f0: 6d61 696c 2e63 6f6d 0a4c 6963 656e 7365  mail.com.License
-00000100: 3a20 554e 4b4e 4f57 4e0a 4465 7363 7269  : UNKNOWN.Descri
-00000110: 7074 696f 6e3a 2021 5b62 6573 7464 6f72  ption: ![bestdor
-00000120: 695f 6170 6920 6c6f 676f 5d28 6874 7470  i_api logo](http
-00000130: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f57  s://github.com/W
-00000140: 696e 646f 7773 536f 7638 666f 7255 732f  indowsSov8forUs/
-00000150: 6265 7374 646f 7269 5f61 7069 2f62 6c6f  bestdori_api/blo
-00000160: 622f 6d61 696e 2f6c 6f67 6f2e 706e 6729  b/main/logo.png)
-00000170: 0a20 2020 2020 2020 203c 6469 7620 616c  .        <div al
-00000180: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00000190: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000001a0: 2042 6573 7464 6f72 695f 6170 690a 2020   Bestdori_api.  
-000001b0: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-000001c0: 2a3a 7761 726e 696e 673a 20e8 afa5 e9a1  *:warning: .....
-000001d0: b9e7 9bae e4bb 8de7 84b6 e680 a5e9 9c80  ................
-000001e0: e69b b4e6 96b0 e4b8 8e20 4465 6275 6720  ......... Debug 
-000001f0: efbc 8ce4 bdbf e794 a8e6 97b6 e88b a5e9  ................
-00000200: 8187 e588 b020 4275 6720 e688 96e5 85b6  ..... Bug ......
-00000210: e4bb 96e9 9c80 e8a6 81e7 9a84 e68e a5e5  ................
-00000220: 8fa3 e8af b7e5 8f8a e697 b6e6 8f90 e587  ................
-00000230: ba2a 2a0a 2020 2020 2020 2020 0a20 2020  .**.        .   
-00000240: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000250: 2020 2020 0a20 2020 2020 2020 2023 20e7      .        # .
-00000260: ae80 e4bb 8b0a 2020 2020 2020 2020 0a20  ......        . 
-00000270: 2020 2020 2020 20e8 bf99 e698 afe4 b880         .........
-00000280: e4b8 aae7 94a8 2050 7974 686f 6e20 e7bc  ...... Python ..
-00000290: 96e5 8699 e79a 84e8 b083 e794 a820 5b42  ............. [B
-000002a0: 6573 7464 6f72 695d 2868 7474 7073 3a2f  estdori](https:/
-000002b0: 2f62 6573 7464 6f72 692e 636f 6d2f 2920  /bestdori.com/) 
-000002c0: e590 84e7 a78d 2041 5049 20e4 b88e e8b5  ...... API .....
-000002d0: 84e6 ba90 e4b8 8be8 bdbd e79a 84e5 ba93  ................
-000002e0: efbc 8ce5 a4a7 e887 b4e5 8c85 e68b ace4  ................
-000002f0: ba86 e7a4 bee5 8cba e5b8 96e5 ad90 e79a  ................
-00000300: 84e5 a484 e790 86e4 bba5 e58f 8ae5 9084  ................
-00000310: e7a7 8d20 5b42 616e 4720 4472 6561 6def  ... [BanG Dream.
-00000320: bc81 e5b0 91e5 a5b3 e4b9 90e5 9ba2 e6b4  ................
-00000330: bee5 afb9 5d28 6874 7470 733a 2f2f 7a68  ....](https://zh
-00000340: 2e6d 6f65 6769 726c 2e6f 7267 2e63 6e2f  .moegirl.org.cn/
-00000350: 4261 6e47 5f44 7265 616d 215f 2545 3525  BanG_Dream!_%E5%
-00000360: 4230 2539 3125 4535 2541 3525 4233 2545  B0%91%E5%A5%B3%E
-00000370: 3425 4239 2539 3025 4535 2539 4225 4132  4%B9%90%E5%9B%A2
-00000380: 2545 3625 4234 2542 4525 4535 2541 4625  %E6%B4%BE%E5%AF%
-00000390: 4239 2545 4625 4243 2538 3129 20e6 b8b8  B9%EF%BC%81) ...
-000003a0: e688 8fe5 8685 e8b5 84e6 ba90 e79a 84e8  ................
-000003b0: 8eb7 e58f 96e3 8082 0a20 2020 2020 2020  .........       
-000003c0: 202a 2ae8 ada6 e591 8aef bc9a e6ad a4e6   **.............
-000003d0: a8a1 e59d 97e7 9bae e589 8de4 bb8d e784  ................
-000003e0: b6e4 ba9f e5be 85e5 ae8c e596 84e4 b88e  ................
-000003f0: e6b5 8be8 af95 efbc 8ce8 afb7 e4b8 8de8  ................
-00000400: a681 e5b0 86e5 85b6 e5bd 93e5 819a e4b8  ................
-00000410: 80e4 b8aa e7a8 b3e5 ae9a e79a 84e5 ba93  ................
-00000420: e4bd bfe7 94a8 e380 822a 2a0a 2020 2020  .........**.    
-00000430: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00000440: e79b aee5 898d e5b7 b2e6 9c89 e79a 8420  ............... 
-00000450: 4150 4920 e4b8 8ee5 8a9f e883 bd0a 2020  API ..........  
-00000460: 2020 2020 2020 0a20 2020 2020 2020 207c        .        |
-00000470: 4150 4920 e7b1 bbe5 88ab 7ce6 98af e590  API ......|.....
-00000480: a6e5 ae8c e596 847c e694 afe6 8c81 e79a  .......|........
-00000490: 84e5 8685 e5ae b97c 0a20 2020 2020 2020  .......|.       
-000004a0: 207c 3a2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d   |:-------|:----
-000004b0: 2d3a 7c3a 2d2d 2d2d 2d2d 7c0a 2020 2020  -:|:------|.    
-000004c0: 2020 2020 7ce7 94a8 e688 b77c f09f 918d      |......|....
-000004d0: 7ce7 99bb e5bd 95e3 8081 e69f a5e8 afa2  |...............
-000004e0: e380 81e5 b896 e5ad 90e8 8eb7 e58f 96e3  ................
-000004f0: 8081 e4bf a1e6 81af e88e b7e5 8f96 7c0a  ..............|.
-00000500: 2020 2020 2020 2020 7ce5 b896 e5ad 907c          |......|
-00000510: f09f 918d 7ce6 909c e7b4 a2e3 8081 e88e  ....|...........
-00000520: b7e5 8f96 e380 81e5 8f91 e8a1 a8e3 8081  ................
-00000530: e8af 84e8 aeba e380 81e5 969c e6ac a27c  ...............|
-00000540: 0a20 2020 2020 2020 207c e8b0 b1e9 9da2  .        |......
-00000550: 7cf0 9f91 8d7c e7a4 bee5 8cba e8b0 b1e9  |....|..........
-00000560: 9da2 e88e b7e5 8f96 e380 81e9 9fb3 e6ba  ................
-00000570: 90e4 b88e e5b0 81e9 9da2 e88e b7e5 8f96  ................
-00000580: e380 81e8 a784 e695 b4e5 8c96 e380 81e6  ................
-00000590: 95b0 e68d aee7 bb9f e8ae a1e3 8081 e6a0  ................
-000005a0: bce5 bc8f e4ba 92e8 bdac 7c0a 2020 2020  ..........|.    
-000005b0: 2020 2020 7ce6 9585 e4ba 8b7c f09f 918e      |......|....
-000005c0: f09f 918e 7ce7 a4be e58c bae6 9585 e4ba  ....|...........
-000005d0: 8be8 8eb7 e58f 967c 0a20 2020 2020 2020  .......|.       
-000005e0: 207c e8a7 92e8 89b2 7cf0 9fa4 947c e4bf   |......|....|..
-000005f0: a1e6 81af e88e b7e5 8f96 e380 81e8 b584  ................
-00000600: e6ba 90e8 8eb7 e58f 967c 0a20 2020 2020  .........|.     
-00000610: 2020 207c e58d a1e7 898c 7cf0 9f91 8e7c     |......|....|
-00000620: e4bf a1e6 81af e88e b7e5 8f96 e380 81e8  ................
-00000630: b584 e6ba 90e8 8eb7 e58f 967c 0a20 2020  ...........|.   
-00000640: 2020 2020 207c e69c 8de8 a385 7cf0 9f91       |......|...
-00000650: 8ef0 9f91 8e7c e4bf a1e6 81af e88e b7e5  .....|..........
-00000660: 8f96 7c0a 2020 2020 2020 2020 7ce6 b4bb  ..|.        |...
-00000670: e58a a87c f09f a494 7ce4 bfa1 e681 afe8  ...|....|.......
-00000680: 8eb7 e58f 96e3 8081 e8b5 84e6 ba90 e88e  ................
-00000690: b7e5 8f96 7c0a 2020 2020 2020 2020 7ce6  ....|.        |.
-000006a0: b4bb e58a a8e6 95b0 e68d ae7c f09f 918e  ...........|....
-000006b0: 7ce6 95b0 e68d aee8 8eb7 e58f 967c 0a20  |............|. 
-000006c0: 2020 2020 2020 207c e68b 9be5 8b9f 7cf0         |......|.
-000006d0: 9fa4 947c e695 b0e6 8dae e88e b7e5 8f96  ...|............
-000006e0: e380 81e8 b584 e6ba 90e8 8eb7 e58f 967c  ...............|
-000006f0: 0a20 2020 2020 2020 207c e6ad 8ce6 9bb2  .        |......
-00000700: 7cf0 9fa4 947c e4bf a1e6 81af e88e b7e5  |....|..........
-00000710: 8f96 e380 81e8 b584 e6ba 90e8 8eb7 e58f  ................
-00000720: 967c 0a20 2020 2020 2020 207c e6ad 8ce6  .|.        |....
-00000730: 9bb2 204d 6574 617c f09f 918e f09f 918e  .. Meta|........
-00000740: 7ce6 95b0 e68d aee8 8eb7 e58f 967c 0a20  |............|. 
-00000750: 2020 2020 2020 207c e799 bbe5 bd95 e5a5         |........
-00000760: 96e5 8ab1 7cf0 9fa4 947c e4bf a1e6 81af  ....|....|......
-00000770: e88e b7e5 8f96 e380 81e8 b584 e6ba 90e8  ................
-00000780: 8eb7 e58f 967c 0a20 2020 2020 2020 207c  .....|.        |
-00000790: e887 aae9 8089 e588 b87c f09f a494 7ce4  .........|....|.
-000007a0: bfa1 e681 afe8 8eb7 e58f 967c 0a20 2020  ...........|.   
-000007b0: 2020 2020 207c e6bc abe7 94bb 7cf0 9fa4       |......|...
-000007c0: 947c e4bf a1e6 81af e88e b7e5 8f96 e380  .|..............
-000007d0: 81e5 9bbe e789 87e8 8eb7 e58f 967c 0a20  .............|. 
-000007e0: 2020 2020 2020 207c e4bb bbe5 8aa1 7cf0         |......|.
-000007f0: 9fa4 947c e4bf a1e6 81af e88e b7e5 8f96  ...|............
-00000800: 7c0a 2020 2020 2020 2020 7c61 7961 6368  |.        |ayach
-00000810: 616e 7cf0 9fa4 947c e8b0 b1e9 9da2 e588  an|....|........
-00000820: 86e6 9e90 e380 81e6 b58b e8af 95e6 9c8d  ................
-00000830: e4b8 8ae4 bca0 e380 81e9 9abe e5ba a6e5  ................
-00000840: 8886 e69e 907c 0a20 2020 2020 2020 207c  .....|.        |
-00000850: e585 b6e4 bb96 e8b5 84e6 ba90 7cf0 9f91  ............|...
-00000860: 8ef0 9f91 8e7c e4bb 85e5 b08f e983 a8e5  .....|..........
-00000870: 8886 e8b5 84e6 ba90 e69c 89e5 8d95 e78b  ................
-00000880: ace8 8eb7 e58f 967c 0a20 2020 2020 2020  .......|.       
-00000890: 200a 2020 2020 2020 2020 2320 e5bf abe9   .        # ....
-000008a0: 809f e4bd bfe7 94a8 0a20 2020 2020 2020  .........       
-000008b0: 200a 2020 2020 2020 2020 e4bb a5e4 b88b   .        ......
-000008c0: e5b0 86e4 bba5 e88e b7e5 8f96 e7a4 bee5  ................
-000008d0: 8cba e887 aae5 88b6 e8b0 b1e9 9da2 205b  .............. [
-000008e0: 5b46 554c 4c5d 20e5 8589 e381 aee4 b8ad  [FULL] .........
-000008f0: e381 b85d 2868 7474 7073 3a2f 2f62 6573  ...](https://bes
-00000900: 7464 6f72 692e 636f 6d2f 636f 6d6d 756e  tdori.com/commun
-00000910: 6974 792f 6368 6172 7473 2f31 3131 3533  ity/charts/11153
-00000920: 332f 5769 6e64 6f77 7353 6f76 382d 4655  3/WindowsSov8-FU
-00000930: 4c4c 2920 e79a 84e4 bfa1 e681 afe4 b8ba  LL) ............
-00000940: e4be 8be3 8082 0a20 2020 2020 2020 200a  .......        .
-00000950: 2020 2020 2020 2020 e9a6 96e5 8588 efbc          ........
-00000960: 8ce4 bdbf e794 a8e4 bba5 e4b8 8be6 8c87  ................
-00000970: e4bb a4e5 ae89 e8a3 85e6 9cac e6a8 a1e5  ................
-00000980: 9d97 efbc 9a0a 2020 2020 2020 2020 6060  ......        ``
-00000990: 6062 6173 680a 2020 2020 2020 2020 2420  `bash.        $ 
-000009a0: 7069 7033 2069 6e73 7461 6c6c 2062 6573  pip3 install bes
-000009b0: 7464 6f72 695f 6170 690a 2020 2020 2020  tdori_api.      
-000009c0: 2020 6060 600a 2020 2020 2020 2020 e68e    ```.        ..
-000009d0: a5e4 b88b e69d a5e5 9ca8 e4b8 80e4 b8aa  ................
-000009e0: 2050 7974 686f 6e20 e884 9ae6 9cac e696   Python ........
-000009f0: 87e4 bbb6 e4b8 adef bc8c e4bd bfe7 94a8  ................
-00000a00: e5a6 82e4 b88b e4bb a3e7 a081 e88e b7e5  ................
-00000a10: 8f96 e68c 87e5 ae9a e5b8 96e5 ad90 e79a  ................
-00000a20: 84e5 85a8 e983 a8e4 bfa1 e681 afef bc88  ................
-00000a30: e8bf 99e9 878c e688 91e4 bbac e5b7 b2e7  ................
-00000a40: 9fa5 e8af a5e5 b896 e5ad 90e7 9a84 2049  .............. I
-00000a50: 4420 e4b8 ba20 6031 3131 3533 3360 efbc  D ... `111533`..
-00000a60: 89ef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
-00000a70: 7079 7468 6f6e 0a20 2020 2020 2020 2066  python.        f
-00000a80: 726f 6d20 6265 7374 646f 7269 2e70 6f73  rom bestdori.pos
-00000a90: 7420 696d 706f 7274 2050 6f73 740a 2020  t import Post.  
-00000aa0: 2020 2020 2020 0a20 2020 2020 2020 2064        .        d
-00000ab0: 6566 206d 6169 6e28 2920 2d3e 204e 6f6e  ef main() -> Non
-00000ac0: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-00000ad0: 20e5 ae9e e4be 8be5 8c96 2050 6f73 7420   ......... Post 
-00000ae0: e7b1 bb0a 2020 2020 2020 2020 2020 2020  ....            
-00000af0: 7020 3d20 506f 7374 2869 643d 2731 3131  p = Post(id='111
-00000b00: 3533 3327 290a 2020 2020 2020 2020 2020  533').          
-00000b10: 2020 2320 e8b0 83e7 94a8 e696 b9e6 b395    # ............
-00000b20: e88e b7e5 8f96 e4bf a1e6 81af 0a20 2020  .............   
-00000b30: 2020 2020 2020 2020 2069 6e66 6f20 3d20           info = 
-00000b40: 702e 6765 745f 6465 7461 696c 7328 290a  p.get_details().
-00000b50: 2020 2020 2020 2020 2020 2020 2320 e689              # ..
-00000b60: 93e5 8db0 e4bf a1e6 81af 0a20 2020 2020  ...........     
-00000b70: 2020 2020 2020 2070 7269 6e74 2869 6e66         print(inf
-00000b80: 6f29 0a20 2020 2020 2020 200a 2020 2020  o).        .    
-00000b90: 2020 2020 6d61 696e 2829 0a20 2020 2020      main().     
-00000ba0: 2020 2060 6060 0a20 2020 2020 2020 20e5     ```.        .
-00000bb0: be97 e588 b0e7 9a84 e8be 93e5 87ba e586  ................
-00000bc0: 85e5 aeb9 e5a6 82e4 b88b efbc 9a0a 2020  ..............  
-00000bd0: 2020 2020 2020 6060 6070 7974 686f 6e0a        ```python.
-00000be0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00000bf0: 2020 2020 2020 2763 6174 6567 6f72 794e        'categoryN
-00000c00: 616d 6527 3a20 2753 454c 465f 504f 5354  ame': 'SELF_POST
-00000c10: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00000c20: 6361 7465 676f 7279 4964 273a 2027 6368  categoryId': 'ch
-00000c30: 6172 7427 2c0a 2020 2020 2020 2020 2020  art',.          
-00000c40: 2020 2774 6974 6c65 273a 2027 5b46 554c    'title': '[FUL
-00000c50: 4c5d 20e5 8589 e381 aee4 b8ad e381 b827  L] ............'
-00000c60: 2c0a 2020 2020 2020 2020 2020 2020 2773  ,.            's
-00000c70: 6f6e 6727 3a20 7b0a 2020 2020 2020 2020  ong': {.        
-00000c80: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
-00000c90: 2763 7573 746f 6d27 2c0a 2020 2020 2020  'custom',.      
-00000ca0: 2020 2020 2020 2020 2020 2761 7564 696f            'audio
-00000cb0: 273a 2027 6874 7470 733a 2f2f 6265 7374  ': 'https://best
-00000cc0: 646f 7269 2e63 6f6d 2f61 7069 2f75 706c  dori.com/api/upl
-00000cd0: 6f61 642f 6669 6c65 2f65 3461 3038 3066  oad/file/e4a080f
-00000ce0: 3834 6266 6132 6361 3437 6232 3362 3339  84bfa2ca47b23b39
-00000cf0: 3061 3436 3463 3831 3965 6331 3765 3730  0a464c819ec17e70
-00000d00: 6227 2c0a 2020 2020 2020 2020 2020 2020  b',.            
-00000d10: 2020 2020 2763 6f76 6572 273a 2027 6874      'cover': 'ht
-00000d20: 7470 733a 2f2f 6265 7374 646f 7269 2e63  tps://bestdori.c
-00000d30: 6f6d 2f61 7069 2f75 706c 6f61 642f 6669  om/api/upload/fi
-00000d40: 6c65 2f65 3335 3335 6562 6234 6337 3430  le/e3535ebb4c740
-00000d50: 6334 3735 3733 3731 3032 3661 3164 6639  c4757371026a1df9
-00000d60: 6666 6230 3830 3130 3330 3727 0a20 2020  ffb08010307'.   
-00000d70: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00000d80: 2020 2020 2020 2020 2761 7274 6973 7473          'artists
-00000d90: 273a 2027 e7b5 90e6 9d9f e383 90e3 83b3  ': '............
-00000da0: e383 8927 2c0a 2020 2020 2020 2020 2020  ...',.          
-00000db0: 2020 2764 6966 6627 3a20 342c 0a20 2020    'diff': 4,.   
-00000dc0: 2020 2020 2020 2020 2027 6c65 7665 6c27           'level'
-00000dd0: 3a20 3330 2c0a 2020 2020 2020 2020 2020  : 30,.          
-00000de0: 2020 2763 6861 7274 273a 205b 0a20 2020    'chart': [.   
-00000df0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2027 6270 6d27 3a20 3139 312c 0a20     'bpm': 191,. 
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 2027 6265 6174 273a 2030 2c0a 2020     'beat': 0,.  
-00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e50: 2020 2774 7970 6527 3a20 2742 504d 270a    'type': 'BPM'.
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00000e80: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000e90: 2020 2020 2020 2020 2027 6265 6174 273a           'beat':
-00000ea0: 2031 3932 2c0a 2020 2020 2020 2020 2020   192,.          
-00000eb0: 2020 2020 2020 2020 2020 276c 616e 6527            'lane'
-00000ec0: 3a20 332e 0a20 2020 2020 2020 2020 2020  : 3..           
-00000ed0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-00000ee0: 2027 5369 6e67 6c65 270a 2020 2020 2020   'Single'.      
-00000ef0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000f00: 2020 2020 2020 2020 2020 2020 202e 2e2e               ...
-00000f10: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00000f20: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00000f30: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00000f40: 2020 6060 600a 2020 2020 2020 2020 e5a6    ```.        ..
-00000f50: 82e6 9e9c e683 b3e8 a681 e88e b7e5 8f96  ................
-00000f60: e8bf 99e4 b8aa e887 aae5 88b6 e8b0 b1e9  ................
-00000f70: 9da2 e79a 84e8 b0b1 e99d a2ef bc8c e688  ................
-00000f80: 96e8 8085 e683 b3e8 a681 e88e b7e5 8f96  ................
-00000f90: e5ae 83e7 9a84 e99f b3e6 ba90 e4b8 8ee5  ................
-00000fa0: b081 e99d a2ef bc8c e4bb a5e4 b88b e4bb  ................
-00000fb0: a3e7 a081 e5b0 86e4 bc9a e8bf 9be8 a18c  ................
-00000fc0: e88e b7e5 8f96 efbc 9a0a 2020 2020 2020  ..........      
-00000fd0: 2020 6060 6070 7974 686f 6e0a 2020 2020    ```python.    
-00000fe0: 2020 2020 6672 6f6d 2062 6573 7464 6f72      from bestdor
-00000ff0: 692e 706f 7374 2069 6d70 6f72 7420 506f  i.post import Po
-00001000: 7374 0a20 2020 2020 2020 200a 2020 2020  st.        .    
-00001010: 2020 2020 6465 6620 6d61 696e 2829 202d      def main() -
-00001020: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
-00001030: 2020 2020 2320 e5ae 9ee4 be8b e58c 9620      # ......... 
-00001040: 506f 7374 20e7 b1bb 0a20 2020 2020 2020  Post ....       
-00001050: 2020 2020 2070 203d 2050 6f73 7428 6964       p = Post(id
-00001060: 3d27 3131 3135 3333 2729 0a20 2020 2020  ='111533').     
-00001070: 2020 2020 2020 2023 20e8 b083 e794 a8e6         # .......
-00001080: 96b9 e6b3 95e8 8eb7 e58f 96e8 b0b1 e99d  ................
-00001090: a20a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-000010a0: 6172 7420 3d20 702e 6765 745f 6368 6172  art = p.get_char
-000010b0: 7428 2920 2320 e88e b7e5 8f96 e79a 84e5  t() # ..........
-000010c0: b086 e698 afe4 b880 e4b8 aae8 b0b1 e99d  ................
-000010d0: a2e5 ae9e e4be 8b0a 2020 2020 2020 2020  ........        
-000010e0: 2020 2020 2320 e8b0 83e7 94a8 e696 b9e6      # ..........
-000010f0: b395 e88e b7e5 8f96 e99f b3e6 ba90 e4b8  ................
-00001100: 8ee5 b081 e99d a20a 2020 2020 2020 2020  ........        
-00001110: 2020 2020 696e 666f 203d 2070 2e67 6574      info = p.get
-00001120: 5f73 6f6e 6728 2920 2320 e88e b7e5 8f96  _song() # ......
-00001130: e79a 84e5 b086 e698 afe4 b880 e4b8 aae5  ................
-00001140: 8c85 e590 abe4 ba86 e99f b3e6 ba90 e4b8  ................
-00001150: 8ee5 b081 e99d a2e7 9a84 2062 7974 6573  .......... bytes
-00001160: 20e5 ad97 e585 b80a 2020 2020 2020 2020   .......        
-00001170: 0a20 2020 2020 2020 206d 6169 6e28 290a  .        main().
-00001180: 2020 2020 2020 2020 6060 600a 506c 6174          ```.Plat
-00001190: 666f 726d 3a20 554e 4b4e 4f57 4e0a 436c  form: UNKNOWN.Cl
-000011a0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000011b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000011c0: 3a20 5079 7468 6f6e 203a 3a20 332e 380a  : Python :: 3.8.
-000011d0: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-000011e0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000011f0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00001200: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
-00001210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00001220: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00001230: 740a 5265 7175 6972 6573 2d50 7974 686f  t.Requires-Pytho
-00001240: 6e3a 203e 3d33 2e38 0a44 6573 6372 6970  n: >=3.8.Descrip
-00001250: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
-00001260: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
-00001270: 0a                                       .
+00000100: 3a20 4d49 540a 4465 7363 7269 7074 696f  : MIT.Descriptio
+00000110: 6e3a 203c 6469 7620 616c 6967 6e3d 2263  n: <div align="c
+00000120: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+00000130: 0a20 2020 2020 2020 2021 5b62 6573 7464  .        ![bestd
+00000140: 6f72 692d 6170 6920 6c6f 676f 5d28 6874  ori-api logo](ht
+00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000160: 2f57 696e 646f 7773 536f 7638 666f 7255  /WindowsSov8forU
+00000170: 732f 6265 7374 646f 7269 2d61 7069 2f62  s/bestdori-api/b
+00000180: 6c6f 622f 6d61 696e 2f6c 6f67 6f2e 706e  lob/main/logo.pn
+00000190: 6729 0a20 2020 2020 2020 200a 2020 2020  g).        .    
+000001a0: 2020 2020 2320 4265 7374 646f 7269 2d61      # Bestdori-a
+000001b0: 7069 0a20 2020 2020 2020 200a 2020 2020  pi.        .    
+000001c0: 2020 2020 5fe2 9ca8 205b 4265 7374 646f      _... [Bestdo
+000001d0: 7269 5d28 6874 7470 733a 2f2f 6265 7374  ri](https://best
+000001e0: 646f 7269 2e63 6f6d 2f29 20e7 9a84 e590  dori.com/) .....
+000001f0: 84e7 a78d 2041 5049 20e8 b083 e794 a8e6  .... API .......
+00000200: 95b4 e590 88ef bc8c e58f a6e5 a496 e999  ................
+00000210: 84e5 b8a6 e983 a8e5 8886 e58a 9fe8 83bd  ................
+00000220: 20e2 9ca8 5f0a 2020 2020 2020 2020 0a20   ..._.        . 
+00000230: 2020 2020 2020 202a 2a3a 7761 726e 696e         **:warnin
+00000240: 673a 20e8 afa5 e9a1 b9e7 9bae e4bb 8de7  g: .............
+00000250: 84b6 e680 a5e9 9c80 e69b b4e6 96b0 e4b8  ................
+00000260: 8e20 4465 6275 6720 efbc 8ce4 bdbf e794  . Debug ........
+00000270: a8e6 97b6 e88b a5e9 8187 e588 b020 4275  ............. Bu
+00000280: 6720 e688 96e5 85b6 e4bb 96e9 9c80 e8a6  g ..............
+00000290: 81e7 9a84 e68e a5e5 8fa3 e8af b7e5 8f8a  ................
+000002a0: e697 b6e6 8f90 e587 ba2a 2a0a 2020 2020  .........**.    
+000002b0: 2020 2020 0a20 2020 2020 2020 203c 2f64      .        </d
+000002c0: 6976 3e0a 2020 2020 2020 2020 0a20 2020  iv>.        .   
+000002d0: 2020 2020 203c 7020 616c 6967 6e3d 2263       <p align="c
+000002e0: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+000002f0: 0a20 2020 2020 2020 203c 6120 6872 6566  .        <a href
+00000300: 3d22 6874 7470 733a 2f2f 6265 7374 646f  ="https://bestdo
+00000310: 7269 2e63 6f6d 2f22 3e0a 2020 2020 2020  ri.com/">.      
+00000320: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000330: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000340: 732e 696f 2f62 6164 6765 2f62 6573 7464  s.io/badge/bestd
+00000350: 6f72 692d 6170 692d 3139 3736 4433 2220  ori-api-1976D3" 
+00000360: 616c 743d 226c 6963 656e 7365 223e 0a20  alt="license">. 
+00000370: 2020 2020 2020 203c 2f61 3e0a 2020 2020         </a>.    
+00000380: 2020 2020 0a20 2020 2020 2020 203c 6120      .        <a 
+00000390: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000003a0: 7468 7562 2e63 6f6d 2f57 696e 646f 7773  thub.com/Windows
+000003b0: 536f 7638 666f 7255 732f 6265 7374 646f  Sov8forUs/bestdo
+000003c0: 7269 2d61 7069 223e 0a20 2020 2020 2020  ri-api">.       
+000003d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+000003e0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000003f0: 2e69 6f2f 6769 7468 7562 2f76 2f72 656c  .io/github/v/rel
+00000400: 6561 7365 2f57 696e 646f 7773 536f 7638  ease/WindowsSov8
+00000410: 666f 7255 732f 6265 7374 646f 7269 2d61  forUs/bestdori-a
+00000420: 7069 2220 616c 743d 224c 6174 6573 7420  pi" alt="Latest 
+00000430: 5265 6c65 6173 6520 5665 7273 696f 6e22  Release Version"
+00000440: 3e0a 2020 2020 2020 2020 3c2f 613e 0a20  >.        </a>. 
+00000450: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000460: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000470: 2f67 6974 6875 622e 636f 6d2f 5769 6e64  /github.com/Wind
+00000480: 6f77 7353 6f76 3866 6f72 5573 2f62 6573  owsSov8forUs/bes
+00000490: 7464 6f72 692d 6170 692f 626c 6f62 2f6d  tdori-api/blob/m
+000004a0: 6169 6e2f 4c49 4345 4e53 4522 3e0a 2020  ain/LICENSE">.  
+000004b0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
+000004c0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000004d0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+000004e0: 6c69 6365 6e73 652f 5769 6e64 6f77 7353  license/WindowsS
+000004f0: 6f76 3866 6f72 5573 2f62 6573 7464 6f72  ov8forUs/bestdor
+00000500: 692d 6170 6922 2061 6c74 3d22 4c69 6365  i-api" alt="Lice
+00000510: 6e73 6522 3e0a 2020 2020 2020 2020 3c2f  nse">.        </
+00000520: 613e 0a20 2020 2020 2020 200a 2020 2020  a>.        .    
+00000530: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000540: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00000550: 6f72 672f 646f 776e 6c6f 6164 732f 223e  org/downloads/">
+00000560: 0a20 2020 2020 2020 2020 203c 696d 6720  .          <img 
+00000570: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000580: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00000590: 2f70 7976 6572 7369 6f6e 732f 6265 7374  /pyversions/best
+000005a0: 646f 7269 2d61 7069 2220 616c 743d 2250  dori-api" alt="P
+000005b0: 7974 686f 6e20 5665 7273 696f 6e22 3e0a  ython Version">.
+000005c0: 2020 2020 2020 2020 3c2f 613e 0a20 2020          </a>.   
+000005d0: 2020 2020 200a 2020 2020 2020 2020 3c2f       .        </
+000005e0: 703e 0a20 2020 2020 2020 200a 2020 2020  p>.        .    
+000005f0: 2020 2020 3e20 6265 7374 646f 7269 5f61      > bestdori_a
+00000600: 7069 20e5 b7b2 e69b b4e5 908d e4b8 ba20  pi ............ 
+00000610: 6265 7374 646f 7269 2d61 7069 0a20 2020  bestdori-api.   
+00000620: 2020 2020 203e 20e8 8ba5 e5ae 89e8 a385       > .........
+00000630: e8bf 87e4 b98b e589 8de7 9a84 2060 6265  ............ `be
+00000640: 7374 646f 7269 5f61 7069 6020 e58c 85ef  stdori_api` ....
+00000650: bc8c e8af b7e4 bdbf e794 a8e6 8c87 e4bb  ................
+00000660: a40a 2020 2020 2020 2020 3e20 6060 6062  ..        > ```b
+00000670: 6173 680a 2020 2020 2020 2020 3e20 7069  ash.        > pi
+00000680: 7020 756e 696e 7374 616c 6c20 6265 7374  p uninstall best
+00000690: 646f 7269 5f61 7069 0a20 2020 2020 2020  dori_api.       
+000006a0: 203e 2060 6060 0a20 2020 2020 2020 203e   > ```.        >
+000006b0: 200a 2020 2020 2020 2020 3e20 e58d b8e8   .        > ....
+000006c0: bdbd e58e 9f20 6062 6573 7464 6f72 695f  ..... `bestdori_
+000006d0: 6170 6960 20e5 8c85 e590 8eef bc8c e987  api` ...........
+000006e0: 8de6 96b0 e5ae 89e8 a385 2060 6265 7374  .......... `best
+000006f0: 646f 7269 2d61 7069 6020 e58c 850a 2020  dori-api` ....  
+00000700: 2020 2020 2020 3e20 e590 a6e5 8899 e58f        > ........
+00000710: afe8 83bd e5af bce8 87b4 e69c aae7 9fa5  ................
+00000720: e79a 84e5 86b2 e7aa 81e9 97ae e9a2 980a  ................
+00000730: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000740: 2023 2320 e7ae 80e4 bb8b 0a20 2020 2020   ## .......     
+00000750: 2020 200a 2020 2020 2020 2020 e8bf 99e6     .        ....
+00000760: 98af e4b8 80e4 b8aa e794 a820 5079 7468  ........... Pyth
+00000770: 6f6e 20e7 bc96 e586 99e7 9a84 e8b0 83e7  on .............
+00000780: 94a8 205b 4265 7374 646f 7269 5d28 6874  .. [Bestdori](ht
+00000790: 7470 733a 2f2f 6265 7374 646f 7269 2e63  tps://bestdori.c
+000007a0: 6f6d 2f29 20e5 9084 e7a7 8d20 4150 4920  om/) ...... API 
+000007b0: e4b8 8ee8 b584 e6ba 90e4 b88b e8bd bde7  ................
+000007c0: 9a84 e5ba 93ef bc8c e5a4 a7e8 87b4 e58c  ................
+000007d0: 85e6 8bac e4ba 86e7 a4be e58c bae5 b896  ................
+000007e0: e5ad 90e7 9a84 e5a4 84e7 9086 e4bb a5e5  ................
+000007f0: 8f8a e590 84e7 a78d 205b 4261 6e47 2044  ........ [BanG D
+00000800: 7265 616d efbc 81e5 b091 e5a5 b3e4 b990  ream............
+00000810: e59b a2e6 b4be e5af b95d 2868 7474 7073  .........](https
+00000820: 3a2f 2f7a 682e 6d6f 6567 6972 6c2e 6f72  ://zh.moegirl.or
+00000830: 672e 636e 2f42 616e 475f 4472 6561 6d21  g.cn/BanG_Dream!
+00000840: 5f25 4535 2542 3025 3931 2545 3525 4135  _%E5%B0%91%E5%A5
+00000850: 2542 3325 4534 2542 3925 3930 2545 3525  %B3%E4%B9%90%E5%
+00000860: 3942 2541 3225 4536 2542 3425 4245 2545  9B%A2%E6%B4%BE%E
+00000870: 3525 4146 2542 3925 4546 2542 4325 3831  5%AF%B9%EF%BC%81
+00000880: 2920 e6b8 b8e6 888f e586 85e8 b584 e6ba  ) ..............
+00000890: 90e7 9a84 e88e b7e5 8f96 e380 820a 2020  ..............  
+000008a0: 2020 2020 2020 2a2a e8ad a6e5 918a efbc        **........
+000008b0: 9ae6 ada4 e6a8 a1e5 9d97 e79b aee5 898d  ................
+000008c0: e4bb 8de7 84b6 e4ba 9fe5 be85 e5ae 8ce5  ................
+000008d0: 9684 e4b8 8ee6 b58b e8af 95ef bc8c e8af  ................
+000008e0: b7e4 b88d e8a6 81e5 b086 e585 b6e5 bd93  ................
+000008f0: e581 9ae4 b880 e4b8 aae7 a8b3 e5ae 9ae7  ................
+00000900: 9a84 e5ba 93e4 bdbf e794 a8e3 8082 2a2a  ..............**
+00000910: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000920: 2020 2323 2320 e79b aee5 898d e5b7 b2e6    ### ..........
+00000930: 9c89 e79a 8420 4150 4920 e4b8 8ee5 8a9f  ..... API ......
+00000940: e883 bd0a 2020 2020 2020 2020 0a20 2020  ....        .   
+00000950: 2020 2020 207c 4150 4920 e7b1 bbe5 88ab       |API ......
+00000960: 7ce6 98af e590 a6e5 ae8c e596 847c e694  |............|..
+00000970: afe6 8c81 e79a 84e5 8685 e5ae b97c 0a20  .............|. 
+00000980: 2020 2020 2020 207c 3a2d 2d2d 2d2d 2d2d         |:-------
+00000990: 7c3a 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  |:-----:|:------
+000009a0: 7c0a 2020 2020 2020 2020 7ce7 94a8 e688  |.        |.....
+000009b0: b77c f09f 918d 7ce7 99bb e5bd 95e3 8081  .|....|.........
+000009c0: e69f a5e8 afa2 e380 81e5 b896 e5ad 90e8  ................
+000009d0: 8eb7 e58f 96e3 8081 e4bf a1e6 81af e88e  ................
+000009e0: b7e5 8f96 7c0a 2020 2020 2020 2020 7ce5  ....|.        |.
+000009f0: b896 e5ad 907c f09f 918d 7ce6 909c e7b4  .....|....|.....
+00000a00: a2e3 8081 e88e b7e5 8f96 e380 81e5 8f91  ................
+00000a10: e8a1 a8e3 8081 e8af 84e8 aeba e380 81e5  ................
+00000a20: 969c e6ac a27c 0a20 2020 2020 2020 207c  .....|.        |
+00000a30: e8b0 b1e9 9da2 7cf0 9f91 8d7c e7a4 bee5  ......|....|....
+00000a40: 8cba e8b0 b1e9 9da2 e88e b7e5 8f96 e380  ................
+00000a50: 81e9 9fb3 e6ba 90e4 b88e e5b0 81e9 9da2  ................
+00000a60: e88e b7e5 8f96 e380 81e8 a784 e695 b4e5  ................
+00000a70: 8c96 e380 81e6 95b0 e68d aee7 bb9f e8ae  ................
+00000a80: a1e3 8081 e6a0 bce5 bc8f e4ba 92e8 bdac  ................
+00000a90: 7c0a 2020 2020 2020 2020 7ce6 9585 e4ba  |.        |.....
+00000aa0: 8b7c f09f 918e f09f 918e 7ce7 a4be e58c  .|........|.....
+00000ab0: bae6 9585 e4ba 8be8 8eb7 e58f 967c 0a20  .............|. 
+00000ac0: 2020 2020 2020 207c e8a7 92e8 89b2 7cf0         |......|.
+00000ad0: 9fa4 947c e4bf a1e6 81af e88e b7e5 8f96  ...|............
+00000ae0: e380 81e8 b584 e6ba 90e8 8eb7 e58f 967c  ...............|
+00000af0: 0a20 2020 2020 2020 207c e58d a1e7 898c  .        |......
+00000b00: 7cf0 9f91 8e7c e4bf a1e6 81af e88e b7e5  |....|..........
+00000b10: 8f96 e380 81e8 b584 e6ba 90e8 8eb7 e58f  ................
+00000b20: 967c 0a20 2020 2020 2020 207c e69c 8de8  .|.        |....
+00000b30: a385 7cf0 9f91 8ef0 9f91 8e7c e4bf a1e6  ..|........|....
+00000b40: 81af e88e b7e5 8f96 7c0a 2020 2020 2020  ........|.      
+00000b50: 2020 7ce6 b4bb e58a a87c f09f a494 7ce4    |......|....|.
+00000b60: bfa1 e681 afe8 8eb7 e58f 96e3 8081 e8b5  ................
+00000b70: 84e6 ba90 e88e b7e5 8f96 7c0a 2020 2020  ..........|.    
+00000b80: 2020 2020 7ce6 b4bb e58a a8e6 95b0 e68d      |...........
+00000b90: ae7c f09f 918e 7ce6 95b0 e68d aee8 8eb7  .|....|.........
+00000ba0: e58f 967c 0a20 2020 2020 2020 207c e68b  ...|.        |..
+00000bb0: 9be5 8b9f 7cf0 9fa4 947c e695 b0e6 8dae  ....|....|......
+00000bc0: e88e b7e5 8f96 e380 81e8 b584 e6ba 90e8  ................
+00000bd0: 8eb7 e58f 967c 0a20 2020 2020 2020 207c  .....|.        |
+00000be0: e6ad 8ce6 9bb2 7cf0 9fa4 947c e4bf a1e6  ......|....|....
+00000bf0: 81af e88e b7e5 8f96 e380 81e8 b584 e6ba  ................
+00000c00: 90e8 8eb7 e58f 967c 0a20 2020 2020 2020  .......|.       
+00000c10: 207c e6ad 8ce6 9bb2 204d 6574 617c f09f   |...... Meta|..
+00000c20: 918e f09f 918e 7ce6 95b0 e68d aee8 8eb7  ......|.........
+00000c30: e58f 967c 0a20 2020 2020 2020 207c e799  ...|.        |..
+00000c40: bbe5 bd95 e5a5 96e5 8ab1 7cf0 9fa4 947c  ..........|....|
+00000c50: e4bf a1e6 81af e88e b7e5 8f96 e380 81e8  ................
+00000c60: b584 e6ba 90e8 8eb7 e58f 967c 0a20 2020  ...........|.   
+00000c70: 2020 2020 207c e887 aae9 8089 e588 b87c       |.........|
+00000c80: f09f a494 7ce4 bfa1 e681 afe8 8eb7 e58f  ....|...........
+00000c90: 967c 0a20 2020 2020 2020 207c e6bc abe7  .|.        |....
+00000ca0: 94bb 7cf0 9fa4 947c e4bf a1e6 81af e88e  ..|....|........
+00000cb0: b7e5 8f96 e380 81e5 9bbe e789 87e8 8eb7  ................
+00000cc0: e58f 967c 0a20 2020 2020 2020 207c e4bb  ...|.        |..
+00000cd0: bbe5 8aa1 7cf0 9fa4 947c e4bf a1e6 81af  ....|....|......
+00000ce0: e88e b7e5 8f96 7c0a 2020 2020 2020 2020  ......|.        
+00000cf0: 7c61 7961 6368 616e 7cf0 9fa4 947c e8b0  |ayachan|....|..
+00000d00: b1e9 9da2 e588 86e6 9e90 e380 81e6 b58b  ................
+00000d10: e8af 95e6 9c8d e4b8 8ae4 bca0 e380 81e9  ................
+00000d20: 9abe e5ba a6e5 8886 e69e 907c 0a20 2020  ...........|.   
+00000d30: 2020 2020 207c e585 b6e4 bb96 e8b5 84e6       |..........
+00000d40: ba90 7cf0 9f91 8ef0 9f91 8e7c e4bb 85e5  ..|........|....
+00000d50: b08f e983 a8e5 8886 e8b5 84e6 ba90 e69c  ................
+00000d60: 89e5 8d95 e78b ace8 8eb7 e58f 967c 0a20  .............|. 
+00000d70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000d80: 2323 20e5 bfab e980 9fe4 bdbf e794 a80a  ## .............
+00000d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00000da0: 20e4 bba5 e4b8 8be5 b086 e4bb a5e8 8eb7   ...............
+00000db0: e58f 96e7 a4be e58c bae8 87aa e588 b6e8  ................
+00000dc0: b0b1 e99d a220 5b5b 4655 4c4c 5d20 e585  ..... [[FULL] ..
+00000dd0: 89e3 81ae e4b8 ade3 81b8 5d28 6874 7470  ..........](http
+00000de0: 733a 2f2f 6265 7374 646f 7269 2e63 6f6d  s://bestdori.com
+00000df0: 2f63 6f6d 6d75 6e69 7479 2f63 6861 7274  /community/chart
+00000e00: 732f 3131 3135 3333 2f57 696e 646f 7773  s/111533/Windows
+00000e10: 536f 7638 2d46 554c 4c29 20e7 9a84 e4bf  Sov8-FULL) .....
+00000e20: a1e6 81af e4b8 bae4 be8b e380 820a 2020  ..............  
+00000e30: 2020 2020 2020 0a20 2020 2020 2020 20e9        .        .
+00000e40: a696 e585 88ef bc8c e4bd bfe7 94a8 e4bb  ................
+00000e50: a5e4 b88b e68c 87e4 bba4 e5ae 89e8 a385  ................
+00000e60: e69c ace6 a8a1 e59d 97ef bc9a 0a20 2020  .............   
+00000e70: 2020 2020 2060 6060 6261 7368 0a20 2020       ```bash.   
+00000e80: 2020 2020 2024 2070 6970 3320 696e 7374       $ pip3 inst
+00000e90: 616c 6c20 6265 7374 646f 7269 2d61 7069  all bestdori-api
+00000ea0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00000eb0: 2020 2020 20e6 8ea5 e4b8 8be6 9da5 e59c       ...........
+00000ec0: a8e4 b880 e4b8 aa20 5079 7468 6f6e 20e8  ....... Python .
+00000ed0: 849a e69c ace6 9687 e4bb b6e4 b8ad efbc  ................
+00000ee0: 8ce4 bdbf e794 a8e5 a682 e4b8 8be4 bba3  ................
+00000ef0: e7a0 81e8 8eb7 e58f 96e6 8c87 e5ae 9ae5  ................
+00000f00: b896 e5ad 90e7 9a84 e585 a8e9 83a8 e4bf  ................
+00000f10: a1e6 81af efbc 88e8 bf99 e987 8ce6 8891  ................
+00000f20: e4bb ace5 b7b2 e79f a5e8 afa5 e5b8 96e5  ................
+00000f30: ad90 e79a 8420 4944 20e4 b8ba 2060 3131  ..... ID ... `11
+00000f40: 3135 3333 60ef bc89 efbc 9a0a 2020 2020  1533`.......    
+00000f50: 2020 2020 6060 6070 7974 686f 6e0a 2020      ```python.  
+00000f60: 2020 2020 2020 6672 6f6d 2062 6573 7464        from bestd
+00000f70: 6f72 692e 706f 7374 2069 6d70 6f72 7420  ori.post import 
+00000f80: 506f 7374 0a20 2020 2020 2020 200a 2020  Post.        .  
+00000f90: 2020 2020 2020 6465 6620 6d61 696e 2829        def main()
+00000fa0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00000fb0: 2020 2020 2020 2320 e5ae 9ee4 be8b e58c        # ........
+00000fc0: 9620 506f 7374 20e7 b1bb 0a20 2020 2020  . Post ....     
+00000fd0: 2020 2020 2020 2070 203d 2050 6f73 7428         p = Post(
+00000fe0: 6964 3d27 3131 3135 3333 2729 0a20 2020  id='111533').   
+00000ff0: 2020 2020 2020 2020 2023 20e8 b083 e794           # .....
+00001000: a8e6 96b9 e6b3 95e8 8eb7 e58f 96e4 bfa1  ................
+00001010: e681 af0a 2020 2020 2020 2020 2020 2020  ....            
+00001020: 696e 666f 203d 2070 2e67 6574 5f64 6574  info = p.get_det
+00001030: 6169 6c73 2829 0a20 2020 2020 2020 2020  ails().         
+00001040: 2020 2023 20e6 8993 e58d b0e4 bfa1 e681     # ...........
+00001050: af0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00001060: 696e 7428 696e 666f 290a 2020 2020 2020  int(info).      
+00001070: 2020 0a20 2020 2020 2020 206d 6169 6e28    .        main(
+00001080: 290a 2020 2020 2020 2020 6060 600a 2020  ).        ```.  
+00001090: 2020 2020 2020 e5be 97e5 88b0 e79a 84e8        ..........
+000010a0: be93 e587 bae5 8685 e5ae b9e5 a682 e4b8  ................
+000010b0: 8bef bc9a 0a20 2020 2020 2020 2060 6060  .....        ```
+000010c0: 7079 7468 6f6e 0a20 2020 2020 2020 207b  python.        {
+000010d0: 0a20 2020 2020 2020 2020 2020 2027 6361  .            'ca
+000010e0: 7465 676f 7279 4e61 6d65 273a 2027 5345  tegoryName': 'SE
+000010f0: 4c46 5f50 4f53 5427 2c0a 2020 2020 2020  LF_POST',.      
+00001100: 2020 2020 2020 2763 6174 6567 6f72 7949        'categoryI
+00001110: 6427 3a20 2763 6861 7274 272c 0a20 2020  d': 'chart',.   
+00001120: 2020 2020 2020 2020 2027 7469 746c 6527           'title'
+00001130: 3a20 275b 4655 4c4c 5d20 e585 89e3 81ae  : '[FULL] ......
+00001140: e4b8 ade3 81b8 272c 0a20 2020 2020 2020  ......',.       
+00001150: 2020 2020 2027 736f 6e67 273a 207b 0a20       'song': {. 
+00001160: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00001170: 7479 7065 273a 2027 6375 7374 6f6d 272c  type': 'custom',
+00001180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001190: 2027 6175 6469 6f27 3a20 2768 7474 7073   'audio': 'https
+000011a0: 3a2f 2f62 6573 7464 6f72 692e 636f 6d2f  ://bestdori.com/
+000011b0: 6170 692f 7570 6c6f 6164 2f66 696c 652f  api/upload/file/
+000011c0: 6534 6130 3830 6638 3462 6661 3263 6134  e4a080f84bfa2ca4
+000011d0: 3762 3233 6233 3930 6134 3634 6338 3139  7b23b390a464c819
+000011e0: 6563 3137 6537 3062 272c 0a20 2020 2020  ec17e70b',.     
+000011f0: 2020 2020 2020 2020 2020 2027 636f 7665             'cove
+00001200: 7227 3a20 2768 7474 7073 3a2f 2f62 6573  r': 'https://bes
+00001210: 7464 6f72 692e 636f 6d2f 6170 692f 7570  tdori.com/api/up
+00001220: 6c6f 6164 2f66 696c 652f 6533 3533 3565  load/file/e3535e
+00001230: 6262 3463 3734 3063 3437 3537 3337 3130  bb4c740c47573710
+00001240: 3236 6131 6466 3966 6662 3038 3031 3033  26a1df9ffb080103
+00001250: 3037 270a 2020 2020 2020 2020 2020 2020  07'.            
+00001260: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
+00001270: 6172 7469 7374 7327 3a20 27e7 b590 e69d  artists': '.....
+00001280: 9fe3 8390 e383 b3e3 8389 272c 0a20 2020  ..........',.   
+00001290: 2020 2020 2020 2020 2027 6469 6666 273a           'diff':
+000012a0: 2034 2c0a 2020 2020 2020 2020 2020 2020   4,.            
+000012b0: 276c 6576 656c 273a 2033 302c 0a20 2020  'level': 30,.   
+000012c0: 2020 2020 2020 2020 2027 6368 6172 7427           'chart'
+000012d0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000012e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000012f0: 2020 2020 2020 2020 2020 2762 706d 273a            'bpm':
+00001300: 2031 3931 2c0a 2020 2020 2020 2020 2020   191,.          
+00001310: 2020 2020 2020 2020 2020 2762 6561 7427            'beat'
+00001320: 3a20 302c 0a20 2020 2020 2020 2020 2020  : 0,.           
+00001330: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+00001340: 2027 4250 4d27 0a20 2020 2020 2020 2020   'BPM'.         
+00001350: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00001360: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2762 6561 7427 3a20 3139 322c 0a20 2020  'beat': 192,.   
+00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013a0: 2027 6c61 6e65 273a 2033 2e0a 2020 2020   'lane': 3..    
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2774 7970 6527 3a20 2753 696e 676c 6527  'type': 'Single'
+000013d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013e0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+000013f0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00001400: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00001410: 2020 202e 2e2e 0a20 2020 2020 2020 207d     ....        }
+00001420: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
+00001430: 2020 2020 20e5 a682 e69e 9ce6 83b3 e8a6       ...........
+00001440: 81e8 8eb7 e58f 96e8 bf99 e4b8 aae8 87aa  ................
+00001450: e588 b6e8 b0b1 e99d a2e7 9a84 e8b0 b1e9  ................
+00001460: 9da2 efbc 8ce6 8896 e880 85e6 83b3 e8a6  ................
+00001470: 81e8 8eb7 e58f 96e5 ae83 e79a 84e9 9fb3  ................
+00001480: e6ba 90e4 b88e e5b0 81e9 9da2 efbc 8ce4  ................
+00001490: bba5 e4b8 8be4 bba3 e7a0 81e5 b086 e4bc  ................
+000014a0: 9ae8 bf9b e8a1 8ce8 8eb7 e58f 96ef bc9a  ................
+000014b0: 0a20 2020 2020 2020 2060 6060 7079 7468  .        ```pyth
+000014c0: 6f6e 0a20 2020 2020 2020 2066 726f 6d20  on.        from 
+000014d0: 6265 7374 646f 7269 2e70 6f73 7420 696d  bestdori.post im
+000014e0: 706f 7274 2050 6f73 740a 2020 2020 2020  port Post.      
+000014f0: 2020 0a20 2020 2020 2020 2064 6566 206d    .        def m
+00001500: 6169 6e28 2920 2d3e 204e 6f6e 653a 0a20  ain() -> None:. 
+00001510: 2020 2020 2020 2020 2020 2023 20e5 ae9e             # ...
+00001520: e4be 8be5 8c96 2050 6f73 7420 e7b1 bb0a  ...... Post ....
+00001530: 2020 2020 2020 2020 2020 2020 7020 3d20              p = 
+00001540: 506f 7374 2869 643d 2731 3131 3533 3327  Post(id='111533'
+00001550: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00001560: e8b0 83e7 94a8 e696 b9e6 b395 e88e b7e5  ................
+00001570: 8f96 e8b0 b1e9 9da2 0a20 2020 2020 2020  .........       
+00001580: 2020 2020 2063 6861 7274 203d 2070 2e67       chart = p.g
+00001590: 6574 5f63 6861 7274 2829 2023 20e8 8eb7  et_chart() # ...
+000015a0: e58f 96e7 9a84 e5b0 86e6 98af e4b8 80e4  ................
+000015b0: b8aa e8b0 b1e9 9da2 e5ae 9ee4 be8b 0a20  ............... 
+000015c0: 2020 2020 2020 2020 2020 2023 20e8 b083             # ...
+000015d0: e794 a8e6 96b9 e6b3 95e8 8eb7 e58f 96e9  ................
+000015e0: 9fb3 e6ba 90e4 b88e e5b0 81e9 9da2 0a20  ............... 
+000015f0: 2020 2020 2020 2020 2020 2069 6e66 6f20             info 
+00001600: 3d20 702e 6765 745f 736f 6e67 2829 2023  = p.get_song() #
+00001610: 20e8 8eb7 e58f 96e7 9a84 e5b0 86e6 98af   ...............
+00001620: e4b8 80e4 b8aa e58c 85e5 90ab e4ba 86e9  ................
+00001630: 9fb3 e6ba 90e4 b88e e5b0 81e9 9da2 e79a  ................
+00001640: 8420 6279 7465 7320 e5ad 97e5 85b8 0a20  . bytes ....... 
+00001650: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001660: 6d61 696e 2829 0a20 2020 2020 2020 2060  main().        `
+00001670: 6060 0a50 6c61 7466 6f72 6d3a 2055 4e4b  ``.Platform: UNK
+00001680: 4e4f 574e 0a43 6c61 7373 6966 6965 723a  NOWN.Classifier:
+00001690: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000016a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000016b0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
+000016c0: 723a 204c 6963 656e 7365 203a 3a20 4f53  r: License :: OS
+000016d0: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+000016e0: 5420 4c69 6365 6e73 650a 436c 6173 7369  T License.Classi
+000016f0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00001700: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00001710: 6570 656e 6465 6e74 0a52 6571 7569 7265  ependent.Require
+00001720: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
+00001730: 4465 7363 7269 7074 696f 6e2d 436f 6e74  Description-Cont
+00001740: 656e 742d 5479 7065 3a20 7465 7874 2f6d  ent-Type: text/m
+00001750: 6172 6b64 6f77 6e0a                      arkdown.
```

### Comparing `bestdori_api-0.1.9/bestdori_api.egg-info/SOURCES.txt` & `bestdori-api-0.2.0/bestdori_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 LICENSE
 README.md
 setup.py
 bestdori/__init__.py
-bestdori/_settings.py
 bestdori/cards.py
 bestdori/characters.py
 bestdori/charts.py
 bestdori/comics.py
 bestdori/costumes.py
 bestdori/eventarchives.py
 bestdori/events.py
 bestdori/exceptions.py
 bestdori/gacha.py
 bestdori/logincampaigns.py
 bestdori/miracleticket.py
 bestdori/missions.py
+bestdori/models.py
+bestdori/player.py
 bestdori/post.py
 bestdori/songmeta.py
 bestdori/songs.py
 bestdori/upload.py
 bestdori/user.py
 bestdori/ayachan/__init__.py
-bestdori/ayachan/_settings.py
+bestdori/ayachan/exceptions.py
 bestdori/ayachan/utils/__init__.py
+bestdori/ayachan/utils/_settings.py
 bestdori/ayachan/utils/network.py
 bestdori/ayachan/utils/utils.py
 bestdori/utils/__init__.py
+bestdori/utils/_settings.py
 bestdori/utils/content.py
 bestdori/utils/network.py
 bestdori/utils/note.py
 bestdori/utils/utils.py
 bestdori_api.egg-info/PKG-INFO
 bestdori_api.egg-info/SOURCES.txt
 bestdori_api.egg-info/dependency_links.txt
```

### Comparing `bestdori_api-0.1.9/setup.py` & `bestdori-api-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
-    name='bestdori_api',
-    version='0.1.9',
+    name='bestdori-api',
+    version='0.2.0',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Bestdori 的各种 API 调用整合，另外附带部分功能',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/WindowsSov8forUs/bestdori_api',
+    url='https://github.com/WindowsSov8forUs/bestdori-api',
     include_package_data=False,
     packages=find_packages(),
+    license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.8',
 )
```

