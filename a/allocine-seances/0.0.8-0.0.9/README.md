# Comparing `tmp/allocine-seances-0.0.8.tar.gz` & `tmp/allocine_seances-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.8.tar", last modified: Sun Sep 10 09:10:43 2023, max compression
+gzip compressed data, was "allocine_seances-0.0.9.tar", last modified: Wed Apr 24 17:14:48 2024, max compression
```

## Comparing `allocine-seances-0.0.8.tar` & `allocine_seances-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-09-10 09:10:43.706592 allocine-seances-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     4724 2023-09-10 09:10:43.705592 allocine-seances-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2865 2023-07-30 17:43:56.000000 allocine-seances-0.0.8/README.md
--rw-rw-rw-   0        0        0      721 2023-09-10 09:10:16.000000 allocine-seances-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-10 09:10:43.706592 allocine-seances-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-10 09:10:43.664675 allocine-seances-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-09-10 09:10:43.671199 allocine-seances-0.0.8/src/allocineAPI/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.8/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-09-10 09:07:42.000000 allocine-seances-0.0.8/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-09-10 09:10:43.703591 allocine-seances-0.0.8/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4724 2023-09-10 09:10:43.000000 allocine-seances-0.0.8/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-09-10 09:10:43.000000 allocine-seances-0.0.8/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-10 09:10:43.000000 allocine-seances-0.0.8/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-09-10 09:10:43.000000 allocine-seances-0.0.8/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-09-10 09:10:43.000000 allocine-seances-0.0.8/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 17:14:48.758997 allocine_seances-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine_seances-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     4724 2024-04-24 17:14:48.755996 allocine_seances-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2865 2023-07-30 17:43:56.000000 allocine_seances-0.0.9/README.md
+-rw-rw-rw-   0        0        0      721 2024-04-24 17:03:07.000000 allocine_seances-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:14:48.758997 allocine_seances-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 17:14:48.726820 allocine_seances-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:14:48.730238 allocine_seances-0.0.9/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine_seances-0.0.9/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0    12022 2024-04-24 17:00:09.000000 allocine_seances-0.0.9/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:14:48.750994 allocine_seances-0.0.9/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4724 2024-04-24 17:14:48.000000 allocine_seances-0.0.9/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-24 17:14:48.000000 allocine_seances-0.0.9/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:14:48.000000 allocine_seances-0.0.9/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 17:14:48.000000 allocine_seances-0.0.9/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 17:14:48.000000 allocine_seances-0.0.9/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.8/LICENSE` & `allocine_seances-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.8/PKG-INFO` & `allocine_seances-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.8
+Version: 0.0.9
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `allocine-seances-0.0.8/README.md` & `allocine_seances-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.8/pyproject.toml` & `allocine_seances-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.8/src/allocineAPI/allocineAPI.py` & `allocine_seances-0.0.9/src/allocineAPI/allocineAPI.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,21 +174,37 @@
                     if title is None:
                         title = "Unknown Title"
 
                     original_title = element["movie"].get("originalTitle")
                     if original_title is None:
                         original_title = "Unknown Original Title"
 
+                    director = ""
+                    try:
+                        for credit in element["movie"]["credits"]:
+                            if credit["position"].get("name") == "DIRECTOR":
+                                if director != "":
+                                    director += " | "
+                                director += credit["person"].get("firstName") + " " + credit["person"].get("lastName")
+                    except:
+                        director = "Error"
+
+                    if director == "":
+                        director = "Unknown Director"
+
                     synopsis_full = element["movie"].get("synopsisFull")
                     if synopsis_full is None:
                         synopsis_full = "No Synopsis Available"
 
-                    url_poster = element["movie"]["poster"].get("url")
-                    if url_poster is None:
+                    if element["movie"]["poster"] is None:
                         url_poster = "No Poster URL Available"
+                    else:
+                        url_poster = element["movie"]["poster"].get("url")
+                        if url_poster is None:
+                            url_poster = "No Poster URL Available"
 
                     releases = element["movie"]["releases"]
                     result_release = list()
                     for release in releases:
                         name = release.get("name")
                         releaseDate = release.get("releaseDate")
                         if releaseDate is not None:
@@ -203,14 +219,15 @@
                     has_dvd_release = element["movie"]["flags"].get("hasDvdRelease", False)
                     is_premiere = element["movie"]["customFlags"].get("isPremiere", False)
                     weekly_outing = element["movie"]["customFlags"].get("weeklyOuting", False)
 
                     formated_data.append({
                         "title": title,
                         "originalTitle": original_title,
+                        "director": director,
                         "synopsisFull": synopsis_full,
                         "urlPoster": url_poster,
                         "releases": result_release,
                         "runtime": runtime,
                         "languages": languages,
                         "hasDvdRelease": has_dvd_release,
                         "isPremiere": is_premiere,
```

### Comparing `allocine-seances-0.0.8/src/allocine_seances.egg-info/PKG-INFO` & `allocine_seances-0.0.9/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.8
+Version: 0.0.9
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

