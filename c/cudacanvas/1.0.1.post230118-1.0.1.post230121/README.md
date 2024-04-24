# Comparing `tmp/cudacanvas-1.0.1.post230118-cp39-cp39-win_amd64.whl.zip` & `tmp/cudacanvas-1.0.1.post230121-cp38-cp38-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 98712 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     1733 b- defN 24-Apr-24 19:12 cudacanvas/__init__.py
--rw-rw-rw-  2.0 fat   222720 b- defN 24-Apr-24 19:34 cudacanvas/cudaGLStream.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-24 19:34 cudacanvas-1.0.1.post230118.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4228 b- defN 24-Apr-24 19:34 cudacanvas-1.0.1.post230118.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-24 19:34 cudacanvas-1.0.1.post230118.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-24 19:34 cudacanvas-1.0.1.post230118.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      637 b- defN 24-Apr-24 19:34 cudacanvas-1.0.1.post230118.dist-info/RECORD
-7 files, 230514 bytes uncompressed, 97572 bytes compressed:  57.7%
+Zip file size: 2726112 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1688 b- defN 24-Apr-24 19:12 cudacanvas/__init__.py
+-rwxr-xr-x  2.0 unx  9804984 b- defN 24-Apr-24 19:16 cudacanvas/cudaGLStream.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-24 19:16 cudacanvas-1.0.1.post230121.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4073 b- defN 24-Apr-24 19:16 cudacanvas-1.0.1.post230121.dist-info/METADATA
+-rw-r--r--  2.0 unx      111 b- defN 24-Apr-24 19:16 cudacanvas-1.0.1.post230121.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-24 19:16 cudacanvas-1.0.1.post230121.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      650 b- defN 24-Apr-24 19:16 cudacanvas-1.0.1.post230121.dist-info/RECORD
+7 files, 9812581 bytes uncompressed, 2724948 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: cudacanvas/__init__.py
 Comment: 
 
-Filename: cudacanvas/cudaGLStream.cp39-win_amd64.pyd
+Filename: cudacanvas/cudaGLStream.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: cudacanvas-1.0.1.post230118.dist-info/LICENSE
+Filename: cudacanvas-1.0.1.post230121.dist-info/LICENSE
 Comment: 
 
-Filename: cudacanvas-1.0.1.post230118.dist-info/METADATA
+Filename: cudacanvas-1.0.1.post230121.dist-info/METADATA
 Comment: 
 
-Filename: cudacanvas-1.0.1.post230118.dist-info/WHEEL
+Filename: cudacanvas-1.0.1.post230121.dist-info/WHEEL
 Comment: 
 
-Filename: cudacanvas-1.0.1.post230118.dist-info/top_level.txt
+Filename: cudacanvas-1.0.1.post230121.dist-info/top_level.txt
 Comment: 
 
-Filename: cudacanvas-1.0.1.post230118.dist-info/RECORD
+Filename: cudacanvas-1.0.1.post230121.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cudacanvas/__init__.py

 * *Ordering differences only*

```diff
@@ -1,45 +1,45 @@
-try:
-    import torch
-    if not torch.cuda.is_available():
-        raise RuntimeError("Torch with CUDA is required for this module!")
-except ImportError:
-    raise ImportError("Torch is not installed!")
-
-try:
-    import pkg_resources
-    
-    __version__ = pkg_resources.get_distribution("cudacanvas").version
-    # Fetching the CUDA version from PyTorch and formatting the version string
-    torch_version = torch.__version__.split('+')[0].replace(".", "")  # Gets the base version of torch, e.g., '2.2.2'
-    cuda_version = torch.version.cuda.replace(".", "")  # Gets CUDA version, e.g., '118'
-    version_base = torch_version  # Base version now uses the PyTorch version
-
-    full_version = "1.0.1" + ".post" + version_base + cuda_version
-
-    if ( not __version__ == full_version): 
-        print(f'You currently installed Cudacanvas v{__version__} which does not match your torch+cuda version ({torch.__version__})')
-        print(f'try:  \033[92mpip install cudacanvas=={full_version} --force-reinstall\033[0m')
-        print('to see if the required version is available')
-               
-except pkg_resources.DistributionNotFound:
-    # package is not installed
-    __version__ = "unknown"
-
-try:
-    import glfw
-except ImportError:
-    raise ImportError("GLFW is not installed!")
-
-from .cudaGLStream import CudaGLStreamer
-
-# Create a global instance of CudaGLStreamer
-_streamer = CudaGLStreamer()
-
-# Expose methods of CudaGLStreamer at the package level
-set_image = _streamer.set_image
-set_title = _streamer.set_title
-create_window = _streamer.create_window
-im_show = _streamer.im_show
-render = _streamer.render
-should_close = _streamer.should_close
-clean_up = _streamer.clean_up
+try:
+    import torch
+    if not torch.cuda.is_available():
+        raise RuntimeError("Torch with CUDA is required for this module!")
+except ImportError:
+    raise ImportError("Torch is not installed!")
+
+try:
+    import pkg_resources
+    
+    __version__ = pkg_resources.get_distribution("cudacanvas").version
+    # Fetching the CUDA version from PyTorch and formatting the version string
+    torch_version = torch.__version__.split('+')[0].replace(".", "")  # Gets the base version of torch, e.g., '2.2.2'
+    cuda_version = torch.version.cuda.replace(".", "")  # Gets CUDA version, e.g., '118'
+    version_base = torch_version  # Base version now uses the PyTorch version
+
+    full_version = "1.0.1" + ".post" + version_base + cuda_version
+
+    if ( not __version__ == full_version): 
+        print(f'You currently installed Cudacanvas v{__version__} which does not match your torch+cuda version ({torch.__version__})')
+        print(f'try:  \033[92mpip install cudacanvas=={full_version} --force-reinstall\033[0m')
+        print('to see if the required version is available')
+               
+except pkg_resources.DistributionNotFound:
+    # package is not installed
+    __version__ = "unknown"
+
+try:
+    import glfw
+except ImportError:
+    raise ImportError("GLFW is not installed!")
+
+from .cudaGLStream import CudaGLStreamer
+
+# Create a global instance of CudaGLStreamer
+_streamer = CudaGLStreamer()
+
+# Expose methods of CudaGLStreamer at the package level
+set_image = _streamer.set_image
+set_title = _streamer.set_title
+create_window = _streamer.create_window
+im_show = _streamer.im_show
+render = _streamer.render
+should_close = _streamer.should_close
+clean_up = _streamer.clean_up
```

## Comparing `cudacanvas-1.0.1.post230118.dist-info/METADATA` & `cudacanvas-1.0.1.post230121.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,114 @@
-Metadata-Version: 2.1
-Name: cudacanvas
-Version: 1.0.1.post230118
-Summary: Real-time PyTorch Tensor Visualisation in CUDA, Eliminating CPU Transfer
-Home-page: https://github.com/OutofAi/cudacanvas
-Author: Ashleigh Watson & Alex Nasa
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: glfw
-
-<a href="https://www.buymeacoffee.com/outofai" target="_blank"><img src="https://img.shields.io/badge/-buy_me_a%C2%A0coffee-red?logo=buy-me-a-coffee" alt="Buy Me A Coffee"></a>
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40Ashleigh%20Watson)](https://twitter.com/OutofAi) 
-[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40Alex%20Nasa)](https://twitter.com/banterless_ai)
-[![PyPI version](https://badge.fury.io/py/cudacanvas.svg)](https://badge.fury.io/py/cudacanvas)
-[![Downloads](https://static.pepy.tech/badge/cudacanvas)](https://pepy.tech/project/cudacanvas)
-
-![image](https://github.com/OutofAi/cudacanvas/assets/145302363/94f1ba88-0991-4690-b09b-7be480ee34ec)
-
-
-# cudacanvas : PyTorch Tensor Image Display in CUDA
-(Real-time PyTorch Tensor Image Visualisation in CUDA, Eliminating CPU Transfer)
-
-CudaCanvas is a simple Python module that eliminates CPU transfer for Pytorch tensors for displaying and rendering images in the training or evaluation phase, ideal for machine learning scientists and engineers. 
-
-Simplified version that directly displays the image without explicit window creation (cudacanvas >= v1.0.1)
-
-```python
-import torch
-import cudacanvas
-
-
-#REPLACE THIS with you training loop
-while (True):
-
-    #REPLACE THIS with you training code and generation of data
-    noise_image = torch.rand((4, 500, 500), device="cuda")
-
-    #Visualise your data in real-time
-    cudacanvas.im_show(noise_image)
-
-    #OPTIONAL: Terminate training when the window is closed
-    if cudacanvas.should_close():
-        cudacanvas.clean_up()
-        #end process if the window is closed
-        break
-
-
-```
-
-And with explicit window creation
-
-```python
-import torch
-import cudacanvas
-
-noise_image = torch.rand((4, 500, 500), device="cuda")
-
-cudacanvas.set_image(noise_image)
-cudacanvas.create_window()
-
-#replace this with you training loop
-while (True):
-
-    cudacanvas.render()
-
-    if cudacanvas.should_close():
-        cudacanvas.clean_up()
-        #end process if the window is closed
-        break
-
-
-```
-
-
-# Installation
-Before instllation make sure you have torch with cuda support already installed on your machine
-
-We aligned pytorch and cuda version with our package the supporting packages are torch (2.0.1, 2.1.2 and 2.2.2) and (11.8 and 12.1)
-
-Identify your current torch and cuda version
-
-```python
-import torch
-torch.__version__
-```
-
-Depending on your torch and cuda you can install the relevant cudacanvas package, for the latest 2.2.2+cu121 you can simply download the latest package
-```
-pip install cudacanvas
-```
-For other torch and cuda packages put the torch and cuda version after that cudacanvas version for example for 2.1.2+cu118 the Cudacanvas package you require
-is 1.0.1.post212118
-
-```
-pip install cudacanvas==1.0.1.post212118 --force-reinstall
-```
-
-# Support
-Also support my channel ☕ ☕ : https://www.buymeacoffee.com/outofai
-
-
+Metadata-Version: 2.1
+Name: cudacanvas
+Version: 1.0.1.post230121
+Summary: Real-time PyTorch Tensor Visualisation in CUDA, Eliminating CPU Transfer
+Home-page: https://github.com/OutofAi/cudacanvas
+Author: Ashleigh Watson & Alex Nasa
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: glfw
+
+<a href="https://www.buymeacoffee.com/outofai" target="_blank"><img src="https://img.shields.io/badge/-buy_me_a%C2%A0coffee-red?logo=buy-me-a-coffee" alt="Buy Me A Coffee"></a>
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40Ashleigh%20Watson)](https://twitter.com/OutofAi) 
+[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40Alex%20Nasa)](https://twitter.com/banterless_ai)
+[![PyPI version](https://badge.fury.io/py/cudacanvas.svg)](https://badge.fury.io/py/cudacanvas)
+[![Downloads](https://static.pepy.tech/badge/cudacanvas)](https://pepy.tech/project/cudacanvas)
+
+![image](https://github.com/OutofAi/cudacanvas/assets/145302363/94f1ba88-0991-4690-b09b-7be480ee34ec)
+
+
+# cudacanvas : PyTorch Tensor Image Display in CUDA
+(Real-time PyTorch Tensor Image Visualisation in CUDA, Eliminating CPU Transfer)
+
+CudaCanvas is a simple Python module that eliminates CPU transfer for Pytorch tensors for displaying and rendering images in the training or evaluation phase, ideal for machine learning scientists and engineers. 
+
+Simplified version that directly displays the image without explicit window creation (cudacanvas >= v1.0.1)
+
+```python
+import torch
+import cudacanvas
+
+
+#REPLACE THIS with you training loop
+while (True):
+
+    #REPLACE THIS with you training code and generation of data
+    noise_image = torch.rand((4, 500, 500), device="cuda")
+
+    #Visualise your data in real-time
+    cudacanvas.im_show(noise_image)
+
+    #OPTIONAL: Terminate training when the window is closed
+    if cudacanvas.should_close():
+        cudacanvas.clean_up()
+        #end process if the window is closed
+        break
+
+
+```
+
+And with explicit window creation
+
+```python
+import torch
+import cudacanvas
+
+noise_image = torch.rand((4, 500, 500), device="cuda")
+
+cudacanvas.set_image(noise_image)
+cudacanvas.create_window()
+
+#replace this with you training loop
+while (True):
+
+    cudacanvas.render()
+
+    if cudacanvas.should_close():
+        cudacanvas.clean_up()
+        #end process if the window is closed
+        break
+
+
+```
+
+
+# Installation
+Before instllation make sure you have torch with cuda support already installed on your machine
+
+We aligned pytorch and cuda version with our package the supporting packages are torch (2.0.1, 2.1.2 and 2.2.2) and (11.8 and 12.1)
+
+Identify your current torch and cuda version
+
+```python
+import torch
+torch.__version__
+```
+
+Depending on your torch and cuda you can install the relevant cudacanvas package, for the latest 2.2.2+cu121 you can simply download the latest package
+```
+pip install cudacanvas
+```
+For other torch and cuda packages put the torch and cuda version after that cudacanvas version for example for 2.1.2+cu118 the Cudacanvas package you require
+is 1.0.1.post212118
+
+```
+pip install cudacanvas==1.0.1.post212118 --force-reinstall
+```
+
+# Support
+Also support my channel ☕ ☕ : https://www.buymeacoffee.com/outofai
```

### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: cudacanvas Version: 1.0.1.post230118 Summary: Real-
+Metadata-Version: 2.1 Name: cudacanvas Version: 1.0.1.post230121 Summary: Real-
 time PyTorch Tensor Visualisation in CUDA, Eliminating CPU Transfer Home-page:
 https://github.com/OutofAi/cudacanvas Author: Ashleigh Watson & Alex Nasa
-License: UNKNOWN Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Education Classifier: Intended Audience :: Science/
-Research Classifier: License :: OSI Approved :: MIT License Classifier: Topic
-:: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Software Development Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-C++ Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown License-File: LICENSE Requires-Dist: glfw _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][!
-[Twitter](https://img.shields.io/twitter/url/https/twitter.com/
-cloudposse.svg?style=social&label=Follow%20%40Ashleigh%20Watson)](https://
-twitter.com/OutofAi) [![Twitter](https://img.shields.io/twitter/url/https/
-twitter.com/cloudposse.svg?style=social&label=Follow%20%40Alex%20Nasa)](https:/
-/twitter.com/banterless_ai) [![PyPI version](https://badge.fury.io/py/
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Education Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+MIT License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development Classifier: Topic :: Software Development :: Libraries Classifier:
+Topic :: Software Development :: Libraries :: Python Modules Classifier:
+Programming Language :: C++ Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+glfw _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_][![Twitter](https://img.shields.io/twitter/url/https/
+twitter.com/cloudposse.svg?style=social&label=Follow%20%40Ashleigh%20Watson)]
+(https://twitter.com/OutofAi) [![Twitter](https://img.shields.io/twitter/url/
+https/twitter.com/cloudposse.svg?style=social&label=Follow%20%40Alex%20Nasa)]
+(https://twitter.com/banterless_ai) [![PyPI version](https://badge.fury.io/py/
 cudacanvas.svg)](https://badge.fury.io/py/cudacanvas) [![Downloads](https://
 static.pepy.tech/badge/cudacanvas)](https://pepy.tech/project/cudacanvas) !
 [image](https://github.com/OutofAi/cudacanvas/assets/145302363/94f1ba88-0991-
 4690-b09b-7be480ee34ec) # cudacanvas : PyTorch Tensor Image Display in CUDA
 (Real-time PyTorch Tensor Image Visualisation in CUDA, Eliminating CPU
 Transfer) CudaCanvas is a simple Python module that eliminates CPU transfer for
 Pytorch tensors for displaying and rendering images in the training or
```

