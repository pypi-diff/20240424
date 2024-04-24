# Comparing `tmp/superb-ai-apps-0.0.4.tar.gz` & `tmp/superb-ai-apps-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superb-ai-apps-0.0.4.tar", last modified: Thu Apr 11 13:22:34 2024, max compression
+gzip compressed data, was "superb-ai-apps-0.0.5.tar", last modified: Wed Apr 24 05:27:41 2024, max compression
```

## Comparing `superb-ai-apps-0.0.4.tar` & `superb-ai-apps-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13943 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/curate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/curate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/curate/superb_curate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/label/superb_label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/spb_apps/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-11 13:22:20.000000 superb-ai-apps-0.0.4/spb_apps/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:22:34.591714 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:22:34.000000 superb-ai-apps-0.0.4/superb_ai_apps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/curate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/curate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/curate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13369 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/superb_curate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14887 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/superb_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/spb_apps/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-04-24 05:27:26.000000 superb-ai-apps-0.0.5/spb_apps/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:27:41.199214 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 05:27:41.000000 superb-ai-apps-0.0.5/superb_ai_apps.egg-info/top_level.txt
```

### Comparing `superb-ai-apps-0.0.4/setup.py` & `superb-ai-apps-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="superb-ai-apps",
-    version="0.0.4",
+    version="0.0.5",
     description="Python Package for Superb-AI Apps",
     install_requires=[
         "asttokens==2.4.1",
         "attrs==23.2.0",
         "backcall==0.2.0",
         "beautifulsoup4==4.12.3",
         "bleach==6.1.0",
```

### Comparing `superb-ai-apps-0.0.4/spb_apps/apps.py` & `superb-ai-apps-0.0.5/spb_apps/superb_curate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,347 +1,363 @@
-from typing import Dict, List, Tuple
+import json
+import os
+import time
+from pathlib import Path
+from timeit import default_timer as timer
+from typing import List, Tuple
+from uuid import uuid4
+
+import requests
+import spb_curate
+from spb_curate.error import ConflictError
 
-from spb_label import sdk as spb_label
-
-from spb_apps.curate.superb_curate import SuperbCurate
-from spb_apps.label.superb_label import SuperbLabel
+from spb_apps.apps import SuperbApps
 from spb_apps.utils.converter import convert_yolo_bbox
-from spb_apps.utils.utils import read_info_from_zip_yolo
+from spb_apps.utils.utils import separate_batches
+
+SLEEP_INTERVAL = 5  # Time in seconds to wait between loop iterations.
 
 
-class SuperbApps:
+class SuperbCurate(SuperbApps):
     """
-    This class manages interactions with Superb applications, specifically Label and Curate platforms.
-    It provides functionalities to download images, upload images and annotations, change project contexts,
-    and more, based on the specified platform.
+    A class to handle dataset curation tasks including image and annotation uploads for Superb AI.
+
+    Attributes:
+        team_name (str): Name of the team.
+        access_key (str): Access key for authentication.
+        dataset_name (str): Name of the dataset.
+        is_dev (bool): Flag to set the environment to development mode.
     """
 
     def __init__(
         self,
         team_name: str,
         access_key: str,
-        platform: str,
-        dev: bool = False,
-        project_id: str = "",
-        project_name: str = "",
         dataset_name: str = "",
+        is_dev: bool = False,
     ):
         """
-        Initializes the SuperbApps instance with necessary details and sets up clients for the specified platform.
+        Initializes the SuperbCurate class with team, dataset, and slice details.
+        Optionally sets the environment to development mode.
 
         Args:
-            team_name (str): The name of the team.
-            access_key (str): The access key for authentication.
-            platform (str): The platform to initialize (either 'label' or 'curate').
-            dev (bool, optional): Flag to indicate if this is a development instance. Defaults to False.
-            project_id (str, optional): The ID of the project for labeling. Only required for 'label' platform. Defaults to "".
-            project_name (str, optional): The name of the project for labeling. Only required for 'label' platform. Defaults to "".
-            dataset_name (str, optional): The name of the dataset for Curate. Only required for 'curate' platform. Defaults to "".
-        """
-        self.team_name = team_name
-        self.access_key = access_key
-        platform = platform.lower()
-        if platform == "label":
-            self.client = SuperbLabel(
-                team_name=team_name,
-                access_key=access_key,
-                project_id=project_id,
-                project_name=project_name,
-            )
-
-            self.label_project_name = self.client.client._project.name
-        if platform == "curate":
-            self.client = SuperbCurate(
-                team_name=team_name,
-                access_key=access_key,
-                dataset_name=dataset_name,
-                is_dev=dev,
-            )
-            self.dataset_name = dataset_name
-        self.platform = platform
+            team_name (str): Name of the team.
+            access_key (str): Access key for authentication.
+            dataset_name (str, optional): Name of the dataset.
+            is_dev (bool, optional): Flag to set the environment to development mode.
+        """
+        super().__init__(team_name, access_key)
+        self.team_name: str = team_name
+        self.access_key: str = access_key
+        self.dataset_name: str = dataset_name
+        spb_curate.team_name = self.team_name
+        spb_curate.access_key = self.access_key
+        if is_dev:
+            spb_curate.api_base = "https://api.dev.superb-ai.com"
+
+        if dataset_name:
+            try:
+                self.dataset = spb_curate.fetch_dataset(name=dataset_name)
+            except ConflictError:
+                print(
+                    f"Dataset does not exist, Creating Dataset {dataset_name}"
+                )
+                self.dataset = spb_curate.create_dataset(
+                    name=dataset_name, description="Demo dataset."
+                )
 
-    def download_image_by_key(self, data_key: str, path: str = None):
+    def get_slice(self, slice_name: str):
         """
-        Downloads an image using its unique data key.
+        Fetches a slice from the dataset using its name.
 
         Args:
-            data_key (str): The unique identifier for the image.
-            path (str, optional): The local file path to save the downloaded image. Defaults to None.
+            slice_name (str): Name of the slice to fetch.
+
+        Returns:
+            The fetched slice object.
         """
-        if self.platform == "label":
-            _, label = self.client.get_labels(data_key=data_key)
-            self.client.download_image(label=label[0], path=path)
-        if self.platform == "curate":
-            self.client.download_image(data_key=data_key, download_path=path)
+        if slice_name:
+            slice = self.dataset.fetch_slice(name=slice_name)
+        return slice
 
-    def download_image_by_filter(
-        self,
-        tags: list = [],
-        data_key: str = "",
-        status: list = [],
-        path: str = None,
-    ):
+    def curate_prep_images(self, images_path: list) -> List[spb_curate.Image]:
         """
-        Downloads images by applying filters such as tags, data key, and status.
+        Prepares local images for Superb Curate by creating a list of Superb Curate images.
 
         Args:
-            tags (list, optional): A list of tags to filter images. Defaults to [].
-            data_key (str, optional): A specific data key to filter images. Defaults to "".
-            status (list, optional): A list of statuses to filter images. Defaults to [].
-            path (str, optional): The local file path to save the downloaded images. Defaults to None.
-        """
-        from concurrent.futures import ThreadPoolExecutor
+            images_path (list): List of paths to images to be uploaded.
 
-        if self.platform == "label":
+        Returns:
+            List[spb_curate.Image]: List of prepared images for upload.
+        """
+        curate_images: List[spb_curate.Image] = []
+        for image in images_path:
+            curate_images.append(
+                spb_curate.Image(
+                    key=image.split("/")[-1],
+                    source=spb_curate.ImageSourceLocal(asset=image),
+                    metadata={},
+                )
+            )
 
-            def download(label):
-                self.client.download_image(label=label, path=path)
+        return curate_images
 
-            count, labels = self.client.get_labels(
-                tags=tags, data_key=data_key, status=status
-            )
-            print(f"Downloading {count} data to {path}")
-            if count > 50:
-                with ThreadPoolExecutor(max_workers=4) as executor:
-                    executor.map(download, labels)
-            else:
-                for label in labels:
-                    download(label)
-        else:
-            print("Curate does not support filters for downloading images.")
-
-    def get_width_height(
-        self, data_hanler: spb_label.DataHandle = None, data_key: str = ""
-    ) -> Tuple[int, int]:
+    def upload_images(self, image_path: list):
         """
-        Retrieves the width and height of an image based on its data key.
+        Uploads images in batches to the dataset.
 
         Args:
-            data_hanler (spb_label.DataHandle, optional): The data handler object for 'label' platform. Defaults to None.
-            data_key (str, optional): The unique identifier for the image for 'curate' platform. Defaults to "".
-
-        Returns:
-            Tuple[int, int]: A tuple containing the width and height of the image.
+            image_path (list): List of image paths to upload.
         """
-        if self.platform == "label":
-            if data_hanler is None:
+        separated_images = separate_batches(
+            image_batch_size=500, to_batch_list=image_path
+        )
+        total_loops = len(separated_images)
+        for idx, sep_images in enumerate(separated_images, start=1):
+            curate_images = self.curate_prep_images(images_path=sep_images)
+            image_import_job = spb_curate.Image.create_bulk(
+                dataset_id=self.dataset["id"], images=curate_images
+            )
+
+            print(f"created an image import job: ({idx}/{total_loops})")
+            start_time = timer()
+
+            while True:
+                image_import_job = spb_curate.Job.fetch(
+                    id=image_import_job["id"]
+                )
                 print(
-                    "Label platform requires a data handler object from spb_label."
+                    f"job progress: {image_import_job['progress']}", end="\r"
                 )
-                return
-            return self.client.get_width_height(label=data_hanler)
-        if self.platform == "curate":
-            if data_key == "":
-                print("Curate platform requires a data key.")
-                return
-            return self.client.get_width_height(data_key=data_key)
 
-    def get_labels(
-        self,
-        data_key: str = "",
-        tags: list = [],
-        assignees: list = [],
-        status: list = [],
-        all: bool = False,
-    ) -> Tuple[int, List]:
-        """
-        Retrieves labels based on filters or all labels if specified.
+                if image_import_job["status"] == "COMPLETE":
+                    if image_import_job["result"]["fail_detail"]:
+                        print(image_import_job["result"]["fail_detail"])
+                        print(image_import_job["fail_reason"])
+                    break
+
+                if image_import_job["status"] == "FAILED":
+                    if image_import_job["result"]["fail_detail"]:
+                        print(
+                            "[INFO] Fail detail: ",
+                            image_import_job["result"]["fail_detail"],
+                        )
+                        print(
+                            "[INFO] Fail reason: ",
+                            image_import_job["fail_reason"],
+                        )
+                    break
+                time.sleep(SLEEP_INTERVAL)
+
+            print(f"total time: {timer() - start_time}")
+
+    def curate_prep_annotations(self, annotation: list) -> List:
+        """
+        Prepares annotations for upload by creating a list of spb_curate.Annotation objects.
 
         Args:
-            data_key (str, optional): A data key to filter labels. Defaults to "".
-            tags (list, optional): A list of tags to filter labels. Defaults to [].
-            assignees (list, optional): A list of assignees to filter labels. Defaults to [].
-            status (list, optional): A list of statuses to filter labels. Defaults to [].
-            all (bool, optional): If True, retrieves all labels ignoring other filters. Defaults to False.
+            annotation (list): List of dictionaries containing annotation details.
 
         Returns:
-            Tuple[int, List]: A tuple containing the count of labels and a list of labels.
+            List[spb_curate.Annotation]: List of prepared annotations for upload.
         """
-        count, labels = self.client.get_labels(
-            data_key=data_key,
-            tags=tags,
-            assignees=assignees,
-            status=status,
-            all=all,
-        )
+        curate_annotations: List[spb_curate.Annotation] = []
+        for anno in annotation:
+            meta = anno.get("metadata", {"iscrowd": 0})
+            curate_annotations.append(
+                spb_curate.Annotation(
+                    image_key=anno["data_key"],
+                    annotation_class=anno["class_name"],
+                    annotation_type=anno["annotation_type"],
+                    annotation_value=anno["annotation"],
+                    metadata=meta,
+                )
+            )
 
-        return count, labels
+        return curate_annotations
 
-    def change_project(self, project_name: str):
+    def curate_upload_annotations(self, annotation_list: list):
         """
-        Changes the project context for the label client.
+        Uploads annotations in batches to the dataset.
 
         Args:
-            project_name (str): The name of the project to switch to.
+            annotation_list (list): List of annotations to upload.
         """
-        if self.platform == "label":
-            self.client.client.set_project(name=project_name)
-            self.label_project_name = self.client.client._project.name
-        else:
-            print("Curate platform does not support changing projects.")
+        separated_annotations = separate_batches(
+            image_batch_size=500, to_batch_list=annotation_list
+        )
+        for idx, sep_annotations in enumerate(separated_annotations, start=1):
+            annotation_import_job = spb_curate.Annotation.create_bulk(
+                dataset_id=self.dataset["id"], annotations=sep_annotations
+            )
+
+            while True:
+                annotation_import_job = spb_curate.Job.fetch(
+                    id=annotation_import_job["id"]
+                )
+                print(
+                    f"[INFO] {(idx-1) * 500 + annotation_import_job['progress']} / {len(annotation_list)} annotations updated"
+                )
+
+                if annotation_import_job["status"] == "COMPLETE":
+                    if annotation_import_job["result"]["fail_detail"]:
+                        print(
+                            "[INFO] Fail detail: ",
+                            annotation_import_job["result"]["fail_detail"],
+                        )
+                        print(
+                            "[INFO] Fail reason: ",
+                            annotation_import_job["fail_reason"],
+                        )
+                    break
 
-    def get_label_interface(self) -> Dict:
+                if annotation_import_job["status"] == "FAILED":
+                    if annotation_import_job["result"]["fail_detail"]:
+                        print(
+                            "[INFO] Fail detail: ",
+                            annotation_import_job["result"]["fail_detail"],
+                        )
+                        print(
+                            "[INFO] Fail reason: ",
+                            annotation_import_job["fail_reason"],
+                        )
+                    break
+                time.sleep(SLEEP_INTERVAL)
+
+    def get_width_height(self, data_key: str) -> Tuple[int, int]:
         """
-        Retrieves the label interface configuration for the 'label' platform.
+        Fetches the width and height of an image using its data key.
+
+        Args:
+            data_key (str): The unique identifier for the image.
 
         Returns:
-            Dict: The label interface configuration, or prints a message if the platform is 'curate'.
+            Tuple[int, int]: A tuple containing the width and height of the image.
         """
-        if self.platform == "label":
-            lb_interface = self.client.client.project.label_interface
-            return lb_interface
-        else:
-            print(
-                "Curate platform does not support label interface retrieval."
-            )
+        image = self.dataset.fetch_images(key=data_key)[0]
+        meta = image["metadata"]
+        width, height = meta["_width"], meta["_height"]
+        return width, height
 
-    def make_bbox(self, class_name: str, annotation: list, data_key: str = ""):
+    def download_image(self, data_key: str, path: str = ""):
         """
-        Creates a bounding box based on the specified platform ('label' or 'curate').
+        Downloads an image from the dataset using its data key.
 
         Args:
-            class_name (str): The class name associated with the bounding box.
-            annotation (list): A list containing the x, y coordinates, width, and height of the bounding box.
-            data_key (str, optional): The unique identifier for the image. Required for 'curate' platform.
-
-        Returns:
-            The result of the bounding box setting operation, which varies by platform.
+            data_key (str): The unique identifier for the image.
+            path (str): The path where the image will be downloaded.
         """
-        if self.platform == "label":
-            return self.client.bbox_setting(
-                class_name=class_name, annotation=annotation
+        image_url = self.dataset.fetch_images(
+            key=data_key, include_image_url=True
+        )[0]["image_url"]
+        try:
+            response = requests.get(image_url)
+            response.raise_for_status()
+            os.makedirs(
+                os.path.dirname(os.path.join(path, data_key)),
+                exist_ok=True,
             )
-        if self.platform == "curate":
-            if data_key == "":
-                print("To make a Curate bbox, you must provide a data_key.")
-                return
-            return self.client.bbox_setting(
-                data_key=data_key, class_name=class_name, annotation=annotation
+            with open(os.path.join(path, data_key), "wb") as f:
+                f.write(response.content)
+            print(
+                f"[INFO] Image downloaded successfully: {os.path.join(path, data_key)}"
             )
+        except requests.exceptions.RequestException as e:
+            print(f"[ERROR] Failed to download image: {e}")
 
-    def upload_images(self, images_path: str, dataset_name: str = ""):
+    def make_bbox_annotation(
+        self, data_key: str, class_name: str, annotation: list
+    ) -> spb_curate.Annotation:
         """
-        Uploads images to the specified platform ('label' or 'curate').
+        Creates a bounding box annotation for a given image.
 
         Args:
-            images_path (str): The path to the images to be uploaded.
-            dataset_name (str, optional): The name of the dataset to upload the images to. Required for 'label' platform.
+            data_key (str): The unique identifier for the image.
+            class_name (str): The class name associated with the bounding box.
+            annotation (list): A list containing the x, y coordinates, width, and height of the bounding box.
 
         Returns:
-            The result of the image upload operation, which varies by platform.
+            spb_curate.Annotation: An Annotation object representing the bounding box.
         """
-        if self.platform == "label":
-            if dataset_name == "":
-                print(
-                    "Must specify a dataset name when uploading to Label platform."
-                )
-                return
-            return self.client.upload_image(images_path, dataset_name)
-        if self.platform == "curate":
-            return self.client.curate_upload_images(images_path)
-
-    def upload_annotations(
-        self, data_key: str, annotations: list, format: str, classes: list = ""
-    ) -> str:
-        """
-        Uploads annotations to the specified platform ('label' or 'curate') based on the provided format.
+        bounding_box = spb_curate.BoundingBox(
+            raw_data={
+                "x": annotation[0],
+                "y": annotation[1],
+                "width": annotation[2],
+                "height": annotation[3],
+            }
+        )
+        bbox_annotation = spb_curate.Annotation(
+            image_key=data_key,
+            annotation_class=class_name,
+            annotation_type="box",
+            annotation_value=bounding_box,
+            metadata={},
+        )
 
-        Args:
-            data_key (str): The unique identifier for the image or dataset.
-            annotations (list): A list of annotations to be uploaded.
-            format (str): The format of the annotations ('yolo' supported).
-            classes (list, optional): The classes associated with the annotations. Required if format is 'yolo'.
+        return bbox_annotation
 
-        Returns:
-            str: The status of the upload operation ('Completed', 'Skipped', or 'Failed').
+    def download_image_by_slice(self, slice_name: str, download_path: str):
         """
-        status = "Completed"
-        if self.platform == "label":
-            _, label = self.client.get_labels(data_key=data_key)
-            if len(label) == 0:
-                print(
-                    f"[SKIPPED] Data key: {data_key}, does not exist in project {self.label_project_name}"
-                )
-                status = "Skipped"
-                return status
-            data_handler = label[0]
-            if format == "yolo":
-                if classes == "":
-                    print(
-                        "To upload yolo annotations, you must provide classes."
-                    )
-                    status = "Failed"
-                    return status
-                width, height = self.get_width_height(
-                    data_handler=data_handler
-                )
-                converted_annotations = convert_yolo_bbox(
-                    data_key, annotations, classes, width, height
-                )
-                if converted_annotations is not None:
-                    self.client.upload_annotation(
-                        data_handler, converted_annotations
-                    )
-
-        if self.platform == "curate":
-            if format == "yolo":
-                if classes == "":
-                    print(
-                        "To upload yolo annotations, you must provide classes."
-                    )
-                    status = "Failed"
-                    return status
-                bbox_annotation = []
-                try:
-                    width, height = self.get_width_height(data_key=data_key)
-                except:
-                    return "Skipped"
-                converted_annotations = convert_yolo_bbox(
-                    data_key, annotations, classes, width, height
-                )
-                if converted_annotations is not None:
-                    for anno in converted_annotations:
-                        bbox = self.client.bbox_setting(
-                            data_key,
-                            anno[0],
-                            anno[1],
-                        )
-                        bbox_annotation.append(bbox)
+        Downloads all images within a specified slice of the dataset.
 
-                self.client.curate_upload_annotations(bbox_annotation)
+        This method fetches all image keys within a given slice and iteratively
+        downloads each image to the specified download path.
 
-        return status
+        Args:
+            slice_name (str): The name of the slice from which to download images.
+            download_path (str): The local file path where the images will be saved.
+        """
+        slice = self.dataset.fetch_images(
+            slice=slice_name, include_image_url=True
+        )
+        for image in slice:
+            self.download_image(data_key=image["key"], path=download_path)
 
-    def build_label_interface(self, class_list: list, bbox: bool = True):
+    def convert_yolo_bbox_to_platform(
+        self, data_key: str, annotations: list, classes: list = ""
+    ) -> list:
         """
-        Builds the label interface for the 'label' platform based on the provided class list and bbox flag.
+        Converts YOLO format annotations to the platform's bounding box format and creates bounding box annotations.
 
         Args:
-            class_list (list): The list of classes to include in the label interface.
-            bbox (bool, optional): Flag to indicate if bounding boxes should be included. Defaults to True.
+            data_key (str): The unique identifier for the image or dataset.
+            annotations (list): A list of YOLO format annotations to be converted.
+            classes (list, optional): The classes associated with the YOLO annotations. Required if format is 'yolo'.
 
         Returns:
-            The result of the label interface building operation for 'label' platform, or prints a message for 'curate'.
+            list: A list of bounding box annotations created from the converted YOLO annotations.
         """
-        if self.platform == "label":
-            return self.client.build_label_interface_from_yolo(
-                class_list, bbox
-            )
-        else:
-            print(
-                "Curate platform does not support building a Label Interface."
-            )
+
+        if classes == "":
+            print("To convert yolo annotations, you must provide classes.")
+            return []
+        bbox_annotation = []
+        try:
+            width, height = self.get_width_height(data_key=data_key)
+        except:
+            return []
+        converted_annotations = convert_yolo_bbox(
+            data_key, annotations, classes, width, height
+        )
+        if converted_annotations is not None:
+            for anno in converted_annotations:
+                bbox = self.make_bbox_annotation(
+                    data_key,
+                    anno[0],
+                    anno[1],
+                )
+                bbox_annotation.append(bbox)
+
+        return bbox_annotation
 
     def download_image_by_slice(self, slice_name: str, download_path: str):
         """
         Downloads an image by its slice name to a specified path. This method is exclusive to the Curate platform.
 
         Args:
             slice_name (str): The name of the slice from which to download the image.
             download_path (str): The local file path where the downloaded image will be saved.
         """
-        if self.platform == "curate":
-            self.client.download_image_by_slice(
-                slice_name=slice_name, download_path=download_path
-            )
-        else:
-            print("Download by slice is only for Curate platform.")
+        self.download_image_by_slice(
+            slice_name=slice_name, download_path=download_path
+        )
```

### Comparing `superb-ai-apps-0.0.4/spb_apps/utils/converter.py` & `superb-ai-apps-0.0.5/spb_apps/utils/converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-def convert_yolo_bbox(data_key: str, annotations: list, classes: list,  width:int, height: int):
+def convert_yolo_bbox(
+    data_key: str, annotations: list, classes: list, width: int, height: int
+):
     converted_annotations = []
     for anno in annotations:
-        class_number, x_norm, y_norm, w_norm, h_norm = anno[0], anno[1], anno[2], anno[3], anno[4]
+        class_number, x_norm, y_norm, w_norm, h_norm = (
+            anno[0],
+            anno[1],
+            anno[2],
+            anno[3],
+            anno[4],
+        )
         class_name = classes[class_number]
         # Check normalization
         if any(value > 1 for value in (x_norm, y_norm, w_norm, h_norm)):
             print(
                 f"[WARNING] [Invalid zip file] {data_key}.txt\n"
                 + f"[[Class index] [x_center] [y_center] [width] [height]]: [{int(class_number)} {x_norm} {y_norm} {w_norm} {h_norm}]\n"
                 + f" YOLO format coordinates, width, and height must be normalized (0 - 1)."
             )
-            return None
-    
+            return []
+
         w = w_norm * width
         h = h_norm * height
         x = x_norm * width - w / 2
         y = y_norm * height - h / 2
         converted_annotations.append([class_name, [x, y, w, h]])
-    
-    return converted_annotations
+
+    return converted_annotations
```

### Comparing `superb-ai-apps-0.0.4/spb_apps/utils/utils.py` & `superb-ai-apps-0.0.5/spb_apps/utils/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 import json
+import logging
 import os
+import time
 from pathlib import Path
+from typing import Callable, TypeVar, Union
+from uuid import uuid4
 from zipfile import BadZipFile, ZipFile
 
+import requests
 from directory_tree import display_tree
+from spb_label.exceptions import (
+    APIException,
+    BadRequestException,
+    ConflictException,
+    # InvaildObjectException,
+)
+from phy_credit.exceptions import InvalidObjectException
+
+logger = logging.getLogger("superb_label")
 
 
 def separate_batches(image_batch_size: int, to_batch_list: list):
     """
     Separates a list of items into batches of a specified size.
 
     Args:
@@ -188,7 +202,76 @@
         Exception: Re-raises the exception after displaying the error message and extracting the zip file.
     """
     print("[Zip File]")
     with ZipFile(dataset_file, "r") as zip_file:
         zip_file.extractall(path=Path(dataset_file).parent)
         display_tree(str(Path(dataset_file).parent), max_depth=2)
     raise Exception(f"[Invalid zip file] {e}")
+
+
+T = TypeVar("T")
+
+
+def call_with_retry(
+    fn: Callable[..., T],
+    *args,
+    _max_retries: int = 5,
+    _sleep_time: int = 6,
+    **kwargs,
+) -> Union[T, None]:
+    retry_count = 0
+    while retry_count < _max_retries:
+        if retry_count == 0:
+            log_id = str(uuid4()).split("-")[0]
+        try:
+            res = fn(*args, **kwargs)
+            break
+        except requests.HTTPError as e:
+            error_code = e.response.status_code
+            if error_code == 503:  # 503: Service Unavailable
+                logger.warning(
+                    f"({log_id}) 503 Error occured, will be retried || fn: {fn.__name__} || Retry count: {retry_count}"
+                )
+            retry_count += 1
+            time.sleep(_sleep_time)
+        except APIException as e:
+            logger.warning(
+                f"({log_id}) 429 Error occured, will be retried || fn: {fn.__name__} || Retry count: {retry_count}"
+            )
+            retry_count += 1
+            time.sleep(_sleep_time)
+        except InvalidObjectException as e:
+            raise Exception(
+                f"({log_id}) Class name is not vaild, check the class list || fn: {fn.__name__} || Retry count: {retry_count}"
+            )
+        except Exception as e:
+
+            if "429" in e.message:  # 429: too many request
+                logger.error(
+                    f"({log_id}) 429 Error occured, will be retried || fn: {fn.__name__} || Retry count: {retry_count}"
+                )
+                time.sleep(_sleep_time)
+                retry_count += 1
+            elif "503" in e.message:  # 503: too many request
+                logger.error(
+                    f"({log_id}) 503 Error occured, will be retried || fn: {fn.__name__} || Retry count: {retry_count}"
+                )
+                time.sleep(_sleep_time)
+                retry_count += 1
+            else:
+                raise Exception(
+                    f"({log_id}) Unknown error occured, will be retried || fn: {fn.__name__} || Retry count: {retry_count}"
+                )
+        if retry_count > 0:
+            logger.debug(
+                f"({log_id}) Retrying || fn: {fn.__name__} || Retry count: {retry_count}"
+            )
+    if retry_count == _max_retries:
+        raise Exception(
+            f"({log_id}) Max retries reached || fn: {fn.__name__} || Retry count: {retry_count}"
+        )
+    if retry_count > 0:
+        logger.debug(
+            f"({log_id}) Successfully completed || fn: {fn.__name__} || Retry count: {retry_count}"
+        )
+
+    return res
```

### Comparing `superb-ai-apps-0.0.4/superb_ai_apps.egg-info/requires.txt` & `superb-ai-apps-0.0.5/superb_ai_apps.egg-info/requires.txt`

 * *Files identical despite different names*

