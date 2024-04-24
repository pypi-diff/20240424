# Comparing `tmp/fileformats_medimage-0.6.7.tar.gz` & `tmp/fileformats_medimage-0.7.0.tar.gz`

## Comparing `fileformats_medimage-0.6.7.tar` & `fileformats_medimage-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.codespell-ignorewords
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.coveragerc
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/pytest.ini
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/LICENSE
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/README.rst
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/pyproject.toml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/_version.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/base.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/dicom.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/diffusion.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/misc.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/nifti.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/surface.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/__init__.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/derivatives.py
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/modality.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/mri/__init__.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/base.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/siemens.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/tests/test_dicom.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/fileformats/medimage/tests/test_nifti.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/LICENSE
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/README.rst
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/pyproject.toml
--rw-r--r--   0        0        0    18984 2020-02-02 00:00:00.000000 fileformats_medimage-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.codespell-ignorewords
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/pytest.ini
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/LICENSE
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/README.rst
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/_version.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/base.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/dicom.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/diffusion.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/itk.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/misc.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/nifti.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/surface.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/anatomical_entity/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/anatomical_entity/anatomical_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/anatomical_entity/immaterial_anatomical_entity.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/anatomical_entity/material_anatomical_entity/anatomical_structure.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/imaging/__init__.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/imaging/derivatives.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/contents/imaging/modality.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/raw/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/raw/mri/__init__.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/raw/pet/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/raw/pet/base.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/raw/pet/siemens.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/tests/test_dicom.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/fileformats/medimage/tests/test_nifti.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/README.rst
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    18984 2020-02-02 00:00:00.000000 fileformats_medimage-0.7.0/PKG-INFO
```

### Comparing `fileformats_medimage-0.6.7/.pre-commit-config.yaml` & `fileformats_medimage-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/conftest.py` & `fileformats_medimage-0.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/.github/workflows/ci-cd.yml` & `fileformats_medimage-0.7.0/.github/workflows/ci-cd.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/LICENSE` & `fileformats_medimage-0.7.0/extras/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/README.rst` & `fileformats_medimage-0.7.0/extras/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/pyproject.toml` & `fileformats_medimage-0.7.0/extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/converters.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/dicom.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/nifti.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/tests/test_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/extras/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage-0.7.0/extras/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/__init__.py` & `fileformats_medimage-0.7.0/fileformats/medimage/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ._version import __version__  # noqa: F401
 from .base import MedicalImage  # noqa: F401
+
 # import Dicom to alias to the medimage namespace it here as well
 from fileformats.application import Dicom  # noqa: F401
 from .misc import (  # noqa: F401
     Analyze,
     Mgh,
     MghGz,
 )
@@ -24,32 +25,31 @@
     NiftiXBvec,
     NiftiGzXBvec,
 )
 from .dicom import (  # noqa: F401
     DicomCollection,
     DicomDir,
     DicomSeries,
-    # SiemensDicomDir,
+    # Vnd_Siemens_Vision,
+    # Vnd_Siemens_VisionDir,
 )
 from .raw import (  # noqa: F401
     Kspace,
     Rda,
     PetListMode,
     PetSinogram,
     PetCountRate,
     PetNormalisation,
     Vnd_Siemens_Biograph128Vision_Vr20b_PetRawData,
     Vnd_Siemens_Biograph128Vision_Vr20b_PetListMode,
     Vnd_Siemens_Biograph128Vision_Vr20b_PetSinogram,
     Vnd_Siemens_Biograph128Vision_Vr20b_PetCountRate,
     Vnd_Siemens_Biograph128Vision_Vr20b_PetNormalisation,
 )
-from .surface import (
-    Gifti  # noqa: F401
-)
+from .surface import Gifti  # noqa: F401
 from .contents.imaging.modality import (  # noqa: F401
     ImagingModality,
     CombinedModalities,
     DualEnergyXrayAbsorptiometry,
     Fluoroscopy,
     MrFluoroscopy,
     RadioFluoroscopy,
@@ -85,14 +85,22 @@
     NM,
     PT,
     PX,
     RF,
     RG,
     US,
 )
-from .contents.imaging.derivatives import (
-    Derivative,
-    Mask
-)
-from .contents.anatomical_entity.material_anatomical_entity.anatomical_structure import (
-    Brain, SpinalCord
-)
+from .contents.imaging.derivatives import Derivative, Mask  # noqa: F401
+from .contents.anatomical_entity.material_anatomical_entity.anatomical_structure import (  # noqa: F401
+    Brain,
+    SpinalCord,
+)
+from .itk import (  # noqa: F401
+    GDCM,
+    GIPL,
+    VTK,
+    PGM,
+    MetaImage,
+    Nrrd,
+    NrrdGz,
+    ItkSupported,
+)
```

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/base.py` & `fileformats_medimage-0.7.0/fileformats/medimage/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/dicom.py` & `fileformats_medimage-0.7.0/fileformats/medimage/dicom.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import typing as ty
-from operator import itemgetter
 from collections import defaultdict, Counter
 from pathlib import Path
 from functools import cached_property
 from fileformats.core import hook, FileSet
 from fileformats.generic import DirectoryContaining, SetOf, TypedSet
 from fileformats.application import Dicom
 from .base import MedicalImage
@@ -36,16 +35,18 @@
 class DicomDir(DicomCollection, DirectoryContaining[Dicom]):
     pass
 
 
 class DicomSeries(DicomCollection, SetOf[Dicom]):
     @classmethod
     def from_paths(
-        cls, fspaths: ty.Iterable[Path], common_ok: bool = False,
-        selected_keys: ty.Optional[ty.Sequence[str]] = None
+        cls,
+        fspaths: ty.Iterable[Path],
+        common_ok: bool = False,
+        selected_keys: ty.Optional[ty.Sequence[str]] = None,
     ) -> ty.Tuple[ty.Set["DicomSeries"], ty.Set[Path]]:
         """Separates a list of DICOM files into separate series from the file-system
         paths
 
         Parameters
         ----------
         fspaths : ty.Iterable[Path]
@@ -63,15 +64,18 @@
             the found dicom series objects and any unrecognised file paths
         """
         dicoms, remaining = Dicom.from_paths(fspaths, common_ok=common_ok)
         series_dict = defaultdict(list)
         for dicom in dicoms:
             dicom.select_metadata(selected_keys)
             series_dict[
-                (str(dicom.metadata["StudyInstanceUID"]), str(dicom.metadata["SeriesNumber"]))
+                (
+                    str(dicom.metadata["StudyInstanceUID"]),
+                    str(dicom.metadata["SeriesNumber"]),
+                )
             ].append(dicom)
         return set([cls(s) for s in series_dict.values()]), remaining
 
 
 @FileSet.read_metadata.register
 def dicom_collection_read_metadata(
     collection: DicomCollection, selected_keys: ty.Optional[ty.Sequence[str]] = None
@@ -79,27 +83,39 @@
     # Collated DICOM headers across series
     collated = {}
     key_repeats = Counter()
     varying_keys = set()
     # We use the "contents" property implementation in TypeSet instead of the overload
     # in DicomCollection because we don't want the metadata to be read ahead of the
     # the `select_metadata` call below
-    base_class = TypedSet if isinstance(collection, DicomSeries) else DirectoryContaining
+    base_class = (
+        TypedSet if isinstance(collection, DicomSeries) else DirectoryContaining
+    )
     for dicom in base_class.contents.fget(collection):
         dicom.select_metadata(selected_keys)
         for key, val in dicom.metadata.items():
             try:
                 prev_val = collated[key]
             except KeyError:
-                collated[key] = val  # Insert initial value (should only happen on first iter)
+                collated[key] = (
+                    val  # Insert initial value (should only happen on first iter)
+                )
                 key_repeats.update([key])
             else:
                 if key in varying_keys:
                     collated[key].append(val)
                 # Check whether the value is the same as the values in the previous
                 # images in the series
                 elif val != prev_val:
                     collated[key] = [prev_val] * key_repeats[key] + [val]
                     varying_keys.add(key)
                 else:
                     key_repeats.update([key])
     return collated
+
+
+# class Vnd_Siemens_Vision(Dicom):
+#     ext = ".ima"
+
+
+# class Vnd_Siemens_VisionDir(DicomDir):
+#     content_types = (Vnd_Siemens_Vision,)
```

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/diffusion.py` & `fileformats_medimage-0.7.0/fileformats/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/misc.py` & `fileformats_medimage-0.7.0/fileformats/medimage/misc.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/nifti.py` & `fileformats_medimage-0.7.0/fileformats/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/contents/imaging/modality.py` & `fileformats_medimage-0.7.0/fileformats/medimage/contents/imaging/modality.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/base.py` & `fileformats_medimage-0.7.0/fileformats/medimage/raw/pet/base.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/raw/pet/siemens.py` & `fileformats_medimage-0.7.0/fileformats/medimage/raw/pet/siemens.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/fileformats/medimage/tests/test_dicom.py` & `fileformats_medimage-0.7.0/fileformats/medimage/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/LICENSE` & `fileformats_medimage-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/README.rst` & `fileformats_medimage-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/pyproject.toml` & `fileformats_medimage-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage-0.6.7/PKG-INFO` & `fileformats_medimage-0.7.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fileformats-medimage
-Version: 0.6.7
+Version: 0.7.0
 Summary: Classes for representing various medical imaging file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

