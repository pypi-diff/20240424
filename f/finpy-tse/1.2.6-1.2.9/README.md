# Comparing `tmp/finpy_tse-1.2.6.tar.gz` & `tmp/finpy_tse-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finpy_tse-1.2.6.tar", last modified: Sat May 27 20:07:51 2023, max compression
+gzip compressed data, was "finpy_tse-1.2.9.tar", last modified: Tue Apr 23 09:47:43 2024, max compression
```

## Comparing `finpy_tse-1.2.6.tar` & `finpy_tse-1.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/finpy_tse/
--rw-r--r--   0 runner    (1001) docker     (123)   182906 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/finpy_tse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/finpy_tse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:47:43.925435 finpy_tse-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-23 09:47:33.000000 finpy_tse-1.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-23 09:47:43.925435 finpy_tse-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11214 2024-04-23 09:47:33.000000 finpy_tse-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:47:43.921435 finpy_tse-1.2.9/finpy_tse/
+-rw-r--r--   0 runner    (1001) docker     (127)   183443 2024-04-23 09:47:33.000000 finpy_tse-1.2.9/finpy_tse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:47:43.925435 finpy_tse-1.2.9/finpy_tse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-04-23 09:47:43.000000 finpy_tse-1.2.9/finpy_tse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 09:47:43.000000 finpy_tse-1.2.9/finpy_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:47:43.000000 finpy_tse-1.2.9/finpy_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 09:47:43.000000 finpy_tse-1.2.9/finpy_tse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:47:43.000000 finpy_tse-1.2.9/finpy_tse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:47:43.925435 finpy_tse-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-23 09:47:33.000000 finpy_tse-1.2.9/setup.py
```

### Comparing `finpy_tse-1.2.6/LICENSE.txt` & `finpy_tse-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.6/PKG-INFO` & `finpy_tse-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 Metadata-Version: 2.1
 Name: finpy_tse
-Version: 1.2.6
+Version: 1.2.9
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: jdatetime
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: asyncio
+Requires-Dist: urllib3
+Requires-Dist: aiohttp
+Requires-Dist: unsync
+Requires-Dist: IPython
+Requires-Dist: persiantools
+Requires-Dist: datetime
+Requires-Dist: XlsxWriter
+Requires-Dist: lxml
 
 [![Downloads](https://static.pepy.tech/personalized-badge/finpy-tse?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/finpy-tse)
 
 <div dir="rtl" align="right">
 
 ##### این ماژول با هدف دسترسی به اطلاعات مربوط به سهام بورس ایران در محیط برنامه‌نویسی پایتون توسعه یافته است. بنابراین شما می‌توانید به راحتی به داده‌های مدنظر خود دسترسی داشته باشید و در توسعه مدل‌های تحلیلی خود از تحلیل تکنیکال گرفته تا تحلیل‌های عددی و یا مبتنی بر ماشین لرنینگ، استفاده کنید. این ماژول از جامعیت و انعطاف‌پذیری فوق‌العاده‌ای در دسترسی به دیتا و پیش‌پردازش آن برخوردار بوده و می‌تواند جایگزین رایگان و مناسبی برای یک اشتراک پولی، به منظور دسترسی به داده‌های بازار سهام باشد. داده‌های خروجی توابع این ماژول، دیتافریم پانداز بوده و شما می‌توانید از آن به عنوان ورودی سایر ماژول‌های آماده موجود از ماژول‌های مصورسازی گرفته تا ماژول‌های تحلیل تکنیکال، مدیریت پرتفوی و ... استفاده کنید
```

### Comparing `finpy_tse-1.2.6/README.md` & `finpy_tse-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.6/finpy_tse/__init__.py` & `finpy_tse-1.2.9/finpy_tse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1880,21 +1880,27 @@
                       'Low','High','Y-Final','EPS','Base-Vol','Sector','Day_UL','Day_LL','Share-No','Mkt-ID']]
     # Just keep: 300 Bourse, 303 Fara-Bourse, 305 Sandoogh, 309 Payeh, 400 H-Bourse, 403 H-FaraBourse, 404 H-Payeh
     Mkt_ID_list = ['300','303','305','309','400','403','404']
     Mkt_df = Mkt_df[Mkt_df['Mkt-ID'].isin(Mkt_ID_list)]
     Mkt_df['Market'] = Mkt_df['Mkt-ID'].map({'300':'بورس','303':'فرابورس','305':'صندوق قابل معامله','309':'پایه','400':'حق تقدم بورس','403':'حق تقدم فرابورس','404':'حق تقدم پایه'})
     Mkt_df.drop(columns=['Mkt-ID'],inplace=True)   # we do not need Mkt-ID column anymore
     # assign sector names:
-    r = requests.get('http://old.tsetmc.com/Loader.aspx?ParTree=111C1213', headers=headers)
-    sectro_lookup = (pd.read_html(r.text)[0]).iloc[1:,:]
-    # convert from Arabic to Farsi and remove half-space
-    sectro_lookup[1] = sectro_lookup[1].apply(lambda x: (str(x).replace('ي','ی')).replace('ك','ک'))
-    sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.replace('\u200c',' '))
-    sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.strip())
-    Mkt_df['Sector'] = Mkt_df['Sector'].map(dict(sectro_lookup[[0, 1]].values))
+    r = requests.get('https://cdn.tsetmc.com/api/StaticData/GetStaticData', headers=headers)
+    sec_df = pd.DataFrame(r.json()['staticData'])
+    sec_df['code'] = (sec_df['code'].astype(str).apply(lambda x: '0' + x if len(x) == 1 else x))
+    sec_df['name'] = (sec_df['name'].apply(lambda x: re.sub(r'\u200c', '', x)).str.strip().apply(characters.ar_to_fa))
+    sec_df = sec_df[sec_df['type'] == 'IndustrialGroup'][['code', 'name']]
+    Mkt_df['Sector'] = Mkt_df['Sector'].map(dict(sec_df[['code', 'name']].values))
+    # r = requests.get('http://old.tsetmc.com/Loader.aspx?ParTree=111C1213', headers=headers)
+    # sectro_lookup = (pd.read_html(r.text)[0]).iloc[1:,:]
+    # # convert from Arabic to Farsi and remove half-space
+    # sectro_lookup[1] = sectro_lookup[1].apply(lambda x: (str(x).replace('ي','ی')).replace('ك','ک'))
+    # sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.replace('\u200c',' '))
+    # sectro_lookup[1] = sectro_lookup[1].apply(lambda x: x.strip())
+    # Mkt_df['Sector'] = Mkt_df['Sector'].map(dict(sectro_lookup[[0, 1]].values))
     # modify format of columns:
     cols = ['Open','Final','Close','No','Volume','Value','Low','High','Y-Final','EPS','Base-Vol','Day_UL','Day_LL','Share-No']
     Mkt_df[cols] = Mkt_df[cols].apply(pd.to_numeric, axis=1)
     Mkt_df['Time'] = Mkt_df['Time'].apply(lambda x: x[:-4]+':'+x[-4:-2]+':'+x[-2:])
     Mkt_df['Ticker'] = Mkt_df['Ticker'].apply(lambda x: (str(x).replace('ي','ی')).replace('ك','ک'))
     Mkt_df['Name'] = Mkt_df['Name'].apply(lambda x: (str(x).replace('ي','ی')).replace('ك','ک'))
     Mkt_df['Name'] = Mkt_df['Name'].apply(lambda x: x.replace('\u200c',' '))
```

### Comparing `finpy_tse-1.2.6/finpy_tse.egg-info/PKG-INFO` & `finpy_tse-1.2.9/finpy_tse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,31 @@
 Metadata-Version: 2.1
-Name: finpy-tse
-Version: 1.2.6
+Name: finpy_tse
+Version: 1.2.9
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: jdatetime
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: bs4
+Requires-Dist: asyncio
+Requires-Dist: urllib3
+Requires-Dist: aiohttp
+Requires-Dist: unsync
+Requires-Dist: IPython
+Requires-Dist: persiantools
+Requires-Dist: datetime
+Requires-Dist: XlsxWriter
+Requires-Dist: lxml
 
 [![Downloads](https://static.pepy.tech/personalized-badge/finpy-tse?period=total&units=international_system&left_color=black&right_color=green&left_text=Downloads)](https://pepy.tech/project/finpy-tse)
 
 <div dir="rtl" align="right">
 
 ##### این ماژول با هدف دسترسی به اطلاعات مربوط به سهام بورس ایران در محیط برنامه‌نویسی پایتون توسعه یافته است. بنابراین شما می‌توانید به راحتی به داده‌های مدنظر خود دسترسی داشته باشید و در توسعه مدل‌های تحلیلی خود از تحلیل تکنیکال گرفته تا تحلیل‌های عددی و یا مبتنی بر ماشین لرنینگ، استفاده کنید. این ماژول از جامعیت و انعطاف‌پذیری فوق‌العاده‌ای در دسترسی به دیتا و پیش‌پردازش آن برخوردار بوده و می‌تواند جایگزین رایگان و مناسبی برای یک اشتراک پولی، به منظور دسترسی به داده‌های بازار سهام باشد. داده‌های خروجی توابع این ماژول، دیتافریم پانداز بوده و شما می‌توانید از آن به عنوان ورودی سایر ماژول‌های آماده موجود از ماژول‌های مصورسازی گرفته تا ماژول‌های تحلیل تکنیکال، مدیریت پرتفوی و ... استفاده کنید
```

### Comparing `finpy_tse-1.2.6/setup.py` & `finpy_tse-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='finpy_tse',                           # should match the package folder
     packages=['finpy_tse'],                     # should match the package folder
-    version='1.2.6',                            # important for updates
+    version='1.2.9',                            # important for updates
     license='BSD (3-clause)',                                  # should match your chosen license
     description='A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='ALI RAHIMI  AND  RASOOL GHAFOURI',
     author_email='a.rahimi.aut@gmail.com',
     install_requires=['requests','jdatetime','pandas','numpy','requests','bs4','asyncio','urllib3','aiohttp','unsync','IPython','persiantools','datetime','XlsxWriter','lxml'],                  # list all packages that your package uses
```

