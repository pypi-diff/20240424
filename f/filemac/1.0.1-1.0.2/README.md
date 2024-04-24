# Comparing `tmp/filemac-1.0.1.tar.gz` & `tmp/filemac-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filemac-1.0.1.tar", last modified: Sun Apr 21 19:24:34 2024, max compression
+gzip compressed data, was "filemac-1.0.2.tar", last modified: Wed Apr 24 09:28:44 2024, max compression
```

## Comparing `filemac-1.0.1.tar` & `filemac-1.0.2.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-21 19:24:34.630000 filemac-1.0.1/
--rwxr-xr-x   0 skye      (1000) skye      (1000)    35149 2024-03-24 06:23:20.000000 filemac-1.0.1/LICENSE
--rwxr-xr-x   0 skye      (1000) skye      (1000)       80 2024-03-24 07:29:02.000000 filemac-1.0.1/MANIFEST.ini
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4747 2024-04-21 19:24:34.630000 filemac-1.0.1/PKG-INFO
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3860 2024-04-21 19:19:57.000000 filemac-1.0.1/README.md
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-21 19:24:34.630000 filemac-1.0.1/__pycache__/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2386 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3992 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/AudioExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     6728 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/OCRTextExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2521 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/Simple_v_Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)    57828 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/converter.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      723 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/formarts.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      725 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/formats.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      957 2024-04-09 15:25:19.000000 filemac-1.0.1/__pycache__/show_progress.cpython-311.pyc
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-21 19:24:34.630000 filemac-1.0.1/filemac/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1957 2024-04-09 17:35:21.000000 filemac-1.0.1/filemac/AudioExtractor.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     3973 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/OCRTextExtractor.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1723 2024-04-09 17:40:51.000000 filemac-1.0.1/filemac/Simple_v_Analyzer.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)       23 2024-03-24 07:50:06.000000 filemac-1.0.1/filemac/__init__.py
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-21 19:24:34.630000 filemac-1.0.1/filemac/__pycache__/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4000 2024-03-24 06:16:58.000000 filemac-1.0.1/filemac/__pycache__/AudioExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     6736 2024-03-24 06:16:58.000000 filemac-1.0.1/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2526 2024-03-24 06:16:56.000000 filemac-1.0.1/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1118 2024-04-18 10:35:04.000000 filemac-1.0.1/filemac/__pycache__/colors.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)    57833 2024-03-24 06:16:56.000000 filemac-1.0.1/filemac/__pycache__/converter.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      730 2024-03-24 06:16:58.000000 filemac-1.0.1/filemac/__pycache__/formats.cpython-311.pyc
--rwxr-xr-x   0 skye      (1000) skye      (1000)      939 2024-04-18 10:35:04.000000 filemac-1.0.1/filemac/colors.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)    41539 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/converter.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)       27 2024-04-18 10:35:04.000000 filemac-1.0.1/filemac/dd.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     7818 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/fmac.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     5580 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/formats.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)      254 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/handle_warnings.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2589 2024-04-21 16:20:31.000000 filemac-1.0.1/filemac/image_op.py
-drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-21 19:24:34.630000 filemac-1.0.1/filemac.egg-info/
--rwxr-xr-x   0 skye      (1000) skye      (1000)     4747 2024-04-21 19:24:33.000000 filemac-1.0.1/filemac.egg-info/PKG-INFO
--rwxr-xr-x   0 skye      (1000) skye      (1000)     1122 2024-04-21 19:24:34.000000 filemac-1.0.1/filemac.egg-info/SOURCES.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-21 19:24:33.000000 filemac-1.0.1/filemac.egg-info/dependency_links.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       41 2024-04-21 19:24:33.000000 filemac-1.0.1/filemac.egg-info/entry_points.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-13 09:48:20.000000 filemac-1.0.1/filemac.egg-info/not-zip-safe
--rwxr-xr-x   0 skye      (1000) skye      (1000)      174 2024-04-21 19:24:33.000000 filemac-1.0.1/filemac.egg-info/requires.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       14 2024-04-21 19:24:33.000000 filemac-1.0.1/filemac.egg-info/top_level.txt
--rwxr-xr-x   0 skye      (1000) skye      (1000)       38 2024-04-21 19:24:34.630000 filemac-1.0.1/setup.cfg
--rwxr-xr-x   0 skye      (1000) skye      (1000)     2459 2024-04-21 19:14:58.000000 filemac-1.0.1/setup.py
--rwxr-xr-x   0 skye      (1000) skye      (1000)        6 2024-04-21 19:24:24.000000 filemac-1.0.1/version.txt
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/.github/
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/.github/workflows/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1070 2024-04-24 09:25:49.000000 filemac-1.0.2/.github/workflows/python-publish.yml
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    35149 2024-03-24 06:23:20.000000 filemac-1.0.2/LICENSE
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       80 2024-03-24 07:29:02.000000 filemac-1.0.2/MANIFEST.ini
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4748 2024-04-24 09:28:44.210000 filemac-1.0.2/PKG-INFO
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3861 2024-04-24 09:25:49.000000 filemac-1.0.2/README.md
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.200000 filemac-1.0.2/__pycache__/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2386 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3992 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/AudioExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     6728 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/OCRTextExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2521 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/Simple_v_Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    57828 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/converter.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      723 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/formarts.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      725 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/formats.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      957 2024-04-09 15:25:19.000000 filemac-1.0.2/__pycache__/show_progress.cpython-311.pyc
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1957 2024-04-09 17:35:21.000000 filemac-1.0.2/filemac/AudioExtractor.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     3978 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/OCRTextExtractor.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1723 2024-04-09 17:40:51.000000 filemac-1.0.2/filemac/Simple_v_Analyzer.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       23 2024-03-24 07:50:06.000000 filemac-1.0.2/filemac/__init__.py
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac/__pycache__/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4000 2024-03-24 06:16:58.000000 filemac-1.0.2/filemac/__pycache__/AudioExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     6471 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2526 2024-03-24 06:16:56.000000 filemac-1.0.2/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1118 2024-04-18 10:35:04.000000 filemac-1.0.2/filemac/__pycache__/colors.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    57833 2024-03-24 06:16:56.000000 filemac-1.0.2/filemac/__pycache__/converter.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      730 2024-03-24 06:16:58.000000 filemac-1.0.2/filemac/__pycache__/formats.cpython-311.pyc
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      939 2024-04-18 10:35:04.000000 filemac-1.0.2/filemac/colors.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)    42300 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/converter.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      307 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/dd.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     8163 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/fmac.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     5580 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/formats.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      254 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/handle_warnings.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2589 2024-04-24 09:25:49.000000 filemac-1.0.2/filemac/image_op.py
+drwxr-xr-x   0 skye      (1000) skye      (1000)        0 2024-04-24 09:28:44.210000 filemac-1.0.2/filemac.egg-info/
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     4748 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/PKG-INFO
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     1159 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/SOURCES.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/dependency_links.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       41 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/entry_points.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        1 2024-04-13 09:48:20.000000 filemac-1.0.2/filemac.egg-info/not-zip-safe
+-rwxr-xr-x   0 skye      (1000) skye      (1000)      174 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/requires.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       14 2024-04-24 09:28:43.000000 filemac-1.0.2/filemac.egg-info/top_level.txt
+-rwxr-xr-x   0 skye      (1000) skye      (1000)       38 2024-04-24 09:28:44.210000 filemac-1.0.2/setup.cfg
+-rwxr-xr-x   0 skye      (1000) skye      (1000)     2459 2024-04-24 09:25:49.000000 filemac-1.0.2/setup.py
+-rwxr-xr-x   0 skye      (1000) skye      (1000)        6 2024-04-24 09:28:39.000000 filemac-1.0.2/version.txt
```

### Comparing `filemac-1.0.1/LICENSE` & `filemac-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/PKG-INFO` & `filemac-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filemac
-Version: 1.0.1
+Version: 1.0.2
 Summary: Open source Python CLI toolkit for conversion, manipulation, Analysis
 Author: wambua
 Author-email: wambuamwiky2001@gmail.com
 License: GPL v3
 Keywords: file-conversion,file-analysis,file-manipulation,ocr,image-conversion
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
@@ -123,15 +123,15 @@
    ```shell
    filemac --convert_image example.png -t jpg
     ```
             ``Supported formats For audio conversion``
                 `1`.JPEG: `.jpg`
                 `2`.PNG": `.png`
                 `3`.GIF": `.gif`
-                `4`.BM":  `bmp`
+                `4`.BM":  `.bmp`
                 `5`.TIFF: `.tiff`
                 `6`.EXR   `.exr`
                 `7`.PDF:  `.pdf`
                 `8`.WebP: `.webp`
                 `9`.ICNS: `.icns`
                 `10`.PSD: `.psd`
                 `11`.SVG: `.svg`
```

### Comparing `filemac-1.0.1/README.md` & `filemac-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
    ```shell
    filemac --convert_image example.png -t jpg
     ```
             ``Supported formats For audio conversion``
                 `1`.JPEG: `.jpg`
                 `2`.PNG": `.png`
                 `3`.GIF": `.gif`
-                `4`.BM":  `bmp`
+                `4`.BM":  `.bmp`
                 `5`.TIFF: `.tiff`
                 `6`.EXR   `.exr`
                 `7`.PDF:  `.pdf`
                 `8`.WebP: `.webp`
                 `9`.ICNS: `.icns`
                 `10`.PSD: `.psd`
                 `11`.SVG: `.svg`
```

### Comparing `filemac-1.0.1/__pycache__/Analyzer.cpython-311.pyc` & `filemac-1.0.2/__pycache__/Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/AudioExtractor.cpython-311.pyc` & `filemac-1.0.2/__pycache__/AudioExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/OCRTextExtractor.cpython-311.pyc` & `filemac-1.0.2/__pycache__/OCRTextExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/Simple_v_Analyzer.cpython-311.pyc` & `filemac-1.0.2/__pycache__/Simple_v_Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/converter.cpython-311.pyc` & `filemac-1.0.2/__pycache__/converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/formarts.cpython-311.pyc` & `filemac-1.0.2/__pycache__/formarts.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/formats.cpython-311.pyc` & `filemac-1.0.2/__pycache__/formats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/__pycache__/show_progress.cpython-311.pyc` & `filemac-1.0.2/__pycache__/show_progress.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/AudioExtractor.py` & `filemac-1.0.2/filemac/AudioExtractor.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/OCRTextExtractor.py` & `filemac-1.0.2/filemac/OCRTextExtractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,24 @@
                 if os.path.isfile(file_path):
                     files_to_process.append(file_path)
 
         return files_to_process
 
     def OCR(self):
         image_list = self.preprocess()
-        ls = {'png', 'jpg'}
+        ls = ['png', 'jpg']
         image_list = [
             item for item in image_list if any(item.lower().endswith(ext)
                                                for ext in ls)]
 
         def ocr_text_extraction(image_path):
             '''Load image using OpenCV'''
             img = cv2.imread(image_path)
 
-            logger.info(f"\033[5;34mprocessing {image_path}...\033[0m")
+            logger.info(f"\033[2;95mprocessing {image_path}...\033[0m")
 
             try:
                 '''Preprocess image for better OCR results'''
                 gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
                 thresh = cv2.threshold(
                     gray, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)[1]
                 img_pil = Image.fromarray(thresh)
@@ -64,21 +64,21 @@
                 '''Remove extra whitespaces and newlines
                 text = ' '.join(text.split()).strip()'''
                 logger.info("\033[36mFound:\n\033[0m")
                 print(text)
                 current_path = os.getcwd()
                 file_path = os.path.join(current_path, OCR_file)
                 ''' Save the extracted text to specified file '''
-                logger.info("\033[32mGenerating text file for the extracted \
+                logger.info("\033[1;92mGenerating text file for the extracted \
 text..\033[0m")
 
                 with open(file_path, 'w') as file:
                     file.write(text)
                 logger.info(
-                    f"File saved as \033[32m{OCR_file}\033[0m:")
+                    f"File saved as \033[1;93m{OCR_file}\033[0m:")
                 '''If there are multiple candidate images for text extraction,
                 wait for key press before proceeding to the next
                 image otherwise don't wait
                 size = [i for i in enumerate(image_list)]'''
                 if len(image_list) >= 2:
                     input("\033[5;97mPress Enter to continue\033[0m")
             except KeyboardInterrupt:
@@ -93,9 +93,9 @@
             except Exception as e:
                 logger.error(f"Error: {type(e).__name__}: {str(e)}")
             except Exception as e:
                 logger.error(f"Error:>>\033[31m{e}\033[0m")
             return text
 
         for image_path in image_list:
-            OCR_file = image_path[:-3] + "txt"
+            OCR_file = image_path[:-4] + ".txt"
             ocr_text_extraction(image_path)
```

### Comparing `filemac-1.0.1/filemac/Simple_v_Analyzer.py` & `filemac-1.0.2/filemac/Simple_v_Analyzer.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/__pycache__/AudioExtractor.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/AudioExtractor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/OCRTextExtractor.cpython-311.pyc`

 * *Files 13% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5234f965 (Tue Mar 19 06:44:34 2024 UTC)
-files sz: 3979
+moddate:  0x5aca2866 (Wed Apr 24 09:01:14 2024 UTC)
+files sz: 3974
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -71,15 +71,15 @@
                128 CALL                     1
                138 STORE_NAME              12 (logger)
    
     12         140 NOP
    
     20         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST               5 (<code object ExtractText, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 20>)
+               146 LOAD_CONST               5 (<code object ExtractText, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 20>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST               6 ('ExtractText')
                152 PRECALL                  2
                156 CALL                     2
                166 STORE_NAME              13 (ExtractText)
                168 LOAD_CONST               1 (None)
                170 RETURN_VALUE
@@ -99,23 +99,23 @@
             045300
           20           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ExtractText')
                        8 STORE_NAME               2 (__qualname__)
          
-          21          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 21>)
+          21          10 LOAD_CONST               1 (<code object __init__, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 21>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          24          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 24>)
+          24          16 LOAD_CONST               2 (<code object preprocess, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 24>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (preprocess)
          
-          40          22 LOAD_CONST               3 (<code object OCR, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 40>)
+          40          22 LOAD_CONST               3 (<code object OCR, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 40>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (OCR)
                       28 LOAD_CONST               4 (None)
                       30 RETURN_VALUE
          consts
             'ExtractText'
             code
@@ -133,15 +133,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('input_file',)
                varnames   ('self', 'input_file')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+               filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                name       '__init__'
                firstlineno 21
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
@@ -261,26 +261,26 @@
                   None
                   'Cannot work with empty folder'
                   1
                names      ('os', 'path', 'isfile', 'input_file', 'append', 'isdir', 'listdir', 'print', 'sys', 'exit', 'join')
                varnames   ('self', 'files_to_process', 'file', 'file_path')
                freevars   ()
                cellvars   ()
-               filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+               filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                name       'preprocess'
                firstlineno 24
                lnotab 0x0201040248013601480132011e01280136014a013e012c02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x87038704870597007c00a0000000000000000000000000000000000000
-                  000000a6000000ab0000000000000000008a046401640268028a05880566
+                  000000a6000000ab0000000000000000008a046401640267028a05880566
                   016403840889044400a6000000ab0000000000000000008a048803880466
                   02640484087d01890444005d1a7d027c0264006405850219000000000000
                   00000064067a0000008a0302007c017c02a6010000ab0100000000000000
                   0001008c1b64005300
                              0 MAKE_CELL                3 (OCR_file)
                              2 MAKE_CELL                4 (image_list)
                              4 MAKE_CELL                5 (ls)
@@ -291,59 +291,59 @@
                             10 LOAD_METHOD              0 (preprocess)
                             32 PRECALL                  0
                             36 CALL                     0
                             46 STORE_DEREF              4 (image_list)
                
                 42          48 LOAD_CONST               1 ('png')
                             50 LOAD_CONST               2 ('jpg')
-                            52 BUILD_SET                2
+                            52 BUILD_LIST               2
                             54 STORE_DEREF              5 (ls)
                
                 43          56 LOAD_CLOSURE             5 (ls)
                             58 BUILD_TUPLE              1
-                            60 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 43>)
+                            60 LOAD_CONST               3 (<code object <listcomp>, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 43>)
                             62 MAKE_FUNCTION            8 (closure)
                
                 44          64 LOAD_DEREF               4 (image_list)
                
                 43          66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 STORE_DEREF              4 (image_list)
                
                 47          84 LOAD_CLOSURE             3 (OCR_file)
                             86 LOAD_CLOSURE             4 (image_list)
                             88 BUILD_TUPLE              2
-                            90 LOAD_CONST               4 (<code object ocr_text_extraction, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 47>)
+                            90 LOAD_CONST               4 (<code object ocr_text_extraction, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 47>)
                             92 MAKE_FUNCTION            8 (closure)
                             94 STORE_FAST               1 (ocr_text_extraction)
                
-               100          96 LOAD_DEREF               4 (image_list)
+                99          96 LOAD_DEREF               4 (image_list)
                             98 GET_ITER
                        >>  100 FOR_ITER                26 (to 154)
                            102 STORE_FAST               2 (image_path)
                
-               101         104 LOAD_FAST                2 (image_path)
+               100         104 LOAD_FAST                2 (image_path)
                            106 LOAD_CONST               0 (None)
-                           108 LOAD_CONST               5 (-3)
+                           108 LOAD_CONST               5 (-4)
                            110 BUILD_SLICE              2
                            112 BINARY_SUBSCR
-                           122 LOAD_CONST               6 ('txt')
+                           122 LOAD_CONST               6 ('.txt')
                            124 BINARY_OP                0 (+)
                            128 STORE_DEREF              3 (OCR_file)
                
-               102         130 PUSH_NULL
+               101         130 PUSH_NULL
                            132 LOAD_FAST                1 (ocr_text_extraction)
                            134 LOAD_FAST                2 (image_path)
                            136 PRECALL                  1
                            140 CALL                     1
                            150 POP_TOP
                            152 JUMP_BACKWARD           27 (to 100)
                
-               100     >>  154 LOAD_CONST               0 (None)
+                99     >>  154 LOAD_CONST               0 (None)
                            156 RETURN_VALUE
                consts
                   None
                   'png'
                   'jpg'
                   code
                      argcount  : 1
@@ -362,15 +362,15 @@
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                31 (to 74)
                      
                       44          12 STORE_DEREF              1 (item)
                                   14 LOAD_GLOBAL              1 (NULL + any)
                                   26 LOAD_CLOSURE             1 (item)
                                   28 BUILD_TUPLE              1
-                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 44>)
+                                  30 LOAD_CONST               0 (<code object <genexpr>, file "/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py", line 44>)
                                   32 MAKE_FUNCTION            8 (closure)
                      
                       45          34 LOAD_DEREF               2 (ls)
                      
                       44          36 GET_ITER
                                   38 PRECALL                  0
                                   42 CALL                     0
@@ -421,29 +421,29 @@
                                        100 RETURN_VALUE
                            consts
                               None
                            names      ('lower', 'endswith')
                            varnames   ('.0', 'ext')
                            freevars   ('item',)
                            cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+                           filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                            name       '<genexpr>'
                            firstlineno 44
                            lnotab 0x0c0102ff
                      names      ('any',)
                      varnames   ('.0',)
                      freevars   ('ls',)
                      cellvars   ('item',)
-                     filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                      name       '<listcomp>'
                      firstlineno 43
                      lnotab 0x0c01160102ff1eff020102ff
                   code
                      argcount  : 1
-                     nlocals   : 12
+                     nlocals   : 11
                      stacksize : 9
                      flags     : 19
                      code
                         0x950297007401000000000000000000006a0100000000000000007c00a6
                         010000ab0100000000000000007d01740400000000000000000000a00300
                         0000000000000000000000000000000000000064017c009b0064029d03a6
                         010000ab0100000000000000000100090009007401000000000000000000
@@ -456,47 +456,46 @@
                         010000ab0100000000000000007d04090064067d05741700000000000000
                         0000006a0c00000000000000007c047c05ac07a6020000ab020000000000
                         0000007d060900740400000000000000000000a003000000000000000000
                         00000000000000000000006408a6010000ab010000000000000000010074
                         1b000000000000000000007c06a6010000ab010000000000000000010074
                         1d000000000000000000006a0f0000000000000000a6000000ab00000000
                         00000000007d07741c000000000000000000006a100000000000000000a0
-                        1100000000000000000000000000000000000000007c07890ca6020000ab
+                        1100000000000000000000000000000000000000007c07890ba6020000ab
                         0200000000000000007d080900740400000000000000000000a003000000
                         00000000000000000000000000000000006409a6010000ab010000000000
                         00000001007425000000000000000000007c08640aa6020000ab02000000
                         000000000035007d097c09a0130000000000000000000000000000000000
                         0000007c06a6010000ab0100000000000000000100640b640b640ba60200
                         00ab02000000000000000001006e0b230031007304770278035900770101
                         00590001000100740400000000000000000000a003000000000000000000
-                        0000000000000000000000640c7c079b00640d890c9b00640e9d05a60100
-                        00ab01000000000000000001000900640f84007429000000000000000000
-                        00890da6010000ab0100000000000000004400a6000000ab000000000000
-                        0000007d0a7c0a64106b0500000000720f742b0000000000000000000064
-                        11a6010000ab010000000000000000010090016e312300742c0000000000
-                        0000000000240072270100741b000000000000000000006412a6010000ab
+                        0000000000000000000000640c890b9b00640d9d03a6010000ab01000000
+                        000000000001000900742900000000000000000000890ca6010000ab0100
+                        00000000000000640e6b0500000000720f742b0000000000000000000064
+                        0fa6010000ab010000000000000000010090016e312300742c0000000000
+                        0000000000240072270100741b000000000000000000006410a6010000ab
                         0100000000000000000100742f000000000000000000006a180000000000
                         0000006403a6010000ab0100000000000000000100590090016e01743200
-                        000000000000000000240072347d0b740400000000000000000000a01a00
-                        000000000000000000000000000000000000006413743700000000000000
-                        0000007c0ba6010000ab0100000000000000009b009d02a6010000ab0100
-                        0000000000000001005900640b7d0b7e0b6ec9640b7d0b7e0b7701743800
-                        000000000000000000240072387d0b740400000000000000000000a01a00
-                        000000000000000000000000000000000000006414890c9b006415743700
-                        0000000000000000007c0ba6010000ab0100000000000000009b0064169d
-                        05a6010000ab01000000000000000001005900640b7d0b7e0b6e89640b7d
-                        0b7e0b7701743a00000000000000000000240072497d0b74040000000000
-                        0000000000a01a0000000000000000000000000000000000000000641374
-                        3d000000000000000000007c0ba6010000ab0100000000000000006a1f00
-                        000000000000009b0064177437000000000000000000007c0ba6010000ab
+                        000000000000000000240072347d0a740400000000000000000000a01a00
+                        000000000000000000000000000000000000006411743700000000000000
+                        0000007c0aa6010000ab0100000000000000009b009d02a6010000ab0100
+                        0000000000000001005900640b7d0a7e0a6ec9640b7d0a7e0a7701743800
+                        000000000000000000240072387d0a740400000000000000000000a01a00
+                        000000000000000000000000000000000000006412890b9b006413743700
+                        0000000000000000007c0aa6010000ab0100000000000000009b0064149d
+                        05a6010000ab01000000000000000001005900640b7d0a7e0a6e89640b7d
+                        0a7e0a7701743a00000000000000000000240072497d0a74040000000000
+                        0000000000a01a0000000000000000000000000000000000000000641174
+                        3d000000000000000000007c0aa6010000ab0100000000000000006a1f00
+                        000000000000009b0064157437000000000000000000007c0aa6010000ab
                         0100000000000000009b009d04a6010000ab010000000000000000010059
-                        00640b7d0b7e0b6e38640b7d0b7e0b7701743a0000000000000000000024
-                        0072287d0b740400000000000000000000a01a0000000000000000000000
-                        00000000000000000064187c0b9b0064169d03a6010000ab010000000000
-                        00000001005900640b7d0b7e0b6e08640b7d0b7e0b770177007803590077
+                        00640b7d0a7e0a6e38640b7d0a7e0a7701743a0000000000000000000024
+                        0072287d0a740400000000000000000000a01a0000000000000000000000
+                        00000000000000000064167c0a9b0064149d03a6010000ab010000000000
+                        00000001005900640b7d0a7e0a6e08640b7d0a7e0a770177007803590077
                         017c065300
                                    0 COPY_FREE_VARS           2
                      
                       47           2 RESUME                   0
                      
                       49           4 LOAD_GLOBAL              1 (NULL + cv2)
                                   16 LOAD_ATTR                1 (imread)
@@ -591,15 +590,15 @@
                                  474 CALL                     0
                                  484 STORE_FAST               7 (current_path)
                      
                       69         486 LOAD_GLOBAL             28 (os)
                                  498 LOAD_ATTR               16 (path)
                                  508 LOAD_METHOD             17 (join)
                                  530 LOAD_FAST                7 (current_path)
-                                 532 LOAD_DEREF              12 (OCR_file)
+                                 532 LOAD_DEREF              11 (OCR_file)
                                  534 PRECALL                  2
                                  538 CALL                     2
                                  548 STORE_FAST               8 (file_path)
                      
                       70         550 NOP
                      
                       71         552 LOAD_GLOBAL              4 (logger)
@@ -642,305 +641,267 @@
                                  720 POP_EXCEPT
                                  722 POP_TOP
                                  724 POP_TOP
                      
                       76     >>  726 LOAD_GLOBAL              4 (logger)
                                  738 LOAD_METHOD              3 (info)
                      
-                      77         760 LOAD_CONST              12 ('File saved in \x1b[33m')
-                                 762 LOAD_FAST                7 (current_path)
+                      77         760 LOAD_CONST              12 ('File saved as \x1b[32m')
+                                 762 LOAD_DEREF              11 (OCR_file)
                                  764 FORMAT_VALUE             0
-                                 766 LOAD_CONST              13 ('\x1b[0m as \x1b[32m')
+                                 766 LOAD_CONST              13 ('\x1b[0m:')
+                                 768 BUILD_STRING             3
                      
-                      78         768 LOAD_DEREF              12 (OCR_file)
-                     
-                      77         770 FORMAT_VALUE             0
-                                 772 LOAD_CONST              14 ('\x1b[0m:')
-                                 774 BUILD_STRING             5
-                     
-                      76         776 PRECALL                  1
-                                 780 CALL                     1
-                                 790 POP_TOP
-                     
-                      79         792 NOP
-                     
-                      82         794 LOAD_CONST              15 (<code object <listcomp>, file "/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py", line 82>)
-                                 796 MAKE_FUNCTION            0
-                                 798 LOAD_GLOBAL             41 (NULL + enumerate)
-                                 810 LOAD_DEREF              13 (image_list)
-                                 812 PRECALL                  1
-                                 816 CALL                     1
-                                 826 GET_ITER
-                                 828 PRECALL                  0
-                                 832 CALL                     0
-                                 842 STORE_FAST              10 (size)
-                     
-                      83         844 LOAD_FAST               10 (size)
-                                 846 LOAD_CONST              16 (2)
-                                 848 COMPARE_OP               5 (>=)
-                                 854 POP_JUMP_FORWARD_IF_FALSE    15 (to 886)
-                     
-                      84         856 LOAD_GLOBAL             43 (NULL + input)
-                                 868 LOAD_CONST              17 ('Press Enter to continue ')
-                                 870 PRECALL                  1
-                                 874 CALL                     1
-                                 884 POP_TOP
-                             >>  886 EXTENDED_ARG             1
-                                 888 JUMP_FORWARD           305 (to 1500)
-                             >>  890 PUSH_EXC_INFO
-                     
-                      85         892 LOAD_GLOBAL             44 (KeyboardInterrupt)
-                                 904 CHECK_EXC_MATCH
-                                 906 POP_JUMP_FORWARD_IF_FALSE    39 (to 986)
+                      76         770 PRECALL                  1
+                                 774 CALL                     1
+                                 784 POP_TOP
+                     
+                      78         786 NOP
+                     
+                      82         788 LOAD_GLOBAL             41 (NULL + len)
+                                 800 LOAD_DEREF              12 (image_list)
+                                 802 PRECALL                  1
+                                 806 CALL                     1
+                                 816 LOAD_CONST              14 (2)
+                                 818 COMPARE_OP               5 (>=)
+                                 824 POP_JUMP_FORWARD_IF_FALSE    15 (to 856)
+                     
+                      83         826 LOAD_GLOBAL             43 (NULL + input)
+                                 838 LOAD_CONST              15 ('\x1b[5;97mPress Enter to continue\x1b[0m')
+                                 840 PRECALL                  1
+                                 844 CALL                     1
+                                 854 POP_TOP
+                             >>  856 EXTENDED_ARG             1
+                                 858 JUMP_FORWARD           305 (to 1470)
+                             >>  860 PUSH_EXC_INFO
+                     
+                      84         862 LOAD_GLOBAL             44 (KeyboardInterrupt)
+                                 874 CHECK_EXC_MATCH
+                                 876 POP_JUMP_FORWARD_IF_FALSE    39 (to 956)
+                                 878 POP_TOP
+                     
+                      85         880 LOAD_GLOBAL             27 (NULL + print)
+                                 892 LOAD_CONST              16 ('\nExiting')
+                                 894 PRECALL                  1
+                                 898 CALL                     1
                                  908 POP_TOP
                      
-                      86         910 LOAD_GLOBAL             27 (NULL + print)
-                                 922 LOAD_CONST              18 ('Exiting')
-                                 924 PRECALL                  1
-                                 928 CALL                     1
-                                 938 POP_TOP
-                     
-                      87         940 LOAD_GLOBAL             47 (NULL + sys)
-                                 952 LOAD_ATTR               24 (exit)
-                                 962 LOAD_CONST               3 (0)
-                                 964 PRECALL                  1
-                                 968 CALL                     1
-                                 978 POP_TOP
-                                 980 POP_EXCEPT
-                                 982 EXTENDED_ARG             1
-                                 984 JUMP_FORWARD           257 (to 1500)
-                     
-                      88     >>  986 LOAD_GLOBAL             50 (FileNotFoundError)
-                                 998 CHECK_EXC_MATCH
-                                1000 POP_JUMP_FORWARD_IF_FALSE    52 (to 1106)
-                                1002 STORE_FAST              11 (e)
-                     
-                      89        1004 LOAD_GLOBAL              4 (logger)
-                                1016 LOAD_METHOD             26 (error)
-                                1038 LOAD_CONST              19 ('Error: ')
-                                1040 LOAD_GLOBAL             55 (NULL + str)
-                                1052 LOAD_FAST               11 (e)
-                                1054 PRECALL                  1
-                                1058 CALL                     1
-                                1068 FORMAT_VALUE             0
-                                1070 BUILD_STRING             2
-                                1072 PRECALL                  1
-                                1076 CALL                     1
-                                1086 POP_TOP
-                                1088 POP_EXCEPT
-                                1090 LOAD_CONST              11 (None)
-                                1092 STORE_FAST              11 (e)
-                                1094 DELETE_FAST             11 (e)
-                                1096 JUMP_FORWARD           201 (to 1500)
-                             >> 1098 LOAD_CONST              11 (None)
-                                1100 STORE_FAST              11 (e)
-                                1102 DELETE_FAST             11 (e)
-                                1104 RERAISE                  1
-                     
-                      90     >> 1106 LOAD_GLOBAL             56 (IOError)
-                                1118 CHECK_EXC_MATCH
-                                1120 POP_JUMP_FORWARD_IF_FALSE    56 (to 1234)
-                                1122 STORE_FAST              11 (e)
-                     
-                      91        1124 LOAD_GLOBAL              4 (logger)
-                                1136 LOAD_METHOD             26 (error)
-                     
-                      92        1158 LOAD_CONST              20 ("Could not write to output file '")
-                                1160 LOAD_DEREF              12 (OCR_file)
-                                1162 FORMAT_VALUE             0
-                                1164 LOAD_CONST              21 ("'. Reason: ")
-                     
-                      93        1166 LOAD_GLOBAL             55 (NULL + str)
-                                1178 LOAD_FAST               11 (e)
-                                1180 PRECALL                  1
-                                1184 CALL                     1
-                     
-                      92        1194 FORMAT_VALUE             0
-                                1196 LOAD_CONST              22 ('\x1b[0m')
-                                1198 BUILD_STRING             5
-                     
-                      91        1200 PRECALL                  1
-                                1204 CALL                     1
-                                1214 POP_TOP
-                                1216 POP_EXCEPT
-                                1218 LOAD_CONST              11 (None)
-                                1220 STORE_FAST              11 (e)
-                                1222 DELETE_FAST             11 (e)
-                                1224 JUMP_FORWARD           137 (to 1500)
-                             >> 1226 LOAD_CONST              11 (None)
-                                1228 STORE_FAST              11 (e)
-                                1230 DELETE_FAST             11 (e)
-                                1232 RERAISE                  1
-                     
-                      94     >> 1234 LOAD_GLOBAL             58 (Exception)
-                                1246 CHECK_EXC_MATCH
-                                1248 POP_JUMP_FORWARD_IF_FALSE    73 (to 1396)
-                                1250 STORE_FAST              11 (e)
-                     
-                      95        1252 LOAD_GLOBAL              4 (logger)
-                                1264 LOAD_METHOD             26 (error)
-                                1286 LOAD_CONST              19 ('Error: ')
-                                1288 LOAD_GLOBAL             61 (NULL + type)
-                                1300 LOAD_FAST               11 (e)
-                                1302 PRECALL                  1
-                                1306 CALL                     1
-                                1316 LOAD_ATTR               31 (__name__)
-                                1326 FORMAT_VALUE             0
-                                1328 LOAD_CONST              23 (': ')
-                                1330 LOAD_GLOBAL             55 (NULL + str)
-                                1342 LOAD_FAST               11 (e)
-                                1344 PRECALL                  1
-                                1348 CALL                     1
-                                1358 FORMAT_VALUE             0
-                                1360 BUILD_STRING             4
-                                1362 PRECALL                  1
-                                1366 CALL                     1
-                                1376 POP_TOP
-                                1378 POP_EXCEPT
-                                1380 LOAD_CONST              11 (None)
-                                1382 STORE_FAST              11 (e)
-                                1384 DELETE_FAST             11 (e)
-                                1386 JUMP_FORWARD            56 (to 1500)
-                             >> 1388 LOAD_CONST              11 (None)
-                                1390 STORE_FAST              11 (e)
-                                1392 DELETE_FAST             11 (e)
-                                1394 RERAISE                  1
-                     
-                      96     >> 1396 LOAD_GLOBAL             58 (Exception)
-                                1408 CHECK_EXC_MATCH
-                                1410 POP_JUMP_FORWARD_IF_FALSE    40 (to 1492)
-                                1412 STORE_FAST              11 (e)
-                     
-                      97        1414 LOAD_GLOBAL              4 (logger)
-                                1426 LOAD_METHOD             26 (error)
-                                1448 LOAD_CONST              24 ('Error:>>\x1b[31m')
-                                1450 LOAD_FAST               11 (e)
-                                1452 FORMAT_VALUE             0
-                                1454 LOAD_CONST              22 ('\x1b[0m')
-                                1456 BUILD_STRING             3
-                                1458 PRECALL                  1
-                                1462 CALL                     1
-                                1472 POP_TOP
-                                1474 POP_EXCEPT
-                                1476 LOAD_CONST              11 (None)
-                                1478 STORE_FAST              11 (e)
-                                1480 DELETE_FAST             11 (e)
-                                1482 JUMP_FORWARD             8 (to 1500)
-                             >> 1484 LOAD_CONST              11 (None)
-                                1486 STORE_FAST              11 (e)
-                                1488 DELETE_FAST             11 (e)
-                                1490 RERAISE                  1
-                     
-                      96     >> 1492 RERAISE                  0
-                             >> 1494 COPY                     3
-                                1496 POP_EXCEPT
-                                1498 RERAISE                  1
+                      86         910 LOAD_GLOBAL             47 (NULL + sys)
+                                 922 LOAD_ATTR               24 (exit)
+                                 932 LOAD_CONST               3 (0)
+                                 934 PRECALL                  1
+                                 938 CALL                     1
+                                 948 POP_TOP
+                                 950 POP_EXCEPT
+                                 952 EXTENDED_ARG             1
+                                 954 JUMP_FORWARD           257 (to 1470)
+                     
+                      87     >>  956 LOAD_GLOBAL             50 (FileNotFoundError)
+                                 968 CHECK_EXC_MATCH
+                                 970 POP_JUMP_FORWARD_IF_FALSE    52 (to 1076)
+                                 972 STORE_FAST              10 (e)
+                     
+                      88         974 LOAD_GLOBAL              4 (logger)
+                                 986 LOAD_METHOD             26 (error)
+                                1008 LOAD_CONST              17 ('Error: ')
+                                1010 LOAD_GLOBAL             55 (NULL + str)
+                                1022 LOAD_FAST               10 (e)
+                                1024 PRECALL                  1
+                                1028 CALL                     1
+                                1038 FORMAT_VALUE             0
+                                1040 BUILD_STRING             2
+                                1042 PRECALL                  1
+                                1046 CALL                     1
+                                1056 POP_TOP
+                                1058 POP_EXCEPT
+                                1060 LOAD_CONST              11 (None)
+                                1062 STORE_FAST              10 (e)
+                                1064 DELETE_FAST             10 (e)
+                                1066 JUMP_FORWARD           201 (to 1470)
+                             >> 1068 LOAD_CONST              11 (None)
+                                1070 STORE_FAST              10 (e)
+                                1072 DELETE_FAST             10 (e)
+                                1074 RERAISE                  1
+                     
+                      89     >> 1076 LOAD_GLOBAL             56 (IOError)
+                                1088 CHECK_EXC_MATCH
+                                1090 POP_JUMP_FORWARD_IF_FALSE    56 (to 1204)
+                                1092 STORE_FAST              10 (e)
+                     
+                      90        1094 LOAD_GLOBAL              4 (logger)
+                                1106 LOAD_METHOD             26 (error)
+                     
+                      91        1128 LOAD_CONST              18 ("Could not write to output file '")
+                                1130 LOAD_DEREF              11 (OCR_file)
+                                1132 FORMAT_VALUE             0
+                                1134 LOAD_CONST              19 ("'. Reason: ")
+                     
+                      92        1136 LOAD_GLOBAL             55 (NULL + str)
+                                1148 LOAD_FAST               10 (e)
+                                1150 PRECALL                  1
+                                1154 CALL                     1
+                     
+                      91        1164 FORMAT_VALUE             0
+                                1166 LOAD_CONST              20 ('\x1b[0m')
+                                1168 BUILD_STRING             5
+                     
+                      90        1170 PRECALL                  1
+                                1174 CALL                     1
+                                1184 POP_TOP
+                                1186 POP_EXCEPT
+                                1188 LOAD_CONST              11 (None)
+                                1190 STORE_FAST              10 (e)
+                                1192 DELETE_FAST             10 (e)
+                                1194 JUMP_FORWARD           137 (to 1470)
+                             >> 1196 LOAD_CONST              11 (None)
+                                1198 STORE_FAST              10 (e)
+                                1200 DELETE_FAST             10 (e)
+                                1202 RERAISE                  1
+                     
+                      93     >> 1204 LOAD_GLOBAL             58 (Exception)
+                                1216 CHECK_EXC_MATCH
+                                1218 POP_JUMP_FORWARD_IF_FALSE    73 (to 1366)
+                                1220 STORE_FAST              10 (e)
+                     
+                      94        1222 LOAD_GLOBAL              4 (logger)
+                                1234 LOAD_METHOD             26 (error)
+                                1256 LOAD_CONST              17 ('Error: ')
+                                1258 LOAD_GLOBAL             61 (NULL + type)
+                                1270 LOAD_FAST               10 (e)
+                                1272 PRECALL                  1
+                                1276 CALL                     1
+                                1286 LOAD_ATTR               31 (__name__)
+                                1296 FORMAT_VALUE             0
+                                1298 LOAD_CONST              21 (': ')
+                                1300 LOAD_GLOBAL             55 (NULL + str)
+                                1312 LOAD_FAST               10 (e)
+                                1314 PRECALL                  1
+                                1318 CALL                     1
+                                1328 FORMAT_VALUE             0
+                                1330 BUILD_STRING             4
+                                1332 PRECALL                  1
+                                1336 CALL                     1
+                                1346 POP_TOP
+                                1348 POP_EXCEPT
+                                1350 LOAD_CONST              11 (None)
+                                1352 STORE_FAST              10 (e)
+                                1354 DELETE_FAST             10 (e)
+                                1356 JUMP_FORWARD            56 (to 1470)
+                             >> 1358 LOAD_CONST              11 (None)
+                                1360 STORE_FAST              10 (e)
+                                1362 DELETE_FAST             10 (e)
+                                1364 RERAISE                  1
+                     
+                      95     >> 1366 LOAD_GLOBAL             58 (Exception)
+                                1378 CHECK_EXC_MATCH
+                                1380 POP_JUMP_FORWARD_IF_FALSE    40 (to 1462)
+                                1382 STORE_FAST              10 (e)
+                     
+                      96        1384 LOAD_GLOBAL              4 (logger)
+                                1396 LOAD_METHOD             26 (error)
+                                1418 LOAD_CONST              22 ('Error:>>\x1b[31m')
+                                1420 LOAD_FAST               10 (e)
+                                1422 FORMAT_VALUE             0
+                                1424 LOAD_CONST              20 ('\x1b[0m')
+                                1426 BUILD_STRING             3
+                                1428 PRECALL                  1
+                                1432 CALL                     1
+                                1442 POP_TOP
+                                1444 POP_EXCEPT
+                                1446 LOAD_CONST              11 (None)
+                                1448 STORE_FAST              10 (e)
+                                1450 DELETE_FAST             10 (e)
+                                1452 JUMP_FORWARD             8 (to 1470)
+                             >> 1454 LOAD_CONST              11 (None)
+                                1456 STORE_FAST              10 (e)
+                                1458 DELETE_FAST             10 (e)
+                                1460 RERAISE                  1
+                     
+                      95     >> 1462 RERAISE                  0
+                             >> 1464 COPY                     3
+                                1466 POP_EXCEPT
+                                1468 RERAISE                  1
                      
-                      98     >> 1500 LOAD_FAST                6 (text)
-                                1502 RETURN_VALUE
+                      97     >> 1470 LOAD_FAST                6 (text)
+                                1472 RETURN_VALUE
                      ExceptionTable:
-                       106 to 634 -> 890 [0]
+                       106 to 634 -> 860 [0]
                        636 to 678 -> 704 [1] lasti
-                       680 to 702 -> 890 [0]
+                       680 to 702 -> 860 [0]
                        704 to 710 -> 712 [3] lasti
-                       712 to 716 -> 890 [0]
+                       712 to 716 -> 860 [0]
                        718 to 718 -> 712 [3] lasti
-                       720 to 884 -> 890 [0]
-                       890 to 978 -> 1494 [1] lasti
-                       986 to 1002 -> 1494 [1] lasti
-                       1004 to 1086 -> 1098 [1] lasti
-                       1098 to 1122 -> 1494 [1] lasti
-                       1124 to 1214 -> 1226 [1] lasti
-                       1226 to 1250 -> 1494 [1] lasti
-                       1252 to 1376 -> 1388 [1] lasti
-                       1388 to 1412 -> 1494 [1] lasti
-                       1414 to 1472 -> 1484 [1] lasti
-                       1484 to 1492 -> 1494 [1] lasti
+                       720 to 854 -> 860 [0]
+                       860 to 948 -> 1464 [1] lasti
+                       956 to 972 -> 1464 [1] lasti
+                       974 to 1056 -> 1068 [1] lasti
+                       1068 to 1092 -> 1464 [1] lasti
+                       1094 to 1184 -> 1196 [1] lasti
+                       1196 to 1220 -> 1464 [1] lasti
+                       1222 to 1346 -> 1358 [1] lasti
+                       1358 to 1382 -> 1464 [1] lasti
+                       1384 to 1442 -> 1454 [1] lasti
+                       1454 to 1462 -> 1464 [1] lasti
                      consts
                         'Load image using OpenCV'
                         '\x1b[5;34mprocessing '
                         '...\x1b[0m'
                         0
                         255
                         1
                         '-l eng --oem 3 --psm 6'
                         ('config',)
                         '\x1b[36mFound:\n\x1b[0m'
                         '\x1b[32mGenerating text file for the extracted text..\x1b[0m'
                         'w'
                         None
-                        'File saved in \x1b[33m'
-                        '\x1b[0m as \x1b[32m'
+                        'File saved as \x1b[32m'
                         '\x1b[0m:'
-                        code
-                           argcount  : 1
-                           nlocals   : 2
-                           stacksize : 3
-                           flags     : 19
-                           code 0x970067007c005d047d017c0191028c055300
-                            82           0 RESUME                   0
-                                         2 BUILD_LIST               0
-                                         4 LOAD_FAST                0 (.0)
-                                   >>    6 FOR_ITER                 4 (to 16)
-                                         8 STORE_FAST               1 (i)
-                                        10 LOAD_FAST                1 (i)
-                                        12 LIST_APPEND              2
-                                        14 JUMP_BACKWARD            5 (to 6)
-                                   >>   16 RETURN_VALUE
-                           consts
-                           names      ()
-                           varnames   ('.0', 'i')
-                           freevars   ()
-                           cellvars   ()
-                           filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
-                           name       '<listcomp>'
-                           firstlineno 82
-                           lnotab 0x
                         2
-                        'Press Enter to continue '
-                        'Exiting'
+                        '\x1b[5;97mPress Enter to continue\x1b[0m'
+                        '\nExiting'
                         'Error: '
                         "Could not write to output file '"
                         "'. Reason: "
                         '\x1b[0m'
                         ': '
                         'Error:>>\x1b[31m'
-                     names      ('cv2', 'imread', 'logger', 'info', 'cvtColor', 'COLOR_BGR2GRAY', 'threshold', 'THRESH_BINARY', 'THRESH_OTSU', 'Image', 'fromarray', 'pytesseract', 'image_to_string', 'print', 'os', 'getcwd', 'path', 'join', 'open', 'write', 'enumerate', 'input', 'KeyboardInterrupt', 'sys', 'exit', 'FileNotFoundError', 'error', 'str', 'IOError', 'Exception', 'type', '__name__')
-                     varnames   ('image_path', 'img', 'gray', 'thresh', 'img_pil', 'config', 'text', 'current_path', 'file_path', 'file', 'size', 'e')
+                     names      ('cv2', 'imread', 'logger', 'info', 'cvtColor', 'COLOR_BGR2GRAY', 'threshold', 'THRESH_BINARY', 'THRESH_OTSU', 'Image', 'fromarray', 'pytesseract', 'image_to_string', 'print', 'os', 'getcwd', 'path', 'join', 'open', 'write', 'len', 'input', 'KeyboardInterrupt', 'sys', 'exit', 'FileNotFoundError', 'error', 'str', 'IOError', 'Exception', 'type', '__name__')
+                     varnames   ('image_path', 'img', 'gray', 'thresh', 'img_pil', 'config', 'text', 'current_path', 'file_path', 'file', 'e')
                      freevars   ('OCR_file', 'image_list')
                      cellvars   ()
-                     filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+                     filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                      name       'ocr_text_extraction'
                      firstlineno 47
                      lnotab
                         0x040228023c02020102013e01160136ff0e0102ff0c022802020104012c
-                        02020234011e01260140010201340322012aff2e022201080102ff06ff10
-                        03020332010c01240112011e012e01120166011201220108011cff06ff22
-                        031201900112014eff0802
-                  -3
-                  'txt'
+                        02020234011e01260140010201340322012aff2e0222010aff1002020426
+                        01240112011e012e01120166011201220108011cff06ff22031201900112
+                        014eff0802
+                  -4
+                  '.txt'
                names      ('preprocess',)
                varnames   ('self', 'ocr_text_extraction', 'image_path')
                freevars   ()
                cellvars   ('OCR_file', 'image_list', 'ls')
-               filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+               filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
                name       'OCR'
                firstlineno 40
-               lnotab 0x080128010801080102ff12040c3508011a0118fe
+               lnotab 0x080128010801080102ff12040c3408011a0118fe
             None
          names      ('__name__', '__module__', '__qualname__', '__init__', 'preprocess', 'OCR')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+         filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
          name       'ExtractText'
          firstlineno 20
          lnotab 0x0a0106030610
       'ExtractText'
    names      ('os', 'sys', 'cv2', 'pytesseract', 'PIL', 'Image', 'logging', 'logging.handlers', 'basicConfig', 'INFO', 'getLogger', '__name__', 'logger', 'ExtractText')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/media/skye/Skye/FileMAC/fmac/OCRTextExtractor.py'
+   filename   '/media/skye/skye/FileMAC/filemac/OCRTextExtractor.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108010801080108010c01080108022e0120020208
```

### Comparing `filemac-1.0.1/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/Simple_v_Analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/__pycache__/colors.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/colors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/__pycache__/converter.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/converter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/__pycache__/formats.cpython-311.pyc` & `filemac-1.0.2/filemac/__pycache__/formats.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/colors.py` & `filemac-1.0.2/filemac/colors.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/converter.py` & `filemac-1.0.2/filemac/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,36 +547,44 @@
                 conn.close()
             except KeyboardInterrupt:
                 print("\nExiting")
                 sys.exit(1)
             except Exception as e:
                 logger.error(f"{e}")
 
+###############################################################################
+# Create image objects from given files
+###############################################################################
     def doc2image(self, outf="png"):
         outf_list = ['png', 'jpg']
         if outf not in outf_list:
             outf = "png"
         path_list = self.preprocess()
-        ls = ["pdf"]
+        ls = ["pdf", "doc", "docx"]
         file_list = [
             item for item in path_list if any(item.lower().endswith(ext)
                                               for ext in ls)]
+        imgs = []
         for file in file_list:
             if file.lower().endswith("pdf"):
                 # Convert the PDF to a list of PIL image objects
                 print("Generate image objects ..")
                 images = convert_from_path(file)
 
                 # Save each image to a file
                 fname = file[:-4]
                 print(f"{YELLOW}Target images{BLUE} {len(images)}{RESET}")
                 for i, image in enumerate(images):
                     print(f"{DBLUE}{i}{RESET}", end="\r")
-                    image.save(f"{fname}_{i+1}.{outf}")
-                print(f"{GREEN}mOk{RESET}")
+                    yd = f"{fname}_{i+1}.{outf}"
+                    image.save(yd)
+                    imgs.append(yd)
+            print(f"{GREEN}Ok{RESET}")
+
+        return imgs
 
 
 class Scanner:
 
     def __init__(self, input_file):
         self.input_file = input_file
 
@@ -617,14 +625,30 @@
             print(f"\n{text}")
             print(F"\n{YELLOW}Write text to {GREEN}{out_f}{RESET}")
             with open(out_f, 'w') as f:
                 f.write(text)
 
             print(F"{DGREEN}Ok{RESET}")
 
+    def scanAsImgs(self):
+        file = self.input_file
+        mc = MakeConversion(file)
+        img_objs = mc.doc2image()
+        # print(img_objs)
+        from .OCRTextExtractor import ExtractText
+        text = ''
+        for i in img_objs:
+            extract = ExtractText(i)
+            tx = extract.OCR()
+            if tx is not None:
+                text += tx
+        print(text)
+        print(f"{GREEN}Ok{RESET}")
+        return text
+
 
 class FileSynthesis:
 
     def __init__(self, input_file):
         self.input_file = input_file
         # self.CHUNK_SIZE = 20_000
```

### Comparing `filemac-1.0.1/filemac/fmac.py` & `filemac-1.0.2/filemac/fmac.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,21 @@
         "--resize_image", help=f"change size of an image compress/decompress \
         example {DYELLOW}filemac --resize_image example.png -t png {RESET}")
 
     parser.add_argument("-t_size", help="used in combination with resize_image \
                         to specify target image size")
 
     parser.add_argument(
-        "--scan", help=f"Scan pdf file and extract text\
+        "-S", "--scan", help=f"Scan pdf file and extract text\
                         example {DYELLOW}filemac --scan example.pdf {RESET}")
 
+    parser.add_argument(
+        "-SA", "--scanAsImg", help=f"Scan pdf file and extract text\
+                        example {DYELLOW}filemac --scanAsImg example.pdf {RESET}")
+
     parser.add_argument("--OCR", help=f"Extract text from an image.\
         example {DYELLOW}filemac --OCR image.png{RESET}")
 
     args = parser.parse_args()
 
 
 # Call function to handle document conversion inputs before begining conversion
@@ -186,14 +190,18 @@
         vi.moviepyextract()
 
 # Call module to scan the input and extract text
     elif args.scan:
         sc = Scanner(args.scan)
         sc.scanPDF()
 
+# Call module to scan the input FILE as image object and extract text
+    elif args.scanAsImg:
+        sc = Scanner(args.scanAsImg)
+        tx = sc.scanAsImgs()
 # Call module to handle Candidate images for text extraction inputs before begining conversion
     elif args.OCR:
         conv = ExtractText(args.OCR)
         conv.OCR()
 
     elif args.Analyze_video:
         analyzer = SA(args.Analyze_video)
```

### Comparing `filemac-1.0.1/filemac/formats.py` & `filemac-1.0.2/filemac/formats.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac/image_op.py` & `filemac-1.0.2/filemac/image_op.py`

 * *Files identical despite different names*

### Comparing `filemac-1.0.1/filemac.egg-info/PKG-INFO` & `filemac-1.0.2/filemac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filemac
-Version: 1.0.1
+Version: 1.0.2
 Summary: Open source Python CLI toolkit for conversion, manipulation, Analysis
 Author: wambua
 Author-email: wambuamwiky2001@gmail.com
 License: GPL v3
 Keywords: file-conversion,file-analysis,file-manipulation,ocr,image-conversion
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
@@ -123,15 +123,15 @@
    ```shell
    filemac --convert_image example.png -t jpg
     ```
             ``Supported formats For audio conversion``
                 `1`.JPEG: `.jpg`
                 `2`.PNG": `.png`
                 `3`.GIF": `.gif`
-                `4`.BM":  `bmp`
+                `4`.BM":  `.bmp`
                 `5`.TIFF: `.tiff`
                 `6`.EXR   `.exr`
                 `7`.PDF:  `.pdf`
                 `8`.WebP: `.webp`
                 `9`.ICNS: `.icns`
                 `10`.PSD: `.psd`
                 `11`.SVG: `.svg`
```

### Comparing `filemac-1.0.1/filemac.egg-info/SOURCES.txt` & `filemac-1.0.2/filemac.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.ini
 README.md
 setup.py
 version.txt
+.github/workflows/python-publish.yml
 __pycache__/Analyzer.cpython-311.pyc
 __pycache__/AudioExtractor.cpython-311.pyc
 __pycache__/OCRTextExtractor.cpython-311.pyc
 __pycache__/Simple_v_Analyzer.cpython-311.pyc
 __pycache__/converter.cpython-311.pyc
 __pycache__/formarts.cpython-311.pyc
 __pycache__/formats.cpython-311.pyc
```

### Comparing `filemac-1.0.1/setup.py` & `filemac-1.0.2/setup.py`

 * *Files identical despite different names*

