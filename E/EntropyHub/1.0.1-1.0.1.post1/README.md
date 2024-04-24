# Comparing `tmp/EntropyHub-1.0.1.tar.gz` & `tmp/EntropyHub-1.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EntropyHub-1.0.1.tar", last modified: Sat Apr 20 00:20:35 2024, max compression
+gzip compressed data, was "EntropyHub-1.0.1.post1.tar", last modified: Wed Apr 24 21:05:28 2024, max compression
```

## Comparing `EntropyHub-1.0.1.tar` & `EntropyHub-1.0.1.post1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.895594 EntropyHub-1.0.1/EntropyHub/
--rw-rw-rw-   0        0        0     3945 2024-01-07 01:04:32.000000 EntropyHub-1.0.1/EntropyHub/_ApEn.py
--rw-rw-rw-   0        0        0     3849 2024-01-01 21:19:20.000000 EntropyHub-1.0.1/EntropyHub/_AttnEn.py
--rw-rw-rw-   0        0        0     3465 2024-01-01 21:19:27.000000 EntropyHub-1.0.1/EntropyHub/_BubbEn.py
--rw-rw-rw-   0        0        0     4286 2024-04-11 12:49:48.000000 EntropyHub-1.0.1/EntropyHub/_CoSiEn.py
--rw-rw-rw-   0        0        0     4310 2024-01-01 21:19:42.000000 EntropyHub-1.0.1/EntropyHub/_CondEn.py
--rw-rw-rw-   0        0        0     7211 2024-02-14 16:53:36.000000 EntropyHub-1.0.1/EntropyHub/_DispEn.py
--rw-rw-rw-   0        0        0     7753 2024-03-19 01:45:42.000000 EntropyHub-1.0.1/EntropyHub/_DispEn2D.py
--rw-rw-rw-   0        0        0     4786 2024-01-01 21:20:51.000000 EntropyHub-1.0.1/EntropyHub/_DistEn.py
--rw-rw-rw-   0        0        0     7342 2024-01-01 21:20:58.000000 EntropyHub-1.0.1/EntropyHub/_DistEn2D.py
--rw-rw-rw-   0        0        0     4378 2023-12-26 22:21:02.000000 EntropyHub-1.0.1/EntropyHub/_DivEn.py
--rw-rw-rw-   0        0        0     3624 2024-01-01 21:21:39.000000 EntropyHub-1.0.1/EntropyHub/_EnofEn.py
--rw-rw-rw-   0        0        0     5292 2024-01-01 21:21:46.000000 EntropyHub-1.0.1/EntropyHub/_EspEn2D.py
--rw-rw-rw-   0        0        0     4568 2024-03-19 20:34:45.000000 EntropyHub-1.0.1/EntropyHub/_ExampleData.py
--rw-rw-rw-   0        0        0    10292 2024-04-10 09:26:28.000000 EntropyHub-1.0.1/EntropyHub/_FuzzEn.py
--rw-rw-rw-   0        0        0    11944 2024-03-19 19:41:05.000000 EntropyHub-1.0.1/EntropyHub/_FuzzEn2D.py
--rw-rw-rw-   0        0        0     5623 2024-01-01 21:22:42.000000 EntropyHub-1.0.1/EntropyHub/_GridEn.py
--rw-rw-rw-   0        0        0     4075 2024-01-01 21:23:44.000000 EntropyHub-1.0.1/EntropyHub/_IncrEn.py
--rw-rw-rw-   0        0        0     3444 2024-02-12 23:37:22.000000 EntropyHub-1.0.1/EntropyHub/_K2En.py
--rw-rw-rw-   0        0        0    11077 2024-03-21 13:57:35.000000 EntropyHub-1.0.1/EntropyHub/_MSEn.py
--rw-rw-rw-   0        0        0     7072 2024-01-01 21:24:34.000000 EntropyHub-1.0.1/EntropyHub/_MSEn2D.py
--rw-rw-rw-   0        0        0     5100 2024-04-12 12:06:16.000000 EntropyHub-1.0.1/EntropyHub/_MSobject.py
--rw-rw-rw-   0        0        0    13201 2023-12-26 22:49:28.000000 EntropyHub-1.0.1/EntropyHub/_PermEn.py
--rw-rw-rw-   0        0        0     7587 2023-12-26 22:56:37.000000 EntropyHub-1.0.1/EntropyHub/_PermEn2D.py
--rw-rw-rw-   0        0        0     4730 2024-01-01 21:25:25.000000 EntropyHub-1.0.1/EntropyHub/_PhasEn.py
--rw-rw-rw-   0        0        0     5738 2023-12-27 00:58:42.000000 EntropyHub-1.0.1/EntropyHub/_RangEn.py
--rw-rw-rw-   0        0        0     6107 2024-01-01 21:26:08.000000 EntropyHub-1.0.1/EntropyHub/_SampEn.py
--rw-rw-rw-   0        0        0     7404 2024-01-01 21:26:15.000000 EntropyHub-1.0.1/EntropyHub/_SampEn2D.py
--rw-rw-rw-   0        0        0     4108 2024-01-01 21:26:42.000000 EntropyHub-1.0.1/EntropyHub/_SlopEn.py
--rw-rw-rw-   0        0        0     4529 2024-01-01 21:26:58.000000 EntropyHub-1.0.1/EntropyHub/_SpecEn.py
--rw-rw-rw-   0        0        0     6120 2024-01-01 21:27:06.000000 EntropyHub-1.0.1/EntropyHub/_SyDyEn.py
--rw-rw-rw-   0        0        0     5541 2024-01-07 00:27:23.000000 EntropyHub-1.0.1/EntropyHub/_XApEn.py
--rw-rw-rw-   0        0        0     5821 2024-01-07 17:34:30.000000 EntropyHub-1.0.1/EntropyHub/_XCondEn.py
--rw-rw-rw-   0        0        0     6378 2024-01-07 18:04:42.000000 EntropyHub-1.0.1/EntropyHub/_XDistEn.py
--rw-rw-rw-   0        0        0    11966 2024-03-19 19:41:33.000000 EntropyHub-1.0.1/EntropyHub/_XFuzzEn.py
--rw-rw-rw-   0        0        0     4880 2024-01-07 18:50:39.000000 EntropyHub-1.0.1/EntropyHub/_XK2En.py
--rw-rw-rw-   0        0        0    10546 2024-03-21 13:57:59.000000 EntropyHub-1.0.1/EntropyHub/_XMSEn.py
--rw-rw-rw-   0        0        0     4404 2024-01-07 19:40:06.000000 EntropyHub-1.0.1/EntropyHub/_XPermEn.py
--rw-rw-rw-   0        0        0     6547 2024-01-06 22:50:26.000000 EntropyHub-1.0.1/EntropyHub/_XSampEn.py
--rw-rw-rw-   0        0        0     5202 2024-03-11 12:29:50.000000 EntropyHub-1.0.1/EntropyHub/_XSpecEn.py
--rw-rw-rw-   0        0        0    14927 2024-04-19 23:50:20.000000 EntropyHub-1.0.1/EntropyHub/__init__.py
--rw-rw-rw-   0        0        0     9959 2024-03-22 20:38:15.000000 EntropyHub-1.0.1/EntropyHub/_cMSEn.py
--rw-rw-rw-   0        0        0    11157 2024-03-22 20:37:30.000000 EntropyHub-1.0.1/EntropyHub/_cXMSEn.py
--rw-rw-rw-   0        0        0     9154 2024-03-21 13:59:16.000000 EntropyHub-1.0.1/EntropyHub/_hMSEn.py
--rw-rw-rw-   0        0        0    10791 2024-03-21 13:57:47.000000 EntropyHub-1.0.1/EntropyHub/_hXMSEn.py
--rw-rw-rw-   0        0        0     8313 2024-03-21 13:58:39.000000 EntropyHub-1.0.1/EntropyHub/_rMSEn.py
--rw-rw-rw-   0        0        0     9180 2024-03-21 13:57:41.000000 EntropyHub-1.0.1/EntropyHub/_rXMSEn.py
-drwxrwxrwx   0        0        0        0 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/EntropyHub.egg-info/
--rw-rw-rw-   0        0        0     9886 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 00:20:35.000000 EntropyHub-1.0.1/EntropyHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11357 2023-01-21 18:52:09.000000 EntropyHub-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      206 2023-01-21 18:52:09.000000 EntropyHub-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9886 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7922 2024-03-25 21:00:39.000000 EntropyHub-1.0.1/README.md
--rw-rw-rw-   0        0        0       85 2024-04-20 00:20:35.925696 EntropyHub-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0    11130 2024-04-20 00:18:33.000000 EntropyHub-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:05:28.448443 EntropyHub-1.0.1.post1/
+drwxrwxrwx   0        0        0        0 2024-04-24 21:05:28.418150 EntropyHub-1.0.1.post1/EntropyHub/
+-rw-rw-rw-   0        0        0     3945 2024-01-07 01:04:32.000000 EntropyHub-1.0.1.post1/EntropyHub/_ApEn.py
+-rw-rw-rw-   0        0        0     3849 2024-01-01 21:19:20.000000 EntropyHub-1.0.1.post1/EntropyHub/_AttnEn.py
+-rw-rw-rw-   0        0        0     3465 2024-01-01 21:19:27.000000 EntropyHub-1.0.1.post1/EntropyHub/_BubbEn.py
+-rw-rw-rw-   0        0        0     4286 2024-04-11 12:49:48.000000 EntropyHub-1.0.1.post1/EntropyHub/_CoSiEn.py
+-rw-rw-rw-   0        0        0     4310 2024-01-01 21:19:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_CondEn.py
+-rw-rw-rw-   0        0        0     7211 2024-02-14 16:53:36.000000 EntropyHub-1.0.1.post1/EntropyHub/_DispEn.py
+-rw-rw-rw-   0        0        0     7753 2024-03-19 01:45:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_DispEn2D.py
+-rw-rw-rw-   0        0        0     4786 2024-01-01 21:20:51.000000 EntropyHub-1.0.1.post1/EntropyHub/_DistEn.py
+-rw-rw-rw-   0        0        0     7342 2024-01-01 21:20:58.000000 EntropyHub-1.0.1.post1/EntropyHub/_DistEn2D.py
+-rw-rw-rw-   0        0        0     4378 2023-12-26 22:21:02.000000 EntropyHub-1.0.1.post1/EntropyHub/_DivEn.py
+-rw-rw-rw-   0        0        0     3624 2024-01-01 21:21:39.000000 EntropyHub-1.0.1.post1/EntropyHub/_EnofEn.py
+-rw-rw-rw-   0        0        0     5292 2024-01-01 21:21:46.000000 EntropyHub-1.0.1.post1/EntropyHub/_EspEn2D.py
+-rw-rw-rw-   0        0        0     4569 2024-04-22 17:24:48.000000 EntropyHub-1.0.1.post1/EntropyHub/_ExampleData.py
+-rw-rw-rw-   0        0        0    10292 2024-04-10 09:26:28.000000 EntropyHub-1.0.1.post1/EntropyHub/_FuzzEn.py
+-rw-rw-rw-   0        0        0    11944 2024-03-19 19:41:05.000000 EntropyHub-1.0.1.post1/EntropyHub/_FuzzEn2D.py
+-rw-rw-rw-   0        0        0     5623 2024-01-01 21:22:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_GridEn.py
+-rw-rw-rw-   0        0        0     4075 2024-01-01 21:23:44.000000 EntropyHub-1.0.1.post1/EntropyHub/_IncrEn.py
+-rw-rw-rw-   0        0        0     3444 2024-02-12 23:37:22.000000 EntropyHub-1.0.1.post1/EntropyHub/_K2En.py
+-rw-rw-rw-   0        0        0    11077 2024-03-21 13:57:35.000000 EntropyHub-1.0.1.post1/EntropyHub/_MSEn.py
+-rw-rw-rw-   0        0        0     7072 2024-01-01 21:24:34.000000 EntropyHub-1.0.1.post1/EntropyHub/_MSEn2D.py
+-rw-rw-rw-   0        0        0     5212 2024-04-24 13:22:13.000000 EntropyHub-1.0.1.post1/EntropyHub/_MSobject.py
+-rw-rw-rw-   0        0        0    13201 2023-12-26 22:49:28.000000 EntropyHub-1.0.1.post1/EntropyHub/_PermEn.py
+-rw-rw-rw-   0        0        0     7632 2024-04-22 21:55:20.000000 EntropyHub-1.0.1.post1/EntropyHub/_PermEn2D.py
+-rw-rw-rw-   0        0        0     4730 2024-01-01 21:25:25.000000 EntropyHub-1.0.1.post1/EntropyHub/_PhasEn.py
+-rw-rw-rw-   0        0        0     5738 2023-12-27 00:58:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_RangEn.py
+-rw-rw-rw-   0        0        0     6107 2024-01-01 21:26:08.000000 EntropyHub-1.0.1.post1/EntropyHub/_SampEn.py
+-rw-rw-rw-   0        0        0     7404 2024-01-01 21:26:15.000000 EntropyHub-1.0.1.post1/EntropyHub/_SampEn2D.py
+-rw-rw-rw-   0        0        0     4108 2024-01-01 21:26:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_SlopEn.py
+-rw-rw-rw-   0        0        0     4529 2024-01-01 21:26:58.000000 EntropyHub-1.0.1.post1/EntropyHub/_SpecEn.py
+-rw-rw-rw-   0        0        0     6120 2024-01-01 21:27:06.000000 EntropyHub-1.0.1.post1/EntropyHub/_SyDyEn.py
+-rw-rw-rw-   0        0        0     5541 2024-01-07 00:27:23.000000 EntropyHub-1.0.1.post1/EntropyHub/_XApEn.py
+-rw-rw-rw-   0        0        0     5821 2024-01-07 17:34:30.000000 EntropyHub-1.0.1.post1/EntropyHub/_XCondEn.py
+-rw-rw-rw-   0        0        0     6378 2024-01-07 18:04:42.000000 EntropyHub-1.0.1.post1/EntropyHub/_XDistEn.py
+-rw-rw-rw-   0        0        0    11966 2024-03-19 19:41:33.000000 EntropyHub-1.0.1.post1/EntropyHub/_XFuzzEn.py
+-rw-rw-rw-   0        0        0     4880 2024-01-07 18:50:39.000000 EntropyHub-1.0.1.post1/EntropyHub/_XK2En.py
+-rw-rw-rw-   0        0        0    10546 2024-03-21 13:57:59.000000 EntropyHub-1.0.1.post1/EntropyHub/_XMSEn.py
+-rw-rw-rw-   0        0        0     4404 2024-01-07 19:40:06.000000 EntropyHub-1.0.1.post1/EntropyHub/_XPermEn.py
+-rw-rw-rw-   0        0        0     6547 2024-01-06 22:50:26.000000 EntropyHub-1.0.1.post1/EntropyHub/_XSampEn.py
+-rw-rw-rw-   0        0        0     5202 2024-03-11 12:29:50.000000 EntropyHub-1.0.1.post1/EntropyHub/_XSpecEn.py
+-rw-rw-rw-   0        0        0    15910 2024-04-24 13:43:46.000000 EntropyHub-1.0.1.post1/EntropyHub/__init__.py
+-rw-rw-rw-   0        0        0     9959 2024-03-22 20:38:15.000000 EntropyHub-1.0.1.post1/EntropyHub/_cMSEn.py
+-rw-rw-rw-   0        0        0    11157 2024-03-22 20:37:30.000000 EntropyHub-1.0.1.post1/EntropyHub/_cXMSEn.py
+-rw-rw-rw-   0        0        0     9154 2024-03-21 13:59:16.000000 EntropyHub-1.0.1.post1/EntropyHub/_hMSEn.py
+-rw-rw-rw-   0        0        0    10791 2024-03-21 13:57:47.000000 EntropyHub-1.0.1.post1/EntropyHub/_hXMSEn.py
+-rw-rw-rw-   0        0        0     8313 2024-03-21 13:58:39.000000 EntropyHub-1.0.1.post1/EntropyHub/_rMSEn.py
+-rw-rw-rw-   0        0        0     9180 2024-03-21 13:57:41.000000 EntropyHub-1.0.1.post1/EntropyHub/_rXMSEn.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:05:28.448443 EntropyHub-1.0.1.post1/EntropyHub.egg-info/
+-rw-rw-rw-   0        0        0    11463 2024-04-24 21:05:28.000000 EntropyHub-1.0.1.post1/EntropyHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2024-04-24 21:05:28.000000 EntropyHub-1.0.1.post1/EntropyHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:05:28.000000 EntropyHub-1.0.1.post1/EntropyHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-24 21:05:28.000000 EntropyHub-1.0.1.post1/EntropyHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:05:28.000000 EntropyHub-1.0.1.post1/EntropyHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11357 2023-01-21 18:52:09.000000 EntropyHub-1.0.1.post1/LICENSE.txt
+-rw-rw-rw-   0        0        0      206 2023-01-21 18:52:09.000000 EntropyHub-1.0.1.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11463 2024-04-24 21:05:28.448443 EntropyHub-1.0.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     9481 2024-04-24 13:34:35.000000 EntropyHub-1.0.1.post1/README.md
+-rw-rw-rw-   0        0        0       85 2024-04-24 21:05:28.455157 EntropyHub-1.0.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0    12704 2024-04-24 21:05:24.000000 EntropyHub-1.0.1.post1/setup.py
```

### Comparing `EntropyHub-1.0.1/EntropyHub/_ApEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_ApEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_AttnEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_AttnEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_BubbEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_BubbEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_CoSiEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_CoSiEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_CondEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_CondEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_DispEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_DispEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_DispEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_DispEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_DistEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_DistEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_DistEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_DistEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_DivEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_DivEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_EnofEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_EnofEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_EspEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_EspEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_ExampleData.py` & `EntropyHub-1.0.1.post1/EntropyHub/_ExampleData.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     Returns sample datasets (time series or matrices) with specific properties 
     that are commonly used as benchmarks for assessing the performance of various
     entropy methods.
     The datasets returned by ExampleData() are used in the examples provided in
     documentation on www.EntropyHub.xyz and elsewhere.
     ***Note*** ExampleData() requires an internet connection to download and import the required datasets!
     
-    ``Data``is the sample dataset imported corresponding to the string input ``SigName``
+    ``Data`` is the sample dataset imported corresponding to the string input ``SigName``
     which can be one of the following:
         :SigName:   - One of the following strings:                           
-                    * ``uniform``          - uniformly distributed random number sequence in range [0 1], N = 5000
-                    * ``randintegers``     - randomly distributed integer sequence in range [1 8], N = 4096
-                    * ``gaussian``         - normally distributed number sequence [mean: 0, SD: 1], N = 5000
-                    * ``henon``            - X and Y components of the Henon attractor [alpha: 1.4, beta: .3, Xo = 0, Yo = 0], N = 4500
-                    * ``lorenz``           - X, Y, and Z components of the Lorenz attractor [sigma: 10, beta: 8/3, rho: 28, Xo = 10, Yo = 20, Zo = 10], N = 5917
-                    * ``chirp``            - chirp signal (f0 = .01, t1 = 4000, f1 = .025), N = 5000
-                    * ``uniform2``         - two uniformly distributed random number sequences in range [0,1], N = 4096
-                    * ``gaussian2``        - two normally distributed number sequences [mean: 0, SD: 1], N = 3000
-                    * ``randintegers2``    - two uniformly distributed pseudorandom integer sequences in range [1 8], N = 3000
-                    * ``uniform_Mat``      - matrix of uniformly distributed random numbers in range [0 1], N = 50 x 50
-                    * ``gaussian_Mat``     - matrix of normally distributed numbers [mean: 0, SD: 1], N = 60 x 120
-                    * ``randintegers_Mat`` - matrix of randomly distributed integers in range [1 8], N = 88 x 88
-                    * ``mandelbrot_Mat``   - matrix representing a Mandelbrot fractal image with values in range [0 255], N = 92 x 115
-                    * ``entropyhub_Mat``   - matrix representing the EntropyHub logo with values in range [0 255], N = 127 x 95
+                    :``uniform``:          - uniformly distributed random number sequence in range [0 1], N = 5000
+                    :``randintegers``:     - randomly distributed integer sequence in range [1 8], N = 4096
+                    :``gaussian``:         - normally distributed number sequence [mean: 0, SD: 1], N = 5000
+                    :``henon``:            - X and Y components of the Henon attractor [alpha: 1.4, beta: .3, Xo = 0, Yo = 0], N = 4500
+                    :``lorenz``:           - X, Y, and Z components of the Lorenz attractor [sigma: 10, beta: 8/3, rho: 28, Xo = 10, Yo = 20, Zo = 10], N = 5917
+                    :``chirp``:            - chirp signal (f0 = .01, t1 = 4000, f1 = .025), N = 5000
+                    :``uniform2``:         - two uniformly distributed random number sequences in range [0,1], N = 4096
+                    :``gaussian2``:        - two normally distributed number sequences [mean: 0, SD: 1], N = 3000
+                    :``randintegers2``:    - two uniformly distributed pseudorandom integer sequences in range [1 8], N = 3000
+                    :``uniform_Mat``:      - matrix of uniformly distributed random numbers in range [0 1], N = 50 x 50
+                    :``gaussian_Mat``:     - matrix of normally distributed numbers [mean: 0, SD: 1], N = 60 x 120
+                    :``randintegers_Mat``: - matrix of randomly distributed integers in range [1 8], N = 88 x 88
+                    :``mandelbrot_Mat``:   - matrix representing a Mandelbrot fractal image with values in range [0 255], N = 92 x 115
+                    :``entropyhub_Mat``:   - matrix representing the EntropyHub logo with values in range [0 255], N = 127 x 95
                          
     For further info on these graining procedures see the `EntropyHub guide <https://github.com/MattWillFlood/EntropyHub/blob/main/EntropyHub%20Guide.pdf>`_.
         
     """
     
     Chk = ["uniform","uniform2","randintegers2","randintegers",
         "henon","chirp","gaussian","gaussian2","lorenz",
```

### Comparing `EntropyHub-1.0.1/EntropyHub/_FuzzEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_FuzzEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_FuzzEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_FuzzEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_GridEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_GridEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_IncrEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_IncrEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_K2En.py` & `EntropyHub-1.0.1.post1/EntropyHub/_K2En.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_MSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_MSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_MSEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_MSEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_MSobject.py` & `EntropyHub-1.0.1.post1/EntropyHub/_MSobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         :``'CoSiEn'``:    - Cosine Similarity Entropy	
         :``'PhasEn'``:    - Phase Entropy	
         :``'SlopEn'``:    - Slope Entropy
         :``'BubbEn'``:    - Bubble Entropy	
         :``'GridEn'``:    - Grid Distribution Entropy	
         :``'EnofEn'``:    - Entropy of Entropy	
         :``'AttnEn'``:    - Attention Entropy
-        [``'DivEn'``]:    - Diversity Entropy
-        [``'RangEn'``]:   - Range Entropy
+        :``'DivEn'``:     - Diversity Entropy
+        :``'RangEn'``:    - Range Entropy
         
     
     :Cross Entropies:    
         :``'XApEn'``:     - Cross-Approximate Entropy
         :``'XSampEn'``:   - Cross-Sample Entropy
         :``'XFuzzEn'``:   - Cross-Fuzzy Entropy
         :``'XK2En'``:     - Cross-Kolmogorov Entropy
@@ -71,15 +71,15 @@
         :``'MvFuzzEn'``:   - Multivariate Fuzzy Entropy
         :``'MvDispEn'``:   - Multivariate Dispersion Entropy
         :``'MvCoSiEn'``:   - Multivariate Cosine Similarity Entropy
         :``'MvPermEn'``:   - Multivariate Permutation Entropy   
 
     
     :See also:
-        ``MSEn``, ``cMSEn``, ``rMSEn``, ``hMSEn``, ``XMSEn``, ``rXMSEn``, ``cXMSEn``, ``hXMSEn``    
+        ``MSEn``, ``MvMSEn``, ``cMSEn``, ``cMvMSEn``,  ``rMSEn``, ``hMSEn``, ``XMSEn``, ``rXMSEn``, ``cXMSEn``, ``hXMSEn``    
     """
         
     Chk = ['_ApEn',   '_SampEn', '_FuzzEn', '_K2En',   '_PermEn', '_CondEn', 
            '_DistEn', '_DispEn', '_SyDyEn', '_IncrEn', '_CoSiEn', '_PhasEn', 
            '_SpecEn', '_SlopEn', '_GridEn', '_BubbEn', '_EnofEn', '_AttnEn',
            '_DivEn', '_RangEn', 
            '_XApEn', '_XSampEn', '_XFuzzEn', '_XPermEn', 
@@ -89,16 +89,16 @@
     assert ('_'+EnType) in Chk, "EnType:      must be a valid entropy function name. \
     See help(EntropyHub.MSobject) for more info."
                 
     class MS_Entropy:
         def __init__(self, EnType, X):
             # _temp = __import__(('_'+EnType), globals(), locals(), [EnType], 0)
             
-            #_temp = __import__(('EntropyHub._'+EnType), fromlist=[EnType])
-            _temp = __import__('_'+EnType)
+            _temp = __import__(('EntropyHub._'+EnType), fromlist=[EnType])  # USE THIS AS METHOD FOR PUBLISHED PACKAGE
+            # _temp = __import__('_'+EnType)        # USE THIS FOR PACKAGE DEVEOPMENT
             
             self.Func = getattr(_temp,EnType) 
             self.Kwargs = X
     
     Mobj = MS_Entropy(EnType, kwargs)   
     return Mobj
```

### Comparing `EntropyHub-1.0.1/EntropyHub/_PermEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_PermEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_PermEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_PermEn2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             
     Returns the bidimensional permutation entropy estimate (``Perm2D``) estimated for 
     the data matrix (``Mat``) using the default parameters: time delay = 1,
     logarithm = natural, template matrix size = [floor(H/10) floor(W/10)]  
     (where H and W represent the height (rows) and width (columns) of the data matrix ``Mat``) 
     ** The minimum number of rows and columns of ``Mat`` must be > 10.
  
-     .. code-block:: python
+    .. code-block:: python
      
          Perm2D = PermEn2D(Mat, keyword = value, ...)
     
     Returns the bidimensional permutation entropy (``Perm2D``) estimates for the data
     matrix (``Mat``) using the specified 'keyword' arguments:
         :m:     - Template submatrix dimensions, an integer scalar (for sub-matrix with same height and width) or a two-element tuple of integers (height, width) with a minimum value > 1. (default: [floor(H/10) floor(W/10)])
         :tau:   - Time Delay, a positive integer > 1   (default: 1)
@@ -28,25 +28,31 @@
                     e.g. For ``Mat`` = [200 x 200], ``m = 3``, and ``tau = 1``, ``PermEn2D`` 
                     creates a vector of 753049836 elements. To enable matrices
                     greater than [128 x 128] elements, set ``'Lock' = false``. (default: true)
                     ``CAUTION: unlocking the permitted matrix size may cause memory``
                     ``errors that could lead your Python IDE to crash.``
                     
         
-    **NOTE**: 
-	     ``The original bidimensional permutation entropy algorithms [1][2]``
-	     ``do not account for equal-valued elements of the embedding matrices.``
+    .. note:: 
+
+	     **The original bidimensional permutation entropy algorithms [1][2]**
+	     **do not account for equal-valued elements of the embedding matrices.**
              To overcome this, PermEn2D uses the lowest common rank for
              such instances. For example, given an embedding matrix A where,
-             A = [3.4  5.5  7.3]         
-                 [2.1  6    9.9]       
-                 [7.3  1.1  2.1]        
-             would normally be mapped to an ordinal pattern like so,      
-             [3.4  5.5  7.3  2.1  6  9.9  7.3  1.1  2.1] =>
-             [ 8    4    9    1   2   5    3    7    6 ]
+
+             :A: 
+		|	[3.4  5.5  7.3]         
+                |   	[2.1  6    9.9]       
+                |   	[7.3  1.1  2.1]      
+  
+             would normally be mapped to an ordinal pattern like so,    
+  
+                |       [3.4  5.5  7.3  2.1  6  9.9  7.3  1.1  2.1] =>
+                |       [ 8    4    9    1   2   5    3    7    6 ]
+
              However, indices 4 & 9, and 3 & 7 have the same values, 2.1
              and 7.3 respectively. Instead, PermEn2D uses the ordinal pattern
              [ 8    4    4    1   2   5    3    3    6 ]
              where the lowest rank (4 & 3) are used instead (of 9 & 7). 
              Therefore, the number of possible permutations is no longer 
              (mx*my)!, but (mx*my)^(mx*my). Here, the PermEn2D value is 
              normalized by the maximum Shannon entropy (Smax = log((mx*my)!)
```

### Comparing `EntropyHub-1.0.1/EntropyHub/_PhasEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_PhasEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_RangEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_RangEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_SampEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_SampEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_SampEn2D.py` & `EntropyHub-1.0.1.post1/EntropyHub/_SampEn2D.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_SlopEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_SlopEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_SpecEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_SpecEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_SyDyEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_SyDyEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XApEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XApEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XCondEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XCondEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XDistEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XDistEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XFuzzEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XFuzzEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XK2En.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XK2En.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XPermEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XPermEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XSampEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XSampEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_XSpecEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_XSpecEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/__init__.py` & `EntropyHub-1.0.1.post1/EntropyHub/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,24 +216,41 @@
         Multiscale Cross-Approximate Entropy                  |	
         Multiscale Cross-Fuzzy Entropy                        |	MSobject
         Multiscale Cross-Permutation Entropy                  |	    +
         Multiscale Cross-Distribution Entropy                 |	XMSEn / cXMSEn
         Multiscale Cross-Kolmogorov Entropy                   |   rXMSEn / hXMSEn
         Multiscale Cross-Conditional Entropy                  |	
         
+        
+        _________________________________________________________________________
+        Multivariate Multiscale Entropy Functions             |	Function Name
+        ______________________________________________________|__________________
+        Multiscale Cross-Entropy Object                       |   MSobject
+                                                              |
+        Multivariate Multiscale Entropy                       |	 MvMSEn
+        Composite/Refined-Composite Multiscale Cross-Entropy  |	 cMvMSEn
+        
+        
         _________________________________________________________________________
         Multivariate Multiscale Entropies                     |	Function Name
         ______________________________________________________|__________________
         Multivariate Multiscale Sample Entropy                |	
         Multivariate Multiscale Fuzzy Entropy                 |	MSobject
         Multivariate Multiscale Dispersion Entropy            |	    +
         Multivariate Multiscale Permutation Entropy           |	MvMSEn / cMvMSEn
         Multivariate Multiscale Cosine Similarity Entropy     |	
         
         
+        _________________________________________________________________________
+        Other  Functions                                      |	Function Name
+        ______________________________________________________|__________________
+        Example Dataset Import Tool                           |	 ExampleData
+        Data Windowing Tool                                   |	 WindowData
+        
+        
         
         This package is open for use by all in accordance with the terms of the 
         attached License agreement. Any scientific outputs obtained using 
         EntropyHub are required to include the following citation:
         
           Matthew W. Flood, 
           "EntropyHub: An open-source toolkit for entropic time series analysis",
```

### Comparing `EntropyHub-1.0.1/EntropyHub/_cMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_cMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_cXMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_cXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_hMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_hMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_hXMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_hXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_rMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_rMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub/_rXMSEn.py` & `EntropyHub-1.0.1.post1/EntropyHub/_rXMSEn.py`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/EntropyHub.egg-info/PKG-INFO` & `EntropyHub-1.0.1.post1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: EntropyHub
-Version: 1.0.1
-Summary: An open-source toolkit for entropic time series analysis.
-Home-page: https://www.EntropyHub.xyz
-Author: Matthew W. Flood
-Author-email: info@entropyhub.xyz, help@entropyhub.xyz
-License: Apache 2.0
-Project-URL: Contact, https://www.entropyhub.xyz/#contact
-Project-URL: Examples, https://www.entropyhub.xyz/python/pyexamples.html
-Project-URL: Collaboration, https://github.com/MattWillFlood/EntropyHub
-Project-URL: Citation, https://doi.org/10.1371/journal.pone.0259448
-Project-URL: Bug Reports, https://github.com/MattWillFlood/EntropyHub/issues
-Project-URL: Source, https://www.EntropyHub.xyz
-Project-URL: Documentation, https://github.com/MattWillFlood/EntropyHub/blob/main/EntropyHub%20Guide.pdf
-Keywords: entropy,nonlinear,time series,statistics,physics,mathematics,signal processing,statistical physics,entropic,toolkit,research,multiscale,regularity,periodic,sample entropy,approximate entropy,fuzzy entropy,permutation entropy,uncertainty,dispersion entropy,kolmogorov,conditional entropy,composite,refined,randomness,random,signal analysis,nonlinearity,julia,matlab,open-source,refined-composite,hierarchical entropy,information theory,shannon entropy,complexity
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # EntropyHub: An open-source toolkit for entropic data analysis
 
 __*Python Edition*__
 
 ![EntropyHub](https://raw.githubusercontent.com/MattWillFlood/EntropyHub/main/Graphics/EntropyHubLogo3.png)
 
 ## Installation
@@ -68,21 +36,25 @@
 which will print the docstrings.
 
 All information on the EntropyHub package is detailed in the *EntropyHub Guide*, a .pdf document available [here](https://github.com/MattWillFlood/EntropyHub/blob/main/EntropyHub%20Guide.pdf).
   
 	
 ## Functions
 
-EntropyHub functions fall into 5 categories: 
+EntropyHub functions fall into 8 categories: 
+
+    * Base                       functions for estimating the entropy of a single univariate time series.
+    * Cross                      functions for estimating the entropy between two univariate time series.
+    * Multivariate               functions for estimating the entropy of a multivariate dataset.
+    * Bidimensional              functions for estimating the entropy of a two-dimensional univariate matrix.
+    * Multiscale                 functions for estimating the multiscale entropy of a single univariate time series using any of the Base entropy functions.
+    * Multiscale Cross           functions for estimating the multiscale entropy between two univariate time series using any of the Cross-entropy functions.
+    * Multivariate Multiscale    functions for estimating the multivariate multiscale entropy of multivariate dataset using any of the Multivariate-entropy functions.
+    * Other                      Supplementary functions for various tasks related to EntropyHub and signal processing.
 
-    * Base                functions for estimating the entropy of a single univariate time series.
-    * Cross               functions for estimating the entropy between two univariate time series.
-    * Bidimensional       functions for estimating the entropy of a two-dimensional univariate matrix.
-    * Multiscale          functions for estimating the multiscale entropy of a single univariate time series using any of the Base entropy functions.
-    * Multiscale Cross    functions for estimating the multiscale entropy between two univariate time series using any of the Cross-entropy functions.
 
 #### The following tables outline the functions available in the EntropyHub package.
 
 *When new entropies are published in the scientific literature, efforts will
 be made to incorporate them in future releases.*
 
 ### Base Entropies:
@@ -123,14 +95,27 @@
 Cross Conditional Entropy                             |	XCondEn
 Cross Distribution Entropy                            |	XDistEn
 Cross Spectral Entropy                          	  |	XSpecEn
 Cross Kolmogorov Entropy                              |	XK2En
 	
 _______________________________________________________________________
 
+
+### Multivariate Entropies:
+
+Entropy Type   |  Function Name 
+--|--
+Multivariate Sample Entropy                                  |	MvSampEn
+Multivariate Fuzzy Entropy                                   |	MvFuzzEn
+Multivariate Permutation Entropy                             |	MvPermEn
+Multivariate Dispersion Entropy                              |	MvDispEn
+Multivariate Cosine Similarity Entropy                       |	MvCoSiEn
+
+_______________________________________________________________________
+
 ### Bidimensional Entropies
 
 Entropy Type   |  Function Name 
 ---|---
 Bidimensional Sample Entropy                         |	SampEn2D
 Bidimensional Fuzzy Entropy                          |	FuzzEn2D
 Bidimensional Distribution Entropy                   |	DistEn2D
@@ -155,14 +140,33 @@
 Entropy Type   |  Function Name 
 ---|---
 Multiscale Cross-Entropy                              |   XMSEn
 Composite/Refined-Composite Multiscale Cross-Entropy  |   cXMSEn
 Refined Multiscale Cross-Entropy                      |   rXMSEn
 Hierarchical Multiscale Cross-Entropy                 |   hXMSEn
 
+_________________________________________________________________________
+
+### Multivariate Multiscale Entropy Functions
+
+Entropy Type   |  Function Name 
+--|--
+Multivariate Multiscale Entropy                                    | MvMSEn
+Composite/Refined-Composite Multivariate Multiscale Entropy        | cMvMSEn
+
+_________________________________________________________________________
+
+### Other Functions
+
+Entropy Type   |  Function Name 
+--|--
+Example Data Import Tool            |  ExampleData
+Window Data Tool                    |  WindowData
+Multiscale Entropy Object           |  MSobject
+
 
 
 ## License and Terms of Use
 EntropyHub is licensed under the Apache License (Version 2.0) and is free to
 use by all on condition that the following reference be included on any outputs
 realized using the software:
  
@@ -204,8 +208,8 @@
 
 __Thank you__ for using EntropyHub.
 
 Matt
 
 
 ![EntropyHub Git](https://raw.githubusercontent.com/MattWillFlood/EntropyHub/main/Graphics/EntropyHubLogo3.png)
-        
+
```

### Comparing `EntropyHub-1.0.1/EntropyHub.egg-info/SOURCES.txt` & `EntropyHub-1.0.1.post1/EntropyHub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/LICENSE.txt` & `EntropyHub-1.0.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EntropyHub-1.0.1/PKG-INFO` & `EntropyHub-1.0.1.post1/EntropyHub.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: EntropyHub
-Version: 1.0.1
+Version: 1.0.1.post1
 Summary: An open-source toolkit for entropic time series analysis.
 Home-page: https://www.EntropyHub.xyz
 Author: Matthew W. Flood
 Author-email: info@entropyhub.xyz, help@entropyhub.xyz
 License: Apache 2.0
 Project-URL: Contact, https://www.entropyhub.xyz/#contact
 Project-URL: Examples, https://www.entropyhub.xyz/python/pyexamples.html
 Project-URL: Collaboration, https://github.com/MattWillFlood/EntropyHub
 Project-URL: Citation, https://doi.org/10.1371/journal.pone.0259448
 Project-URL: Bug Reports, https://github.com/MattWillFlood/EntropyHub/issues
 Project-URL: Source, https://www.EntropyHub.xyz
 Project-URL: Documentation, https://github.com/MattWillFlood/EntropyHub/blob/main/EntropyHub%20Guide.pdf
-Keywords: entropy,nonlinear,time series,statistics,physics,mathematics,signal processing,statistical physics,entropic,toolkit,research,multiscale,regularity,periodic,sample entropy,approximate entropy,fuzzy entropy,permutation entropy,uncertainty,dispersion entropy,kolmogorov,conditional entropy,composite,refined,randomness,random,signal analysis,nonlinearity,julia,matlab,open-source,refined-composite,hierarchical entropy,information theory,shannon entropy,complexity
+Keywords: entropy,nonlinear,time series,statistics,physics,mathematics,signal processing,statistical physics,entropic,toolkit,research,multiscale,regularity,periodic,sample entropy,approximate entropy,fuzzy entropy,permutation entropy,uncertainty,dispersion entropy,kolmogorov,conditional entropy,composite,refined,multivariaterandomness,random,signal analysis,nonlinearity,julia,matlab,open-source,refined-composite,hierarchical entropy,information theory,shannon entropy,complexity
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -68,21 +68,25 @@
 which will print the docstrings.
 
 All information on the EntropyHub package is detailed in the *EntropyHub Guide*, a .pdf document available [here](https://github.com/MattWillFlood/EntropyHub/blob/main/EntropyHub%20Guide.pdf).
   
 	
 ## Functions
 
-EntropyHub functions fall into 5 categories: 
+EntropyHub functions fall into 8 categories: 
+
+    * Base                       functions for estimating the entropy of a single univariate time series.
+    * Cross                      functions for estimating the entropy between two univariate time series.
+    * Multivariate               functions for estimating the entropy of a multivariate dataset.
+    * Bidimensional              functions for estimating the entropy of a two-dimensional univariate matrix.
+    * Multiscale                 functions for estimating the multiscale entropy of a single univariate time series using any of the Base entropy functions.
+    * Multiscale Cross           functions for estimating the multiscale entropy between two univariate time series using any of the Cross-entropy functions.
+    * Multivariate Multiscale    functions for estimating the multivariate multiscale entropy of multivariate dataset using any of the Multivariate-entropy functions.
+    * Other                      Supplementary functions for various tasks related to EntropyHub and signal processing.
 
-    * Base                functions for estimating the entropy of a single univariate time series.
-    * Cross               functions for estimating the entropy between two univariate time series.
-    * Bidimensional       functions for estimating the entropy of a two-dimensional univariate matrix.
-    * Multiscale          functions for estimating the multiscale entropy of a single univariate time series using any of the Base entropy functions.
-    * Multiscale Cross    functions for estimating the multiscale entropy between two univariate time series using any of the Cross-entropy functions.
 
 #### The following tables outline the functions available in the EntropyHub package.
 
 *When new entropies are published in the scientific literature, efforts will
 be made to incorporate them in future releases.*
 
 ### Base Entropies:
@@ -123,14 +127,27 @@
 Cross Conditional Entropy                             |	XCondEn
 Cross Distribution Entropy                            |	XDistEn
 Cross Spectral Entropy                          	  |	XSpecEn
 Cross Kolmogorov Entropy                              |	XK2En
 	
 _______________________________________________________________________
 
+
+### Multivariate Entropies:
+
+Entropy Type   |  Function Name 
+--|--
+Multivariate Sample Entropy                                  |	MvSampEn
+Multivariate Fuzzy Entropy                                   |	MvFuzzEn
+Multivariate Permutation Entropy                             |	MvPermEn
+Multivariate Dispersion Entropy                              |	MvDispEn
+Multivariate Cosine Similarity Entropy                       |	MvCoSiEn
+
+_______________________________________________________________________
+
 ### Bidimensional Entropies
 
 Entropy Type   |  Function Name 
 ---|---
 Bidimensional Sample Entropy                         |	SampEn2D
 Bidimensional Fuzzy Entropy                          |	FuzzEn2D
 Bidimensional Distribution Entropy                   |	DistEn2D
@@ -155,14 +172,33 @@
 Entropy Type   |  Function Name 
 ---|---
 Multiscale Cross-Entropy                              |   XMSEn
 Composite/Refined-Composite Multiscale Cross-Entropy  |   cXMSEn
 Refined Multiscale Cross-Entropy                      |   rXMSEn
 Hierarchical Multiscale Cross-Entropy                 |   hXMSEn
 
+_________________________________________________________________________
+
+### Multivariate Multiscale Entropy Functions
+
+Entropy Type   |  Function Name 
+--|--
+Multivariate Multiscale Entropy                                    | MvMSEn
+Composite/Refined-Composite Multivariate Multiscale Entropy        | cMvMSEn
+
+_________________________________________________________________________
+
+### Other Functions
+
+Entropy Type   |  Function Name 
+--|--
+Example Data Import Tool            |  ExampleData
+Window Data Tool                    |  WindowData
+Multiscale Entropy Object           |  MSobject
+
 
 
 ## License and Terms of Use
 EntropyHub is licensed under the Apache License (Version 2.0) and is free to
 use by all on condition that the following reference be included on any outputs
 realized using the software:
```

### Comparing `EntropyHub-1.0.1/setup.py` & `EntropyHub-1.0.1.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """
 EntropyHub - An open source toolkit for entropic time series analysis
 
   EntropyHub functions belong to one of five main classes/categories:
-    Base Entropies             >>  e.g. Approximate Entropy (ApEn),
-                                        Sample Entropy (SampEn)
-    Cross Entropies            >>  e.g. Cross-Approximate Entropy (XApEn)
-                                        Cross-Sample Entropy (XSampEn)
-    Bidimensional Entropies    >>  e.g. Bidimensional Sample Entropy (SampEn2D)
-                                        Bidimensional Fuzzy Entropy (FuzzEn2D)
-    Multiscale Entropies       >>  e.g. Multiscale Sample Entropy (MSEn)
-                                        Refined Multiscale Sample Entropy (rMSEn)
-                                        Composite Multiscale Sample Entropy (cMSEn)
-    Multiscale Cross Entropies >>  e.g. Multiscale Cross-Sample Entropy (XMSEn)
-                                        Refined Multiscale Cross-Sample Entropy (rXMSEn)
+    Base Entropies                    >>  e.g. Approximate Entropy (ApEn),
+                                               Sample Entropy (SampEn)
+    Cross Entropies                   >>  e.g. Cross-Approximate Entropy (XApEn)
+                                               Cross-Sample Entropy (XSampEn)
+    Multivariate Entropies            >>  e.g. Multivariate Dispersion Entropy (MvDispEn)
+                                               Multivariate Fuzzy Entropy (MvFuzzEn)
+    Bidimensional Entropies           >>  e.g. Bidimensional Sample Entropy (SampEn2D)
+                                               Bidimensional Fuzzy Entropy (FuzzEn2D)
+    Multiscale Entropies              >>  e.g. Multiscale Sample Entropy (MSEn)
+                                               Refined Multiscale Sample Entropy (rMSEn)
+                                               Composite Multiscale Sample Entropy (cMSEn)
+    Multiscale Cross Entropies        >>  e.g. Multiscale Cross-Sample Entropy (XMSEn)
+                                               Refined Multiscale Cross-Sample Entropy (rXMSEn)
+    Multivariate Multiscale Entropies >>  e.g. Multivariate Multiscale Sample Entropy (MvMSEn)
+                                               Refined-composite Multivariate Multiscale Fuzzy Entropy (cMvMSEn)
 
 _________________________________________________________________________
 Base Entropies                                        |	Function Name	
 ______________________________________________________|__________________
 Approximate Entropy                               	  |	ApEn
 Sample Entropy                                		  |	SampEn
 Fuzzy Entropy                                 		  |	FuzzEn
@@ -47,14 +51,23 @@
 Cross Permutation Entropy                             |	XPermEn
 Cross Conditional Entropy                             |	XCondEn
 Cross Distribution Entropy                            |	XDistEn
 Cross Spectral Entropy                          	  |	XSpecEn
 Cross Kolmogorov Entropy                              |	XK2En
 	
 _________________________________________________________________________
+Multivariate Entropies                               |	Function Name
+_____________________________________________________|___________________
+Multivariate Sample Entropy                          |	MvSampEn
+Multivariate Fuzzy Entropy                           |	MvFuzzEn
+Multivariate Cosine Similarity Entropy               |	MvCoSiEn
+Multivariate Dispersion Entropy                      |	MvDispEn
+Multivariate Permutation Entropy                     |	MvPermEn
+
+_________________________________________________________________________
 Bidimensional Entropies                              |	Function Name
 _____________________________________________________|___________________
 Bidimensional Sample Entropy                         |	SampEn2D
 Bidimensional Fuzzy Entropy                          |	FuzzEn2D
 Bidimensional Distribution Entropy                   |	DistEn2D
 Bidimensional Dispersion Entropy                     |	DispEn2D
 Bidimensional Permutation Entropy                    |	PermEn2D
@@ -108,14 +121,24 @@
 Multiscale Cross-Approximate Entropy                  |	
 Multiscale Cross-Fuzzy Entropy                        |	MSobject
 Multiscale Cross-Permutation Entropy                  |	    +
 Multiscale Cross-Distribution Entropy                 |	XMSEn / cXMSEn
 Multiscale Cross-Kolmogorov Entropy                   | rXMSEn / hXMSEn
 Multiscale Cross-Conditional Entropy                  |	
 
+_________________________________________________________________________
+Multivariate Multiscale Entropies                     |	Function Name
+______________________________________________________|__________________
+Multivariate Multiscale Sample Entropy                |	
+Multivariate Multiscale Fuzzy Entropy                 |	MSobject
+Multivariate Multiscale Dispersion Entropy            |	    +
+Multivariate Multiscale Permutation Entropy           |	MvMSEn / cMvMSEn
+Multivariate Multiscale Cosine Similarity Entropy     |	
+
+
 
 We kindly ask that if you use EntropyHub in your research, to please 
 include the following citation with the appropriate version number,
 as well as original articles upon which functions are derived:
 
 Matthew W. Flood and Bernd Grimm (2021), 
 "EntropyHub - An open source toolkit for entropic time series analysis"
@@ -145,15 +168,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='EntropyHub',  # Required
-    version='1.0.1',  # Required
+    version='1.0.1.post1',  # Required
     description='An open-source toolkit for entropic time series analysis.',  # Optional
     long_description=long_desc,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
 
     url='https://www.EntropyHub.xyz',  # Optional
     author='Matthew W. Flood',  # Optional
     author_email='info@entropyhub.xyz, help@entropyhub.xyz',  # Optional
@@ -177,15 +200,15 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
     ],
 
     keywords=('entropy, nonlinear, time series, statistics, physics, mathematics, signal processing,'
                 'statistical physics, entropic, toolkit, research, multiscale, regularity, periodic,'
                 'sample entropy, approximate entropy, fuzzy entropy, permutation entropy, uncertainty,'
-                'dispersion entropy, kolmogorov, conditional entropy, composite, refined,'
+                'dispersion entropy, kolmogorov, conditional entropy, composite, refined, multivariate'
                 'randomness, random, signal analysis, nonlinearity, julia, matlab, open-source,'
                 'refined-composite, hierarchical entropy, information theory, shannon entropy, complexity'),  # Optional
 
     packages = find_packages("EntropyHub", exclude=["__pycache__",".spyproject"]),
     #packages = ['EntropyHub'], #find_packages(include ='EntropyHub*'),  # Required
     python_requires='>=3.6, <4',
     install_requires=['numpy', 'matplotlib', 'scipy', 'EMD-signal', 'requests'],  #'itertools', 'copy', #wheel?  Optional
```

