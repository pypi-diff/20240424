# Comparing `tmp/stonksfeed-0.1.6.tar.gz` & `tmp/stonksfeed-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stonksfeed-0.1.6.tar", max compression
+gzip compressed data, was "stonksfeed-0.1.7.tar", max compression
```

## Comparing `stonksfeed-0.1.6.tar` & `stonksfeed-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    35129 2024-01-12 01:56:57.158427 stonksfeed-0.1.6/LICENSE
--rw-r--r--   0        0        0       14 2024-01-21 20:38:44.542770 stonksfeed-0.1.6/README.md
--rw-r--r--   0        0        0      599 2024-02-01 04:04:33.985216 stonksfeed-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-24 05:05:26.788319 stonksfeed-0.1.6/stonksfeed/__init__.py
--rw-r--r--   0        0        0     2350 2024-01-27 20:02:17.097766 stonksfeed-0.1.6/stonksfeed/base.py
--rw-r--r--   0        0        0     2765 2024-01-03 21:41:11.603242 stonksfeed-0.1.6/stonksfeed/measures.py
--rw-r--r--   0        0        0        0 2023-12-24 05:05:47.286752 stonksfeed-0.1.6/stonksfeed/rss/__init__.py
--rw-r--r--   0        0        0      603 2024-01-22 05:20:18.226398 stonksfeed-0.1.6/stonksfeed/rss/marketwatch.py
--rw-r--r--   0        0        0      211 2023-12-25 18:53:44.665414 stonksfeed-0.1.6/stonksfeed/rss/wsj.py
--rw-r--r--   0        0        0        0 2023-12-25 00:11:02.120142 stonksfeed-0.1.6/stonksfeed/web/__init__.py
--rw-r--r--   0        0        0     1561 2024-02-01 03:49:44.866506 stonksfeed-0.1.6/stonksfeed/web/siliconinvestor.py
--rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 stonksfeed-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35129 2024-01-12 01:56:57.158427 stonksfeed-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1394 2024-02-29 04:35:46.719514 stonksfeed-0.1.7/README.md
+-rw-r--r--   0        0        0      619 2024-04-24 03:09:32.041058 stonksfeed-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-24 05:05:26.788319 stonksfeed-0.1.7/stonksfeed/__init__.py
+-rw-r--r--   0        0        0      724 2024-03-01 16:31:16.205009 stonksfeed-0.1.7/stonksfeed/config.py
+-rw-r--r--   0        0        0     2784 2024-03-01 16:31:42.820999 stonksfeed-0.1.7/stonksfeed/measures.py
+-rw-r--r--   0        0        0      542 2024-03-19 22:56:26.449421 stonksfeed-0.1.7/stonksfeed/models/article.py
+-rw-r--r--   0        0        0        0 2024-03-20 02:05:25.902515 stonksfeed-0.1.7/stonksfeed/rss/__init__.py
+-rw-r--r--   0        0        0      900 2024-03-19 22:57:27.983006 stonksfeed-0.1.7/stonksfeed/rss/base.py
+-rw-r--r--   0        0        0     1160 2024-03-20 02:08:08.015597 stonksfeed-0.1.7/stonksfeed/rss/rss_reader.py
+-rw-r--r--   0        0        0        0 2023-12-25 00:11:02.120142 stonksfeed-0.1.7/stonksfeed/web/__init__.py
+-rw-r--r--   0        0        0     1629 2024-03-20 02:14:48.241139 stonksfeed-0.1.7/stonksfeed/web/siliconinvestor.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 stonksfeed-0.1.7/PKG-INFO
```

### Comparing `stonksfeed-0.1.6/LICENSE` & `stonksfeed-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stonksfeed-0.1.6/pyproject.toml` & `stonksfeed-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stonksfeed"
-version = "0.1.6"
+version = "0.1.7"
 description = "A stock investor's news feed par excelance!"
 authors = ["m1yag1 <mike.arbelaez@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -17,11 +17,12 @@
 
 [tool.poetry.group.dev.dependencies]
 aws-sam-cli = "^1.106.0"
 checkov = "^3.1.53"
 setuptools = "69.0.3"
 pytest = "^7.4.3"
 boto3 = "^1.34.7"
+coverage = "^7.4.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stonksfeed-0.1.6/stonksfeed/measures.py` & `stonksfeed-0.1.7/stonksfeed/measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pragma: no cover
 measures = [
     {
         "name": "Price-to-Earnings Ratio (P/E)",
         "definition": "Compares the price of a stock to its earnings per share (EPS). It indicates how much investors are willing to pay for each dollar of earnings.",
         "math": "P/E Ratio = Price per Share / Earnings per Share (EPS)",
         "importance": "A high P/E might suggest that a stock's price is high relative to earnings and potentially overvalued, whereas a low P/E might indicate the opposite. For instance, a tech company with high growth prospects might have a high P/E ratio as investors are willing to pay more for future earnings.",
     },
```

### Comparing `stonksfeed-0.1.6/stonksfeed/web/siliconinvestor.py` & `stonksfeed-0.1.7/stonksfeed/web/siliconinvestor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 import pytz
-from stonksfeed.base import Article, BaseReader
+from stonksfeed.models.article import Article
+from stonksfeed.rss.base import BaseReader
 
 
 class SiliconInvestorPage(BaseReader):
     def __init__(self, title, url):
         self.root_url = "http://www.siliconinvestor.com/"
         self.source_type = "forum post"
         super().__init__("Silicon Investor", title, url)
@@ -20,28 +21,29 @@
         for item in soup.select("a[href*=readmsg]"):
             publisher = self.author
             title = self.title
             headline = item.text
             link = self._build_link(item["href"])
             # FIXME: No easy way to get pub_date so using current time.
             pubdate = self.get_current_epoch()
-            article = Article(publisher, title, headline, link, pubdate, self.source_type)
+            article = Article(
+                publisher, title, headline, link, pubdate, self.source_type
+            )
             articles.append(article)
 
         return articles
 
     def get_current_epoch(self):
         # Get the current time with timezone information
         current_time = datetime.now(pytz.timezone("GMT"))
         return int(current_time.timestamp())
 
 
-
 si_ai_robotics_forum = SiliconInvestorPage(
     title="Artificial Intelligence, Robotics, Chat bots - ChatGPT",
-    url="https://www.siliconinvestor.com/subject.aspx?subjectid=59856"
-    )
+    url="https://www.siliconinvestor.com/subject.aspx?subjectid=59856",
+)
 
 si_amd_intel_nvda_forum = SiliconInvestorPage(
     title="AMD, ARMH, INTC, NVDA",
-    url="https://www.siliconinvestor.com/subject.aspx?subjectid=58128"
+    url="https://www.siliconinvestor.com/subject.aspx?subjectid=58128",
 )
```

