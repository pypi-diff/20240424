# Comparing `tmp/qamlib-0.8.0.tar.gz` & `tmp/qamlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qamlib-0.8.0.tar", last modified: Thu Mar  7 13:32:47 2024, max compression
+gzip compressed data, was "qamlib-0.9.0.tar", last modified: Wed Apr 24 12:04:29 2024, max compression
```

## Comparing `qamlib-0.8.0.tar` & `qamlib-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0    16989 2024-03-07 13:22:11.000000 qamlib-0.8.0/.clang-format
--rw-r--r--   0        0        0      276 2024-03-07 13:22:11.000000 qamlib-0.8.0/.gitignore
--rw-r--r--   0        0        0     2413 2024-03-07 13:22:11.000000 qamlib-0.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     4450 2024-03-07 13:22:11.000000 qamlib-0.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0      200 2024-03-07 13:22:11.000000 qamlib-0.8.0/Doxyfile
--rw-r--r--   0        0        0    26530 2024-03-07 13:22:11.000000 qamlib-0.8.0/LICENSE.LGPL2.1
--rw-r--r--   0        0        0       52 2024-03-07 13:22:11.000000 qamlib-0.8.0/MANIFEST.in
--rw-r--r--   0        0        0     1888 2024-03-07 13:22:11.000000 qamlib-0.8.0/README.md
--rw-r--r--   0        0        0       28 2024-03-07 13:22:11.000000 qamlib-0.8.0/compile_flags.txt
--rw-r--r--   0        0        0      326 2024-03-07 13:22:11.000000 qamlib-0.8.0/docker.sh
--rw-r--r--   0        0        0       51 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/changelog.rst
--rw-r--r--   0        0        0      905 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     2556 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/cpp-reference.rst
--rw-r--r--   0        0        0      247 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/index.rst
--rw-r--r--   0        0        0     1622 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/internals.rst
--rw-r--r--   0        0        0     1446 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/reference.rst
--rw-r--r--   0        0        0     1194 2024-03-07 13:22:11.000000 qamlib-0.8.0/docs/usage.rst
--rw-r--r--   0        0        0      699 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/cpp/small_example.cpp
--rw-r--r--   0        0        0      498 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/events.py
--rw-r--r--   0        0        0      708 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/extended_controls.py
--rw-r--r--   0        0        0     1572 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/hdr_capture_and_save.py
--rw-r--r--   0        0        0    14823 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/qamlib_json.py
--rw-r--r--   0        0        0     1493 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/qamlib_json_client.py
--rw-r--r--   0        0        0     1963 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/qamlib_tcp_client.py
--rw-r--r--   0        0        0     3087 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/qamlib_test.py
--rw-r--r--   0        0        0      291 2024-03-07 13:22:11.000000 qamlib-0.8.0/examples/save_to_file.py
--rw-r--r--   0        0        0     5766 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/camera.h
--rw-r--r--   0        0        0     8414 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/control.h
--rw-r--r--   0        0        0     2202 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/device.h
--rw-r--r--   0        0        0     1453 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/event_device.h
--rw-r--r--   0        0        0     2470 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/events.h
--rw-r--r--   0        0        0     4467 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/format.h
--rw-r--r--   0        0        0     1260 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/framerate.h
--rw-r--r--   0        0        0      263 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/meson.build
--rw-r--r--   0        0        0      212 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/qamlib.h
--rw-r--r--   0        0        0     1610 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/streaming_device.h
--rw-r--r--   0        0        0     3139 2024-03-07 13:22:11.000000 qamlib-0.8.0/includes/utils.h
--rw-r--r--   0        0        0     1414 2024-03-07 13:22:11.000000 qamlib-0.8.0/meson.build
--rw-r--r--   0        0        0      119 2024-03-07 13:22:11.000000 qamlib-0.8.0/meson_options.txt
--rw-r--r--   0        0        0     1031 2024-03-07 13:22:11.000000 qamlib-0.8.0/noxfile.py
--rw-r--r--   0        0        0      965 2024-03-07 13:22:11.000000 qamlib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1485 2024-03-07 13:22:11.000000 qamlib-0.8.0/setup.py
--rw-r--r--   0        0        0      351 2024-03-07 13:22:11.000000 qamlib-0.8.0/shell.nix
--rw-r--r--   0        0        0    18515 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/camera.cpp
--rw-r--r--   0        0        0    16828 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/control.cpp
--rw-r--r--   0        0        0    11236 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/device.cpp
--rw-r--r--   0        0        0     3168 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/event_device.cpp
--rw-r--r--   0        0        0     1972 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/events.cpp
--rw-r--r--   0        0        0     6379 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/format.cpp
--rw-r--r--   0        0        0      977 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/framerate.cpp
--rw-r--r--   0        0        0     1119 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/meson.build
--rw-r--r--   0        0        0    37019 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/pymod.cpp
--rw-r--r--   0        0        0     7725 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/streaming_device.cpp
--rw-r--r--   0        0        0      573 2024-03-07 13:22:11.000000 qamlib-0.8.0/src/utils.cpp
--rw-r--r--   0        0        0      352 2024-03-07 13:22:11.000000 qamlib-0.8.0/subprojects/nlohmann_json.wrap
--rw-r--r--   0        0        0      351 2024-03-07 13:22:11.000000 qamlib-0.8.0/subprojects/packagecache/pybind11_json_patch.zip
--rw-r--r--   0        0        0      296 2024-03-07 13:22:11.000000 qamlib-0.8.0/subprojects/pybind11_json.wrap
--rw-r--r--   0        0        0      998 2024-03-07 13:22:11.000000 qamlib-0.8.0/tests/test_events.py
--rw-r--r--   0        0        0      416 2024-03-07 13:22:11.000000 qamlib-0.8.0/tests/test_formats.py
--rw-r--r--   0        0        0     6173 2024-03-07 13:22:11.000000 qamlib-0.8.0/tests/test_long.py
--rw-r--r--   0        0        0    33216 2024-03-07 13:32:47.052604 qamlib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    16989 2024-04-24 12:01:34.000000 qamlib-0.9.0/.clang-format
+-rw-r--r--   0        0        0      190 2024-04-24 12:01:34.000000 qamlib-0.9.0/.clangd
+-rw-r--r--   0        0        0      276 2024-04-24 12:01:34.000000 qamlib-0.9.0/.gitignore
+-rw-r--r--   0        0        0     2413 2024-04-24 12:01:34.000000 qamlib-0.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     4904 2024-04-24 12:01:34.000000 qamlib-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      200 2024-04-24 12:01:34.000000 qamlib-0.9.0/Doxyfile
+-rw-r--r--   0        0        0    26530 2024-04-24 12:01:34.000000 qamlib-0.9.0/LICENSE.LGPL2.1
+-rw-r--r--   0        0        0       52 2024-04-24 12:01:34.000000 qamlib-0.9.0/MANIFEST.in
+-rw-r--r--   0        0        0     1901 2024-04-24 12:01:34.000000 qamlib-0.9.0/README.md
+-rw-r--r--   0        0        0       28 2024-04-24 12:01:34.000000 qamlib-0.9.0/compile_flags.txt
+-rw-r--r--   0        0        0      326 2024-04-24 12:01:34.000000 qamlib-0.9.0/docker.sh
+-rw-r--r--   0        0        0       51 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/changelog.rst
+-rw-r--r--   0        0        0      905 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     2556 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/cpp-reference.rst
+-rw-r--r--   0        0        0      247 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0     1430 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/internals.rst
+-rw-r--r--   0        0        0     1446 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/reference.rst
+-rw-r--r--   0        0        0     1194 2024-04-24 12:01:34.000000 qamlib-0.9.0/docs/usage.rst
+-rw-r--r--   0        0        0      699 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/cpp/small_example.cpp
+-rw-r--r--   0        0        0     3874 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/dual_camera.py
+-rw-r--r--   0        0        0      498 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/events.py
+-rw-r--r--   0        0        0      708 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/extended_controls.py
+-rw-r--r--   0        0        0     1621 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/hdr_capture_and_save.py
+-rw-r--r--   0        0        0    14823 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/qamlib_json.py
+-rw-r--r--   0        0        0     1493 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/qamlib_json_client.py
+-rw-r--r--   0        0        0     1963 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/qamlib_tcp_client.py
+-rw-r--r--   0        0        0     3087 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/qamlib_test.py
+-rw-r--r--   0        0        0      291 2024-04-24 12:01:34.000000 qamlib-0.9.0/examples/save_to_file.py
+-rw-r--r--   0        0        0     5766 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/camera.h
+-rw-r--r--   0        0        0     8681 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/control.h
+-rw-r--r--   0        0        0     2202 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/device.h
+-rw-r--r--   0        0        0     1453 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/event_device.h
+-rw-r--r--   0        0        0     2470 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/events.h
+-rw-r--r--   0        0        0     4467 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/format.h
+-rw-r--r--   0        0        0     1260 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/framerate.h
+-rw-r--r--   0        0        0      263 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/meson.build
+-rw-r--r--   0        0        0      212 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/qamlib.h
+-rw-r--r--   0        0        0     1610 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/streaming_device.h
+-rw-r--r--   0        0        0     4152 2024-04-24 12:01:34.000000 qamlib-0.9.0/includes/utils.h
+-rw-r--r--   0        0        0     1414 2024-04-24 12:01:34.000000 qamlib-0.9.0/meson.build
+-rw-r--r--   0        0        0      119 2024-04-24 12:01:34.000000 qamlib-0.9.0/meson_options.txt
+-rw-r--r--   0        0        0     1031 2024-04-24 12:01:34.000000 qamlib-0.9.0/noxfile.py
+-rw-r--r--   0        0        0      965 2024-04-24 12:01:34.000000 qamlib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1485 2024-04-24 12:01:34.000000 qamlib-0.9.0/setup.py
+-rw-r--r--   0        0        0      351 2024-04-24 12:01:34.000000 qamlib-0.9.0/shell.nix
+-rw-r--r--   0        0        0    18216 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/camera.cpp
+-rw-r--r--   0        0        0    17985 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/control.cpp
+-rw-r--r--   0        0        0    11142 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/device.cpp
+-rw-r--r--   0        0        0     3148 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/event_device.cpp
+-rw-r--r--   0        0        0     1972 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/events.cpp
+-rw-r--r--   0        0        0     6379 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/format.cpp
+-rw-r--r--   0        0        0      977 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/framerate.cpp
+-rw-r--r--   0        0        0     1119 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/meson.build
+-rw-r--r--   0        0        0    38095 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/pymod.cpp
+-rw-r--r--   0        0        0     6572 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/streaming_device.cpp
+-rw-r--r--   0        0        0      573 2024-04-24 12:01:34.000000 qamlib-0.9.0/src/utils.cpp
+-rw-r--r--   0        0        0      352 2024-04-24 12:01:34.000000 qamlib-0.9.0/subprojects/nlohmann_json.wrap
+-rw-r--r--   0        0        0      351 2024-04-24 12:01:34.000000 qamlib-0.9.0/subprojects/packagecache/pybind11_json_patch.zip
+-rw-r--r--   0        0        0      296 2024-04-24 12:01:34.000000 qamlib-0.9.0/subprojects/pybind11_json.wrap
+-rw-r--r--   0        0        0      998 2024-04-24 12:01:34.000000 qamlib-0.9.0/tests/test_events.py
+-rw-r--r--   0        0        0      416 2024-04-24 12:01:34.000000 qamlib-0.9.0/tests/test_formats.py
+-rw-r--r--   0        0        0     6173 2024-04-24 12:01:34.000000 qamlib-0.9.0/tests/test_long.py
+-rw-r--r--   0        0        0    33229 2024-04-24 12:04:29.548703 qamlib-0.9.0/PKG-INFO
```

### Comparing `qamlib-0.8.0/.clang-format` & `qamlib-0.9.0/.clang-format`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/.gitlab-ci.yml` & `qamlib-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/CHANGELOG.rst` & `qamlib-0.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Version 0.9.0
+=============
+
+New
+---
+
+* Added :py:class:`V4L2BusyException` to signal ``EBUSY`` errors.
+
+* Added minimal support for newer V4L2 controls types, e.g. ``AV1`` control
+  types.
+
+* Now adding `-qtec` to the ``__version__`` field if the module is built with
+  Qtec headers.
+
+Changes
+-------
+
+* No longer stop and restart stream in functions where it could be necessary for
+  the function to succeed, rather let the user handle the exception.
+
 Version 0.8.0
 =============
 
 New
 ---
 
 * Add :py:class:`DeviceInfo` to hold some V4L2 driver information for the
```

### Comparing `qamlib-0.8.0/LICENSE.LGPL2.1` & `qamlib-0.9.0/LICENSE.LGPL2.1`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/README.md` & `qamlib-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,20 +64,21 @@
 
 ```sh
 python -m build
 ```
 
 ### C++
 
-Dependicies
+Dependencies
 
 - `gcc`
 - `meson`
 - `ninja`
 - `nlohmann-json`
+- `opencv4`
 
 To build the library we start by running `meson` setup:
 
 ```sh
 meson setup build -Dpython=false
 ```
```

### Comparing `qamlib-0.8.0/docs/conf.py` & `qamlib-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/docs/cpp-reference.rst` & `qamlib-0.9.0/docs/cpp-reference.rst`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/docs/reference.rst` & `qamlib-0.9.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/docs/usage.rst` & `qamlib-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/cpp/small_example.cpp` & `qamlib-0.9.0/examples/cpp/small_example.cpp`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/extended_controls.py` & `qamlib-0.9.0/examples/extended_controls.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/hdr_capture_and_save.py` & `qamlib-0.9.0/examples/hdr_capture_and_save.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 exposures = [5000, 15000, 29000, 41000, 50000]
 
 # Defaults to /dev/qtec/video0
 cam = qamlib.Camera()
 
 # External trigger sequence
-cam.set_control("Trigger Mode", 5)
+cam.set_control("trigger_mode", 5)
 
 trig_seq = qamlib.TriggerSequenceValue()
 
 # Used to calculate minimal frame delay
-ft = cam.get_control("frame time")
-rot = cam.get_control("read-out time")
+fot = cam.get_control("frame_overhead_time")
+rot = cam.get_control("read_out_time")
 
 # Create trigger sequence with minimal delay
 for i in range(len(exposures)):
     exp = exposures[i]
     if i+1 >= len(exposures):
-        delay = exp + ft
+        delay = max(exp + fot, exp + fot + rot - exposures[0])
     else:
-        delay = max(exp + ft, exp + ft + rot - exposures[i+1])
+        delay = max(exp + fot, exp + fot + rot - exposures[i+1])
 
     trig_seq.add_exposure(exp, exp, delay, 0)
 
 # Set trigger sequence
 cam.set_ext_control("trigger sequence", trig_seq)
 
 # Set white balance, values from qtec-camera-gwt
@@ -57,8 +57,8 @@
         _, img = cam.get_frame(timeout=1, buffered=True)
 
         cv2.imwrite(name, img)
 
         images.append(img)
 
     fusion = merge.process(images)
-    cv2.imwrite(f"fusion.png", fusion*255) # Values after merge are in [0, 1]
+    cv2.imwrite("fusion.png", fusion*255) # Values after merge are in [0, 1]
```

### Comparing `qamlib-0.8.0/examples/qamlib_json.py` & `qamlib-0.9.0/examples/qamlib_json.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/qamlib_json_client.py` & `qamlib-0.9.0/examples/qamlib_json_client.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/qamlib_tcp_client.py` & `qamlib-0.9.0/examples/qamlib_tcp_client.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/examples/qamlib_test.py` & `qamlib-0.9.0/examples/qamlib_test.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/camera.h` & `qamlib-0.9.0/includes/camera.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/control.h` & `qamlib-0.9.0/includes/control.h`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,25 @@
 
 class Control {
     public:
 	uint32_t id;
 	std::string name;
 	v4l2_ctrl_type type;
 	ControlFlags flags;
+	uint32_t elem_size;
+	uint32_t elems;
+	std::vector<uint32_t> dimensions;
 
 	Control(v4l2_query_ext_ctrl *query)
 		: id(query->id), name(static_cast<char *>(query->name)),
 		  type(static_cast<v4l2_ctrl_type>(query->type)),
-		  flags(query->flags)
+		  flags(query->flags), elem_size(query->elem_size),
+		  elems(query->elems),
+		  dimensions(query->dims, query->dims + query->nr_of_dims)
+
 	{
 	}
 
 	// This is to let Pybind11 do automatic downcasting
 	virtual ~Control() = default;
 
 	virtual std::string to_string() const;
@@ -131,32 +137,14 @@
 	}
 
 	std::string to_string() const override;
 
 	json to_json() const override;
 };
 
-class ExtendedControl : public ValueControl {
-    public:
-	uint32_t elem_size;
-	uint32_t elems;
-	std::vector<uint32_t> dimensions;
-
-	ExtendedControl(v4l2_query_ext_ctrl *query)
-		: ValueControl(query), elem_size(query->elem_size),
-		  elems(query->elems),
-		  dimensions(query->dims, query->dims + query->nr_of_dims)
-	{
-	}
-
-	std::string to_string() const override;
-
-	json to_json() const override;
-};
-
 class ControlValue {
     public:
 	virtual ~ControlValue() = default;
 
 	/**
 	 * Internal ``qamlib`` function not to be used otherwise
 	 */
@@ -348,14 +336,38 @@
 	}
 
 	std::string to_string() const override;
 
 	json to_json() const override;
 };
 
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
+std::string representation_area(const struct v4l2_area &area);
+
+class AreaControlValue : public ControlValue {
+	struct v4l2_area area;
+
+    public:
+	AreaControlValue() : area({ 0, 0 })
+	{
+	}
+	AreaControlValue(struct v4l2_area area) : area(area)
+	{
+	}
+
+	void ready_control(v4l2_ext_control &ctrl) override;
+
+	struct v4l2_area get_area() const;
+
+	std::string to_string() const override;
+
+	json to_json() const override;
+};
+#endif
+
 // Have local versions of the v4l2_trigger_sequence structs when not building
 // with the Qtec headers.
 #ifndef QTEC_HEADER
 struct trigger_sequence {
 	__u32 exposure_time;
 	__u32 flash_time;
 	__u32 frame_delay;
```

### Comparing `qamlib-0.8.0/includes/device.h` & `qamlib-0.9.0/includes/device.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/event_device.h` & `qamlib-0.9.0/includes/event_device.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/events.h` & `qamlib-0.9.0/includes/events.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/format.h` & `qamlib-0.9.0/includes/format.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/framerate.h` & `qamlib-0.9.0/includes/framerate.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/includes/streaming_device.h` & `qamlib-0.9.0/includes/streaming_device.h`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/meson.build` & `qamlib-0.9.0/meson.build`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   'qamlib',
   'cpp',
   default_options : [
     'warning_level=3',
     'buildtype=debugoptimized',
     'cpp_std=c++20',
   ],
-  version : '0.8.0'
+  version : '0.9.0'
 )
 
 # Option to build the Python module or the C++ library
 build_python = get_option('python')
 
 add_project_arguments(
   [
```

### Comparing `qamlib-0.8.0/noxfile.py` & `qamlib-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/pyproject.toml` & `qamlib-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/setup.py` & `qamlib-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 from pybind11.setup_helpers import build_ext
 from pybind11.setup_helpers import Pybind11Extension
 from setuptools import setup
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 # We will try to keep warning free
 compile_args = ["-Werror", "-std=c++20"]
 
 macros = [
     ("VERSION_INFO", __version__),
     ("PYTHON", None),  # Enable Python for camera.cpp
```

### Comparing `qamlib-0.8.0/src/camera.cpp` & `qamlib-0.9.0/src/camera.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -56,19 +56,17 @@
 
 #if PYTHON
 	// Import NumPy now, so that it does not need to be done when creating
 	// the first NumPy array for a requested frame
 	py::module_(py::module_::import("numpy"));
 #endif
 
-	enum v4l2_buf_type type;
-	type = V4L2_BUF_TYPE_VIDEO_CAPTURE;
-	if (0 != ioctl(fd, VIDIOC_STREAMON, &type)) {
+	if (0 != ioctl(fd, VIDIOC_STREAMON, &device_type)) {
 		unmap();
-		throw V4L2Exception("Failed to start streaming", errno);
+		v4l2_exception("Failed to start streaming", errno);
 	}
 
 	// Update format to make sure it is fully up to date
 	update_format();
 
 	buffer_thread = std::thread(&Camera::buffer_manager, this);
 
@@ -270,15 +268,15 @@
 		current_format.fmt.pix.xfer_func = tmp.xfer_func;
 	} else {
 		throw V4L2Exception(
 			"set_format does not support this buffer type");
 	}
 
 	if (ioctl(fd, VIDIOC_S_FMT, &current_format)) {
-		throw V4L2Exception("Failed to set format", errno);
+		v4l2_exception("Failed to set format", errno);
 	}
 
 	if (current_format.type == V4L2_BUF_TYPE_VIDEO_CAPTURE) {
 		return std::unique_ptr<Format>(new SinglePlaneFormat(
 			&current_format.fmt.pix, V4L2_BUF_TYPE_VIDEO_CAPTURE));
 	}
 
@@ -297,40 +295,29 @@
 
 	if (it == formats.end()) {
 		throw V4L2Exception("Could not find format: " + name);
 	}
 
 	auto format = it->second;
 
-	bool restart_stream = false;
-	if (streaming) {
-		stop();
-	}
-
 	if (ioctl(fd, VIDIOC_G_FMT, &current_format)) {
-		throw V4L2Exception("Failed to get format", errno);
+		v4l2_exception("Failed to get format", errno);
 	}
 
 	current_format.fmt.pix.pixelformat = format.pixelformat.get_code();
 
 	auto old_default = get_crop_default();
 	auto selection = get_crop();
 
 	if (ioctl(fd, VIDIOC_S_FMT, &current_format)) {
-		if (restart_stream) {
-			start();
-		}
-		throw V4L2Exception("Failed to set format", errno);
+		v4l2_exception("Failed to set format", errno);
 	}
 
 	update_selection(selection, old_default, get_crop_default());
 
-	if (restart_stream) {
-		start();
-	}
 	return std::unique_ptr<Format>(new SinglePlaneFormat(
 		&current_format.fmt.pix, V4L2_BUF_TYPE_VIDEO_CAPTURE));
 }
 
 /*
  * FRAMERATE
  */
@@ -369,15 +356,15 @@
 		.index = 0,
 		.pixel_format = pixelformat,
 		.width = width,
 		.height = height,
 	};
 
 	if (ioctl(fd, VIDIOC_ENUM_FRAMEINTERVALS, &frenum) != 0) {
-		throw V4L2Exception("Could not enumerate framerates", errno);
+		v4l2_exception("Could not enumerate framerates", errno);
 	}
 
 	if (frenum.type == V4L2_FRMIVAL_TYPE_DISCRETE) {
 		double fps = static_cast<double>(frenum.discrete.denominator) /
 			     frenum.discrete.numerator;
 		std::vector<double> values = { fps };
 
@@ -385,15 +372,15 @@
 		while (ioctl(fd, VIDIOC_ENUM_FRAMEINTERVALS, &frenum) == 0) {
 			fps = static_cast<double>(frenum.discrete.denominator) /
 			      frenum.discrete.numerator;
 			values.push_back(fps);
 			frenum.index++;
 		}
 		if (errno != EINVAL) {
-			throw V4L2Exception(
+			v4l2_exception(
 				"Got error while enumerating discrete framerates",
 				errno);
 		}
 
 		auto val = new DiscreteFrameRate(values);
 
 		return std::unique_ptr<FrameRate>(val);
@@ -422,16 +409,15 @@
 double Camera::get_framerate()
 {
 	struct v4l2_streamparm parm = {
 		.type = V4L2_BUF_TYPE_VIDEO_CAPTURE,
 	};
 
 	if (ioctl(fd, VIDIOC_G_PARM, &parm) != 0) {
-		throw V4L2Exception("Could not query framerate parameters",
-				    errno);
+		v4l2_exception("Could not query framerate parameters", errno);
 	}
 
 	auto frametime = parm.parm.capture.timeperframe;
 	return static_cast<double>(frametime.denominator) / frametime.numerator;
 }
 
 double Camera::set_framerate(double value)
@@ -448,16 +434,15 @@
 					.denominator = den
 				},
 			},
 		},
 	};
 
 	if (ioctl(fd, VIDIOC_S_PARM, &parm) != 0) {
-		throw V4L2Exception("Could not set framerate parameters",
-				    errno);
+		v4l2_exception("Could not set framerate parameters", errno);
 	}
 
 	auto frametime = parm.parm.capture.timeperframe;
 	return static_cast<double>(frametime.denominator) / frametime.numerator;
 }
 
 /*
@@ -533,15 +518,15 @@
 	// Default to requesting 10 buffers for userspace
 	userspace_buffers = req_usr_buffers.value_or(10);
 	driver_buffers = req_drv_buffers;
 
 	reqBuf.count = userspace_buffers + driver_buffers;
 
 	if (ioctl(fd, VIDIOC_REQBUFS, &reqBuf) != 0) {
-		throw V4L2Exception("Failed to request buffers", errno);
+		v4l2_exception("Failed to request buffers", errno);
 	}
 
 	// Check if we got enough buffers to continue
 	if (reqBuf.count < userspace_buffers + driver_buffers) {
 		std::cerr << "Got fewer V4L2 buffers than expected"
 			  << std::endl;
 
@@ -575,16 +560,15 @@
 		CLEAR(buf);
 
 		buf.type = V4L2_BUF_TYPE_VIDEO_CAPTURE;
 		buf.memory = V4L2_MEMORY_MMAP;
 		buf.index = i;
 
 		if (ioctl(fd, VIDIOC_QUERYBUF, &buf) != 0) {
-			throw V4L2Exception("Failed to query V4L2 buffer",
-					    errno);
+			v4l2_exception("Failed to query V4L2 buffer", errno);
 		}
 
 		newBuffers[i].length = buf.length;
 		newBuffers[i].start =
 			mmap(NULL, buf.length, PROT_READ | PROT_WRITE,
 			     MAP_SHARED, fd, buf.m.offset);
 	}
@@ -620,16 +604,15 @@
 		// Index starting from where we left with userspace ringbuffer
 		buf.index = i + userspace_buffers;
 		buf.type = device_type;
 		buf.memory = V4L2_MEMORY_MMAP;
 
 		if (ioctl(fd, VIDIOC_QBUF, &buf) != 0) {
 			DPRINT("VIDIOC_QBUF");
-			throw V4L2Exception("Failed to queue V4L2 buffer",
-					    errno);
+			v4l2_exception("Failed to queue V4L2 buffer", errno);
 		}
 	}
 }
 
 void Camera::unmap()
 {
 	if (!mmaped) {
@@ -678,23 +661,23 @@
 			ret = select(fd + 1, &fds, NULL, NULL, &tv);
 		} while ((ret == -1 && (errno == EINTR)));
 
 		if (ret == 0) {
 			// Timeout, so we try again
 			continue;
 		} else if (ret == -1) {
-			throw V4L2Exception("Got error on select()", errno);
+			v4l2_exception("Got error on select()", errno);
 		}
 
 		CLEAR(buf);
 		buf.type = device_type;
 		buf.memory = V4L2_MEMORY_MMAP;
 
 		if (ioctl(fd, VIDIOC_DQBUF, &buf) != 0) {
-			throw V4L2Exception("Failed to dequeue buffer", errno);
+			v4l2_exception("Failed to dequeue buffer", errno);
 		}
 
 		std::unique_lock<std::mutex> lock(frame_lock);
 
 		frames->insert(buf);
 
 		//frame_lock.unlock();
@@ -711,15 +694,15 @@
 		pop();
 	}
 
 	increment_end();
 
 	// Queue previous buffer
 	if (ioctl(cam.fd, VIDIOC_QBUF, buffers + end)) {
-		throw V4L2Exception("Failed to queue buffer", errno);
+		v4l2_exception("Failed to queue buffer", errno);
 	}
 
 	// If we reach start, we have dropped a frame
 	full = start == end;
 
 	buffers[end] = buffer;
 }
```

### Comparing `qamlib-0.8.0/src/control.cpp` & `qamlib-0.9.0/src/control.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -163,33 +163,70 @@
 #endif
 #if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 17, 0)
 	case V4L2_CTRL_TYPE_VP9_COMPRESSED_HDR:
 		return "VP9 compressed HDR";
 	case V4L2_CTRL_TYPE_VP9_FRAME:
 		return "VP9 frame";
 #endif
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(6, 0, 0)
+	case V4L2_CTRL_TYPE_HEVC_SPS:
+		return "HEVC Sequence Parameters";
+	case V4L2_CTRL_TYPE_HEVC_PPS:
+		return "HEVC Picture Parameters";
+	case V4L2_CTRL_TYPE_HEVC_SLICE_PARAMS:
+		return "HEVC Slice Parameters";
+	case V4L2_CTRL_TYPE_HEVC_SCALING_MATRIX:
+		return "HEVC Scaling Matrices";
+	case V4L2_CTRL_TYPE_HEVC_DECODE_PARAMS:
+		return "";
+#endif
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(6, 5, 0)
+	case V4L2_CTRL_TYPE_AV1_SEQUENCE:
+		return "AV1 Sequence";
+	case V4L2_CTRL_TYPE_AV1_TILE_GROUP_ENTRY:
+		return "AV1 Tile Group";
+	case V4L2_CTRL_TYPE_AV1_FRAME:
+		return "AV1 Frame";
+	case V4L2_CTRL_TYPE_AV1_FILM_GRAIN:
+		return "AV1 Film Grain Parameters";
+#endif
 	default:
 		return "Unkown type";
 	}
 }
 std::string Control::to_string() const
 {
 	std::string res = "ID: " + std::to_string(id) + ", Name: " + name +
 			  ", Type: " + type_to_string(type) +
-			  ", Flags: " + flags.to_string();
+			  ", Flags: " + flags.to_string() +
+			  ", Elements: " + std::to_string(elems) +
+			  ", Element size: " + std::to_string(elem_size);
+
+	if (dimensions.size() > 0) {
+		res += ", Dimensions: [";
+		for (auto dim : dimensions) {
+			res += " " + std::to_string(dim);
+		}
+		res += " ]";
+	}
 
 	return res;
 }
 
 json Control::to_json() const
 {
-	return json{ { "id", id },
-		     { "name", name },
-		     { "type", type_to_string(type) },
-		     { "flags", flags.to_json() } };
+	return json{
+		{ "id", id },
+		{ "name", name },
+		{ "type", type_to_string(type) },
+		{ "flags", flags.to_json() },
+		{ "elements", elems },
+		{ "element_size", elem_size },
+		{ "dimensions", dimensions },
+	};
 }
 
 std::string ValueControl::to_string() const
 {
 	return Control::to_string() + ", Min: " + std::to_string(min) +
 	       ", Max: " + std::to_string(max) +
 	       ", Default value: " + std::to_string(default_value) +
@@ -261,48 +298,23 @@
 	for (auto it = items.begin(); it != items.end(); ++it) {
 		res["items"][std::to_string(it->first)] = it->second;
 	}
 
 	return res;
 }
 
-std::string ExtendedControl::to_string() const
-{
-	auto res = ValueControl::to_string() +
-		   ", Elements: " + std::to_string(elems) +
-		   ", Element size: " + std::to_string(elem_size) +
-		   ", Dimensions: [";
-
-	for (auto dim : dimensions) {
-		res += " " + std::to_string(dim);
-	}
-
-	return res + " ]";
-}
-
-json ExtendedControl::to_json() const
-{
-	auto res = ValueControl::to_json();
-
-	res["elements"] = elems;
-	res["element_size"] = elem_size;
-	res["dimensions"] = dimensions;
-
-	return res;
-}
-
 void StringControlValue::ready_control(v4l2_ext_control &ctrl)
 {
 	ctrl.size = size + 1;
 	ctrl.string = value;
 }
 
 void StringControlValue::check_value(std::shared_ptr<Control> ctrl)
 {
-	auto ext_ctrl = std::static_pointer_cast<ExtendedControl>(ctrl);
+	auto ext_ctrl = std::static_pointer_cast<ValueControl>(ctrl);
 
 	if (ext_ctrl->min > size || ext_ctrl->max < size) {
 		throw V4L2Exception("String size does not match control limits:"
 				    " (min: " +
 				    std::to_string(ext_ctrl->min) +
 				    ", max: " + std::to_string(ext_ctrl->max) +
 				    "), size: " + std::to_string(size));
@@ -422,15 +434,15 @@
 		throw std::logic_error(
 			"Invalid type size in ArrayControlValue");
 	}
 }
 
 void ArrayControlValue::check_value(std::shared_ptr<Control> ctrl)
 {
-	auto ext_ctrl = std::static_pointer_cast<ExtendedControl>(ctrl);
+	auto ext_ctrl = std::static_pointer_cast<ValueControl>(ctrl);
 
 	// Ensure we the array type is supported by V4L2
 	if (sign && (element_size < 4)) {
 		throw V4L2Exception(ctrl->name,
 				    ">32bit signed arrays are not supported");
 	}
 
@@ -665,14 +677,43 @@
 		throw std::logic_error(
 			"Invalid type size in ArrayControlValue");
 	}
 
 	return json{ { "value", array } };
 }
 
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
+struct v4l2_area AreaControlValue::get_area() const
+{
+	return area;
+}
+
+void AreaControlValue::ready_control(v4l2_ext_control &ctrl)
+{
+	ctrl.size = sizeof(v4l2_area);
+	ctrl.p_area = &area;
+}
+
+std::string representation_area(const struct v4l2_area &area)
+{
+	return "Width x Height: " + std::to_string(area.width) + " x " +
+	       std::to_string(area.height);
+}
+
+std::string AreaControlValue::to_string() const
+{
+	return representation_area(area);
+}
+
+json AreaControlValue::to_json() const
+{
+	return json{ { "width", area.width }, { "height", area.height } };
+}
+#endif
+
 std::string
 representation_trigger_sequence(const struct trigger_sequence &trig_seq)
 {
 	return "Exposure time: " + std::to_string(trig_seq.exposure_time) +
 	       ", Flash time: " + std::to_string(trig_seq.flash_time) +
 	       ", Frame delay: " + std::to_string(trig_seq.frame_delay) +
 	       ", Trigger delay: " + std::to_string(trig_seq.trigger_delay);
```

### Comparing `qamlib-0.8.0/src/device.cpp` & `qamlib-0.9.0/src/device.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 	if (fd == -1) {
 		throw V4L2Exception("Failed to open device");
 	}
 
 	struct v4l2_capability caps;
 	if (ioctl(fd, VIDIOC_QUERYCAP, &caps)) {
-		throw V4L2Exception("Error querying device capabilities",
-				    errno);
+		v4l2_exception("Error querying device capabilities", errno);
 	}
 
 	if (needed_cap != 0 && !(caps.device_caps & needed_cap)) {
 		throw V4L2Exception(
 			"Device does not support necessary capabilities");
 	}
 
@@ -79,15 +78,15 @@
 			     i++) {
 				qmenu.index = i;
 
 				if (ioctl(fd, VIDIOC_QUERYMENU, &qmenu)) {
 					if (errno == EINVAL) {
 						continue;
 					}
-					throw V4L2Exception(
+					v4l2_exception(
 						"Error while querying menu items",
 						errno);
 				}
 
 				items[qmenu.index] = std::string(
 					reinterpret_cast<char *>(qmenu.name));
 			}
@@ -107,47 +106,40 @@
 
 				if (ioctl(fd, VIDIOC_QUERYMENU, &qmenu)) {
 					// Not all indices in the range have to
 					// be populated
 					if (errno == EINVAL) {
 						continue;
 					}
-					throw V4L2Exception(
+					v4l2_exception(
 						"Error while querying menu items",
 						errno);
 				}
 
 				items[qmenu.index] = qmenu.value;
 			}
 
 			ctrl = std::shared_ptr<Control>(
 				new IntegerMenuControl(&query, items));
 			break;
 		}
 		case V4L2_CTRL_TYPE_INTEGER:
 		case V4L2_CTRL_TYPE_INTEGER64:
-			if (query.flags & V4L2_CTRL_FLAG_HAS_PAYLOAD) {
-				ctrl = std::shared_ptr<Control>(
-					new ExtendedControl(&query));
-				break;
-			}
-			// fall through
+		case V4L2_CTRL_TYPE_U8:
+		case V4L2_CTRL_TYPE_U16:
+		case V4L2_CTRL_TYPE_U32:
 		case V4L2_CTRL_TYPE_BOOLEAN:
 		case V4L2_CTRL_TYPE_BITMASK:
 		case V4L2_CTRL_TYPE_STRING:
 			ctrl = std::shared_ptr<Control>(
 				new ValueControl(&query));
 			break;
-		case V4L2_CTRL_TYPE_BUTTON:
-		case V4L2_CTRL_TYPE_CTRL_CLASS:
-			ctrl = std::shared_ptr<Control>(new Control(&query));
-			break;
 		default:
-			ctrl = std::shared_ptr<Control>(
-				new ExtendedControl(&query));
+			// All other controls do not use min/step/max
+			ctrl = std::shared_ptr<Control>(new Control(&query));
 			break;
 		}
 
 		controls[name] = ctrl;
 
 		query.id |=
 			V4L2_CTRL_FLAG_NEXT_CTRL | V4L2_CTRL_FLAG_NEXT_COMPOUND;
@@ -182,27 +174,27 @@
 
 	struct v4l2_control control = {
 		.id = ctrl->id,
 		.value = value,
 	};
 
 	if (ioctl(fd, VIDIOC_S_CTRL, &control) != 0) {
-		throw V4L2Exception("Failed to set control", errno);
+		v4l2_exception("Failed to set control", errno);
 	}
 }
 
 void Device::set_control(uint32_t id, int value)
 {
 	struct v4l2_control control = {
 		.id = id,
 		.value = value,
 	};
 
 	if (ioctl(fd, VIDIOC_S_CTRL, &control) != 0) {
-		throw V4L2Exception("Failed to set control", errno);
+		v4l2_exception("Failed to set control", errno);
 	}
 }
 
 int Device::get_control(const std::string &ctrl_name)
 {
 	auto name = name_to_key(ctrl_name);
 	auto controls = list_controls();
@@ -227,28 +219,28 @@
 	}
 
 	struct v4l2_control control = {
 		.id = ctrl->id,
 	};
 
 	if (ioctl(fd, VIDIOC_G_CTRL, &control) != 0) {
-		throw V4L2Exception("Failed to get control", errno);
+		v4l2_exception("Failed to get control", errno);
 	}
 
 	return control.value;
 }
 
 int Device::get_control(uint32_t id)
 {
 	struct v4l2_control control = {
 		.id = id,
 	};
 
 	if (ioctl(fd, VIDIOC_G_CTRL, &control) != 0) {
-		throw V4L2Exception("Failed to get control", errno);
+		v4l2_exception("Failed to get control", errno);
 	}
 
 	return control.value;
 }
 
 /*
  * Gives an "empty" ControlValue object
@@ -261,24 +253,24 @@
 		auto string_ctrl = std::static_pointer_cast<ValueControl>(ctrl);
 		return std::unique_ptr<ControlValue>(
 			new StringControlValue(string_ctrl->max));
 	}
 	case V4L2_CTRL_TYPE_U8:
 	case V4L2_CTRL_TYPE_U16:
 	case V4L2_CTRL_TYPE_U32: {
-		auto ext_ctrl = std::static_pointer_cast<ExtendedControl>(ctrl);
+		auto ext_ctrl = std::static_pointer_cast<ValueControl>(ctrl);
 		return std::unique_ptr<ControlValue>(new ArrayControlValue(
 			ext_ctrl->elems, ext_ctrl->elem_size,
 			ext_ctrl->dimensions));
 	}
 	case V4L2_CTRL_TYPE_INTEGER:
 	case V4L2_CTRL_TYPE_INTEGER64: {
 		if (ctrl->flags.has_payload()) {
 			auto ext_ctrl =
-				std::static_pointer_cast<ExtendedControl>(ctrl);
+				std::static_pointer_cast<ValueControl>(ctrl);
 			return std::unique_ptr<ControlValue>(
 				new ArrayControlValue(
 					ext_ctrl->elems, ext_ctrl->elem_size,
 					ext_ctrl->dimensions, true));
 		} else {
 			return std::unique_ptr<ControlValue>(
 				new IntegerControlValue(ctrl->type));
@@ -287,14 +279,18 @@
 	case V4L2_CTRL_TYPE_BOOLEAN:
 	case V4L2_CTRL_TYPE_MENU:
 	case V4L2_CTRL_TYPE_INTEGER_MENU:
 	case V4L2_CTRL_TYPE_BITMASK:
 	case V4L2_CTRL_TYPE_BUTTON:
 		return std::unique_ptr<ControlValue>(
 			new IntegerControlValue(ctrl->type));
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
+	case V4L2_CTRL_TYPE_AREA:
+		return std::unique_ptr<ControlValue>(new AreaControlValue());
+#endif
 #ifdef QTEC_HEADER
 	case V4L2_CTRL_TYPE_TRIG_SEQ:
 		return std::unique_ptr<ControlValue>(
 			new TriggerSequenceValue());
 #endif
 	default:
 		throw V4L2Exception("Extended control class not implemented for"
@@ -330,15 +326,15 @@
 	struct v4l2_ext_controls ext_ctrl = {
 		.which = V4L2_CTRL_WHICH_CUR_VAL,
 		.count = 1,
 		.controls = ctrls,
 	};
 
 	if (ioctl(fd, VIDIOC_S_EXT_CTRLS, &ext_ctrl) != 0) {
-		throw V4L2Exception("Failed to set extended control", errno);
+		v4l2_exception("Failed to set extended control", errno);
 	}
 }
 
 std::unique_ptr<ControlValue>
 Device::get_ext_control(const std::string &ctrl_name, bool default_value)
 {
 	auto name = name_to_key(ctrl_name);
@@ -367,15 +363,15 @@
 	struct v4l2_ext_controls ext_ctrl = {
 		.which = which,
 		.count = 1,
 		.controls = ctrls,
 	};
 
 	if (ioctl(fd, VIDIOC_G_EXT_CTRLS, &ext_ctrl) != 0) {
-		throw V4L2Exception("Failed to get extended control", errno);
+		v4l2_exception("Failed to get extended control", errno);
 	}
 
 	// Ponter to the ext_control
 	ctrl_val->update_value(ctrls[0]);
 
 	return ctrl_val;
 }
@@ -421,15 +417,15 @@
 	struct v4l2_ext_controls ext_ctrl = {
 		.which = which,
 		.count = static_cast<uint32_t>(names.size()),
 		.controls = &ctrls[0], // vector data is contiguous
 	};
 
 	if (ioctl(fd, VIDIOC_G_EXT_CTRLS, &ext_ctrl) != 0) {
-		throw V4L2Exception("Failed to get controls", errno);
+		v4l2_exception("Failed to get controls", errno);
 	}
 
 	std::map<std::string, std::unique_ptr<ControlValue> > result;
 
 	for (size_t i = 0; i < values.size(); i++) {
 		values[i]->update_value(ctrls[i]);
 
@@ -468,11 +464,11 @@
 	struct v4l2_ext_controls ext_ctrl = {
 		.which = V4L2_CTRL_WHICH_CUR_VAL,
 		.count = static_cast<uint32_t>(values.size()),
 		.controls = &ctrls[0], // vector data is contiguous
 	};
 
 	if (ioctl(fd, VIDIOC_S_EXT_CTRLS, &ext_ctrl) != 0) {
-		throw V4L2Exception("Failed to set controls", errno);
+		v4l2_exception("Failed to set controls", errno);
 	}
 }
 } // namespace qamlib
```

### Comparing `qamlib-0.8.0/src/event_device.cpp` & `qamlib-0.9.0/src/event_device.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 			ret = select(fd + 1, NULL, NULL, &fds, &tv);
 		} while ((ret == -1 && (errno == EINTR)));
 
 		if (ret == 0) {
 			// Timeout, so we try again
 			continue;
 		} else if (ret == -1) {
-			throw V4L2Exception("Got error on select()", errno);
+			v4l2_exception("Got error on select()", errno);
 		}
 
 		CLEAR(event);
 
 		if (ioctl(fd, VIDIOC_DQEVENT, &event)) {
-			throw V4L2Exception("Could not dequeue event", errno);
+			v4l2_exception("Could not dequeue event", errno);
 		}
 
 		switch (event.type) {
 		case V4L2_EVENT_VSYNC:
 		case V4L2_EVENT_EOS:
 		case V4L2_EVENT_FRAME_SYNC:
 		case V4L2_EVENT_MOTION_DET:
@@ -114,15 +114,15 @@
 		break;
 
 	default:
 		throw V4L2Exception("Unknown event type");
 	}
 
 	if (ioctl(fd, VIDIOC_SUBSCRIBE_EVENT, &event_sub)) {
-		throw V4L2Exception("Could not subscribe to event", errno);
+		v4l2_exception("Could not subscribe to event", errno);
 	}
 }
 
 void EventDevice::unsubscribe(uint32_t type, uint32_t id)
 {
 	struct v4l2_event_subscription event_sub;
 
@@ -144,11 +144,11 @@
 		break;
 
 	default:
 		throw V4L2Exception("Unknown event type");
 	}
 
 	if (ioctl(fd, VIDIOC_UNSUBSCRIBE_EVENT, &event_sub)) {
-		throw V4L2Exception("Could not unsubscribe from event", errno);
+		v4l2_exception("Could not unsubscribe from event", errno);
 	}
 }
 } // namespace qamlib
```

### Comparing `qamlib-0.8.0/src/events.cpp` & `qamlib-0.9.0/src/events.cpp`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/src/format.cpp` & `qamlib-0.9.0/src/format.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -259,31 +259,31 @@
 	default:
 		return "Unkown";
 	}
 }
 
 std::string SinglePlaneFormat::to_string() const
 {
-	std::string res = "Height: " + std::to_string(height) +
-			  ", Width: " + std::to_string(width) +
+	std::string res = "Width: " + std::to_string(width) +
+			  ", Height: " + std::to_string(height) +
 			  ", Pixel format: " + pixelformat.to_string() +
 			  ", Colorspace: " + colorspace_to_string(colorspace) +
 			  ", Field: " + field_to_string(field) +
 			  ", Bytes per line: " + std::to_string(bytesperline) +
 			  ", Size image: " + std::to_string(sizeimage) +
 			  ", Priv: " + (priv ? "True" : "False") +
 			  ", Flags: " + flags.to_string();
 
 	return res;
 }
 
 json SinglePlaneFormat::to_json() const
 {
-	return json{ { "height", height },
-		     { "width", width },
+	return json{ { "width", width },
+		     { "height", height },
 		     { "pixelformat", pixelformat.to_string() },
 		     { "colorspace", colorspace_to_string(colorspace) },
 		     { "field", field_to_string(field) },
 		     { "bytes_per_line", bytesperline },
 		     { "size", sizeimage },
 		     { "priv", (priv ? "true" : "false") },
 		     { "flags", flags.to_json() } };
```

### Comparing `qamlib-0.8.0/src/framerate.cpp` & `qamlib-0.9.0/src/framerate.cpp`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/src/meson.build` & `qamlib-0.9.0/src/meson.build`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/src/pymod.cpp` & `qamlib-0.9.0/src/pymod.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,15 @@
 char list_controls_docs[] =
 	"List all the controls for the device\n\n"
 	":returns: A list of all controls and their information.";
 
 char set_control_docs0[] =
 	"Set a normal named control to desired value.\n\n"
 	":param name: Full name of the control, case is ignored.\n\n"
-	":param value: Integer value to set.\n\n"
-	"NOTE: If the chosen control is either VFLIP or HFLIP, it tries to flip"
-	" the selection as well";
+	":param value: Integer value to set.\n\n";
 
 char set_control_docs1[] =
 	"Set a normal control, by id to desired value\n\n"
 	":param id: ID of the control, there is no check if a control with that"
 	" ID actually exists.\n\n"
 	":param value: Integer value to set.\n\n"
 	" NOTE: This function does not do any checks of the control ID or value";
@@ -122,20 +120,21 @@
 char exit_docs[] = "Exit runtime context, stops the stream";
 char get_crop_docs[] = "Get current crop selection (left, top, width, height)";
 char get_crop_bounds_docs[] = "Get crop selection bounds (left, top, width, "
 			      "height)";
 char get_crop_default_docs[] = "Get default crop selection (left, top, width, "
 			       "height)";
 char list_formats_docs[] = "List all available formats for the device";
-char set_crop_docs0[] = "Set crop selection using V4L2s selection API";
+char set_crop_docs0[] = "Set crop selection using V4L2s selection API. This "
+			"function will change the resolution if needed.";
 char set_crop_docs1[] =
 	"Set crop selections, using V4L2s selection API, there "
 	"are some driver and logic limitations to multi-crop, because of this, "
-	"all lefts/widths will be the same as the first rectangle, and the "
-	"rectangles cannot overlap (this will result in an exception)";
+	"the rectangles cannot overlap in the height dimension. This function "
+	"will change the resolution if needed.";
 char start_docs[] = "Starts the device stream";
 char stop_docs[] = "Stops the device stream";
 char get_resolution_docs[] = "Get current resolution";
 char set_format_docs0[] = "Set image format";
 char set_format_docs1[] = "Set image format by format name, this function also"
 			  "scales selection for the new format";
 char set_framerate_docs[] = "Tries to set the desired framerate, returns the "
@@ -221,15 +220,19 @@
 
 PYBIND11_MODULE(qamlib, m)
 {
 	m.doc() =
 		"The qamlib module is an interface to V4L2 IOCTL calls, written "
 		"in C++"; // optional module docstring
 
+#ifdef QTEC_HEADER
+	m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO) "-qtec";
+#else
 	m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
+#endif
 
 	/*
 	 * Custom iterators for vectors, could not get pybind11::make_iterator
 	 * to work.
 	 */
 	py::class_<VectorIterator<int> >(m, "IntVectorIterator")
 		.def("__next__", &VectorIterator<int>::next);
@@ -312,14 +315,17 @@
 		.value("U16", v4l2_ctrl_type::V4L2_CTRL_TYPE_U16)
 		.value("U32", v4l2_ctrl_type::V4L2_CTRL_TYPE_U32)
 #ifdef QTEC_HEADER
 		.value("TRIG_SEQ", v4l2_ctrl_type::V4L2_CTRL_TYPE_TRIG_SEQ)
 		.value("POINT", v4l2_ctrl_type::V4L2_CTRL_TYPE_POINT)
 #endif
 // Make sure kernel is new enough to have all the encoding controls
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
+		.value("AREA", v4l2_ctrl_type::V4L2_CTRL_TYPE_AREA)
+#endif
 #if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 14, 0)
 		.value("HDR10_CLL_INFO",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_HDR10_CLL_INFO)
 		.value("HDR10_MASTERING_DISPLAY",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_HDR10_MASTERING_DISPLAY)
 		.value("MPEG2_QUANTISATION",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_MPEG2_QUANTISATION)
@@ -337,22 +343,38 @@
 		.value("H264_DECODE_PARAMS",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_H264_DECODE_PARAMS)
 
 		.value("FWHT_PARAMS",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_FWHT_PARAMS)
 		.value("VP8_FRAME", v4l2_ctrl_type::V4L2_CTRL_TYPE_VP8_FRAME)
 #endif
-#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
-		.value("AREA", v4l2_ctrl_type::V4L2_CTRL_TYPE_AREA)
-#endif
 #if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 17, 0)
 		.value("VP9_COMPRESSED_HDR",
 		       v4l2_ctrl_type::V4L2_CTRL_TYPE_VP9_COMPRESSED_HDR)
 		.value("VP9_FRAME", v4l2_ctrl_type::V4L2_CTRL_TYPE_VP9_FRAME)
 #endif
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(6, 0, 0)
+		.value("HEVC_SPS", v4l2_ctrl_type::V4L2_CTRL_TYPE_HEVC_SPS)
+		.value("HEVC_PPS", v4l2_ctrl_type::V4L2_CTRL_TYPE_HEVC_PPS)
+		.value("HEVC_SLICE_PARAMS",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_HEVC_SLICE_PARAMS)
+		.value("HEVC_SCALING_MATRIX",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_HEVC_SCALING_MATRIX)
+		.value("HEVC_DECODE_PARAMS",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_HEVC_DECODE_PARAMS)
+#endif
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(6, 5, 0)
+		.value("AV1_SEQUENCE",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_AV1_SEQUENCE)
+		.value("AV1_TILE_GROUP_ENTRY",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_AV1_TILE_GROUP_ENTRY)
+		.value("AV1_FRAME", v4l2_ctrl_type::V4L2_CTRL_TYPE_AV1_FRAME)
+		.value("AV1_FILM_GRAIN",
+		       v4l2_ctrl_type::V4L2_CTRL_TYPE_AV1_FILM_GRAIN)
+#endif
 		// This is moved to last, just to have a permanent line ending
 		// with a semicolon (;)
 		.value("CTRL_CLASS", v4l2_ctrl_type::V4L2_CTRL_TYPE_CTRL_CLASS);
 
 	py::class_<Control, std::shared_ptr<Control> >(
 		m, "Control",
 		"This class represents the information about a camera "
@@ -360,14 +382,20 @@
 		.def_readonly("id", &Control::id, "ID of the camera control")
 		.def_readonly("name", &Control::name,
 			      "Name of the camera control")
 		.def_readonly("type", &Control::type,
 			      "Type of the camera control")
 		.def_readonly("flags", &Control::flags,
 			      "Class representing the control flags")
+		.def_readonly("element_size", &Control::elem_size,
+			      "The size of the control elements")
+		.def_readonly("elements", &Control::elems,
+			      "The number of control elemets")
+		.def_readonly("dimensions", &Control::dimensions,
+			      "The dimensions of the element array")
 		.def("to_json", &Control::to_json)
 		.def("__repr__", &Control::to_string)
 		.def("__str__", &Control::to_string);
 
 	py::class_<ValueControl, std::shared_ptr<ValueControl>, Control>(
 		m, "ValueControl",
 		"Inherits from Control, represents a normal control with a "
@@ -401,29 +429,14 @@
 		"with the values of the items")
 		.def_readonly("items", &IntegerMenuControl::items,
 			      "Values of the menu items")
 		.def("to_json", &IntegerMenuControl::to_json)
 		.def("__repr__", &IntegerMenuControl::to_string)
 		.def("__str__", &IntegerMenuControl::to_string);
 
-	py::class_<ExtendedControl, std::shared_ptr<ExtendedControl>,
-		   ValueControl>(
-		m, "ExtendedControl",
-		"Inherits from Control, represents a extended control "
-		"control with a single value")
-		.def_readonly("element_size", &ExtendedControl::elem_size,
-			      "The size of the control elements")
-		.def_readonly("elements", &ExtendedControl::elems,
-			      "The number of control elemets")
-		.def_readonly("dimensions", &ExtendedControl::dimensions,
-			      "The dimensions of the element array")
-		.def("to_json", &ExtendedControl::to_json)
-		.def("__repr__", &ExtendedControl::to_string)
-		.def("__str__", &ExtendedControl::to_string);
-
 	py::class_<ControlFlags>(
 		m, "ControlFlags",
 		"Class that represents the flags of a control.\nFor more "
 		"information about their meaning see `here "
 		"<https://www.kernel.org/doc/html/latest/userspace-api/media/v4l/vidioc-queryctrl.html#control-flags>`__.")
 		.def_readonly("raw_flags", &ControlFlags::flags,
 			      "The integer containing the V4L2 control flags")
@@ -478,14 +491,32 @@
 		m, "ArrayControlValue",
 		"Class that represents an array control value")
 		.def(py::init<py::array>(), py::arg("array"))
 		.def_property_readonly("value", &ArrayControlValue::get_array)
 		.def("to_json", &ArrayControlValue::to_json)
 		.def("__repr__", &ArrayControlValue::to_string)
 		.def("__str__", &ArrayControlValue::to_string);
+
+#if LINUX_VERSION_CODE >= KERNEL_VERSION(5, 5, 0)
+	py::class_<v4l2_area>(m, "area", "V4L2 struct for an area")
+		.def_readwrite("width", &v4l2_area::width)
+		.def_readwrite("height", &v4l2_area::height)
+		.def("__str__", &representation_area)
+		.def("__repr__", &representation_area);
+
+	py::class_<AreaControlValue, ControlValue>(
+		m, "AreaControlValue",
+		"Class that represents the value of an area control")
+		.def(py::init<v4l2_area>(), py::arg("area"))
+		.def("value", &AreaControlValue::get_area)
+		.def("to_json", &AreaControlValue::to_json)
+		.def("__repr__", &AreaControlValue::to_string)
+		.def("__str__", &AreaControlValue::to_string);
+#endif
+
 	py::class_<trigger_sequence>(m, "trigger_sequence",
 				     "V4L2 struct for a sequence")
 		.def_readwrite("exposure_time",
 			       &trigger_sequence::exposure_time)
 		.def_readwrite("flash_time", &trigger_sequence::flash_time)
 		.def_readwrite("frame_delay", &trigger_sequence::frame_delay)
 		.def_readwrite("trigger_delay",
@@ -906,23 +937,17 @@
 		.def_readonly("changes", &SourceEvent::changes,
 			      "Flags that show what has changed for the source")
 		.def("__repr__", &SourceEvent::to_string)
 		.def("__str__", &SourceEvent::to_string);
 	/*
 	 * EXCEPTIONS
 	 */
-	// Translation of V4l2Exception to Python exception of same name
-	static py::exception<V4L2Exception> ex(m, "V4L2Exception");
-	py::register_exception_translator([](std::exception_ptr p) {
-		try {
-			if (p) {
-				rethrow_exception(p);
-			}
-		} catch (const V4L2Exception &e) {
-			ex(e.what());
-		}
-	});
+	py::register_exception<V4L2Exception>(m, "V4L2Exception");
+
+	const py::object V4L2ExceptionBase = m.attr("V4L2Exception");
+	py::register_exception<V4L2BusyException>(m, "V4L2BusyException",
+						  V4L2ExceptionBase);
 
 	py::register_exception<TimeoutException>(m, "TimeoutException");
 	py::register_exception<DroppedFrameException>(m,
 						      "DroppedFrameException");
 }
```

### Comparing `qamlib-0.8.0/src/streaming_device.cpp` & `qamlib-0.9.0/src/streaming_device.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 struct v4l2_format StreamingDevice::read_format()
 {
 	struct v4l2_format fmt {
 		.type = device_type,
 	};
 
 	if (0 != ioctl(fd, VIDIOC_G_FMT, &fmt)) {
-		throw V4L2Exception("Error getting format from V4L2", errno);
+		v4l2_exception("Error getting format from V4L2", errno);
 	}
 
 	return fmt;
 }
 
 void StreamingDevice::update_format()
 {
@@ -93,44 +93,33 @@
 /*
  * Set camera resolution
  * Returns actual new resolution
  */
 std::tuple<uint32_t, uint32_t>
 StreamingDevice::set_resolution(uint32_t newWidth, uint32_t newHeight)
 {
-	bool restart = false;
-
 	// Make sure 'format' is up to date
 	struct v4l2_format current_format = read_format();
 
 	current_format.fmt.pix.width = newWidth;
 	current_format.fmt.pix.height = newHeight;
 
-	if (streaming) {
-		stop();
-		restart = true;
-	}
-
 	if (0 != ioctl(fd, VIDIOC_S_FMT, &current_format)) {
-		throw V4L2Exception("Error setting format for new resolution",
-				    errno);
+		v4l2_exception("Error setting format for new resolution",
+			       errno);
 	}
 
 #if DEBUG
 	uint32_t height = current_format.fmt.pix.height;
 	uint32_t width = current_format.fmt.pix.width;
 	if (width != newWidth || height != newHeight) {
 		DPRINT("Failed to get the requested resolution\n");
 	}
 #endif
 
-	if (restart) {
-		start();
-	}
-
 	return { current_format.fmt.pix.width, current_format.fmt.pix.height };
 }
 
 /*
  * CROPPING
  */
 
@@ -148,17 +137,16 @@
 #ifdef QTEC_HEADER
 	struct v4l2_ext_rect rects[MAX_CROP_RECTS];
 	selection.pr = rects;
 	selection.rectangles = MAX_CROP_RECTS;
 #endif
 
 	if (ioctl(fd, VIDIOC_G_SELECTION, &selection) != 0) {
-		throw V4L2Exception(
-			"Selection likely not supported for this device",
-			errno);
+		v4l2_exception("Selection likely not supported for this device",
+			       errno);
 	}
 
 #ifdef QTEC_HEADER
 	// If there is only one crop rectangle, rectangles is set to 0 and the
 	// "normal" selection rectangle is populated
 	if (selection.rectangles == 0) {
 		auto rect = Rectangle(selection.r.left, selection.r.top,
@@ -188,20 +176,14 @@
 	auto rect = Rectangle(left, top, width, height);
 
 	set_crop(rect);
 }
 
 void StreamingDevice::set_crop(Rectangle rectangle)
 {
-	bool restart_stream = false;
-	if (streaming) {
-		stop();
-		restart_stream = true;
-	}
-
 	auto [cur_width, cur_height] = get_resolution();
 	if (cur_width != rectangle.width || cur_height != rectangle.height) {
 		// Set resolution before selection
 		set_resolution(rectangle.width, rectangle.height);
 	}
 
 	struct v4l2_selection selection = {
@@ -210,22 +192,15 @@
 	};
 	selection.r.left = rectangle.left;
 	selection.r.top = rectangle.top;
 	selection.r.width = rectangle.width;
 	selection.r.height = rectangle.height;
 
 	if (ioctl(fd, VIDIOC_S_SELECTION, &selection) != 0) {
-		if (restart_stream) {
-			start();
-		}
-		throw V4L2Exception("Could not set desired selection", errno);
-	}
-
-	if (restart_stream) {
-		start();
+		v4l2_exception("Could not set desired selection", errno);
 	}
 }
 
 #ifdef QTEC_HEADER
 void StreamingDevice::set_crop(std::vector<Rectangle> rectangles)
 {
 	if (rectangles.size() == 1) {
@@ -234,47 +209,20 @@
 	}
 
 	if (rectangles.size() > MAX_CROP_RECTS) {
 		throw V4L2Exception(
 			"More than 8 crop rectangles not supported");
 	}
 
-	bool restart_stream = false;
-	if (streaming) {
-		stop();
-		restart_stream = true;
-	}
-
 	uint32_t width = rectangles[0].width;
 	uint32_t height = 0;
 
-	// Check for overlapping rectangles, we only check in height, since
-	// they should all be at the same left and width.
 	for (size_t i = 0; i < rectangles.size(); i++) {
-		auto a = rectangles[i];
-
-		// Only check for the remaining part of the list, since we have
-		// already checked with the previous rectangles.
-		for (size_t j = i + 1; j < rectangles.size(); j++) {
-			auto b = rectangles[j];
-
-			// Bottom most point for the rectangles
-			int a_bottom = a.top + static_cast<int>(a.height);
-			int b_bottom = b.top + static_cast<int>(b.height);
-
-			if (a.top == b.top ||
-			    (a.top < b.top && a_bottom > b.top) ||
-			    (a.top > b.top && b_bottom > a.top)) {
-				throw V4L2Exception("Multi-crop rectangles "
-						    "must not overlap");
-			}
-		}
-
 		// Sum height for the new resolution
-		height += a.height;
+		height += rectangles[i].height;
 	}
 
 	auto [cur_width, cur_height] = get_resolution();
 	if (cur_width != width || cur_height != height) {
 		// Set resolution before selection
 		set_resolution(width, height);
 	}
@@ -292,54 +240,45 @@
 		.type = device_type,
 		.target = V4L2_SEL_TGT_CROP,
 		.rectangles = static_cast<uint32_t>(rectangles.size()),
 		.pr = rects,
 	};
 
 	if (ioctl(fd, VIDIOC_S_SELECTION, &selection) != 0) {
-		if (restart_stream) {
-			start();
-		}
-		throw V4L2Exception("Could not set desired selection", errno);
-	}
-
-	if (restart_stream) {
-		start();
+		v4l2_exception("Could not set desired selection", errno);
 	}
 }
 #endif
 
 Rectangle StreamingDevice::get_crop_default()
 {
 	struct v4l2_selection selection = {
 		.type = device_type,
 		.target = V4L2_SEL_TGT_CROP_DEFAULT,
 	};
 
 	if (ioctl(fd, VIDIOC_G_SELECTION, &selection) != 0) {
-		throw V4L2Exception(
-			"Selection likely not supported for this device",
-			errno);
+		v4l2_exception("Selection likely not supported for this device",
+			       errno);
 	}
 
 	return Rectangle(selection.r.left, selection.r.top, selection.r.width,
 			 selection.r.height);
 }
 
 Rectangle StreamingDevice::get_crop_bounds()
 {
 	struct v4l2_selection selection = {
 		.type = device_type,
 		.target = V4L2_SEL_TGT_CROP_BOUNDS,
 	};
 
 	if (ioctl(fd, VIDIOC_G_SELECTION, &selection) != 0) {
-		throw V4L2Exception(
-			"Selection likely not supported for this device",
-			errno);
+		v4l2_exception("Selection likely not supported for this device",
+			       errno);
 	}
 
 	return Rectangle(selection.r.left, selection.r.top, selection.r.width,
 			 selection.r.height);
 }
 
 /*
```

### Comparing `qamlib-0.8.0/src/utils.cpp` & `qamlib-0.9.0/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/tests/test_events.py` & `qamlib-0.9.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/tests/test_long.py` & `qamlib-0.9.0/tests/test_long.py`

 * *Files identical despite different names*

### Comparing `qamlib-0.8.0/PKG-INFO` & `qamlib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qamlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: A library for interacting with Video4Linux2 (V4L2) video devices
 Author-Email: Daniel Lundberg Pedersen <dlp@qtec.com>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -584,20 +584,21 @@
 
 ```sh
 python -m build
 ```
 
 ### C++
 
-Dependicies
+Dependencies
 
 - `gcc`
 - `meson`
 - `ninja`
 - `nlohmann-json`
+- `opencv4`
 
 To build the library we start by running `meson` setup:
 
 ```sh
 meson setup build -Dpython=false
 ```
```

