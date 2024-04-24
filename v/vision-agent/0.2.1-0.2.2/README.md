# Comparing `tmp/vision_agent-0.2.1.tar.gz` & `tmp/vision_agent-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.1.tar", max compression
+gzip compressed data, was "vision_agent-0.2.2.tar", max compression
```

## Comparing `vision_agent-0.2.1.tar` & `vision_agent-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-22 21:17:07.433079 vision_agent-0.2.1/LICENSE
--rw-r--r--   0        0        0     5376 2024-04-22 21:17:07.433079 vision_agent-0.2.1/README.md
--rw-r--r--   0        0        0     2099 2024-04-22 21:17:07.993080 vision_agent-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    23588 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-22 21:17:07.445079 vision_agent-0.2.1/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7555 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5168 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10197 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      328 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-22 21:17:07.453079 vision_agent-0.2.1/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    34979 2024-04-22 21:17:07.457079 vision_agent-0.2.1/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-22 21:17:07.457079 vision_agent-0.2.1/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-22 21:17:07.457079 vision_agent-0.2.1/vision_agent/type_defs.py
--rw-r--r--   0        0        0     6434 1970-01-01 00:00:00.000000 vision_agent-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 16:58:36.558365 vision_agent-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5376 2024-04-23 16:58:36.558365 vision_agent-0.2.2/README.md
+-rw-r--r--   0        0        0     2099 2024-04-23 16:58:37.110367 vision_agent-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4526 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    24235 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     7342 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:58:36.570365 vision_agent-0.2.2/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7554 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5168 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10197 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      328 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    34979 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-23 16:58:36.582365 vision_agent-0.2.2/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     6434 1970-01-01 00:00:00.000000 vision_agent-0.2.2/PKG-INFO
```

### Comparing `vision_agent-0.2.1/LICENSE` & `vision_agent-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/README.md` & `vision_agent-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/pyproject.toml` & `vision_agent-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.1"
+version = "0.2.2"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.1/vision_agent/agent/agent.py` & `vision_agent-0.2.2/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/agent/easytool.py` & `vision_agent-0.2.2/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.2/vision_agent/agent/easytool_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/agent/reflexion.py` & `vision_agent-0.2.2/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.2/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.2/vision_agent/agent/vision_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 import tempfile
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 from PIL import Image
 from tabulate import tabulate
 
-from vision_agent.image_utils import overlay_bboxes, overlay_masks, overlay_heat_map
+from vision_agent.image_utils import (
+    convert_to_b64,
+    overlay_bboxes,
+    overlay_heat_map,
+    overlay_masks,
+)
 from vision_agent.llm import LLM, OpenAILLM
 from vision_agent.lmm import LMM, OpenAILMM
 from vision_agent.tools import TOOLS
 
 from .agent import Agent
 from .easytool_prompts import (
     ANSWER_GENERATE,
@@ -477,14 +482,25 @@
         )
 
     def log_progress(self, description: str) -> None:
         _LOGGER.info(description)
         if self.report_progress_callback:
             self.report_progress_callback(description)
 
+    def _report_visualization_via_callback(
+        self, images: Sequence[Union[str, Path]]
+    ) -> None:
+        """This is intended for streaming the visualization images via the callback to the client side."""
+        if self.report_progress_callback:
+            self.report_progress_callback("<VIZ>")
+            if images:
+                for img in images:
+                    self.report_progress_callback(f"<IMG>{convert_to_b64(img)}</IMG>")
+            self.report_progress_callback("</VIZ>")
+
     def chat_with_workflow(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
         reference_data: Optional[Dict[str, str]] = None,
         visualize_output: Optional[bool] = False,
     ) -> Tuple[str, List[Dict]]:
@@ -573,17 +589,20 @@
                 reflections += "\n" + parsed_reflection["Reflection"]
         # '<ANSWER>' is a symbol to indicate the end of the chat, which is useful for streaming logs.
         self.log_progress(
             f"The Vision Agent has concluded this chat. <ANSWER>{final_answer}</ANSWER>"
         )
 
         if visualize_output:
-            visualized_output = all_tool_results[-1]["visualized_output"]
-            for image in visualized_output:
-                Image.open(image).show()
+            viz_images: Sequence[Union[str, Path]] = all_tool_results[-1][
+                "visualized_output"
+            ]
+            self._report_visualization_via_callback(viz_images)
+            for img in viz_images:
+                Image.open(img).show()
 
         return final_answer, all_tool_results
 
     def chat(
         self,
         chat: List[Dict[str, str]],
         image: Optional[Union[str, Path]] = None,
```

### Comparing `vision_agent-0.2.1/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.2/vision_agent/agent/vision_agent_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.2/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/image_utils.py` & `vision_agent-0.2.2/vision_agent/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utility functions for image processing."""
 
 import base64
 from importlib import resources
 from io import BytesIO
 from pathlib import Path
-from typing import Dict, Tuple, Union, List
+from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 from PIL.Image import Image as ImageType
 
 COLORS = [
     (158, 218, 229),
@@ -104,15 +104,15 @@
     """
     if data is None:
         raise ValueError(f"Invalid input image: {data}. Input image can't be None.")
     if isinstance(data, (str, Path)):
         data = Image.open(data)
     if isinstance(data, Image.Image):
         buffer = BytesIO()
-        data.convert("RGB").save(buffer, format="JPEG")
+        data.convert("RGB").save(buffer, format="PNG")
         return base64.b64encode(buffer.getvalue()).decode("utf-8")
     else:
         arr_bytes = data.tobytes()
         return base64.b64encode(arr_bytes).decode("utf-8")
 
 
 def denormalize_bbox(
```

### Comparing `vision_agent-0.2.1/vision_agent/llm/llm.py` & `vision_agent-0.2.2/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/lmm/lmm.py` & `vision_agent-0.2.2/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/tools/prompts.py` & `vision_agent-0.2.2/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/tools/tools.py` & `vision_agent-0.2.2/vision_agent/tools/tools.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/tools/video.py` & `vision_agent-0.2.2/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/vision_agent/type_defs.py` & `vision_agent-0.2.2/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.1/PKG-INFO` & `vision_agent-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.1
+Version: 0.2.2
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

