# Comparing `tmp/organoids-1.1.0.tar.gz` & `tmp/organoids-1.2.0.tar.gz`

## Comparing `organoids-1.1.0.tar` & `organoids-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 organoids-1.1.0/organoids/__main__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 organoids-1.1.0/organoids/utils.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 organoids-1.1.0/organoids/commands/analyze.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 organoids-1.1.0/organoids/commands/segment.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 organoids-1.1.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 organoids-1.1.0/LICENSE
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 organoids-1.1.0/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 organoids-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 organoids-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 organoids-1.2.0/organoids/__main__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 organoids-1.2.0/organoids/utils.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 organoids-1.2.0/organoids/commands/analyze.py
+-rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 organoids-1.2.0/organoids/commands/segment.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 organoids-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 organoids-1.2.0/LICENSE
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 organoids-1.2.0/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 organoids-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 organoids-1.2.0/PKG-INFO
```

### Comparing `organoids-1.1.0/organoids/utils.py` & `organoids-1.2.0/organoids/utils.py`

 * *Files identical despite different names*

### Comparing `organoids-1.1.0/organoids/commands/analyze.py` & `organoids-1.2.0/organoids/commands/analyze.py`

 * *Files identical despite different names*

### Comparing `organoids-1.1.0/organoids/commands/segment.py` & `organoids-1.2.0/organoids/commands/segment.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,20 @@
     pass
 @_segment.command()
 @click.argument("file-or-directory", type=click.Path(exists=True), nargs=-1)
 @click.option("--model", default="facebook/sam-vit-base", help="Model to use for segmentation (default: facebook/sam-vit-base)")
 @click.option("--ext", default=".jpg", help="File extension to search for (default: .jpg)")
 @click.option("--json-ext", default=".json", help="File extension to save meta data to (default: .json)")
 @click.option("--eps", default=0.001, help="Epsilon for polygon approximation (default: .001)")
-def segment(file_or_directory, model, ext, json_ext, eps):
+@click.option("--points-per-crop", default=24, help="Number of points per crop (default: 24)")
+@click.option("--min-size", default=0.001, help="Minimum size of mask as fraction of total area (default: 0.001)")
+@click.option("--max-size", default=0.5, help="Maximum size of mask as fraction of total area (default: 0.5)")
+@click.option("--brightness-threshold", default=1.25, help="Brightness threshold for masks (default: 1.25)")
+@click.option("--regularity-threshold", default=2, help="Regularity threshold for masks (default: 2)")
+def segment(file_or_directory, model, ext, json_ext, eps, points_per_crop, min_size, max_size, brightness_threshold, regularity_threshold):
     start("Scanning for files")
     todo = list(file_or_directory)
     found = []
     while todo:
         file_or_directory = todo.pop()
         if os.path.isfile(file_or_directory) and file_or_directory.endswith(ext):
             found.append(file_or_directory)
@@ -58,27 +63,27 @@
     end()
     start("Segmenting images")
     for entry in tqdm.tqdm(meta, desc="Segmenting images"):
         width = meta[entry]["width"]
         height = meta[entry]["height"]
         print(f"Segmenting {entry}")
         image = PIL.Image.open(entry).convert("RGB")
-        outputs = generator(image, points_per_batch=96, points_per_crop=24)
+        outputs = generator(image, points_per_batch=points_per_crop, points_per_crop=points_per_crop)
         masks = []
         for mask in outputs["masks"]:
             if any(row[0] for row in mask) or any(row[-1] for row in mask):
                 print("Skipping as mask touches left or right image border")
                 continue
             masked = sum(1 for row in mask for pixel in row if pixel)
             total = sum(len(row) for row in mask)
-            if masked/total < 0.001:
-                print(f"Skipping as mask is less than 0.1% of total area: {masked/total*100}%")
+            if masked/total < min_size:
+                print(f"Skipping as mask is less than {min_size*100}% of total area: {masked/total*100}%")
                 continue
-            if masked/total > 0.50:
-                print(f"Skipping as mask is more than 50% of total area: {masked/total*100}%")
+            if masked/total > max_size:
+                print(f"Skipping as mask is more than {max_size*100}% of total area: {masked/total*100}%")
                 continue
             print(f"Mask is {masked/total*100}% of total area")
             masks.append(mask)
         super_masks = []
         for i, m1 in enumerate(masks):
             for j, m2 in enumerate(masks):
                 if i != j and m2[m1].all():
@@ -88,28 +93,28 @@
                 super_masks.append(m1)
         polygons = []
         for mask in super_masks:
             image_pixels = np.array(image)
             masked_pixels = image_pixels[mask]
             masked_pixels_mean = masked_pixels.mean()
             image_pixels_mean = image_pixels[height//3:2*height//3,width//3:2*width//3].mean()
-            if masked_pixels_mean >= 1.25*image_pixels_mean:
-                print(f"Skipping as mask is too bright: {masked_pixels_mean} vs ")
+            if masked_pixels_mean > brightness_threshold*image_pixels_mean:
+                print(f"Skipping as mask is too bright: {masked_pixels_mean} > {brightness_threshold} * {image_pixels_mean}")
                 continue
             contours, _ = cv2.findContours(mask.astype(np.uint8), cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
             obj = max(contours, key=cv2.contourArea)
             peri = cv2.arcLength(obj, True)
             approx = cv2.approxPolyDP(obj, eps*peri, True)
             approx_x = approx[:,:,0]
             approx_y = approx[:,:,1]
             center, _ = cv2.minEnclosingCircle(approx)
             distances = np.sqrt((approx_x-center[0])**2 + (approx_y-center[1])**2)
             min_dist, max_dist = distances.min(), distances.max()
-            if max_dist > 2*min_dist:
-                print(f"Skipping as mask is too irregular: {max_dist/min_dist}")
+            if max_dist > regularity_threshold*min_dist:
+                print(f"Skipping as mask is too irregular: {max_dist/min_dist} > {regularity_threshold}")
                 continue
             poly = [
                 [int(p[0][0]), int(p[0][1])] for p in approx
             ]
             polygons.append(poly)
         areas = []
         for poly in polygons:
```

### Comparing `organoids-1.1.0/LICENSE` & `organoids-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `organoids-1.1.0/pyproject.toml` & `organoids-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "organoids"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "A segmentation and area estimation for organoids on microscope images."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `organoids-1.1.0/PKG-INFO` & `organoids-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: organoids
-Version: 1.1.0
+Version: 1.2.0
 Summary: A segmentation and area estimation for organoids on microscope images.
 Project-URL: Homepage, https://github.com/schneiderkamplab/organoids
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/organoids/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

