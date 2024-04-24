# Comparing `tmp/ndbioimage-2024.4.6.tar.gz` & `tmp/ndbioimage-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.6.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.7.tar", max compression
```

## Comparing `ndbioimage-2024.4.6.tar` & `ndbioimage-2024.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.6/LICENSE
--rw-r--r--   0        0        0     2608 2024-04-03 13:37:34.891216 ndbioimage-2024.4.6/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.6/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    54071 2024-04-12 13:42:57.566891 ndbioimage-2024.4.6/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.6/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.6/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.6/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    29149 2024-04-12 14:01:22.722103 ndbioimage-2024.4.6/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.6/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.6/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.6/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.6/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.6/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.6/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1241 2024-04-12 15:38:36.426189 ndbioimage-2024.4.6/pyproject.toml
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 ndbioimage-2024.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.7/LICENSE
+-rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.4.7/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.7/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54330 2024-04-19 14:08:16.717040 ndbioimage-2024.4.7/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.7/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.7/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.7/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28169 2024-04-24 15:10:18.268539 ndbioimage-2024.4.7/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.7/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.7/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.7/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.7/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.7/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.7/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1248 2024-04-24 15:11:52.416478 ndbioimage-2024.4.7/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.4.7/PKG-INFO
```

### Comparing `ndbioimage-2024.4.6/LICENSE` & `ndbioimage-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/README.md` & `ndbioimage-2024.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,19 +59,19 @@
 
 ## Adding more formats
 Readers for image formats subclass AbstractReader. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
-- property ome: reads metadata from file and adds them to an OME object imported
-from the ome-types library 
 - \_\_frame__(self, c, z, t): return the frame at channel=c, z-slice=z, time=t from the file
 
 Optional methods:
+- get_ome: reads metadata from file and adds them to an OME object imported
+from the ome-types library 
 - open(self): maybe open some file handle
 - close(self): close any file handles
 
 Optional fields:
 - priority (int): Imread will try readers with a lower number first, default: 99
 - do_not_pickle (strings): any attributes that should not be included when the object is pickled,
 for example: any file handles
```

### Comparing `ndbioimage-2024.4.6/ndbioimage/.DS_Store` & `ndbioimage-2024.4.7/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/__init__.py` & `ndbioimage-2024.4.7/ndbioimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,19 +252,24 @@
                 subclass_do_not_pickle = (subclass.do_not_pickle,) if isinstance(subclass.do_not_pickle, str) \
                     else subclass.do_not_pickle if hasattr(subclass, 'do_not_pickle') else ()
                 subclass.do_not_pickle = set(do_not_pickle).union(set(subclass_do_not_pickle))
 
                 return super().__new__(subclass)
         raise ReaderNotFoundError(f'No reader found for {path}.')
 
-    def __init__(self, base: Imread = None,
-                 slice: tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray] = None,  # noqa
-                 shape: tuple[int, ...] = (0, 0, 0, 0, 0),
-                 dtype: DTypeLike = None,
-                 frame_decorator: Callable[[Imread, np.ndarray, int, int, int], np.ndarray] = None) -> None:
+    def __init__(self, *args: Any, **kwargs: Any):
+        def parse(base: Imread = None,  # noqa
+                  slice: tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray] = None,  # noqa
+                  shape: tuple[int, ...] = (0, 0, 0, 0, 0),  # noqa
+                  dtype: DTypeLike = None,  # noqa
+                  frame_decorator: Callable[[Imread, np.ndarray, int, int, int], np.ndarray] = None  # noqa
+                  ) -> tuple[Any, ...]:
+            return base, slice, shape, dtype, frame_decorator
+
+        base, slice, shape, dtype, frame_decorator = parse(*args, **kwargs)  # noqa
         self.base = base or self
         self.slice = slice
         self._shape = Shape(shape)
         self.dtype = dtype
         self.frame_decorator = frame_decorator
         self.transform = Transforms()
         self.flags = dict(C_CONTIGUOUS=False, F_CONTIGUOUS=False, OWNDATA=False, WRITEABLE=False,
```

### Comparing `ndbioimage-2024.4.6/ndbioimage/jvm.py` & `ndbioimage-2024.4.7/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/cziread.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 import warnings
 from abc import ABC
+from functools import cached_property
 from io import BytesIO
 from itertools import product
 from pathlib import Path
-from typing import Any, TypeVar, Optional
+from typing import Any, Callable, Optional, TypeVar
 
 import czifile
 import imagecodecs
 import numpy as np
 from lxml import etree
-from ome_types import model, OME
+from ome_types import OME, model
 from tifffile import repeat_nd
 
 from .. import AbstractReader
 
 try:
     # TODO: use zoom from imagecodecs implementation when available
     from scipy.ndimage.interpolation import zoom
@@ -168,439 +169,426 @@
                 for c in range(*idx[self.reader.axes.index('C')]):
                     for z in range(*idx[self.reader.axes.index('Z')]):
                         for t in range(*idx[self.reader.axes.index('T')]):
                             if (c, z, t) in filedict:
                                 filedict[c, z, t].append(directory_entry)
                             else:
                                 filedict[c, z, t] = [directory_entry]
+        if len(filedict) == 0:
+            raise FileNotFoundError(f'Series {self.series} not found in {self.path}.')
         self.filedict = filedict  # noqa
 
     def close(self) -> None:
         self.reader.close()
 
     def get_ome(self) -> OME:
-        xml = self.reader.metadata()
-        attachments = {i.attachment_entry.name: i.attachment_entry.data_segment()
-                       for i in self.reader.attachments()}
-        tree = etree.fromstring(xml)
-        metadata = tree.find('Metadata')
-        version = metadata.find('Version')
-        if version is not None:
-            version = version.text
-        else:
-            version = metadata.find('Experiment').attrib['Version']
-
-        if version == '1.0':
-            return self.ome_10(tree, attachments)
-        elif version == '1.2':
-            return self.ome_12(tree, attachments)
-
-    def ome_12(self, tree: etree, attachments: dict[str, Any]) -> OME:
-        def text(item: Optional[Element], default: str = "") -> str:
-            return default if item is None else item.text
-
-        def def_list(item: Any) -> list[Any]:
-            return [] if item is None else item
-
-        ome = OME()
-
-        metadata = tree.find('Metadata')
-
-        information = metadata.find('Information')
-        display_setting = metadata.find('DisplaySetting')
-        ome.experimenters = [model.Experimenter(id='Experimenter:0',
-                                                user_name=information.find('Document').find('UserName').text)]
-
-        instrument = information.find('Instrument')
-        for _ in instrument.find('Microscopes'):
-            ome.instruments.append(model.Instrument(id='Instrument:0'))
-
-        for detector in instrument.find('Detectors'):
-            try:
-                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
-            except ValueError:
-                detector_type = model.Detector_Type.OTHER
-
-            ome.instruments[0].detectors.append(
-                model.Detector(
-                    id=detector.attrib['Id'].replace(' ', ''), model=text(detector.find('Manufacturer').find('Model')),
-                    type=detector_type
-                ))
-
-        for objective in instrument.find('Objectives'):
-            ome.instruments[0].objectives.append(
-                model.Objective(
-                    id=objective.attrib['Id'],
-                    model=text(objective.find('Manufacturer').find('Model')),
-                    immersion=text(objective.find('Immersion')),
-                    lens_na=float(text(objective.find('LensNA'))),
-                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
-
-        for tubelens in instrument.find('TubeLenses'):
-            try:
-                nominal_magnification = float(re.findall(r'\d+(?:[,.]\d*)?',
-                                                         tubelens.attrib['Name'])[0].replace(',', '.'))
-            except Exception:  # noqa
-                nominal_magnification = 1.0
+        return OmeParse.get_ome(self.reader, self.filedict)
 
-            ome.instruments[0].objectives.append(
-                model.Objective(
-                    id=f"Objective:{tubelens.attrib['Id']}",
-                    model=tubelens.attrib['Name'],
-                    nominal_magnification=nominal_magnification))
-
-        for light_source in def_list(instrument.find('LightSources')):
-            if light_source.find('LightSourceType').find('Laser') is not None:
-                ome.instruments[0].lasers.append(
-                    model.Laser(
-                        id=f"LightSource:{light_source.attrib['Id']}",
-                        power=float(text(light_source.find('Power'))),
-                        wavelength=float(light_source.attrib['Id'][-3:])))
-
-        x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
-        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        size_x = x_max - x_min
-        size_y = y_max - y_min
-        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
-                                  for directory_entry in 'CZT')
+    def __frame__(self, c: int = 0, z: int = 0, t: int = 0) -> np.ndarray:
+        f = np.zeros(self.base.shape['yx'], self.dtype)
+        if (c, z, t) in self.filedict:
+            directory_entries = self.filedict[c, z, t]
+            x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
+            y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
+            xy_min = {'X': x_min, 'Y': y_min}
+            for directory_entry in directory_entries:
+                subblock = directory_entry.data_segment()
+                tile = subblock.data(resize=True, order=0)
+                axes_min = [xy_min.get(ax, 0) for ax in directory_entry.axes]
+                index = [slice(i - j - m, i - j + k)
+                         for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
+                index = tuple(index[self.reader.axes.index(i)] for i in 'YX')
+                f[index] = tile.squeeze()
+        return f
 
-        image = information.find('Image')
-        pixel_type = text(image.find('PixelType'), 'Gray16')
-        if pixel_type.startswith('Gray'):
-            pixel_type = 'uint' + pixel_type[4:]
-        objective_settings = image.find('ObjectiveSettings')
-        try:  # TODO
-            scenes = image.find('Dimensions').find('S').find('Scenes')
-            center_position = [float(pos) for pos in text(scenes[0].find('CenterPosition')).split(',')]
-        except AttributeError:
-            center_position = [0, 0]
-        um = model.UnitsLength.MICROMETER
-        nm = model.UnitsLength.NANOMETER
+    @staticmethod
+    def get_index(directory_entry: czifile.DirectoryEntryDV, start: tuple[int]) -> list[tuple[int, int]]:
+        return [(i - j, i - j + k) for i, j, k in zip(directory_entry.start, start, directory_entry.shape)]
 
-        ome.images.append(
-            model.Image(
-                id='Image:0',
-                name=f"{text(information.find('Document').find('Name'))} #1",
-                pixels=model.Pixels(
-                    id='Pixels:0', size_x=size_x, size_y=size_y,
-                    size_c=size_c, size_z=size_z, size_t=size_t,
-                    dimension_order='XYCZT', type=pixel_type,
-                    significant_bits=int(text(image.find('ComponentBitCount'))),
-                    big_endian=False, interleaved=False, metadata_only=True),
-                experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
-                instrument_ref=model.InstrumentRef(id='Instrument:0'),
-                objective_settings=model.ObjectiveSettings(
-                    id=objective_settings.find('ObjectiveRef').attrib['Id'],
-                    medium=text(objective_settings.find('Medium')),
-                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
-                stage_label=model.StageLabel(
-                    name=f'Scene position #0',
-                    x=center_position[0], x_unit=um,
-                    y=center_position[1], y_unit=um)))
 
-        for distance in metadata.find('Scaling').find('Items'):
-            if distance.attrib['Id'] == 'X':
-                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
-            elif distance.attrib['Id'] == 'Y':
-                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
-            elif size_z > 1 and distance.attrib['Id'] == 'Z':
-                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
-
-        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
-        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
-
-        for idx, (key, channel) in enumerate(channels_im.items()):
-            detector_settings = channel.find('DetectorSettings')
-            laser_scan_info = channel.find('LaserScanInfo')
-            detector = detector_settings.find('Detector')
-            try:
-                binning = model.Binning(text(detector_settings.find('Binning')))
-            except ValueError:
-                binning = model.Binning.OTHER
-
-            light_sources_settings = channel.find('LightSourcesSettings')
-            # no space in ome for multiple lightsources simultaneously
-            if light_sources_settings is not None:
-                light_source_settings = light_sources_settings[0]
-                light_source_settings = model.LightSourceSettings(
-                    id='LightSource:' + '_'.join([light_source_settings.find('LightSource').attrib['Id']
-                                                  for light_source_settings in light_sources_settings]),
-                    attenuation=float(text(light_source_settings.find('Attenuation'))),
-                    wavelength=float(text(light_source_settings.find('Wavelength'))),
-                    wavelength_unit=nm)
-            else:
-                light_source_settings = None
-
-            ome.images[0].pixels.channels.append(
-                model.Channel(
-                    id=f'Channel:{idx}',
-                    name=channel.attrib['Name'],
-                    acquisition_mode=text(channel.find('AcquisitionMode')).replace('SingleMoleculeLocalisation',
-                                                                                   'SingleMoleculeImaging'),
-                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
-                    detector_settings=model.DetectorSettings(
-                        id=detector.attrib['Id'].replace(' ', ""),
-                        binning=binning),
-                    emission_wavelength=i if (i := text(channel.find('EmissionWavelength'))) != '0' else '100',
-                    excitation_wavelength=text(channel.find('ExcitationWavelength')),
-                    # filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
-                    illumination_type=text(channel.find('IlluminationType')),
-                    light_source_settings=light_source_settings,
-                    samples_per_pixel=int(text(laser_scan_info.find('Averaging'), '1'))))
-
-        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'), '100')) for channel in
-                          channels_im.values()]
-        delta_ts = attachments['TimeStamps'].data()
-        dt = np.diff(delta_ts)
-        if np.std(dt) / np.mean(dt) > 0.02:
-            dt = np.median(dt[dt > 0])
-            delta_ts = dt * np.arange(len(delta_ts))
-            warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
+class OmeParse:
+    size_x: int
+    size_y: int
+    size_c: int
+    size_z: int
+    size_t: int
+
+    nm = model.UnitsLength.NANOMETER
+    um = model.UnitsLength.MICROMETER
+
+    @classmethod
+    def get_ome(cls, reader: czifile.CziFile, filedict: dict[tuple[int, int, int], Any]) -> OME:
+        new = cls(reader, filedict)
+        new.parse()
+        return new.ome
+
+    def __init__(self, reader: czifile.CziFile, filedict: dict[tuple[int, int, int], Any]) -> None:
+        self.reader = reader
+        self.filedict = filedict
+        xml = reader.metadata()
+        self.attachments = {i.attachment_entry.name: i.attachment_entry.data_segment()
+                            for i in reader.attachments()}
+        self.tree = etree.fromstring(xml)
+        self.metadata = self.tree.find('Metadata')
+        version = self.metadata.find('Version')
+        if version is not None:
+            self.version = version.text
+        else:
+            self.version = self.metadata.find('Experiment').attrib['Version']
 
-        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
-            ome.images[0].pixels.planes.append(
-                model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t], exposure_time=exposure_times[c]))
+        self.ome = OME()
+        self.information = self.metadata.find('Information')
+        self.display_setting = self.metadata.find('DisplaySetting')
+        self.experiment = self.metadata.find('Experiment')
+        self.acquisition_block = self.experiment.find('ExperimentBlocks').find('AcquisitionBlock')
+        self.instrument = self.information.find('Instrument')
+        self.image = self.information.find('Image')
+
+        if self.version == '1.0':
+            self.experiment = self.metadata.find('Experiment')
+            self.acquisition_block = self.experiment.find('ExperimentBlocks').find('AcquisitionBlock')
+            self.multi_track_setup = self.acquisition_block.find('MultiTrackSetup')
+        else:
+            self.experiment = None
+            self.acquisition_block = None
+            self.multi_track_setup = None
+
+    def parse(self) -> None:
+        self.get_experimenters()
+        self.get_instruments()
+        self.get_detectors()
+        self.get_objectives()
+        self.get_tubelenses()
+        self.get_light_sources()
+        self.get_filters()
+        self.get_pixels()
 
-        idx = 0
-        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
-            rectangle = layer.find('Elements').find('Rectangle')
-            if rectangle is not None:
-                geometry = rectangle.find('Geometry')
-                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
-                roi.union.append(
-                    model.Rectangle(
-                        id='Shape:0:0',
-                        height=float(text(geometry.find('Height'))),
-                        width=float(text(geometry.find('Width'))),
-                        x=float(text(geometry.find('Left'))),
-                        y=float(text(geometry.find('Top')))))
-                ome.rois.append(roi)
-                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
-                idx += 1
-        return ome
+    @staticmethod
+    def text(item: Optional[Element], default: str = "") -> str:
+        return default if item is None else item.text
 
-    def ome_10(self, tree: etree, attachments: dict[str, Any]) -> OME:
-        def text(item: Optional[Element], default: str = "") -> str:
-            return default if item is None else item.text
-
-        def def_list(item: Any) -> list[Any]:
-            return [] if item is None else item
-
-        ome = OME()
-
-        metadata = tree.find('Metadata')
-
-        information = metadata.find('Information')
-        display_setting = metadata.find('DisplaySetting')
-        experiment = metadata.find('Experiment')
-        acquisition_block = experiment.find('ExperimentBlocks').find('AcquisitionBlock')
-
-        ome.experimenters = [model.Experimenter(id='Experimenter:0',
-                                                user_name=information.find('User').find('DisplayName').text)]
-
-        instrument = information.find('Instrument')
-        ome.instruments.append(model.Instrument(id=instrument.attrib['Id']))
-
-        for detector in instrument.find('Detectors'):
-            try:
-                detector_type = model.Detector_Type(text(detector.find('Type')).upper() or "")
-            except ValueError:
-                detector_type = model.Detector_Type.OTHER
-
-            ome.instruments[0].detectors.append(
-                model.Detector(
-                    id=detector.attrib['Id'], model=text(detector.find('Manufacturer').find('Model')),
-                    amplification_gain=float(text(detector.find('AmplificationGain'))),
-                    gain=float(text(detector.find('Gain'))), zoom=float(text(detector.find('Zoom'))),
-                    type=detector_type
-                ))
+    @staticmethod
+    def def_list(item: Any) -> list[Any]:
+        return [] if item is None else item
 
-        for objective in instrument.find('Objectives'):
-            ome.instruments[0].objectives.append(
+    @staticmethod
+    def try_default(fun: Callable[[Any, ...], Any] | type, default: Any = None, *args: Any, **kwargs: Any) -> Any:
+        try:
+            return fun(*args, **kwargs)
+        except Exception:  # noqa
+            return default
+
+    def get_experimenters(self) -> None:
+        if self.version == '1.0':
+            self.ome.experimenters = [
+                model.Experimenter(id='Experimenter:0',
+                                   user_name=self.information.find('User').find('DisplayName').text)]
+        elif self.version in ('1.1', '1.2'):
+            self.ome.experimenters = [
+                model.Experimenter(id='Experimenter:0',
+                                   user_name=self.information.find('Document').find('UserName').text)]
+
+    def get_instruments(self) -> None:
+        if self.version == '1.0':
+            self.ome.instruments.append(model.Instrument(id=self.instrument.attrib['Id']))
+        elif self.version in ('1.1', '1.2'):
+            for _ in self.instrument.find('Microscopes'):
+                self.ome.instruments.append(model.Instrument(id='Instrument:0'))
+
+    def get_detectors(self) -> None:
+        if self.version == '1.0':
+            for detector in self.instrument.find('Detectors'):
+                try:
+                    detector_type = model.Detector_Type(self.text(detector.find('Type')).upper() or "")
+                except ValueError:
+                    detector_type = model.Detector_Type.OTHER
+
+                self.ome.instruments[0].detectors.append(
+                    model.Detector(
+                        id=detector.attrib['Id'], model=self.text(detector.find('Manufacturer').find('Model')),
+                        amplification_gain=float(self.text(detector.find('AmplificationGain'))),
+                        gain=float(self.text(detector.find('Gain'))), zoom=float(self.text(detector.find('Zoom'))),
+                        type=detector_type
+                    ))
+        elif self.version in ('1.1', '1.2'):
+            for detector in self.instrument.find('Detectors'):
+                try:
+                    detector_type = model.Detector_Type(self.text(detector.find('Type')).upper() or "")
+                except ValueError:
+                    detector_type = model.Detector_Type.OTHER
+
+                self.ome.instruments[0].detectors.append(
+                    model.Detector(
+                        id=detector.attrib['Id'].replace(' ', ''),
+                        model=self.text(detector.find('Manufacturer').find('Model')),
+                        type=detector_type
+                    ))
+
+    def get_objectives(self) -> None:
+        for objective in self.instrument.find('Objectives'):
+            self.ome.instruments[0].objectives.append(
                 model.Objective(
                     id=objective.attrib['Id'],
-                    model=text(objective.find('Manufacturer').find('Model')),
-                    immersion=text(objective.find('Immersion')),
-                    lens_na=float(text(objective.find('LensNA'))),
-                    nominal_magnification=float(text(objective.find('NominalMagnification')))))
-
-        for light_source in def_list(instrument.find('LightSources')):
-            if light_source.find('LightSourceType').find('Laser') is not None:
-                ome.instruments[0].lasers.append(
-                    model.Laser(
-                        id=light_source.attrib['Id'],
-                        model=text(light_source.find('Manufacturer').find('Model')),
-                        power=float(text(light_source.find('Power'))),
-                        wavelength=float(
-                            text(light_source.find('LightSourceType').find('Laser').find('Wavelength')))))
-
-        multi_track_setup = acquisition_block.find('MultiTrackSetup')
-        for idx, tube_lens in enumerate({text(track_setup.find('TubeLensPosition'))
-                                         for track_setup in multi_track_setup}):
-            ome.instruments[0].objectives.append(
-                model.Objective(id=f'Objective:Tubelens:{idx}', model=tube_lens,
-                                nominal_magnification=float(
-                                    re.findall(r'\d+[,.]\d*', tube_lens)[0].replace(',', '.'))
-                                ))
-
-        for idx, filter_ in enumerate({text(beam_splitter.find('Filter'))
-                                       for track_setup in multi_track_setup
-                                       for beam_splitter in track_setup.find('BeamSplitters')}):
-            ome.instruments[0].filter_sets.append(
-                model.FilterSet(id=f'FilterSet:{idx}', model=filter_)
-            )
-
-        for idx, collimator in enumerate({text(track_setup.find('FWFOVPosition'))
-                                          for track_setup in multi_track_setup}):
-            ome.instruments[0].filters.append(model.Filter(id=f'Filter:Collimator:{idx}', model=collimator))
+                    model=self.text(objective.find('Manufacturer').find('Model')),
+                    immersion=self.text(objective.find('Immersion')),
+                    lens_na=float(self.text(objective.find('LensNA'))),
+                    nominal_magnification=float(self.text(objective.find('NominalMagnification')))))
+
+    def get_tubelenses(self) -> None:
+        if self.version == '1.0':
+            for idx, tube_lens in enumerate({self.text(track_setup.find('TubeLensPosition'))
+                                             for track_setup in self.multi_track_setup}):
+                self.ome.instruments[0].objectives.append(
+                    model.Objective(id=f'Objective:Tubelens:{idx}', model=tube_lens,
+                                    nominal_magnification=float(
+                                        re.findall(r'\d+[,.]\d*', tube_lens)[0].replace(',', '.'))
+                                    ))
+        elif self.version in ('1.1', '1.2'):
+            for tubelens in self.instrument.find('TubeLenses'):
+                try:
+                    nominal_magnification = float(re.findall(r'\d+(?:[,.]\d*)?',
+                                                             tubelens.attrib['Name'])[0].replace(',', '.'))
+                except Exception:  # noqa
+                    nominal_magnification = 1.0
+
+                self.ome.instruments[0].objectives.append(
+                    model.Objective(
+                        id=f"Objective:{tubelens.attrib['Id']}",
+                        model=tubelens.attrib['Name'],
+                        nominal_magnification=nominal_magnification))
+
+    def get_light_sources(self) -> None:
+        if self.version == '1.0':
+            for light_source in self.def_list(self.instrument.find('LightSources')):
+                if light_source.find('LightSourceType').find('Laser') is not None:
+                    self.ome.instruments[0].lasers.append(
+                        model.Laser(
+                            id=light_source.attrib['Id'],
+                            model=self.text(light_source.find('Manufacturer').find('Model')),
+                            power=float(self.text(light_source.find('Power'))),
+                            wavelength=float(
+                                self.text(light_source.find('LightSourceType').find('Laser').find('Wavelength')))))
+        elif self.version in ('1.1', '1.2'):
+            for light_source in self.def_list(self.instrument.find('LightSources')):
+                if light_source.find('LightSourceType').find('Laser') is not None:
+                    self.ome.instruments[0].lasers.append(
+                        model.Laser(
+                            id=f"LightSource:{light_source.attrib['Id']}",
+                            power=float(self.text(light_source.find('Power'))),
+                            wavelength=float(light_source.attrib['Id'][-3:])))
+
+    def get_filters(self) -> None:
+        if self.version == '1.0':
+            for idx, filter_ in enumerate({self.text(beam_splitter.find('Filter'))
+                                           for track_setup in self.multi_track_setup
+                                           for beam_splitter in track_setup.find('BeamSplitters')}):
+                self.ome.instruments[0].filter_sets.append(
+                    model.FilterSet(id=f'FilterSet:{idx}', model=filter_)
+                )
 
+    def get_pixels(self) -> None:
         x_min = min([f.start[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
         y_min = min([f.start[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
         x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in self.filedict[0, 0, 0]])
         y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in self.filedict[0, 0, 0]])
-        size_x = x_max - x_min
-        size_y = y_max - y_min
-        size_c, size_z, size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
-                                  for directory_entry in 'CZT')
-
-        image = information.find('Image')
-        pixel_type = text(image.find('PixelType'), 'Gray16')
+        self.size_x = x_max - x_min
+        self.size_y = y_max - y_min
+        self.size_c, self.size_z, self.size_t = (self.reader.shape[self.reader.axes.index(directory_entry)]
+                                                 for directory_entry in 'CZT')
+        image = self.information.find('Image')
+        pixel_type = self.text(image.find('PixelType'), 'Gray16')
         if pixel_type.startswith('Gray'):
             pixel_type = 'uint' + pixel_type[4:]
         objective_settings = image.find('ObjectiveSettings')
-        scenes = image.find('Dimensions').find('S').find('Scenes')
-        positions = scenes[0].find('Positions')[0]
-        um = model.UnitsLength.MICROMETER
-        nm = model.UnitsLength.NANOMETER
 
-        ome.images.append(
+        self.ome.images.append(
             model.Image(
                 id='Image:0',
-                name=f"{text(information.find('Document').find('Name'))} #1",
+                name=f"{self.text(self.information.find('Document').find('Name'))} #1",
                 pixels=model.Pixels(
-                    id='Pixels:0', size_x=size_x, size_y=size_y,
-                    size_c=size_c, size_z=size_z, size_t=size_t,
+                    id='Pixels:0', size_x=self.size_x, size_y=self.size_y,
+                    size_c=self.size_c, size_z=self.size_z, size_t=self.size_t,
                     dimension_order='XYCZT', type=pixel_type,
-                    significant_bits=int(text(image.find('ComponentBitCount'))),
+                    significant_bits=int(self.text(image.find('ComponentBitCount'))),
                     big_endian=False, interleaved=False, metadata_only=True),
                 experimenter_ref=model.ExperimenterRef(id='Experimenter:0'),
                 instrument_ref=model.InstrumentRef(id='Instrument:0'),
                 objective_settings=model.ObjectiveSettings(
                     id=objective_settings.find('ObjectiveRef').attrib['Id'],
-                    medium=text(objective_settings.find('Medium')),
-                    refractive_index=float(text(objective_settings.find('RefractiveIndex')))),
+                    medium=self.text(objective_settings.find('Medium')),
+                    refractive_index=float(self.text(objective_settings.find('RefractiveIndex')))),
                 stage_label=model.StageLabel(
                     name=f'Scene position #0',
-                    x=float(positions.attrib['X']), x_unit=um,
-                    y=float(positions.attrib['Y']), y_unit=um,
-                    z=float(positions.attrib['Z']), z_unit=um)))
+                    x=self.positions[0], x_unit=self.um,
+                    y=self.positions[1], y_unit=self.um,
+                    z=self.positions[2], z_unit=self.um)))
 
-        for distance in metadata.find('Scaling').find('Items'):
+        for distance in self.metadata.find('Scaling').find('Items'):
             if distance.attrib['Id'] == 'X':
-                ome.images[0].pixels.physical_size_x = float(text(distance.find('Value'))) * 1e6
+                self.ome.images[0].pixels.physical_size_x = float(self.text(distance.find('Value'))) * 1e6
             elif distance.attrib['Id'] == 'Y':
-                ome.images[0].pixels.physical_size_y = float(text(distance.find('Value'))) * 1e6
-            elif size_z > 1 and distance.attrib['Id'] == 'Z':
-                ome.images[0].pixels.physical_size_z = float(text(distance.find('Value'))) * 1e6
-
-        channels_im = {channel.attrib['Id']: channel for channel in image.find('Dimensions').find('Channels')}
-        channels_ds = {channel.attrib['Id']: channel for channel in display_setting.find('Channels')}
-        channels_ts = {detector.attrib['Id']: track_setup
-                       for track_setup in
-                       experiment.find('ExperimentBlocks').find('AcquisitionBlock').find('MultiTrackSetup')
-                       for detector in track_setup.find('Detectors')}
-
-        for idx, (key, channel) in enumerate(channels_im.items()):
-            detector_settings = channel.find('DetectorSettings')
-            laser_scan_info = channel.find('LaserScanInfo')
-            detector = detector_settings.find('Detector')
-            try:
-                binning = model.Binning(text(detector_settings.find('Binning')))
-            except ValueError:
-                binning = model.Binning.OTHER
-
-            filterset = text(channels_ts[key].find('BeamSplitters')[0].find('Filter'))
-            filterset_idx = [filterset.model for filterset in ome.instruments[0].filter_sets].index(filterset)
-
-            light_sources_settings = channel.find('LightSourcesSettings')
-            # no space in ome for multiple lightsources simultaneously
-            if len(light_sources_settings) > idx:
-                light_source_settings = light_sources_settings[idx]
-            else:
-                light_source_settings = light_sources_settings[0]
-            light_source_settings = model.LightSourceSettings(
-                id=light_source_settings.find('LightSource').attrib['Id'],
-                attenuation=float(text(light_source_settings.find('Attenuation'))),
-                wavelength=float(text(light_source_settings.find('Wavelength'))),
-                wavelength_unit=nm)
-
-            ome.images[0].pixels.channels.append(
-                model.Channel(
-                    id=f'Channel:{idx}',
-                    name=channel.attrib['Name'],
-                    acquisition_mode=text(channel.find('AcquisitionMode')),
-                    color=model.Color(text(channels_ds[channel.attrib['Id']].find('Color'), 'white')),
-                    detector_settings=model.DetectorSettings(id=detector.attrib['Id'], binning=binning),
-                    # emission_wavelength=text(channel.find('EmissionWavelength')),  # TODO: fix
-                    excitation_wavelength=light_source_settings.wavelength,
-                    filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
-                    illumination_type=text(channel.find('IlluminationType')),
-                    light_source_settings=light_source_settings,
-                    samples_per_pixel=int(text(laser_scan_info.find('Averaging')))))
-
-        exposure_times = [float(text(channel.find('LaserScanInfo').find('FrameTime'))) for channel in
-                          channels_im.values()]
-        delta_ts = attachments['TimeStamps'].data()
+                self.ome.images[0].pixels.physical_size_y = float(self.text(distance.find('Value'))) * 1e6
+            elif self.size_z > 1 and distance.attrib['Id'] == 'Z':
+                self.ome.images[0].pixels.physical_size_z = float(self.text(distance.find('Value'))) * 1e6
+
+    @cached_property
+    def positions(self) -> tuple[float, float, Optional[float]]:
+        if self.version == '1.0':
+            scenes = self.image.find('Dimensions').find('S').find('Scenes')
+            positions = scenes[0].find('Positions')[0]
+            return float(positions.attrib['X']), float(positions.attrib['Y']), float(positions.attrib['Z'])
+        elif self.version in ('1.1', '1.2'):
+            try:  # TODO
+                scenes = self.image.find('Dimensions').find('S').find('Scenes')
+                center_position = [float(pos) for pos in self.text(scenes[0].find('CenterPosition')).split(',')]
+            except AttributeError:
+                center_position = [0, 0]
+            return center_position[0], center_position[1], None
+
+    @cached_property
+    def channels_im(self) -> dict:
+        return {channel.attrib['Id']: channel for channel in self.image.find('Dimensions').find('Channels')}
+
+    @cached_property
+    def channels_ds(self) -> dict:
+        return {channel.attrib['Id']: channel for channel in self.display_setting.find('Channels')}
+
+    @cached_property
+    def channels_ts(self) -> dict:
+        return {detector.attrib['Id']: track_setup
+                for track_setup in
+                self.experiment.find('ExperimentBlocks').find('AcquisitionBlock').find('MultiTrackSetup')
+                for detector in track_setup.find('Detectors')}
+
+    def get_channels(self) -> None:
+        if self.version == '1.0':
+            for idx, (key, channel) in enumerate(self.channels_im.items()):
+                detector_settings = channel.find('DetectorSettings')
+                laser_scan_info = channel.find('LaserScanInfo')
+                detector = detector_settings.find('Detector')
+                try:
+                    binning = model.Binning(self.text(detector_settings.find('Binning')))
+                except ValueError:
+                    binning = model.Binning.OTHER
+
+                filterset = self.text(self.channels_ts[key].find('BeamSplitters')[0].find('Filter'))
+                filterset_idx = [filterset.model for filterset in self.ome.instruments[0].filter_sets].index(filterset)
+
+                light_sources_settings = channel.find('LightSourcesSettings')
+                # no space in ome for multiple lightsources simultaneously
+                if len(light_sources_settings) > idx:
+                    light_source_settings = light_sources_settings[idx]
+                else:
+                    light_source_settings = light_sources_settings[0]
+                light_source_settings = model.LightSourceSettings(
+                    id=light_source_settings.find('LightSource').attrib['Id'],
+                    attenuation=float(self.text(light_source_settings.find('Attenuation'))),
+                    wavelength=float(self.text(light_source_settings.find('Wavelength'))),
+                    wavelength_unit=self.nm)
+
+                self.ome.images[0].pixels.channels.append(
+                    model.Channel(
+                        id=f'Channel:{idx}',
+                        name=channel.attrib['Name'],
+                        acquisition_mode=self.text(channel.find('AcquisitionMode')),
+                        color=model.Color(self.text(self.channels_ds[channel.attrib['Id']].find('Color'), 'white')),
+                        detector_settings=model.DetectorSettings(id=detector.attrib['Id'], binning=binning),
+                        # emission_wavelength=text(channel.find('EmissionWavelength')),  # TODO: fix
+                        excitation_wavelength=light_source_settings.wavelength,
+                        filter_set_ref=model.FilterSetRef(id=self.ome.instruments[0].filter_sets[filterset_idx].id),
+                        illumination_type=self.text(channel.find('IlluminationType')),
+                        light_source_settings=light_source_settings,
+                        samples_per_pixel=int(self.text(laser_scan_info.find('Averaging')))))
+        elif self.version in ('1.1', '1.2'):
+            for idx, (key, channel) in enumerate(self.channels_im.items()):
+                detector_settings = channel.find('DetectorSettings')
+                laser_scan_info = channel.find('LaserScanInfo')
+                detector = detector_settings.find('Detector')
+                try:
+                    color = model.Color(self.text(self.channels_ds[channel.attrib['Id']].find('Color'), 'white'))
+                except Exception:  # noqa
+                    color = None
+                try:
+                    if (i := self.text(channel.find('EmissionWavelength'))) != '0':
+                        emission_wavelength = float(i)
+                    else:
+                        emission_wavelength = None
+                except Exception:  # noqa
+                    emission_wavelength = None
+                if laser_scan_info is not None:
+                    samples_per_pixel = int(self.text(laser_scan_info.find('Averaging'), '1'))
+                else:
+                    samples_per_pixel = 1
+                try:
+                    binning = model.Binning(self.text(detector_settings.find('Binning')))
+                except ValueError:
+                    binning = model.Binning.OTHER
+
+                light_sources_settings = channel.find('LightSourcesSettings')
+                # no space in ome for multiple lightsources simultaneously
+                if light_sources_settings is not None:
+                    light_source_settings = light_sources_settings[0]
+                    light_source_settings = model.LightSourceSettings(
+                        id='LightSource:' + '_'.join([light_source_settings.find('LightSource').attrib['Id']
+                                                      for light_source_settings in light_sources_settings]),
+                        attenuation=self.try_default(float, None, self.text(light_source_settings.find('Attenuation'))),
+                        wavelength=self.try_default(float, None, self.text(light_source_settings.find('Wavelength'))),
+                        wavelength_unit=self.nm)
+                else:
+                    light_source_settings = None
+
+                self.ome.images[0].pixels.channels.append(
+                    model.Channel(
+                        id=f'Channel:{idx}',
+                        name=channel.attrib['Name'],
+                        acquisition_mode=self.text(channel.find('AcquisitionMode')).replace(
+                            'SingleMoleculeLocalisation', 'SingleMoleculeImaging'),
+                        color=color,
+                        detector_settings=model.DetectorSettings(
+                            id=detector.attrib['Id'].replace(' ', ""),
+                            binning=binning),
+                        emission_wavelength=emission_wavelength,
+                        excitation_wavelength=self.try_default(float, None,
+                                                               self.text(channel.find('ExcitationWavelength'))),
+                        # filter_set_ref=model.FilterSetRef(id=ome.instruments[0].filter_sets[filterset_idx].id),
+                        illumination_type=self.text(channel.find('IlluminationType')),
+                        light_source_settings=light_source_settings,
+                        samples_per_pixel=samples_per_pixel))
+
+    def get_planes(self) -> None:
+        try:
+            exposure_times = [float(self.text(channel.find('LaserScanInfo').find('FrameTime')))
+                              for channel in self.channels_im.values()]
+        except Exception:  # noqa
+            exposure_times = [None] * len(self.channels_im)
+        delta_ts = self.attachments['TimeStamps'].data()
         dt = np.diff(delta_ts)
         if np.std(dt) / np.mean(dt) > 0.02:
             dt = np.median(dt[dt > 0])
             delta_ts = dt * np.arange(len(delta_ts))
             warnings.warn(f'delta_t is inconsistent, using median value: {dt}')
 
-        for t, z, c in product(range(size_t), range(size_z), range(size_c)):
-            ome.images[0].pixels.planes.append(
+        for t, z, c in product(range(self.size_t), range(self.size_z), range(self.size_c)):
+            self.ome.images[0].pixels.planes.append(
                 model.Plane(the_c=c, the_z=z, the_t=t, delta_t=delta_ts[t],
                             exposure_time=exposure_times[c],
-                            position_x=float(positions.attrib['X']), position_x_unit=um,
-                            position_y=float(positions.attrib['Y']), position_y_unit=um,
-                            position_z=float(positions.attrib['Z']), position_z_unit=um))
+                            position_x=self.positions[0], position_x_unit=self.um,
+                            position_y=self.positions[1], position_y_unit=self.um,
+                            position_z=self.positions[2], position_z_unit=self.um))
 
+    def get_annotations(self) -> None:
         idx = 0
-        for layer in [] if (ml := metadata.find('Layers')) is None else ml:
+        for layer in [] if (ml := self.metadata.find('Layers')) is None else ml:
             rectangle = layer.find('Elements').find('Rectangle')
             if rectangle is not None:
                 geometry = rectangle.find('Geometry')
-                roi = model.ROI(id=f'ROI:{idx}', description=text(layer.find('Usage')))
+                roi = model.ROI(id=f'ROI:{idx}', description=self.text(layer.find('Usage')))
                 roi.union.append(
                     model.Rectangle(
                         id='Shape:0:0',
-                        height=float(text(geometry.find('Height'))),
-                        width=float(text(geometry.find('Width'))),
-                        x=float(text(geometry.find('Left'))),
-                        y=float(text(geometry.find('Top')))))
-                ome.rois.append(roi)
-                ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
+                        height=float(self.text(geometry.find('Height'))),
+                        width=float(self.text(geometry.find('Width'))),
+                        x=float(self.text(geometry.find('Left'))),
+                        y=float(self.text(geometry.find('Top')))))
+                self.ome.rois.append(roi)
+                self.ome.images[0].roi_refs.append(model.ROIRef(id=f'ROI:{idx}'))
                 idx += 1
-        return ome
-
-    def __frame__(self, c: int = 0, z: int = 0, t: int = 0) -> np.ndarray:
-        f = np.zeros(self.base.shape['yx'], self.dtype)
-        if (c, z, t) in self.filedict:
-            directory_entries = self.filedict[c, z, t]
-            x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
-            y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
-            xy_min = {'X': x_min, 'Y': y_min}
-            for directory_entry in directory_entries:
-                subblock = directory_entry.data_segment()
-                tile = subblock.data(resize=True, order=0)
-                axes_min = [xy_min.get(ax, 0) for ax in directory_entry.axes]
-                index = [slice(i - j - m, i - j + k)
-                         for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
-                index = tuple(index[self.reader.axes.index(i)] for i in 'YX')
-                f[index] = tile.squeeze()
-        return f
-
-    @staticmethod
-    def get_index(directory_entry: czifile.DirectoryEntryDV, start: tuple[int]) -> list[tuple[int, int]]:
-        return [(i - j, i - j + k) for i, j, k in zip(directory_entry.start, start, directory_entry.shape)]
```

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.7/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/ndbioimage/transforms.py` & `ndbioimage-2024.4.7/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.6/pyproject.toml` & `ndbioimage-2024.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.6"
+version = "2024.4.7"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
 exclude = ["ndbioimage/jars"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "*"
+numpy = ">=1.20.0"
 pandas = "*"
 tifffile = "*"
 czifile = "2019.7.2"
 tiffwrite = "*"
 ome-types = "^0.4.0"
 pint = "*"
 tqdm = "*"
```

### Comparing `ndbioimage-2024.4.6/PKG-INFO` & `ndbioimage-2024.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.6
+Version: 2024.4.7
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.10,<4.0
@@ -17,15 +17,15 @@
 Requires-Dist: JPype1
 Requires-Dist: SimpleITK-SimpleElastix ; platform_machine == "aarch64" and python_version >= "3.12"
 Requires-Dist: SimpleITK-SimpleElastix ; python_version < "3.12"
 Requires-Dist: SimpleITK-SimpleElastix ; sys_platform != "darwin" and python_version >= "3.12"
 Requires-Dist: czifile (==2019.7.2)
 Requires-Dist: imagecodecs
 Requires-Dist: lxml
-Requires-Dist: numpy
+Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: ome-types (>=0.4.0,<0.5.0)
 Requires-Dist: pandas
 Requires-Dist: parfor (>=2024.3.0)
 Requires-Dist: pint
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pyyaml
 Requires-Dist: scikit-image
@@ -97,19 +97,19 @@
 
 ## Adding more formats
 Readers for image formats subclass AbstractReader. When an image reader is imported, Imread will
 automatically recognize it and use it to open the appropriate file format. Image readers
 are required to implement the following methods:
 
 - staticmethod _can_open(path): return True if path can be opened by this reader
-- property ome: reads metadata from file and adds them to an OME object imported
-from the ome-types library 
 - \_\_frame__(self, c, z, t): return the frame at channel=c, z-slice=z, time=t from the file
 
 Optional methods:
+- get_ome: reads metadata from file and adds them to an OME object imported
+from the ome-types library 
 - open(self): maybe open some file handle
 - close(self): close any file handles
 
 Optional fields:
 - priority (int): Imread will try readers with a lower number first, default: 99
 - do_not_pickle (strings): any attributes that should not be included when the object is pickled,
 for example: any file handles
```

