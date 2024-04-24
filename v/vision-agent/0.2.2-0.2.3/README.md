# Comparing `tmp/vision_agent-0.2.2.tar.gz` & `tmp/vision_agent-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.2.tar", max compression
+gzip compressed data, was "vision_agent-0.2.3.tar", max compression
```

## Comparing `vision_agent-0.2.2.tar` & `vision_agent-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-23 16:58:36.558365 vision_agent-0.2.2/LICENSE
--rw-r--r--   0        0        0     5376 2024-04-23 16:58:36.558365 vision_agent-0.2.2/README.md
--rw-r--r--   0        0        0     2099 2024-04-23 16:58:37.110367 vision_agent-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    24235 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7554 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5168 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10197 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      328 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    34979 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/type_defs.py
--rw-r--r--   0        0        0     6434 1970-01-01 00:00:00.000000 vision_agent-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 00:18:30.252870 vision_agent-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5690 2024-04-24 00:18:30.252870 vision_agent-0.2.3/README.md
+-rw-r--r--   0        0        0     2099 2024-04-24 00:18:30.812873 vision_agent-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    25002 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-24 00:18:30.264870 vision_agent-0.2.3/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7554 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5168 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10197 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      328 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    34751 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-24 00:18:30.276870 vision_agent-0.2.3/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 vision_agent-0.2.3/PKG-INFO
```

### Comparing `vision_agent-0.2.2/LICENSE` & `vision_agent-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/README.md` & `vision_agent-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -95,23 +95,26 @@
   ]
 }]
 ```
 
 | Tool | Description |
 | --- | --- |
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
+| ImageCaption| ImageCaption is a tool that can generate a caption for an image. |
 | GroundingDINO | GroundingDINO is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. |
 | GroundingSAM | GroundingSAM is a tool that can detect and segment arbitrary objects with inputs such as category names or referring expressions. |
-| Counter | Counter detects and counts the number of objects in an image given an input such as a category name or referring expression. |
+| DINOv | DINOv is a tool that can detect arbitrary objects with using a referring mask. |
+| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 | Crop | Crop crops an image given a bounding box and returns a file name of the cropped image. |
 | BboxArea | BboxArea returns the area of the bounding box in pixels normalized to 2 decimal places. |
 | SegArea | SegArea returns the area of the segmentation mask in pixels normalized to 2 decimal places. |
 | BboxIoU | BboxIoU returns the intersection over union of two bounding boxes normalized to 2 decimal places. |
 | SegIoU | SegIoU returns the intersection over union of two segmentation masks normalized to 2 decimal places. |
-| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
+| BoxDistance | BoxDistance returns the minimum distance between two bounding boxes normalized to 2 decimal places. |
+| BboxContains | BboxContains returns the intersection of two boxes over the target box area. It is good for check if one box is contained within another box. |
 | ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 | ZeroShotCounting | ZeroShotCounting returns the total number of objects belonging to a single class in a given image |
 | VisualPromptCounting | VisualPromptCounting returns the total number of objects belonging to a single class given an image and visual prompt |
 
 
 It also has a basic set of calculate tools such as add, subtract, multiply and divide.
```

### Comparing `vision_agent-0.2.2/pyproject.toml` & `vision_agent-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.2"
+version = "0.2.3"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.2/vision_agent/agent/agent.py` & `vision_agent-0.2.3/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/agent/easytool.py` & `vision_agent-0.2.3/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.3/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/agent/reflexion.py` & `vision_agent-0.2.3/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.3/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.3/vision_agent/agent/vision_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,15 +424,15 @@
         reflect_model: Optional[Union[LLM, LMM]] = None,
         max_retries: int = 3,
         verbose: bool = False,
         report_progress_callback: Optional[Callable[[str], None]] = None,
     ):
         """VisionAgent constructor.
 
-        Parameters
+        Parameters:
             task_model: the model to use for task decomposition.
             answer_model: the model to use for reasoning and concluding the answer.
             reflect_model: the model to use for self reflection.
             max_retries: maximum number of retries to attempt to complete the task.
             verbose: whether to print more logs.
             report_progress_callback: a callback to report the progress of the agent. This is useful for streaming logs in a web application where multiple VisionAgent instances are running in parallel. This callback ensures that the progress are not mixed up.
         """
@@ -500,14 +500,29 @@
     def chat_with_workflow(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
         reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> Tuple[str, List[Dict]]:
+        """Chat with the vision agent and return the final answer and all tool results.
+
+        Parameters:
+            chat: a conversation in the format of
+                [{"role": "user", "content": "describe your task here..."}].
+            image: the input image referenced in the chat parameter.
+            reference_data: a dictionary containing the reference image and mask. in the
+                format of {"image": "image.jpg", "mask": "mask.jpg}
+            visualize_output: whether to visualize the output.
+
+        Returns:
+            A tuple where the first item is the final answer and the second item is a
+            list of all the tool results. The last item in the tool results also
+            contains the visualized output.
+        """
         question = chat[0]["content"]
         if image:
             question += f" Image name: {image}"
         if reference_data:
             if not (
                 "image" in reference_data
                 and ("mask" in reference_data or "bbox" in reference_data)
```

### Comparing `vision_agent-0.2.2/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.3/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.3/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/image_utils.py` & `vision_agent-0.2.3/vision_agent/image_utils.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/llm/llm.py` & `vision_agent-0.2.3/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/lmm/lmm.py` & `vision_agent-0.2.3/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/tools/prompts.py` & `vision_agent-0.2.3/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/tools/tools.py` & `vision_agent-0.2.3/vision_agent/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,46 +104,39 @@
         }
         resp_data = _send_inference_request(data, "tools")
         resp_data["scores"] = [round(prob, 4) for prob in resp_data["scores"]]
         return resp_data
 
 
 class ImageCaption(Tool):
-    r"""ImageCaption is a tool that can caption an image based on its contents
-    or tags.
+    r"""ImageCaption is a tool that can caption an image based on its contents or tags.
 
     Example
     -------
         >>> import vision_agent as va
         >>> caption = va.tools.ImageCaption()
         >>> caption("image1.jpg")
         {'text': ['a box of orange and white socks']}
     """
 
     name = "image_caption_"
-    description = "'image_caption_' is a tool that can caption an image based on its contents or tags. It returns a text describing the image"
+    description = "'image_caption_' is a tool that can caption an image based on its contents or tags. It returns a text describing the image."
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
         ],
         "examples": [
             {
-                "scenario": "Can you describe this image ? Image name: cat.jpg",
+                "scenario": "Can you describe this image? Image name: cat.jpg",
                 "parameters": {"image": "cat.jpg"},
             },
             {
-                "scenario": "Can you caption this image with their main contents ? Image name: cat_dog.jpg",
+                "scenario": "Can you caption this image with their main contents? Image name: cat_dog.jpg",
                 "parameters": {"image": "cat_dog.jpg"},
             },
-            {
-                "scenario": "Can you build me a image captioning tool ? Image name: shirts.jpg",
-                "parameters": {
-                    "image": "shirts.jpg",
-                },
-            },
         ],
     }
 
     # TODO: Add support for input multiple images, which aligns with the output type.
     def __call__(self, image: Union[str, ImageType]) -> Dict:
         """Invoke the Image captioning model.
 
@@ -483,23 +476,23 @@
 
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
         ],
         "examples": [
             {
-                "scenario": "Can you count the lids in the image ? Image name: lids.jpg",
+                "scenario": "Can you count the lids in the image? Image name: lids.jpg",
                 "parameters": {"image": "lids.jpg"},
             },
             {
-                "scenario": "Can you count the total number of objects in this image ? Image name: tray.jpg",
+                "scenario": "Can you count the total number of objects in this image? Image name: tray.jpg",
                 "parameters": {"image": "tray.jpg"},
             },
             {
-                "scenario": "Can you build me an object counting tool ? Image name: shirts.jpg",
+                "scenario": "Can you build me an object counting tool? Image name: shirts.jpg",
                 "parameters": {
                     "image": "shirts.jpg",
                 },
             },
         ],
     }
```

### Comparing `vision_agent-0.2.2/vision_agent/tools/video.py` & `vision_agent-0.2.3/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/vision_agent/type_defs.py` & `vision_agent-0.2.3/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.2/PKG-INFO` & `vision_agent-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.2
+Version: 0.2.3
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -122,23 +122,26 @@
   ]
 }]
 ```
 
 | Tool | Description |
 | --- | --- |
 | CLIP | CLIP is a tool that can classify or tag any image given a set of input classes or tags. |
+| ImageCaption| ImageCaption is a tool that can generate a caption for an image. |
 | GroundingDINO | GroundingDINO is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. |
 | GroundingSAM | GroundingSAM is a tool that can detect and segment arbitrary objects with inputs such as category names or referring expressions. |
-| Counter | Counter detects and counts the number of objects in an image given an input such as a category name or referring expression. |
+| DINOv | DINOv is a tool that can detect arbitrary objects with using a referring mask. |
+| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 | Crop | Crop crops an image given a bounding box and returns a file name of the cropped image. |
 | BboxArea | BboxArea returns the area of the bounding box in pixels normalized to 2 decimal places. |
 | SegArea | SegArea returns the area of the segmentation mask in pixels normalized to 2 decimal places. |
 | BboxIoU | BboxIoU returns the intersection over union of two bounding boxes normalized to 2 decimal places. |
 | SegIoU | SegIoU returns the intersection over union of two segmentation masks normalized to 2 decimal places. |
-| ExtractFrames | ExtractFrames extracts frames with motion from a video. |
+| BoxDistance | BoxDistance returns the minimum distance between two bounding boxes normalized to 2 decimal places. |
+| BboxContains | BboxContains returns the intersection of two boxes over the target box area. It is good for check if one box is contained within another box. |
 | ExtractFrames | ExtractFrames extracts frames with motion from a video. |
 | ZeroShotCounting | ZeroShotCounting returns the total number of objects belonging to a single class in a given image |
 | VisualPromptCounting | VisualPromptCounting returns the total number of objects belonging to a single class given an image and visual prompt |
 
 
 It also has a basic set of calculate tools such as add, subtract, multiply and divide.
```

