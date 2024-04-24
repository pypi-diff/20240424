# Comparing `tmp/cyclomonitor-2024.4.19.tar.gz` & `tmp/cyclomonitor-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclomonitor-2024.4.19.tar", last modified: Fri Apr 19 01:30:52 2024, max compression
+gzip compressed data, was "cyclomonitor-2024.4.24.tar", last modified: Wed Apr 24 12:05:34 2024, max compression
```

## Comparing `cyclomonitor-2024.4.19.tar` & `cyclomonitor-2024.4.24.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/LICENSE
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.4.19/MANIFEST.in
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43192 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/PKG-INFO
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1908 2024-04-19 01:01:12.000000 cyclomonitor-2024.4.19/README.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/privacy-policy.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1519 2024-04-15 01:29:25.000000 cyclomonitor-2024.4.19/pyproject.toml
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       28 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/requirements.txt
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-04-19 01:30:52.484628 cyclomonitor-2024.4.19/setup.cfg
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1828 2024-04-19 00:44:11.000000 cyclomonitor-2024.4.19/setup.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.476628 cyclomonitor-2024.4.19/src/
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.4.19/src/cyclomonitor/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    39238 2024-04-19 01:27:30.000000 cyclomonitor-2024.4.19/src/cyclomonitor/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10557 2024-04-14 12:51:51.000000 cyclomonitor-2024.4.19/src/cyclomonitor/atcf.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/src/cyclomonitor/dir_calc.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.19/src/cyclomonitor/errors.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/global_vars.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12661 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5062 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5070 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/en_US.json
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     7200 2024-04-15 01:00:35.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12395 2024-04-15 01:00:29.000000 cyclomonitor-2024.4.19/src/cyclomonitor/locales/en_US.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/server_vars.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.19/src/cyclomonitor/uptime.py
-drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-19 01:30:52.480628 cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      710 2024-04-19 01:30:52.000000 cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/SOURCES.txt
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.181500 cyclomonitor-2024.4.24/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.24/LICENSE
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.4.24/MANIFEST.in
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43244 2024-04-24 12:05:34.181500 cyclomonitor-2024.4.24/PKG-INFO
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1908 2024-04-19 01:01:12.000000 cyclomonitor-2024.4.24/README.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.24/privacy-policy.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1561 2024-04-24 11:52:30.000000 cyclomonitor-2024.4.24/pyproject.toml
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       28 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/requirements.txt
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-04-24 12:05:34.181500 cyclomonitor-2024.4.24/setup.cfg
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1828 2024-04-24 12:04:38.000000 cyclomonitor-2024.4.24/setup.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.173500 cyclomonitor-2024.4.24/src/
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.177500 cyclomonitor-2024.4.24/src/cyclomonitor/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.4.24/src/cyclomonitor/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    39510 2024-04-24 12:02:06.000000 cyclomonitor-2024.4.24/src/cyclomonitor/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10557 2024-04-14 12:51:51.000000 cyclomonitor-2024.4.24/src/cyclomonitor/atcf.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.24/src/cyclomonitor/dir_calc.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.4.24/src/cyclomonitor/errors.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/global_vars.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.177500 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12661 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5062 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5070 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.177500 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/en_US.json
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.177500 cyclomonitor-2024.4.24/src/cyclomonitor/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12456 2024-04-24 11:54:02.000000 cyclomonitor-2024.4.24/src/cyclomonitor/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     7224 2024-04-24 11:54:25.000000 cyclomonitor-2024.4.24/src/cyclomonitor/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    12456 2024-04-24 11:54:02.000000 cyclomonitor-2024.4.24/src/cyclomonitor/locales/en_US.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/server_vars.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.4.24/src/cyclomonitor/uptime.py
+drwxr-xr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-04-24 12:05:34.177500 cyclomonitor-2024.4.24/src/cyclomonitor.egg-info/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      710 2024-04-24 12:05:34.000000 cyclomonitor-2024.4.24/src/cyclomonitor.egg-info/SOURCES.txt
```

### Comparing `cyclomonitor-2024.4.19/LICENSE` & `cyclomonitor-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/PKG-INFO` & `cyclomonitor-2024.4.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclomonitor
-Version: 2024.4.19
+Version: 2024.4.24
 Summary: Discord bot that helps you keep tabs on tropical cyclones.
 Home-page: https://github.com/ntvmb/cyclomonitor
 Author: Nathaniel Greenwell
 Author-email: Nathaniel Greenwell <nategreenwell@live.com>
 Maintainer-email: Nathaniel Greenwell <nategreenwell@live.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -667,14 +667,15 @@
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Project-URL: Repository, https://github.com/ntvmb/cyclomonitor.git
 Project-URL: Issues, https://github.com/ntvmb/cyclomonitor/issues
 Project-URL: Changelog, https://github.com/ntvmb/cyclomonitor/blob/master/CHANGELOG.md
+Project-URL: Discord, https://discord.gg/xBHESnJYz5
 Keywords: weather,discord,discord bot,discord-py,typhoon,hurricane,tropical cyclone,atcf,py-cord,ibtracs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cyclomonitor-2024.4.19/README.md` & `cyclomonitor-2024.4.24/README.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/privacy-policy.md` & `cyclomonitor-2024.4.24/privacy-policy.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/pyproject.toml` & `cyclomonitor-2024.4.24/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,8 @@
 [project.optional-dependencies]
 single-instance = ["tendo"]
 
 [project.urls]
 Repository = "https://github.com/ntvmb/cyclomonitor.git"
 Issues = "https://github.com/ntvmb/cyclomonitor/issues"
 Changelog = "https://github.com/ntvmb/cyclomonitor/blob/master/CHANGELOG.md"
+Discord = "https://discord.gg/xBHESnJYz5"
```

### Comparing `cyclomonitor-2024.4.19/setup.py` & `cyclomonitor-2024.4.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "2024.4.19"
+__version__ = "2024.4.24"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
```

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/__main__.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 GNU Affero General Public License along with this program. If not, see
 <https://www.gnu.org/licenses/>.
 """
 logname = "bot.log"
 # PLEASE CHANGE THESE LINKS IF YOU ARE FORKING THIS PROJECT.
 INVITE = "https://discord.com/api/oauth2/authorize?client_id={0}&permissions=67496000&scope=bot"
 GITHUB = "GITHUB_LINK"
+SERVER = "SERVER_INVITE"
 languages = ["C", "en_US"]
 emojis = {}
 
 # increase compatibility with python<3.11
 if not hasattr(datetime, "UTC"):
     datetime.UTC = datetime.timezone.utc
 
@@ -974,19 +975,24 @@
                 )
             )
         else:
             with open(f"forecast.{ext}", "rb") as f:
                 await ctx.respond(file=discord.File(f))
 
 
+@bot.slash_command(name="server", description=CM_SERVER)
+async def server(ctx: discord.ApplicationContext):
+    await ctx.respond(SERVER, ephemeral=True)
+
+
 def main():
     import argparse
     import json
 
-    global GITHUB, INVITE
+    global GITHUB, INVITE, SERVER
     locale_init()
     parser = argparse.ArgumentParser(
         prog="cyclomonitor",
         description=DESCRIPTION,
         epilog=HELP_EPILOG.format(GITHUB),
     )
     parser.add_argument("-b", "--bot", help=HELP_BOT, action="store_true")
@@ -1028,14 +1034,16 @@
             log_params["filename"] = config["log_file"]
             log_params["filemode"] = "a"
             logging.captureWarnings(True)
         if config.get("github") is not None:
             GITHUB = config["github"]
         if config.get("client_id") is not None:
             INVITE = INVITE.format(config["client_id"])
+        if config.get("server") is not None:
+            SERVER = config["server"]
         if isinstance(config.get("emojis"), dict):
             emojis.update(config["emojis"])
     if args.verbose:
         log_params["level"] = logging.DEBUG
     else:
         log_params["level"] = logging.INFO
     logging.basicConfig(
```

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/atcf.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/atcf.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/dir_calc.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/dir_calc.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/global_vars.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/global_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/__init__.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_ALL.sql` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/ibtracs_ALL.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/C.json` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/__init__.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/ibtracs/locales/en_US.json` & `cyclomonitor-2024.4.24/src/cyclomonitor/ibtracs/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/locales/C.json` & `cyclomonitor-2024.4.24/src/cyclomonitor/locales/C.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939759036144579%*

 * *Differences: {"'CM_SERVER'": '"Join the bot\'s official Discord server!"'}*

```diff
@@ -81,14 +81,15 @@
     "CM_PING": "Test the response time",
     "CM_PONG": "Pong! {0} ms",
     "CM_RESUME_UPDATES": "Resume automatic updates.",
     "CM_RESUME_UPDATES_SUCCESS": "Resumed automatic updates.",
     "CM_RSMC_LIST": "A list of links Regional Specialized Meteorological Center (RSMC) websites.",
     "CM_RSMC_LIST_RESPONSE": "# RSMC list\nAtlantic (NATL) and Eastern Pacific (EPAC) - National Hurricane Center (NHC, RSMC Miami): <https://www.nhc.noaa.gov/> (Active May 15th through November 30th)\nCentral Pacific (CPAC) - Central Pacific Hurricane Center (CPHC, RSMC Honolulu): <https://www.nhc.noaa.gov/?cpac> (Active June 1st through November 30th)\nWestern Pacific (WPAC) - Japan Meteorological Agency (JMA, RSMC Tokyo): <https://www.jma.go.jp/bosai/map.html#contents=typhoon&lang=en>\nNorth Indian Ocean (NIO) - India Meteorological Department (IMD, RSMC New Delhi): <https://mausam.imd.gov.in/responsive/cycloneinformation.php>\nSouthwest Indian Ocean (SWIO) - Meteo France La R\u00e9union (MFR, RSMC La R\u00e9union): <https://meteofrance.re/fr/cyclone>\nAustralia Region (AUS) - Bureau of Meteorology (BOM, RSMC Melbourne): <http://www.bom.gov.au/cyclone> (Active November 1st through April 30th)\nSouth Pacific (SPAC) - Fiji Meteorological Service (FMS, RSMC Nadi): <https://www.met.gov.fj> (Active November 1st through April 30th)\n## Some other tropical cyclone warning centers (TCWC)\nJoint Typhoon Warning Center (JTWC): <https://www.metoc.navy.mil/jtwc/jtwc.html>\nPhilippine Atmospheric, Geophysical and Astronomical Services Administration (PAGASA): <https://bagong.pagasa.dost.gov.ph/>",
     "CM_SEARCHING": "Searching...",
+    "CM_SERVER": "Join the bot's official Discord server!",
     "CM_SET_BASINS": "Set basins to track",
     "CM_SET_CHANNEL_SUCCESS": "Successfully set the tracking channel to {0}!",
     "CM_SET_LANGUAGE": "Set the language for this server.",
     "CM_SET_LANGUAGE_SUCCESS": "Set the language to {0}.",
     "CM_SET_TRACKING_CHANNEL": "Set the tracking channel",
     "CM_SHEM": "Southern hemisphere",
     "CM_STATISTICS": "# CycloMonitor statistics\nCurrently serving {0} guilds.\nStrongest cyclone recorded by this bot: {1[0]} {1[1]} {1[2]} ({1[3]})\n- Wind peak: {1[5]} kt ({1[6]} mph/{1[7]} kph)\n- Pressure peak: {1[8]} mb\n- Time recorded: <t:{1[4]}:f>\nCurrent yikes counter: {2}\nBot uptime: {3}",
```

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/locales/__init__.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/locales/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 HELP_TOKEN = "HELP_TOKEN"
 HELP_INTERACTIVE = "HELP_INTERACTIVE"
 HELP_LOG_FILE = "HELP_LOG_FILE"
 HELP_VERBOSE = "HELP_VERBOSE"
 HELP_CONFIG = "HELP_CONFIG"
 ERROR_BOT_AND_INTERACTIVE = "ERROR_BOT_AND_INTERACTIVE"
 ERROR_NO_TOKEN = "ERROR_NO_TOKEN"
+CM_SERVER = "CM_SERVER"
 
 _log = _logging.getLogger(__name__)
 locale.setlocale(locale.LC_ALL, "")
 _PATH = os.path.dirname(os.path.realpath(__file__))
 
 
 def set_locale(lang="C"):
```

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/locales/en_US.json` & `cyclomonitor-2024.4.24/src/cyclomonitor/locales/en_US.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939759036144579%*

 * *Differences: {"'CM_SERVER'": '"Join the bot\'s official Discord server!"'}*

```diff
@@ -81,14 +81,15 @@
     "CM_PING": "Test the response time",
     "CM_PONG": "Pong! {0} ms",
     "CM_RESUME_UPDATES": "Resume automatic updates.",
     "CM_RESUME_UPDATES_SUCCESS": "Resumed automatic updates.",
     "CM_RSMC_LIST": "A list of links Regional Specialized Meteorological Center (RSMC) websites.",
     "CM_RSMC_LIST_RESPONSE": "# RSMC list\nAtlantic (NATL) and Eastern Pacific (EPAC) - National Hurricane Center (NHC, RSMC Miami): <https://www.nhc.noaa.gov/> (Active May 15th through November 30th)\nCentral Pacific (CPAC) - Central Pacific Hurricane Center (CPHC, RSMC Honolulu): <https://www.nhc.noaa.gov/?cpac> (Active June 1st through November 30th)\nWestern Pacific (WPAC) - Japan Meteorological Agency (JMA, RSMC Tokyo): <https://www.jma.go.jp/bosai/map.html#contents=typhoon&lang=en>\nNorth Indian Ocean (NIO) - India Meteorological Department (IMD, RSMC New Delhi): <https://mausam.imd.gov.in/responsive/cycloneinformation.php>\nSouthwest Indian Ocean (SWIO) - Meteo France La R\u00e9union (MFR, RSMC La R\u00e9union): <https://meteofrance.re/fr/cyclone>\nAustralia Region (AUS) - Bureau of Meteorology (BOM, RSMC Melbourne): <http://www.bom.gov.au/cyclone> (Active November 1st through April 30th)\nSouth Pacific (SPAC) - Fiji Meteorological Service (FMS, RSMC Nadi): <https://www.met.gov.fj> (Active November 1st through April 30th)\n## Some other tropical cyclone warning centers (TCWC)\nJoint Typhoon Warning Center (JTWC): <https://www.metoc.navy.mil/jtwc/jtwc.html>\nPhilippine Atmospheric, Geophysical and Astronomical Services Administration (PAGASA): <https://bagong.pagasa.dost.gov.ph/>",
     "CM_SEARCHING": "Searching...",
+    "CM_SERVER": "Join the bot's official Discord server!",
     "CM_SET_BASINS": "Set basins to track",
     "CM_SET_CHANNEL_SUCCESS": "Successfully set the tracking channel to {0}!",
     "CM_SET_LANGUAGE": "Set the language for this server.",
     "CM_SET_LANGUAGE_SUCCESS": "Set the language to {0}.",
     "CM_SET_TRACKING_CHANNEL": "Set the tracking channel",
     "CM_SHEM": "Southern hemisphere",
     "CM_STATISTICS": "# CycloMonitor statistics\nCurrently serving {0} guilds.\nStrongest cyclone recorded by this bot: {1[0]} {1[1]} {1[2]} ({1[3]})\n- Wind peak: {1[5]} kt ({1[6]} mph/{1[7]} kph)\n- Pressure peak: {1[8]} mb\n- Time recorded: <t:{1[4]}:f>\nCurrent yikes counter: {2}\nBot uptime: {3}",
```

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/server_vars.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/server_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor/uptime.py` & `cyclomonitor-2024.4.24/src/cyclomonitor/uptime.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.4.19/src/cyclomonitor.egg-info/SOURCES.txt` & `cyclomonitor-2024.4.24/src/cyclomonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

