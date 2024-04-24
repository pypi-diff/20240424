# Comparing `tmp/wavelink-3.2.0.tar.gz` & `tmp/wavelink-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wavelink-3.2.0.tar", last modified: Sun Feb  4 10:26:53 2024, max compression
+gzip compressed data, was "wavelink-3.3.0.tar", last modified: Wed Apr 24 02:45:55 2024, max compression
```

## Comparing `wavelink-3.2.0.tar` & `wavelink-3.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:26:53.397089 wavelink-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-04 10:26:41.000000 wavelink-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-02-04 10:26:53.397089 wavelink-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-04 10:26:41.000000 wavelink-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-04 10:26:41.000000 wavelink-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-04 10:26:41.000000 wavelink-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 10:26:53.397089 wavelink-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:26:53.397089 wavelink-3.2.0/wavelink/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27264 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/lfu.py
--rw-r--r--   0 runner    (1001) docker     (127)    34003 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/payloads.py
--rw-r--r--   0 runner    (1001) docker     (127)    35626 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/player.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20099 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:26:53.397089 wavelink-3.2.0/wavelink/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/tracks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/types/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-02-04 10:26:41.000000 wavelink-3.2.0/wavelink/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 10:26:53.397089 wavelink-3.2.0/wavelink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-02-04 10:26:53.000000 wavelink-3.2.0/wavelink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-02-04 10:26:53.000000 wavelink-3.2.0/wavelink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 10:26:53.000000 wavelink-3.2.0/wavelink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-04 10:26:53.000000 wavelink-3.2.0/wavelink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-04 10:26:53.000000 wavelink-3.2.0/wavelink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:45:55.789512 wavelink-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 02:45:48.000000 wavelink-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-24 02:45:55.789512 wavelink-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-24 02:45:48.000000 wavelink-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-24 02:45:48.000000 wavelink-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 02:45:48.000000 wavelink-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:45:55.789512 wavelink-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:45:55.789512 wavelink-3.3.0/wavelink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29479 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/lfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34562 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18972 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/payloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37517 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20117 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22558 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:45:55.789512 wavelink-3.3.0/wavelink/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/types/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-24 02:45:48.000000 wavelink-3.3.0/wavelink/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:45:55.789512 wavelink-3.3.0/wavelink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-24 02:45:55.000000 wavelink-3.3.0/wavelink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 02:45:55.000000 wavelink-3.3.0/wavelink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:45:55.000000 wavelink-3.3.0/wavelink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 02:45:55.000000 wavelink-3.3.0/wavelink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 02:45:55.000000 wavelink-3.3.0/wavelink.egg-info/top_level.txt
```

### Comparing `wavelink-3.2.0/LICENSE` & `wavelink-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wavelink-3.2.0/PKG-INFO` & `wavelink-3.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavelink
-Version: 3.2.0
+Version: 3.3.0
 Summary: A robust and powerful, fully asynchronous Lavalink wrapper built for discord.py in Python.
 Author-email: "PythonistaGuild, EvieePy" <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>=3.7.4
 Requires-Dist: discord.py>=2.0.1
 Requires-Dist: yarl>=1.9.2
 Requires-Dist: async_timeout
+Requires-Dist: typing_extensions
 
 <div align="center">
 
 
 ![Logo](https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/Wavelink)
```

### Comparing `wavelink-3.2.0/README.md` & `wavelink-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wavelink-3.2.0/wavelink/__init__.py` & `wavelink-3.3.0/wavelink/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "3.2.0"
+__version__ = "3.3.0"
 
 
 from .enums import *
 from .exceptions import *
 from .filters import *
-from .lfu import CapacityZero as CapacityZero
-from .lfu import LFUCache as LFUCache
+from .lfu import CapacityZero as CapacityZero, LFUCache as LFUCache
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .queue import *
 from .tracks import *
 from .utils import ExtrasNamespace as ExtrasNamespace
```

### Comparing `wavelink-3.2.0/wavelink/__main__.py` & `wavelink-3.3.0/wavelink/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import argparse
 import platform
 import subprocess
 import sys
 
 import wavelink
 
+
 parser = argparse.ArgumentParser(prog="wavelink")
 parser.add_argument("--version", action="store_true", help="Get version and debug information for wavelink.")
 
 
 args = parser.parse_args()
 
 
 def get_debug_info() -> None:
     python_info = "\n".join(sys.version.split("\n"))
     java_version = subprocess.check_output(["java", "-version"], stderr=subprocess.STDOUT)
     java_version = f'\n{" " * 8}- '.join(v for v in java_version.decode().split("\r\n") if v)
 
     info: str = f"""
     wavelink: {wavelink.__version__}
-    
+
     Python:
         - {python_info}
     System:
         - {platform.platform()}
     Java:
         - {java_version or "Version Not Found"}
     """
```

### Comparing `wavelink-3.2.0/wavelink/backoff.py` & `wavelink-3.3.0/wavelink/backoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,23 @@
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
+
 from __future__ import annotations
 
 import random
-from collections.abc import Callable
+from typing import TYPE_CHECKING
+
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
 
 
 class Backoff:
     """An implementation of an Exponential Backoff.
 
     Parameters
     ----------
```

### Comparing `wavelink-3.2.0/wavelink/enums.py` & `wavelink-3.3.0/wavelink/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 import enum
 
+
 __all__ = ("NodeStatus", "TrackSource", "DiscordVoiceCloseType", "AutoPlayMode", "QueueMode")
 
 
 class NodeStatus(enum.Enum):
     """Enum representing the connection status of a Node.
 
     Attributes
```

### Comparing `wavelink-3.2.0/wavelink/exceptions.py` & `wavelink-3.3.0/wavelink/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+
 if TYPE_CHECKING:
     from .types.response import ErrorResponse, LoadedErrorPayload
 
 
 __all__ = (
     "WavelinkException",
     "NodeException",
```

### Comparing `wavelink-3.2.0/wavelink/filters.py` & `wavelink-3.3.0/wavelink/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,31 +17,35 @@
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, TypedDict
 
+
 if TYPE_CHECKING:
     from typing_extensions import Self, Unpack
 
-    from .types.filters import ChannelMix as ChannelMixPayload
-    from .types.filters import Distortion as DistortionPayload
-    from .types.filters import Equalizer as EqualizerPayload
-    from .types.filters import FilterPayload
-    from .types.filters import Karaoke as KaraokePayload
-    from .types.filters import LowPass as LowPassPayload
-    from .types.filters import Rotation as RotationPayload
-    from .types.filters import Timescale as TimescalePayload
-    from .types.filters import Tremolo as TremoloPayload
-    from .types.filters import Vibrato as VibratoPayload
+    from .types.filters import (
+        ChannelMix as ChannelMixPayload,
+        Distortion as DistortionPayload,
+        Equalizer as EqualizerPayload,
+        FilterPayload,
+        Karaoke as KaraokePayload,
+        LowPass as LowPassPayload,
+        Rotation as RotationPayload,
+        Timescale as TimescalePayload,
+        Tremolo as TremoloPayload,
+        Vibrato as VibratoPayload,
+    )
 
 
 __all__ = (
     "FiltersOptions",
     "Filters",
     "Equalizer",
     "Karaoke",
@@ -676,35 +680,62 @@
         self._equalizer = filters.get("equalizer", Equalizer(None))
         self._karaoke = filters.get("karaoke", Karaoke({}))
         self._timescale = filters.get("timescale", Timescale({}))
         self._tremolo = filters.get("tremolo", Tremolo({}))
         self._vibrato = filters.get("vibrato", Vibrato({}))
         self._rotation = filters.get("rotation", Rotation({}))
         self._distortion = filters.get("distortion", Distortion({}))
-        self._channel_mix = filters.get("channelMix", ChannelMix({}))
-        self._low_pass = filters.get("lowPass", LowPass({}))
+        self._channel_mix = filters.get("channel_mix", ChannelMix({}))
+        self._low_pass = filters.get("low_pass", LowPass({}))
 
     def set_filters(self, **filters: Unpack[FiltersOptions]) -> None:
-        # TODO: document this later maybe?
+        """Set multiple filters at once to a standalone Filter object.
+        To set the filters to the player directly see :meth:`wavelink.Player.set_filters`
+
+        Parameters
+        ----------
+        volume: float
+            The Volume filter to apply to the player.
+        equalizer: :class:`wavelink.Equalizer`
+            The Equalizer filter to apply to the player.
+        karaoke: :class:`wavelink.Karaoke`
+            The Karaoke filter to apply to the player.
+        timescale: :class:`wavelink.Timescale`
+            The Timescale filter to apply to the player.
+        tremolo: :class:`wavelink.Tremolo`
+            The Tremolo filter to apply to the player.
+        vibrato: :class:`wavelink.Vibrato`
+            The Vibrato filter to apply to the player.
+        rotation: :class:`wavelink.Rotation`
+            The Rotation filter to apply to the player.
+        distortion: :class:`wavelink.Distortion`
+            The Distortion filter to apply to the player.
+        channel_mix: :class:`wavelink.ChannelMix`
+            The ChannelMix filter to apply to the player.
+        low_pass: :class:`wavelink.LowPass`
+            The LowPass filter to apply to the player.
+        reset: bool
+            Whether to reset all filters that were not specified.
+        """
 
         reset: bool = filters.get("reset", False)
         if reset:
             self._set_with_reset(filters)
             return
 
         self._volume = filters.get("volume", self._volume)
         self._equalizer = filters.get("equalizer", self._equalizer)
         self._karaoke = filters.get("karaoke", self._karaoke)
         self._timescale = filters.get("timescale", self._timescale)
         self._tremolo = filters.get("tremolo", self._tremolo)
         self._vibrato = filters.get("vibrato", self._vibrato)
         self._rotation = filters.get("rotation", self._rotation)
         self._distortion = filters.get("distortion", self._distortion)
-        self._channel_mix = filters.get("channelMix", self._channel_mix)
-        self._low_pass = filters.get("lowPass", self._low_pass)
+        self._channel_mix = filters.get("channel_mix", self._channel_mix)
+        self._low_pass = filters.get("low_pass", self._low_pass)
 
     def _reset(self) -> None:
         self._volume = None
         self._equalizer = Equalizer(None)
         self._karaoke = Karaoke({})
         self._timescale = Timescale({})
         self._tremolo = Tremolo({})
@@ -713,21 +744,47 @@
         self._distortion = Distortion({})
         self._channel_mix = ChannelMix({})
         self._low_pass = LowPass({})
 
     def reset(self) -> None:
         """Method which resets this object to an original state.
 
-        Using this method will clear all indivdual filters, and assign the wavelink default classes.
+        This method will clear all individual filters, and assign the wavelink default classes.
         """
         self._reset()
 
     @classmethod
     def from_filters(cls, **filters: Unpack[FiltersOptions]) -> Self:
-        # TODO: document this later maybe?
+        """Creates a Filters object with specified filters.
+
+        Parameters
+        ----------
+        volume: float
+            The Volume filter to apply to the player.
+        equalizer: :class:`wavelink.Equalizer`
+            The Equalizer filter to apply to the player.
+        karaoke: :class:`wavelink.Karaoke`
+            The Karaoke filter to apply to the player.
+        timescale: :class:`wavelink.Timescale`
+            The Timescale filter to apply to the player.
+        tremolo: :class:`wavelink.Tremolo`
+            The Tremolo filter to apply to the player.
+        vibrato: :class:`wavelink.Vibrato`
+            The Vibrato filter to apply to the player.
+        rotation: :class:`wavelink.Rotation`
+            The Rotation filter to apply to the player.
+        distortion: :class:`wavelink.Distortion`
+            The Distortion filter to apply to the player.
+        channel_mix: :class:`wavelink.ChannelMix`
+            The ChannelMix filter to apply to the player.
+        low_pass: :class:`wavelink.LowPass`
+            The LowPass filter to apply to the player.
+        reset: bool
+            Whether to reset all filters that were not specified.
+        """
 
         self = cls()
         self._set_with_reset(filters)
 
         return self
 
     @property
```

### Comparing `wavelink-3.2.0/wavelink/lfu.py` & `wavelink-3.3.0/wavelink/lfu.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import Any
 
 from .exceptions import WavelinkException
 
 
-class CapacityZero(WavelinkException):
-    ...
+class CapacityZero(WavelinkException): ...
 
 
 class _MissingSentinel:
     __slots__ = ()
 
     def __eq__(self, other: object) -> bool:
         return False
```

### Comparing `wavelink-3.2.0/wavelink/node.py` & `wavelink-3.3.0/wavelink/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,24 +17,23 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 import logging
 import secrets
 import urllib.parse
-from collections.abc import Iterable
-from typing import TYPE_CHECKING, Any, Literal, TypeAlias
+from typing import TYPE_CHECKING, Any, ClassVar, Literal, TypeAlias
 
 import aiohttp
-import discord
 from discord.utils import classproperty
 
 from . import __version__
 from .enums import NodeStatus
 from .exceptions import (
     AuthorizationFailedException,
     InvalidClientException,
@@ -44,15 +43,20 @@
     NodeException,
 )
 from .lfu import LFUCache
 from .payloads import *
 from .tracks import Playable, Playlist
 from .websocket import Websocket
 
+
 if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    import discord
+
     from .player import Player
     from .types.request import Request, UpdateSessionRequest
     from .types.response import (
         EmptyLoadedResponse,
         ErrorLoadedResponse,
         ErrorResponse,
         InfoResponse,
@@ -156,15 +160,15 @@
         self._total_player_count: int | None = None
 
         self._spotify_enabled: bool = False
 
         self._websocket: Websocket | None = None
 
         if inactive_player_timeout and inactive_player_timeout < 10:
-            logger.warn('Setting "inactive_player_timeout" below 10 seconds may result in unwanted side effects.')
+            logger.warning('Setting "inactive_player_timeout" below 10 seconds may result in unwanted side effects.')
 
         self._inactive_player_timeout = (
             inactive_player_timeout if inactive_player_timeout and inactive_player_timeout > 0 else None
         )
 
     def __repr__(self) -> str:
         return f"Node(identifier={self.identifier}, uri={self.uri}, status={self.status}, players={len(self.players)})"
@@ -263,46 +267,60 @@
         .. versionadded:: 3.0.0
         """
         return self._session_id
 
     async def _pool_closer(self) -> None:
         try:
             await self._session.close()
-        except:
+        except Exception:
             pass
 
         if not self._has_closed:
             await self.close()
 
-    async def close(self) -> None:
+    async def close(self, eject: bool = False) -> None:
         """Method to close this Node and cleanup.
 
         After this method has finished, the event ``on_wavelink_node_closed`` will be fired.
 
         This method renders the Node websocket disconnected and disconnects all players.
+
+        Parameters
+        ----------
+        eject: bool
+            If ``True``, this will remove the Node from the Pool. Defaults to ``False``.
+
+
+        .. versionchanged:: 3.2.1
+
+            Added the ``eject`` parameter. Fixed a bug where the connected Players were not being disconnected.
         """
         disconnected: list[Player] = []
 
-        for player in self._players.values():
+        for player in self._players.copy().values():
             try:
-                await player._destroy()
-            except LavalinkException:
+                await player.disconnect()
+            except Exception as e:
+                logger.debug("An error occured while disconnecting a player in the close method of %r: %s", self, e)
                 pass
 
             disconnected.append(player)
 
         if self._websocket is not None:
             await self._websocket.cleanup()
 
         self._status = NodeStatus.DISCONNECTED
         self._session_id = None
         self._players = {}
 
         self._has_closed = True
 
+        if eject:
+            getattr(Pool, "_Pool__nodes").pop(self.identifier, None)
+
         # Dispatch Node Closed Event... node, list of disconnected players
         if self.client is not None:
             self.client.dispatch("wavelink_node_closed", self, disconnected)
 
     async def _connect(self, *, client: discord.Client | None) -> None:
         client_ = self._client or client
 
@@ -374,15 +392,15 @@
             if resp.status == 204:
                 return
 
             if resp.status >= 300:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
             try:
                 rdata: Any = await resp.json()
             except aiohttp.ContentTypeError:
@@ -405,15 +423,15 @@
                 resp_data: list[PlayerResponse] = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def fetch_players(self) -> list[PlayerResponsePayload]:
         """Method to fetch the player information Lavalink holds for every connected player on this node.
 
@@ -452,15 +470,15 @@
                 resp_data: PlayerResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def fetch_player_info(self, guild_id: int, /) -> PlayerResponsePayload | None:
         """Method to fetch the player information Lavalink holds for the specific guild.
 
@@ -513,30 +531,30 @@
                 resp_data: PlayerResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def _destroy_player(self, guild_id: int, /) -> None:
         uri: str = f"{self.uri}/v4/sessions/{self.session_id}/players/{guild_id}"
 
         async with self._session.delete(url=uri, headers=self.headers) as resp:
             if resp.status == 204:
                 return
 
             try:
                 exc_data: ErrorResponse = await resp.json()
             except Exception as e:
-                logger.warning(f"An error occured making a request on {self!r}: {e}")
+                logger.warning("An error occured making a request on %r: %s", self, e)
                 raise NodeException(status=resp.status)
 
             raise LavalinkException(data=exc_data)
 
     async def _update_session(self, *, data: UpdateSessionRequest) -> UpdateResponse:
         uri: str = f"{self.uri}/v4/sessions/{self.session_id}"
 
@@ -545,15 +563,15 @@
                 resp_data: UpdateResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def _fetch_tracks(self, query: str) -> LoadedResponse:
         uri: str = f"{self.uri}/v4/loadtracks?identifier={query}"
 
@@ -562,38 +580,36 @@
                 resp_data: LoadedResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
-    async def _decode_track(self) -> TrackPayload:
-        ...
+    async def _decode_track(self) -> TrackPayload: ...
 
-    async def _decode_tracks(self) -> list[TrackPayload]:
-        ...
+    async def _decode_tracks(self) -> list[TrackPayload]: ...
 
     async def _fetch_info(self) -> InfoResponse:
         uri: str = f"{self.uri}/v4/info"
 
         async with self._session.get(url=uri, headers=self.headers) as resp:
             if resp.status == 200:
                 resp_data: InfoResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def fetch_info(self) -> InfoResponsePayload:
         """Method to fetch this Lavalink Nodes info response data.
 
@@ -626,15 +642,15 @@
                 resp_data: StatsResponse = await resp.json()
                 return resp_data
 
             else:
                 try:
                     exc_data: ErrorResponse = await resp.json()
                 except Exception as e:
-                    logger.warning(f"An error occured making a request on {self!r}: {e}")
+                    logger.warning("An error occured making a request on %r: %s", self, e)
                     raise NodeException(status=resp.status)
 
                 raise LavalinkException(data=exc_data)
 
     async def fetch_stats(self) -> StatsResponsePayload:
         """Method to fetch this Lavalink Nodes stats response data.
 
@@ -665,15 +681,15 @@
         async with self._session.get(url=uri, headers=self.headers) as resp:
             if resp.status == 200:
                 return await resp.text()
 
             try:
                 exc_data: ErrorResponse = await resp.json()
             except Exception as e:
-                logger.warning(f"An error occured making a request on {self!r}: {e}")
+                logger.warning("An error occured making a request on %r: %s", self, e)
                 raise NodeException(status=resp.status)
 
             raise LavalinkException(data=exc_data)
 
     async def fetch_version(self) -> str:
         """Method to fetch this Lavalink version string.
 
@@ -719,15 +735,15 @@
     To connect a :class:`~wavelink.Node` please use this Pool.
 
     .. note::
 
         All methods and attributes on this class are class level, not instance. Do not create an instance of this class.
     """
 
-    __nodes: dict[str, Node] = {}
+    __nodes: ClassVar[dict[str, Node]] = {}
     __cache: LFUCache | None = None
 
     @classmethod
     async def connect(
         cls, *, nodes: Iterable[Node], client: discord.Client | None = None, cache_capacity: int | None = None
     ) -> dict[str, Node]:
         """Connect the provided Iterable[:class:`Node`] to Lavalink.
@@ -770,27 +786,27 @@
             if node.identifier in cls.__nodes:
                 msg: str = f'Unable to connect {node!r} as you already have a node with identifier "{node.identifier}"'
                 logger.error(msg)
 
                 continue
 
             if node.status in (NodeStatus.CONNECTING, NodeStatus.CONNECTED):
-                logger.error(f"Unable to connect {node!r} as it is already in a connecting or connected state.")
+                logger.error("Unable to connect %r as it is already in a connecting or connected state.", node)
                 continue
 
             try:
                 await node._connect(client=client_)
             except InvalidClientException as e:
                 logger.error(e)
             except AuthorizationFailedException:
-                logger.error(f"Failed to authenticate {node!r} on Lavalink with the provided password.")
+                logger.error("Failed to authenticate %r on Lavalink with the provided password.", node)
             except NodeException:
                 logger.error(
-                    f"Failed to connect to {node!r}. Check that your Lavalink major version is '4' "
-                    "and that you are trying to connect to Lavalink on the correct port."
+                    "Failed to connect to %r. Check that your Lavalink major version is '4' and that you are trying to connect to Lavalink on the correct port.",
+                    node,
                 )
             else:
                 cls.__nodes[node.identifier] = node
 
         if cache_capacity is not None and cls.nodes:
             if cache_capacity <= 0:
                 logger.warning("LFU Request cache capacity must be > 0. Not enabling cache.")
@@ -808,19 +824,19 @@
                 continue
 
             try:
                 await node._connect(client=None)
             except InvalidClientException as e:
                 logger.error(e)
             except AuthorizationFailedException:
-                logger.error(f"Failed to authenticate {node!r} on Lavalink with the provided password.")
+                logger.error("Failed to authenticate %r on Lavalink with the provided password.", node)
             except NodeException:
                 logger.error(
-                    f"Failed to connect to {node!r}. Check that your Lavalink major version is '4' "
-                    "and that you are trying to connect to Lavalink on the correct port."
+                    "Failed to connect to %r. Check that your Lavalink major version is '4' and that you are trying to connect to Lavalink on the correct port.",
+                    node,
                 )
 
         return cls.nodes
 
     @classmethod
     async def close(cls) -> None:
         """Close and clean up all :class:`~wavelink.Node` on this Pool.
```

### Comparing `wavelink-3.2.0/wavelink/payloads.py` & `wavelink-3.3.0/wavelink/payloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, cast
 
 import wavelink
 
 from .enums import DiscordVoiceCloseType
 from .filters import Filters
 from .tracks import Playable
 
+
 if TYPE_CHECKING:
     from .node import Node
     from .player import Player
     from .types.filters import *
     from .types.response import *
     from .types.state import PlayerState
     from .types.stats import CPUStats, FrameStats, MemoryStats
```

### Comparing `wavelink-3.2.0/wavelink/player.py` & `wavelink-3.3.0/wavelink/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 import asyncio
 import logging
 import random
 import time
-from collections import deque
 from typing import TYPE_CHECKING, Any, TypeAlias
 
 import async_timeout
 import discord
 from discord.abc import Connectable
 from discord.utils import MISSING
 
@@ -51,20 +51,31 @@
     PlayerUpdateEventPayload,
     TrackEndEventPayload,
     TrackStartEventPayload,
 )
 from .queue import Queue
 from .tracks import Playable, Playlist
 
+
 if TYPE_CHECKING:
-    from discord.types.voice import GuildVoiceState as GuildVoiceStatePayload
-    from discord.types.voice import VoiceServerUpdate as VoiceServerUpdatePayload
+    from collections import deque
+
+    from discord.abc import Connectable
+    from discord.types.voice import (
+        GuildVoiceState as GuildVoiceStatePayload,
+        VoiceServerUpdate as VoiceServerUpdatePayload,
+    )
     from typing_extensions import Self
 
     from .node import Node
+    from .payloads import (
+        PlayerUpdateEventPayload,
+        TrackEndEventPayload,
+        TrackStartEventPayload,
+    )
     from .types.request import Request as RequestPayload
     from .types.state import PlayerVoiceState, VoiceState
 
     VocalGuildChannel = discord.VoiceChannel | discord.StageChannel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -224,29 +235,30 @@
         elif payload.reason == "loadFailed":
             self._error_count += 1
 
         else:
             self._error_count = 0
 
         if self.node.status is not NodeStatus.CONNECTED:
-            logger.warning(f'"Unable to use AutoPlay on Player for Guild "{self.guild}" due to disconnected Node.')
+            logger.warning(
+                '"Unable to use AutoPlay on Player for Guild "%s" due to disconnected Node.', str(self.guild)
+            )
             return
 
         if not isinstance(self.queue, Queue) or not isinstance(self.auto_queue, Queue):  # type: ignore
-            logger.warning(f'"Unable to use AutoPlay on Player for Guild "{self.guild}" due to unsupported Queue.')
+            logger.warning(
+                '"Unable to use AutoPlay on Player for Guild "%s" due to unsupported Queue.', str(self.guild)
+            )
             self._inactivity_start()
             return
 
         if self.queue.mode is QueueMode.loop:
             await self._do_partial(history=False)
 
-        elif self.queue.mode is QueueMode.loop_all:
-            await self._do_partial()
-
-        elif self._autoplay is AutoPlayMode.partial or self.queue:
+        elif self.queue.mode is QueueMode.loop_all or (self._autoplay is AutoPlayMode.partial or self.queue):
             await self._do_partial()
 
         elif self._autoplay is AutoPlayMode.enabled:
             async with self._auto_lock:
                 await self._do_recommendation()
 
     async def _do_partial(self, *, history: bool = True) -> None:
@@ -258,19 +270,26 @@
             try:
                 track: Playable = self.queue.get()
             except QueueEmpty:
                 return
 
             await self.play(track, add_history=history)
 
-    async def _do_recommendation(self):
+    async def _do_recommendation(
+        self,
+        *,
+        populate_track: wavelink.Playable | None = None,
+        max_population: int | None = None,
+    ) -> None:
         assert self.guild is not None
         assert self.queue.history is not None and self.auto_queue.history is not None
 
-        if len(self.auto_queue) > self._auto_cutoff + 1:
+        max_population_: int = max_population if max_population else self._auto_cutoff
+
+        if len(self.auto_queue) > self._auto_cutoff + 1 and not populate_track:
             # We still do the inactivity start here since if play fails and we have no more tracks...
             # we should eventually fire the inactivity event...
             self._inactivity_start()
 
             track: Playable = self.auto_queue.get()
             self.auto_queue.history.put(track)
 
@@ -282,14 +301,17 @@
         choices: list[Playable | None] = [*weighted_history, *weighted_upcoming, self._current, self._previous]
 
         # Filter out tracks which are None...
         _previous: deque[str] = self.__previous_seeds._queue  # type: ignore
         seeds: list[Playable] = [t for t in choices if t is not None and t.identifier not in _previous]
         random.shuffle(seeds)
 
+        if populate_track:
+            seeds.insert(0, populate_track)
+
         spotify: list[str] = [t.identifier for t in seeds if t.source == "spotify"]
         youtube: list[str] = [t.identifier for t in seeds if t.source == "youtube"]
 
         spotify_query: str | None = None
         youtube_query: str | None = None
 
         count: int = len(self.queue.history)
@@ -334,57 +356,56 @@
                 search: wavelink.Search = await Pool.fetch_tracks(query)
             except (LavalinkLoadException, LavalinkException):
                 return []
 
             if not search:
                 return []
 
-            tracks: list[Playable]
-            if isinstance(search, Playlist):
-                tracks = search.tracks.copy()
-            else:
-                tracks = search
-
+            tracks: list[Playable] = search.tracks.copy() if isinstance(search, Playlist) else search
             return tracks
 
         results: tuple[T_a, T_a] = await asyncio.gather(_search(spotify_query), _search(youtube_query))
 
         # track for result in results for track in result...
         filtered_r: list[Playable] = [t for r in results for t in r]
 
-        if not filtered_r:
-            logger.debug(f'Player "{self.guild.id}" could not load any songs via AutoPlay.')
+        if not filtered_r and not self.auto_queue:
+            logger.info('Player "%s" could not load any songs via AutoPlay.', self.guild.id)
             self._inactivity_start()
             return
 
-        if not self._current:
-            now: Playable = filtered_r.pop(1)
-            now._recommended = True
-            self.auto_queue.history.put(now)
-
-            await self.play(now, add_history=False)
-
         # Possibly adjust these thresholds?
         history: list[Playable] = (
             self.auto_queue[:40] + self.queue[:40] + self.queue.history[:-41:-1] + self.auto_queue.history[:-61:-1]
         )
 
         added: int = 0
+
+        random.shuffle(filtered_r)
         for track in filtered_r:
             if track in history:
                 continue
 
             track._recommended = True
             added += await self.auto_queue.put_wait(track)
 
-        random.shuffle(self.auto_queue._items)
-        logger.debug(f'Player "{self.guild.id}" added "{added}" tracks to the auto_queue via AutoPlay.')
+            if added >= max_population_:
+                break
+
+        logger.debug('Player "%s" added "%s" tracks to the auto_queue via AutoPlay.', self.guild.id, added)
 
-        # Probably don't need this here as it's likely to be cancelled instantly...
-        self._inactivity_start()
+        if not self._current and not populate_track:
+            try:
+                now: Playable = self.auto_queue.get()
+                self.auto_queue.history.put(now)
+
+                await self.play(now, add_history=False)
+            except wavelink.QueueEmpty:
+                logger.info('Player "%s" could not load any songs via AutoPlay.', self.guild.id)
+                self._inactivity_start()
 
     @property
     def inactive_timeout(self) -> int | None:
         """A property which returns the time as an ``int`` of seconds to wait before this player dispatches the
         :func:`on_wavelink_inactive_player` event.
 
         This property could return ``None`` if no time has been set.
@@ -419,15 +440,15 @@
     def inactive_timeout(self, value: int | None) -> None:
         if not value or value <= 0:
             self._inactivity_wait = None
             self._inactivity_cancel()
             return
 
         if value < 10:
-            logger.warn('Setting "inactive_timeout" below 10 seconds may result in unwanted side effects.')
+            logger.warning('Setting "inactive_timeout" below 10 seconds may result in unwanted side effects.')
 
         self._inactivity_wait = value
         self._inactivity_cancel()
 
         if self.connected and not self.playing:
             self._inactivity_start()
 
@@ -610,15 +631,15 @@
         try:
             await self.node._update_player(self.guild.id, data=request)
         except LavalinkException:
             await self.disconnect()
         else:
             self._connection_event.set()
 
-        logger.debug(f"Player {self.guild.id} is dispatching VOICE_UPDATE.")
+        logger.debug("Player %s is dispatching VOICE_UPDATE.", self.guild.id)
 
     async def connect(
         self, *, timeout: float = 10.0, reconnect: bool, self_deaf: bool = False, self_mute: bool = False
     ) -> None:
         """
 
         .. warning::
@@ -719,14 +740,16 @@
         replace: bool = True,
         start: int = 0,
         end: int | None = None,
         volume: int | None = None,
         paused: bool | None = None,
         add_history: bool = True,
         filters: Filters | None = None,
+        populate: bool = False,
+        max_populate: int = 5,
     ) -> Playable:
         """Play the provided :class:`~wavelink.Playable`.
 
         Parameters
         ----------
         track: :class:`~wavelink.Playable`
             The track to being playing.
@@ -751,14 +774,31 @@
             If this argument is set to ``True``, the :class:`~Player` will add this track into the
             :class:`wavelink.Queue` history, if loading the track was successful. If ``False`` this track will not be
             added to your history. This does not directly affect the ``AutoPlay Queue`` but will alter how ``AutoPlay``
             recommends songs in the future. Defaults to ``True``.
         filters: Optional[:class:`~wavelink.Filters`]
             An Optional[:class:`~wavelink.Filters`] to apply when playing this track. Defaults to ``None``.
             If this is ``None`` the currently set filters on the player will be applied.
+        populate: bool
+            Whether the player should find and fill AutoQueue with recommended tracks based on the track provided.
+            Defaults to ``False``.
+
+            Populate will only search for recommended tracks when the current tracks has been accepted by Lavalink.
+            E.g. if this method does not raise an error.
+
+            You should consider when you use the ``populate`` keyword argument as populating the AutoQueue on every
+            request could potentially lead to a large amount of tracks being populated.
+        max_populate: int
+            The maximum amount of tracks that should be added to the AutoQueue when the ``populate`` keyword argument is
+            set to ``True``. This is NOT the exact amount of tracks that will be added. You should set this to a lower
+            amount to avoid the AutoQueue from being overfilled.
+
+            This argument has no effect when ``populate`` is set to ``False``.
+
+            Defaults to ``5``.
 
 
         Returns
         -------
         :class:`~wavelink.Playable`
             The track that began playing.
 
@@ -767,14 +807,19 @@
 
             Added the ``paused`` parameter. Parameters ``replace``, ``start``, ``end``, ``volume`` and ``paused``
             are now all keyword-only arguments.
 
             Added the ``add_history`` keyword-only argument.
 
             Added the ``filters`` keyword-only argument.
+
+
+        .. versionchanged:: 3.3.0
+
+            Added the ``populate`` keyword-only argument.
         """
         assert self.guild is not None
 
         original_vol: int = self._volume
         vol: int = volume or self._volume
 
         if vol != self._volume:
@@ -782,20 +827,17 @@
 
         if replace or not self._current:
             self._current = track
             self._original = track
 
         old_previous = self._previous
         self._previous = self._current
+        self.queue._loaded = track
 
-        pause: bool
-        if paused is not None:
-            pause = paused
-        else:
-            pause = self._paused
+        pause: bool = paused if paused is not None else self._paused
 
         if filters:
             self._filters = filters
 
         request: RequestPayload = {
             "track": {"encoded": track.encoded, "userData": dict(track.extras)},
             "volume": vol,
@@ -804,26 +846,30 @@
             "paused": pause,
             "filters": self._filters(),
         }
 
         try:
             await self.node._update_player(self.guild.id, data=request, replace=replace)
         except LavalinkException as e:
+            self.queue._loaded = old_previous
             self._current = None
             self._original = None
             self._previous = old_previous
             self._volume = original_vol
             raise e
 
         self._paused = pause
 
         if add_history:
             assert self.queue.history is not None
             self.queue.history.put(track)
 
+        if populate:
+            await self._do_recommendation(populate_track=track, max_population=max_populate)
+
         return track
 
     async def pause(self, value: bool, /) -> None:
         """Set the paused or resume state of the player.
 
         Parameters
         ----------
```

### Comparing `wavelink-3.2.0/wavelink/queue.py` & `wavelink-3.3.0/wavelink/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 import asyncio
 import random
 from collections import deque
 from collections.abc import Iterable, Iterator
 from typing import SupportsIndex, TypeGuard, overload
 
 from .enums import QueueMode
 from .exceptions import QueueEmpty
 from .tracks import Playable, Playlist
 
+
 __all__ = ("Queue",)
 
 
 class Queue:
     """The default custom wavelink Queue designed specifically for :class:`wavelink.Player`.
 
     .. note::
@@ -166,20 +168,18 @@
     def __call__(self, item: Playable) -> None:
         self.put(item)
 
     def __bool__(self) -> bool:
         return bool(self._items)
 
     @overload
-    def __getitem__(self, __index: SupportsIndex, /) -> Playable:
-        ...
+    def __getitem__(self, __index: SupportsIndex, /) -> Playable: ...
 
     @overload
-    def __getitem__(self, __index: slice, /) -> list[Playable]:
-        ...
+    def __getitem__(self, __index: slice, /) -> list[Playable]: ...
 
     def __getitem__(self, __index: SupportsIndex | slice, /) -> Playable | list[Playable]:
         return self._items[__index]
 
     def __setitem__(self, __index: SupportsIndex, __value: Playable, /) -> None:
         self._check_compatibility(__value)
         self._items[__index] = __value
@@ -349,15 +349,15 @@
             loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
             waiter: asyncio.Future[None] = loop.create_future()
 
             self._waiters.append(waiter)
 
             try:
                 await waiter
-            except:  # noqa
+            except:
                 waiter.cancel()
 
                 try:
                     self._waiters.remove(waiter)
                 except ValueError:  # pragma: no branch
                     pass
 
@@ -439,14 +439,15 @@
         added: int = 0
 
         async with self._lock:
             if isinstance(item, Iterable):
                 if atomic:
                     self._check_atomic(item)
                     self._items.extend(item)
+                    self._wakeup_next()
                     return len(item)
 
                 for track in item:
                     try:
                         self._check_compatibility(track)
                     except TypeError:
                         pass
```

### Comparing `wavelink-3.2.0/wavelink/tracks.py` & `wavelink-3.3.0/wavelink/tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,30 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
-from collections.abc import Iterator
 from typing import TYPE_CHECKING, Any, TypeAlias, overload
 
 import yarl
 
 import wavelink
 
 from .enums import TrackSource
 from .utils import ExtrasNamespace
 
+
 if TYPE_CHECKING:
+    from collections.abc import Iterator
+
     from .types.tracks import (
         PlaylistInfoPayload,
         PlaylistPayload,
         TrackInfoPayload,
         TrackPayload,
     )
 
@@ -529,20 +532,18 @@
 
         return self.name == other.name and self.tracks == other.tracks
 
     def __len__(self) -> int:
         return len(self.tracks)
 
     @overload
-    def __getitem__(self, index: int) -> Playable:
-        ...
+    def __getitem__(self, index: int) -> Playable: ...
 
     @overload
-    def __getitem__(self, index: slice) -> list[Playable]:
-        ...
+    def __getitem__(self, index: slice) -> list[Playable]: ...
 
     def __getitem__(self, index: int | slice) -> Playable | list[Playable]:
         return self.tracks[index]
 
     def __iter__(self) -> Iterator[Playable]:
         return self.tracks.__iter__()
 
@@ -588,15 +589,15 @@
     def extras(self) -> ExtrasNamespace:
         """Property returning a :class:`~wavelink.ExtrasNamespace` of extras for this :class:`Playlist`.
 
         You can set this property with a :class:`dict` of valid :class:`str` keys to any valid ``JSON`` value,
         or a :class:`~wavelink.ExtrasNamespace`.
 
         If a dict is passed, it will be converted into an :class:`~wavelink.ExtrasNamespace`,
-        which can be converted back to a dict with dict(...). Additionally, you can also use list or tuple on
+        which can be converted back to a dict with ``dict(...)``. Additionally, you can also use list or tuple on
         :class:`~wavelink.ExtrasNamespace`.
 
         The extras dict will be sent to Lavalink as the ``userData`` field for each track in the playlist.
 
 
         .. warning::
 
@@ -608,33 +609,32 @@
 
             .. code:: python
 
                 playlist: wavelink.Search = wavelink.Playable.search("QUERY")
                 playlist.extras = {"requester_id": 1234567890}
 
                 # later...
-                print(playlist.extras.requester_id)
+                print(track.extras.requester_id)
                 # or
-                print(dict(playlist.extras)["requester_id"])
+                print(dict(track.extras)["requester_id"])
 
 
         .. versionadded:: 3.2.0
         """
         return self._extras
 
     @extras.setter
     def extras(self, __value: ExtrasNamespace | dict[str, Any]) -> None:
         if isinstance(__value, ExtrasNamespace):
             self._extras = __value
         else:
             self._extras = ExtrasNamespace(__value)
 
         for track in self.tracks:
-            for name, value in dict(self._extras).items():
-                setattr(track, name, value)
+            track.extras = __value
 
 
 class PlaylistInfo:
     """The wavelink PlaylistInfo container class.
 
     It contains various information about the playlist but **does not** contain the tracks associated with this
     playlist.
```

### Comparing `wavelink-3.2.0/wavelink/types/__init__.py` & `wavelink-3.3.0/wavelink/types/__init__.py`

 * *Files identical despite different names*

### Comparing `wavelink-3.2.0/wavelink/types/filters.py` & `wavelink-3.3.0/wavelink/types/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from typing import Any, TypedDict
 
 
 class Equalizer(TypedDict):
     band: int
     gain: float
```

### Comparing `wavelink-3.2.0/wavelink/types/request.py` & `wavelink-3.3.0/wavelink/types/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, TypeAlias, TypedDict
 
+
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
     from .filters import FilterPayload
 
 
 class VoiceRequest(TypedDict):
```

### Comparing `wavelink-3.2.0/wavelink/types/response.py` & `wavelink-3.3.0/wavelink/types/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import TYPE_CHECKING, Literal, TypedDict
 
-if TYPE_CHECKING:
-    from typing_extensions import Never, NotRequired
+from typing import Literal, TypedDict
 
-    from .filters import FilterPayload
-    from .state import PlayerState
-    from .stats import CPUStats, FrameStats, MemoryStats
-    from .tracks import PlaylistPayload, TrackPayload
+from typing_extensions import Never, NotRequired
+
+from .filters import FilterPayload
+from .state import PlayerState
+from .stats import CPUStats, FrameStats, MemoryStats
+from .tracks import PlaylistPayload, TrackPayload
 
 
 class ErrorResponse(TypedDict):
     timestamp: int
     status: int
     error: str
     trace: NotRequired[str]
```

### Comparing `wavelink-3.2.0/wavelink/types/state.py` & `wavelink-3.3.0/wavelink/types/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import TYPE_CHECKING, TypedDict
 
-if TYPE_CHECKING:
-    from typing_extensions import NotRequired
+from typing import TypedDict
+
+from typing_extensions import NotRequired
 
 
 class PlayerState(TypedDict):
     time: int
     position: int
     connected: bool
     ping: int
```

### Comparing `wavelink-3.2.0/wavelink/types/stats.py` & `wavelink-3.3.0/wavelink/types/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from typing import TypedDict
 
 
 class MemoryStats(TypedDict):
     free: int
     used: int
     allocated: int
```

### Comparing `wavelink-3.2.0/wavelink/types/tracks.py` & `wavelink-3.3.0/wavelink/types/tracks.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import TYPE_CHECKING, Any, TypedDict
 
-if TYPE_CHECKING:
-    from typing_extensions import NotRequired
+from typing import Any, TypedDict
+
+from typing_extensions import NotRequired
 
 
 class TrackInfoPayload(TypedDict):
     identifier: str
     isSeekable: bool
     author: str
     length: int
```

### Comparing `wavelink-3.2.0/wavelink/types/websocket.py` & `wavelink-3.3.0/wavelink/types/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal, TypeAlias, TypedDict
 
+
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
     from .state import PlayerState
     from .stats import CPUStats, FrameStats, MemoryStats
     from .tracks import TrackPayload
```

### Comparing `wavelink-3.2.0/wavelink/utils.py` & `wavelink-3.3.0/wavelink/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
+from collections.abc import Iterator
 from types import SimpleNamespace
-from typing import Any, Iterator
+from typing import Any
+
 
 __all__ = (
     "Namespace",
     "ExtrasNamespace",
 )
```

### Comparing `wavelink-3.2.0/wavelink/websocket.py` & `wavelink-3.3.0/wavelink/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Any
 
 import aiohttp
@@ -32,14 +33,15 @@
 from . import __version__
 from .backoff import Backoff
 from .enums import NodeStatus
 from .exceptions import AuthorizationFailedException, NodeException
 from .payloads import *
 from .tracks import Playable
 
+
 if TYPE_CHECKING:
     from .node import Node
     from .player import Player
     from .types.request import UpdateSessionRequest
     from .types.response import InfoResponse
     from .types.state import PlayerState
     from .types.websocket import TrackExceptionPayload, WebsocketOP
@@ -89,16 +91,16 @@
         self.node._status = NodeStatus.CONNECTING
 
         if self.keep_alive_task:
             try:
                 self.keep_alive_task.cancel()
             except Exception as e:
                 logger.debug(
-                    "Failed to cancel websocket keep alive while connecting. "
-                    f"This is most likely not a problem and will not affect websocket connection: '{e}'"
+                    "Failed to cancel websocket keep alive while connecting. This is most likely not a problem and will not affect websocket connection: '%s'",
+                    e,
                 )
 
         retries: int | None = self.node._retries
         session: aiohttp.ClientSession = self.node._session
         heartbeat: float = self.node.heartbeat
         uri: str = f"{self.node.uri.removesuffix('/')}/v4/websocket"
         github: str = "https://github.com/PythonistaGuild/Wavelink/issues"
@@ -111,36 +113,39 @@
                     await self.cleanup()
                     raise AuthorizationFailedException from e
                 elif isinstance(e, aiohttp.WSServerHandshakeError) and e.status == 404:
                     await self.cleanup()
                     raise NodeException from e
                 else:
                     logger.warning(
-                        f'An unexpected error occurred while connecting {self.node!r} to Lavalink: "{e}"\n'
-                        f"If this error persists or wavelink is unable to reconnect, please see: {github}"
+                        'An unexpected error occurred while connecting %r to Lavalink: "%s"\nIf this error persists or wavelink is unable to reconnect, please see: %s',
+                        self.node,
+                        e,
+                        github,
                     )
 
             if self.is_connected():
                 self.keep_alive_task = asyncio.create_task(self.keep_alive())
                 break
 
             if retries == 0:
                 logger.warning(
-                    f"{self.node!r} was unable to successfully connect/reconnect to Lavalink after "
-                    f'"{retries + 1}" connection attempt. This Node has exhausted the retry count.'
+                    '%r was unable to successfully connect/reconnect to Lavalink after "%s" connection attempt. This Node has exhausted the retry count.',
+                    self.node,
+                    retries + 1,
                 )
 
                 await self.cleanup()
                 break
 
             if retries:
                 retries -= 1
 
             delay: float = self.backoff.calculate()
-            logger.info(f'{self.node!r} retrying websocket connection in "{delay}" seconds.')
+            logger.info('%r retrying websocket connection in "%s" seconds.', self.node, delay)
 
             await asyncio.sleep(delay)
 
     async def keep_alive(self) -> None:
         assert self.socket is not None
 
         while True:
@@ -241,38 +246,38 @@
                     )
                     self.dispatch("websocket_closed", wcpayload)
 
                 else:
                     other_payload: ExtraEventPayload = ExtraEventPayload(node=self.node, player=player, data=data)
                     self.dispatch("extra_event", other_payload)
             else:
-                logger.debug(f"'Received an unknown OP from Lavalink '{data['op']}'. Disregarding.")
+                logger.debug("'Received an unknown OP from Lavalink '%s'. Disregarding.", data["op"])
 
     def get_player(self, guild_id: str | int) -> Player | None:
         return self.node.get_player(int(guild_id))
 
     def dispatch(self, event: str, /, *args: Any, **kwargs: Any) -> None:
         assert self.node.client is not None
 
         self.node.client.dispatch(f"wavelink_{event}", *args, **kwargs)
-        logger.debug(f"{self.node!r} dispatched the event 'on_wavelink_{event}'")
+        logger.debug("%r dispatched the event 'on_wavelink_%s'", self.node, event)
 
     async def cleanup(self) -> None:
-        if self.socket:
+        if self.keep_alive_task:
             try:
-                await self.socket.close()
-            except:
+                self.keep_alive_task.cancel()
+            except Exception:
                 pass
 
-        if self.keep_alive_task:
+        if self.socket:
             try:
-                self.keep_alive_task.cancel()
-            except:
+                await self.socket.close()
+            except Exception:
                 pass
 
         self.node._status = NodeStatus.DISCONNECTED
         self.node._session_id = None
         self.node._players = {}
 
         self.node._websocket = None
 
-        logger.debug(f"Successfully cleaned up the websocket for {self.node!r}")
+        logger.debug("Successfully cleaned up the websocket for %r", self.node)
```

### Comparing `wavelink-3.2.0/wavelink.egg-info/PKG-INFO` & `wavelink-3.3.0/wavelink.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wavelink
-Version: 3.2.0
+Version: 3.3.0
 Summary: A robust and powerful, fully asynchronous Lavalink wrapper built for discord.py in Python.
 Author-email: "PythonistaGuild, EvieePy" <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp<4,>=3.7.4
 Requires-Dist: discord.py>=2.0.1
 Requires-Dist: yarl>=1.9.2
 Requires-Dist: async_timeout
+Requires-Dist: typing_extensions
 
 <div align="center">
 
 
 ![Logo](https://raw.githubusercontent.com/PythonistaGuild/Wavelink/master/logo.png)
 
 ![Python Version](https://img.shields.io/pypi/pyversions/Wavelink)
```

### Comparing `wavelink-3.2.0/wavelink.egg-info/SOURCES.txt` & `wavelink-3.3.0/wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

