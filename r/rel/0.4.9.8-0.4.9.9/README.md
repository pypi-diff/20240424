# Comparing `tmp/rel-0.4.9.8-py3-none-any.whl.zip` & `tmp/rel-0.4.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 13624 bytes, number of entries: 14
--rw-r--r--  2.0 unx      304 b- defN 24-Mar-07 00:18 rel/__init__.py
+Zip file size: 13953 bytes, number of entries: 14
+-rw-r--r--  2.0 unx      304 b- defN 24-Mar-23 21:12 rel/__init__.py
 -rw-r--r--  2.0 unx       35 b- defN 23-Jul-26 21:30 rel/errors.py
 -rw-r--r--  2.0 unx     5986 b- defN 23-Jul-26 21:30 rel/listener.py
 -rw-r--r--  2.0 unx    10350 b- defN 23-Dec-28 05:37 rel/registrar.py
 -rw-r--r--  2.0 unx     7573 b- defN 23-Dec-28 03:05 rel/rel.py
 -rw-r--r--  2.0 unx     6178 b- defN 24-Jan-29 04:21 rel/test.py
--rw-r--r--  2.0 unx     4847 b- defN 24-Feb-29 23:54 rel/tools.py
+-rw-r--r--  2.0 unx     5895 b- defN 24-Mar-23 20:30 rel/tools.py
 -rw-r--r--  2.0 unx     1643 b- defN 24-Mar-01 05:59 rel/util.py
--rw-r--r--  2.0 unx       24 b- defN 24-Mar-07 00:18 rel/version.py
--rw-r--r--  2.0 unx      805 b- defN 24-Mar-07 00:18 rel-0.4.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-07 00:18 rel-0.4.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-07 00:18 rel-0.4.9.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-07 00:18 rel-0.4.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1007 b- defN 24-Mar-07 00:18 rel-0.4.9.8.dist-info/RECORD
-14 files, 38894 bytes uncompressed, 11988 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx       24 b- defN 24-Mar-23 21:12 rel/version.py
+-rw-r--r--  2.0 unx     1030 b- defN 24-Mar-23 21:13 rel-0.4.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-23 21:13 rel-0.4.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-Mar-23 21:13 rel-0.4.9.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Mar-23 21:13 rel-0.4.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1008 b- defN 24-Mar-23 21:13 rel-0.4.9.9.dist-info/RECORD
+14 files, 40168 bytes uncompressed, 12317 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: rel/util.py
 Comment: 
 
 Filename: rel/version.py
 Comment: 
 
-Filename: rel-0.4.9.8.dist-info/METADATA
+Filename: rel-0.4.9.9.dist-info/METADATA
 Comment: 
 
-Filename: rel-0.4.9.8.dist-info/WHEEL
+Filename: rel-0.4.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: rel-0.4.9.8.dist-info/entry_points.txt
+Filename: rel-0.4.9.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: rel-0.4.9.8.dist-info/top_level.txt
+Filename: rel-0.4.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: rel-0.4.9.8.dist-info/RECORD
+Filename: rel-0.4.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rel/tools.py

```diff
@@ -34,17 +34,21 @@
 means run for 15 seconds, 30 minutes, and 2 hours, printing
 a notice every 60 seconds.
 
     rtimer 0 5
 
 means run for 5 minutes, printing no incremental updates.
 
+The -s, -m, -r, and -i flags may also be used to indicate
+seconds, minutes, hours, and increment, and if any flag is
+specified, update_increment defaults to 1 (instead of 0).
+
 When the time runs out, a sound will play on two conditions:
 there is a readable file at the specified path (configurable
-via the -m flag, with default: ~/.rtimer/),
+via the -p flag, with default: ~/.rtimer/),
 and mplayer is installed.
 """
 
 import rel, os, random
 try:
     from subprocess import getoutput # py3
 except:
@@ -69,15 +73,15 @@
     exit()
 
 ### the tools themselves
 
 # rtimer
 
 RT_MEDIA = os.path.join(os.path.expanduser("~"), ".rtimer")
-RT_USAGE = 'rtimer [seconds] [minutes] [hours] [update_increment]\n--\nall arguments default to zero. so, rtimer 15 30 2 60 means run for 15 seconds, 30 minutes, and 2 hours, printing a notice every 60 seconds. rtimer 0 5 means run for 5 minutes, printing no incremental updates. when the time runs out, a sound will play on two conditions: there is a readable file at the specified path (default: %s), and mplayer is installed.'%(RT_MEDIA,)
+RT_USAGE = 'rtimer [seconds] [minutes] [hours] [update_increment]\n--\nall arguments default to zero. so, rtimer 15 30 2 60 means run for 15 seconds, 30 minutes, and 2 hours, printing a notice every 60 seconds. rtimer 0 5 means run for 5 minutes, printing no incremental updates. the -s, -m, -r, and -i flags may also be used to indicate seconds, minutes, hours, and increment, and if any flag is specified, update_increment defaults to 1 (instead of 0). when the time runs out, a sound will play on two conditions: there is a readable file at the specified path (default: %s), and mplayer is installed.'%(RT_MEDIA,)
 
 class Timer(object):
     def __init__(self, s, m, h, interval=0, mediapath=RT_MEDIA):
         try:
             s, m, h, self.interval = int(s), int(m), int(h), int(interval)
         except:
             error("invalid input", "seconds, minutes, hours, and interval must all be integers")
@@ -130,20 +134,29 @@
 ### functions for interpreting command-line instructions
 
 # rtimer
 
 def timerCLI():
     from optparse import OptionParser
     parser = OptionParser(RT_USAGE)
-    parser.add_option("-m", "--media_path", dest="media", default=RT_MEDIA, help="location of alarm media (audio/video) directory. default: %s"%(RT_MEDIA,))
+    parser.add_option("-r", "--hours", dest="hours", default=0, help="hours. default: 0")
+    parser.add_option("-m", "--minutes", dest="minutes", default=0, help="minutes. default: 0")
+    parser.add_option("-s", "--seconds", dest="seconds", default=0, help="seconds. default: 0")
+    parser.add_option("-i", "--increment", dest="increment", default=1, help="increment. default: 1")
+    parser.add_option("-p", "--path", dest="path", default=RT_MEDIA, help="location of alarm media (audio/video) directory. default: %s"%(RT_MEDIA,))
     parser.add_option("-v", "--verbose", dest="verbose", default=False, action="store_true", help="run timer in verbose mode")
     options, arguments = parser.parse_args()
     if options.verbose:
         rel.initialize(options=["verbose"])
     try:
         arguments = [int(arg) for arg in arguments]
     except:
         error("non-integer argument", "USAGE: %s"%(RT_USAGE,))
     while len(arguments) < 4:
         arguments.append(0)
-    arguments.append(options.media)
+    if options.seconds or options.minutes or options.hours or options.increment:
+        arguments[0] = arguments[0] or int(options.seconds)
+        arguments[1] = arguments[1] or int(options.minutes)
+        arguments[2] = arguments[2] or int(options.hours)
+        arguments[3] = arguments[3] or int(options.increment)
+    arguments.append(options.path)
     Timer(*arguments).start()
```

## rel/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.4.9.8"
+__version__ = "0.4.9.9"
```

## Comparing `rel-0.4.9.8.dist-info/RECORD` & `rel-0.4.9.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 rel/__init__.py,sha256=imo6mXTwYjOAM2Oh4p1NyvYdeOxGmf17ibtmFOLy2n4,304
 rel/errors.py,sha256=bm4gn6h_-7Uc-OPi6-2Cumpi3rlRrQnoDJLZqH-dbVg,35
 rel/listener.py,sha256=V0100lpU6ACZ75yBEiaU2tsefzqKt55J0GWkUUS90JQ,5986
 rel/registrar.py,sha256=EHOMKnw9Nz-3Yqh9Hx0KTxJibiAPD5DRIsYsb7ZlEFo,10350
 rel/rel.py,sha256=-lEYiokkjq3d4jejlpQR1uCOrBCOAnvCiPNq6iMxaD0,7573
 rel/test.py,sha256=L6qvgdJ2a1clZtRbXTzZxFSe8oj9ITfnVJfcz_QTOR4,6178
-rel/tools.py,sha256=kseqm7tjLh3t6m8veX5VO4GIDiwiXIHhQYko4_AeXho,4847
+rel/tools.py,sha256=y0y4qsdRkBSgI4TnIXFsgldCnZq7wrqLR7BBUvjCsdw,5895
 rel/util.py,sha256=TmjhJV6j9FcPNm2h1HaS-1X2LIRyiR3iXIsO06kdPAg,1643
-rel/version.py,sha256=caX1HNqgCdF-1DxNxeqfw2VgVtOn83GUNhmugz6WASk,24
-rel-0.4.9.8.dist-info/METADATA,sha256=MEJZ6f83K-lkY2liJ07kTUAJmUT20Un27PjJ3ZHJB9E,805
-rel-0.4.9.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-rel-0.4.9.8.dist-info/entry_points.txt,sha256=uwtYDZu73cZRTs5NJHEG-ROuyz6vPXduMS19hJc4zT8,46
-rel-0.4.9.8.dist-info/top_level.txt,sha256=h3cwul_Qg5WBxhC7CRNPKczsdyAYE-aG3-LFvM_OM68,4
-rel-0.4.9.8.dist-info/RECORD,,
+rel/version.py,sha256=BGVpVefgzGfhTb2wZQHNO78_hVx5kcjbAjGlDHwBHOM,24
+rel-0.4.9.9.dist-info/METADATA,sha256=Qo0xWnHuTcAiWj05XgHrrBaMQSO-EXvMZFL8N-YzkWg,1030
+rel-0.4.9.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+rel-0.4.9.9.dist-info/entry_points.txt,sha256=uwtYDZu73cZRTs5NJHEG-ROuyz6vPXduMS19hJc4zT8,46
+rel-0.4.9.9.dist-info/top_level.txt,sha256=h3cwul_Qg5WBxhC7CRNPKczsdyAYE-aG3-LFvM_OM68,4
+rel-0.4.9.9.dist-info/RECORD,,
```

