# Comparing `tmp/cellmap_schemas-0.6.0.tar.gz` & `tmp/cellmap_schemas-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmap_schemas-0.6.0.tar", max compression
+gzip compressed data, was "cellmap_schemas-0.7.0.tar", max compression
```

## Comparing `cellmap_schemas-0.6.0.tar` & `cellmap_schemas-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1466 2024-04-02 13:34:59.790001 cellmap_schemas-0.6.0/LICENSE
--rw-r--r--   0        0        0      122 2024-04-02 13:34:59.790001 cellmap_schemas-0.6.0/README.md
--rw-r--r--   0        0        0      976 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/__init__.py
--rw-r--r--   0        0        0    16120 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/annotation.py
--rw-r--r--   0        0        0     1393 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/base.py
--rw-r--r--   0        0        0     4274 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/cli.py
--rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/__init__.py
--rw-r--r--   0        0        0    20877 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/cosem.py
--rw-r--r--   0        0        0     8679 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
--rw-r--r--   0        0        0    10559 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/n5_wrap.py
--rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/py.typed
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1466 2024-04-03 16:36:23.549826 cellmap_schemas-0.7.0/LICENSE
+-rw-r--r--   0        0        0      122 2024-04-03 16:36:23.549826 cellmap_schemas-0.7.0/README.md
+-rw-r--r--   0        0        0      976 2024-04-03 16:36:23.553826 cellmap_schemas-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/__init__.py
+-rw-r--r--   0        0        0    16120 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/annotation.py
+-rw-r--r--   0        0        0     1393 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/base.py
+-rw-r--r--   0        0        0     4274 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/cli.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/multiscale/__init__.py
+-rw-r--r--   0        0        0    22565 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/multiscale/cosem.py
+-rw-r--r--   0        0        0    11382 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
+-rw-r--r--   0        0        0    10559 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/n5_wrap.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:36:23.557826 cellmap_schemas-0.7.0/src/cellmap_schemas/py.typed
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.7.0/PKG-INFO
```

### Comparing `cellmap_schemas-0.6.0/LICENSE` & `cellmap_schemas-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.6.0/pyproject.toml` & `cellmap_schemas-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cellmap-schemas"
-version = "0.6.0"
+version = "0.7.0"
 description = "Schemas for data used by the Cellmap project team at Janelia Research Campus."
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cellmap_schemas", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/annotation.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/annotation.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/base.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/base.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/cli.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/cosem.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/multiscale/cosem.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,23 @@
 are  stored in the [N5](https://github.com/saalfeldlab/n5) format, and use a layout / metadata
 that's compatible with the [Neuroglancer](https://github.com/google/neuroglancer) visualization tool.
 
 Note that the hierarchy convention modeled here will likely be superceded by conventions defined
 in the [OME-NGFF](https://ngff.openmicroscopy.org/) specification.
 """
 from __future__ import annotations
-from typing import Annotated, Dict, List, Literal, Optional, Sequence, Tuple
+from typing import Annotated, Any, Literal, Optional, Sequence, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Type
+    from typing_extensions import Self
+
 import numpy as np
+from numcodecs.abc import Codec
+from numpy.typing import NDArray
 from pydantic_zarr.v2 import GroupSpec, ArraySpec
 from pydantic import BaseModel, Field, model_validator
 from cellmap_schemas.multiscale import neuroglancer_n5
 from cellmap_schemas.multiscale.neuroglancer_n5 import PixelResolution
 
 
 class STTransform(BaseModel):
@@ -51,21 +58,21 @@
         express a scaling + translation in the axis order that is native to that
         ecosystem, while retaining compatibility with numpy-based tools.
 
         The default is "C". If `order` is missing, it should be assumed to be "C".
     """
 
     order: Optional[Literal["C", "F"]] = "C"
-    axes: Tuple[str, ...]
-    units: Tuple[str, ...]
-    translate: Tuple[float, ...]
-    scale: Tuple[float, ...]
+    axes: tuple[str, ...]
+    units: tuple[str, ...]
+    translate: tuple[float, ...]
+    scale: tuple[float, ...]
 
     @model_validator(mode="after")
-    def validate_argument_length(self: "STTransform"):
+    def validate_argument_length(self: Self):
         if not len(self.axes) == len(self.units) == len(self.translate) == len(self.scale):
             raise ValueError(
                 "The length of all arguments must match. "
                 f"len(axes) = {len(self.axes)}, "
                 f"len(units) = {len(self.units)}, "
                 f"len(translate) = {len(self.translate)}, "
                 f"len(scale) = {len(self.scale)}."
@@ -98,15 +105,15 @@
         if transform.order == "C":
             pixr = PixelResolution(dimensions=transform.scale[::-1], unit=transform.units[-1])
         else:
             pixr = PixelResolution(dimensions=transform.scale, unit=transform.units[0])
         return cls(transform=transform, pixelResolution=pixr)
 
     @model_validator(mode="after")
-    def check_dimensionality(self: "ArrayMetadata"):
+    def check_dimensionality(self: Self):
         """
         Check that `pixelResolution` and `transform` are consistent.
         """
 
         pixr = self.pixelResolution
         tx = self.transform
 
@@ -166,36 +173,36 @@
     Inspired by [this discussion](https://github.com/zarr-developers/zarr-specs/issues/50).
 
     This metadata should be present in the attributes of an N5 group under the key
     `multiscales`.
 
     Attributes
     ----------
-    name: Optional[str]
+    name: str | None
         A name for this multiscale group. Rarely used.
-    datasets: Sequence[ScaleMetadata]
+    datasets: tuple[ScaleMetadata, ...]
         A sequence of [`ScaleMetadata`][cellmap_schemas.multiscale.cosem.ScaleMetadata] elements
-            that refer to the arrays contained inside the group bearing this metadata.
-            Each element of `MultiscaleMetadata.datasets` references an array contained
-            within the group that bears this metadata. These references contain
-        the name of the array, under the `ScaleMeta.path` attribute, and the coordinate
-        metadata for the array, under the `ScaleMeta.transform` attribute.
+        that refer to the arrays contained inside the group bearing this metadata.
+        Each element of `MultiscaleMetadata.datasets` references an array contained
+        within the group that bears this metadata. These references contain
+        the name of the array, under the `ScaleMetadata.path` attribute, and the coordinate
+        metadata for the array, under the `ScaleMetadata.transform` attribute.
     """
 
-    name: Optional[str] = None
-    datasets: Sequence[ScaleMetadata]
+    name: str | None = None
+    datasets: tuple[ScaleMetadata, ...]
 
     @classmethod
-    def from_transforms(cls, transforms: Dict[str, STTransform], *, name: Optional[str] = None):
+    def from_transforms(cls, *, transforms: dict[str, STTransform], name: str | None = None):
         """
         Create an instance of `MultiscaleMetadata` from a dict of `STTransform` and an optional name.
         """
         return cls(
             name=name,
-            datasets=list(ScaleMetadata(path=key, transform=tx) for key, tx in transforms.items()),
+            datasets=tuple(ScaleMetadata(path=key, transform=tx) for key, tx in transforms.items()),
         )
 
 
 class GroupMetadata(neuroglancer_n5.GroupMetadata):
     """
     Multiscale metadata used by COSEM/Cellmap for multiscale datasets saved in N5 groups.
 
@@ -213,18 +220,18 @@
     Attributes
     ----------
     multiscales: List[MultiscaleMetadata]
         This metadata identifies the group as a multiscale group, i.e. a collection of
         images at different levels of detail.
     """
 
-    multiscales: Annotated[List[MultiscaleMetadata], Field(..., max_length=1, min_length=1)]
+    multiscales: Annotated[tuple[MultiscaleMetadata, ...], Field(..., max_length=1, min_length=1)]
 
     @classmethod
-    def from_transforms(cls, transforms: Dict[str, STTransform], *, name: Optional[str] = None):
+    def from_transforms(cls, transforms: dict[str, STTransform], *, name: str | None = None):
         """
         Create `MultiscaleMetadata` from a dict of `STTransform` and an optional name.
         """
         s0 = transforms["s0"]
         if s0.order in ("C", None):
             reorder = slice(None, None, -1)
         else:
@@ -234,15 +241,15 @@
         for scale in [a.scale for a in transforms.values()]:
             scales.append([s // b for s, b in zip(scale, s0.scale)])
 
         axes = s0.axes[reorder]
         units = s0.units[reorder]
         pixr = PixelResolution(dimensions=s0.scale[reorder], unit=units[0])
 
-        multiscales = MultiscaleMetadata.from_transforms(transforms, name=name)
+        multiscales = MultiscaleMetadata.from_transforms(transforms=transforms, name=name)
 
         return cls(
             pixelResolution=pixr, axes=axes, units=units, multiscales=[multiscales], scales=scales
         )
 
 
 class Array(ArraySpec):
@@ -282,24 +289,23 @@
 
     Attributes
     ----------
     attributes: GroupMetadata
         Metadata that conveys that this is a multiscale group, and the coordinate
             information of the arrays it contains.
     members: dict[str, MultiscaleArray]
-        The members of this group must be instances of
+        The members of this group. Must be instances of
             [`MultiscaleArray`][cellmap_schemas.multiscale.cosem.Array]
-
     """
 
     attributes: GroupMetadata
     members: dict[str, Array]
 
     @model_validator(mode="after")
-    def check_arrays_consistent(self: "Group"):
+    def check_arrays_consistent(self: Self):
         """
         Check that the arrays referenced by `GroupMetadata` are consist with the
         arrays in `members`.
         """
 
         axes = self.attributes.axes
         multiscales = self.attributes.multiscales[0]
@@ -353,33 +359,70 @@
                                 f"is {element.transform.axes[::-1]},  which does not match `attributes.axes` ({axes})."
                             )
                             raise ValueError(msg)
 
         return self
 
     @classmethod
-    def from_arrays(cls, arrays: Dict[str, Array], *, name: Optional[str] = None):
-        """
-        Create a `Group` from a dict of `Array` instances
-        """
+    def from_arrays(
+        cls: Type[Self],
+        *,
+        arrays: Sequence[NDArray[Any]],
+        paths: Sequence[str],
+        transforms: Sequence[STTransform],
+        name: str | None = None,
+        chunks: tuple[int, ...] | tuple[tuple[int, ...]] | Literal["auto"] = "auto",
+        compressor: Codec | None | Literal["auto"] = "auto",
+    ) -> Self:
+        """
+        Create a COSEM / Cellmap multiscale group from a collection of array-like objects and
+        spatial metadata. This group should be stored in the N5 format.
+
+        For documentation about this layout, see [https://janelia-cellmap.github.io//cellmap-schemas/cellmap-conventions/s3-overview/](https://janelia-cellmap.github.io//cellmap-schemas/cellmap-conventions/s3-overview/)
+
+        Parameters
+        ----------
+        arrays: Sequence[NDArray[Any]]
+            A sequence of arrays that define a multiscale image.
+        paths: Sequence[str]
+            The names of the arrays in storage.
+        transforms: Sequence[STTransform]
+            Spatial metadata for each image.
+        name: str | None = None
+            A name for this multiscale image
+        chunks: tuple[int, ...] | tuple[tuple[int, ...], ...] | Literal["auto"] = "auto"
+            The chunks to use for the Zarr arrays.
+        compressor: Codec | None | Literal["auto"] = "auto"
+            The compressor to use for the Zarr arrays.
+        """
+        members = {
+            path: Array.from_array(
+                array=array,
+                chunks=chunks,
+                compressor=compressor,
+                dimension_separator="/",
+                attributes=ArrayMetadata.from_transform(transform),
+            )
+            for path, array, transform in zip(paths, arrays, transforms)
+        }
 
         metadata = GroupMetadata.from_transforms(
-            {key: array.attributes.transform for key, array in arrays.items()}, name=name
+            {key: array.attributes.transform for key, array in members.items()}, name=name
         )
-        return cls(attributes=metadata, members=arrays)
+        return cls(attributes=metadata, members=members)
 
 
 def new_sttransform(
     meta: STTransform,
     *,
-    scale: Optional[Tuple[float, ...]] = None,
-    axes: Optional[Tuple[str, ...]] = None,
-    order: Optional[Literal["C", "F"]] = None,
-    translate: Optional[Tuple[float, ...]] = None,
-    units: Optional[Tuple[str, ...]] = None,
+    scale: tuple[float, ...] | None = None,
+    axes: tuple[str, ...] | None = None,
+    order: Literal["C", "F"] | None = None,
+    translate: tuple[float, ...] | None = None,
+    units: tuple[str, ...] | None = None,
 ) -> STTransform:
     if scale is None:
         scale = meta.scale
     if axes is None:
         axes = meta.axes
     if order is None:
         order = meta.order
@@ -390,38 +433,38 @@
 
     return STTransform(scale=scale, order=order, axes=axes, translate=translate, units=units)
 
 
 def new_multiscalemetadata(
     meta: MultiscaleMetadata,
     *,
-    scale: Optional[Tuple[float, ...]] = None,
-    axes: Optional[Tuple[str, ...]] = None,
-    order: Optional[Literal["C", "F"]] = None,
-    translate: Optional[Tuple[float, ...]] = None,
-    units: Optional[Tuple[str, ...]] = None,
+    scale: tuple[float, ...] | None = None,
+    axes: tuple[str, ...] | None = None,
+    order: Literal["C", "F"] | None = None,
+    translate: tuple[float, ...] | None = None,
+    units: tuple[str, ...] | None = None,
 ) -> MultiscaleMetadata:
     new_datasets = []
     for dataset in meta.datasets:
         new_transform = new_sttransform(
             dataset.transform, scale=scale, axes=axes, order=order, translate=translate, units=units
         )
         new_datasets.append(ScaleMetadata(path=dataset.path, transform=new_transform))
 
     return MultiscaleMetadata(name=meta.name, datasets=new_datasets)
 
 
 def new_groupmetadata(
     meta: GroupMetadata,
     *,
-    scale: Optional[Tuple[float, ...]] = None,
-    axes: Optional[Tuple[str, ...]] = None,
-    order: Optional[Literal["C", "F"]] = None,
-    translate: Optional[Tuple[float, ...]] = None,
-    units: Optional[Tuple[str, ...]] = None,
+    scale: tuple[float, ...] | None = None,
+    axes: tuple[str, ...] | None = None,
+    order: Literal["C", "F"] | None = None,
+    translate: tuple[float, ...] | None = None,
+    units: tuple[str, ...] | None = None,
 ) -> GroupMetadata:
     new_multiscales = [
         new_multiscalemetadata(
             meta=meta.multiscales[0],
             scale=scale,
             axes=axes,
             order=order,
@@ -461,19 +504,19 @@
         multiscales=new_multiscales,
     )
 
 
 def change_coordinates(
     group: Group,
     *,
-    scale: Optional[Tuple[float, ...]] = None,
-    axes: Optional[Tuple[str, ...]] = None,
-    order: Optional[Literal["C", "F"]] = None,
-    translate: Optional[Tuple[float, ...]] = None,
-    units: Optional[Tuple[str, ...]] = None,
+    scale: tuple[float, ...] | None = None,
+    axes: tuple[str, ...] | None = None,
+    order: Literal["C", "F"] | None = None,
+    translate: tuple[float, ...] | None = None,
+    units: tuple[str, ...] | None = None,
 ):
     """
     Return a Group with new coordinates, i.e., new scale, axes, order, translate, or units. If any of these
     paramters are set to None (the default), then the old values are used.
 
     The `units`, `axes`, and `order` attributes can be changed globally.
     The `scale` and `translation` changes will be applied to the largest image, then a scaling / translation vector will be calculated to express this change, and that
```

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """
 This module contains Pydantic models for Neuroglancer-compatible multiscale images stored 
 in N5 groups. See Neuroglancer's [N5-specific documentation](https://github.com/google/neuroglancer/tree/master/src/neuroglancer/datasource/n5) 
 for details on what Neuroglancer expects when it reads N5 data.
 """
 from __future__ import annotations
-from typing import Annotated, Sequence
-from pydantic import BaseModel, PositiveInt, model_validator, AfterValidator
-from pydantic_zarr.v2 import ArraySpec
+from typing import TYPE_CHECKING, Any, Sequence
+
+if TYPE_CHECKING:
+    from typing_extensions import Self, Type, Literal
+    from numcodecs.abc import Codec
+from pydantic import BaseModel, PositiveInt, model_validator
+from pydantic_zarr.v2 import ArraySpec, GroupSpec
 
 from cellmap_schemas.n5_wrap import N5GroupSpec
+from numpy.typing import NDArray
 
 
 class PixelResolution(BaseModel):
     """
     This attribute is used by N5-fluent tools like Neuroglancer to convey the
     spacing between points on a N-dimensional coordinate grid, and the unit of measure
     for the coordinate grid, for data stored in the N5 format.
@@ -53,18 +58,25 @@
     dimensions: Sequence[float]
             The distance, in units given by the `unit` attribute, between samples, per axis.
             Conventionally referred to as the "resolution" of the image.
     unit: str
             The physical unit for the `dimensions` attribute.
     """  # noqa: E501
 
-    dimensions: Sequence[float]
+    dimensions: tuple[float, ...]
     unit: str
 
 
+class ArrayMetadata(BaseModel):
+    pixelResolution: PixelResolution
+
+
+Array = ArraySpec[ArrayMetadata]
+
+
 # todo: validate argument lengths
 class GroupMetadata(BaseModel):
     """
     Metadata to enable displaying an N5 group containing several datasets
     as a multiresolution image in neuroglancer, based on
     [this comment](https://github.com/google/neuroglancer/issues/176#issuecomment-553027775).
 
@@ -72,54 +84,53 @@
 
     The attributes `axes`, `units`, and the elements of `scales` should be indexed
     colexicographically, i.e. the opposite order from Numpy-standard order,
     which is lexicographic.
 
     Attributes
     ----------
-    axes : Sequence[str]
+    axes : tuple[str]
             The names of the axes of the data
-    units : Sequence[str]
+    units : tuple[str]
             The units for the axes of the data
-    scales : Sequence[Sequence[PositiveInt]]
+    scales : tuple[tuple[PositiveInt]]
             The relative scales of each axis. E.g., if this metadata describes a 3D dataset
             that was downsampled isotropically by 2 along each axis over two iterations,
             resulting in 3 total arrays, then `scales` would be the list
             `[[1,1,1], [2,2,2], [4,4,4]]`.
     pixelResolution: PixelResolution
             An instance of `PixelResolution` that specifies the interval, in physical units,
             between adjacent samples, per axis. Note that `PixelResolution` also defines a
             `unit` attribute, which is redundant with the `units` attribute defined on this
             class.
     """  # noqa: E501
 
-    axes: Sequence[str]
-    units: Sequence[str]
-    scales: Sequence[Sequence[PositiveInt]]
+    axes: tuple[str, ...]
+    units: tuple[str, ...]
+    scales: tuple[tuple[PositiveInt, ...], ...]
     pixelResolution: PixelResolution
 
     @model_validator(mode="after")
     def check_dimensionality(self: "GroupMetadata"):
         if not len(self.axes) == len(self.units):
             msg = (
                 f"The number of elements in `axes` ({len(self.axes)}) does not"
                 f"match the number of elements in `units` ({len(self.units)})."
             )
             raise ValueError(msg)
-        for idx, scale in enumerate(self.scales):
-            if idx == 0 and not all(s == 1 for s in scale):
-                msg = f"The first element of `scales` must be all 1s. Got {scale} instead."
-                raise ValueError(msg)
+        if not all(s == 1 for s in self.scales[0]):
+            msg = f"The first element of `scales` must be all 1s. Got {self.scales[0]} instead."
+            raise ValueError(msg)
+        for idx, scale in tuple(enumerate(self.scales)):
             if not len(scale) == len(self.axes):
                 msg = (
                     f"The number of elements in `axes` ({len(self.axes)}) does not"
                     f"match the number of elements in the {idx}th element in `scales`"
                     f"({len(self.units)})."
                 )
-
                 raise ValueError(msg)
 
         if not len(self.pixelResolution.dimensions) == len(self.axes):
             raise ValueError(
                 f"The number of elements in `axes` ({len(self.axes)})"
                 "does not match the number of elements in `pixelResolution.dimensions`"
                 f"({len(self.pixelResolution.dimensions)})"
@@ -128,91 +139,127 @@
         for idx, u in enumerate(self.units):
             if not u == self.pixelResolution.unit:
                 msg = (
                     f"The {idx}th element of `units` ({u}) does not "
                     f"match `pixelResolution.unit` ({self.pixelResolution.unit})"
                 )
                 raise ValueError(msg)
-
         return self
 
 
-def check_members(members: dict[str, ArraySpec]) -> dict[str, ArraySpec]:
-    # check that the names of the arrays are s0, s1, s2, etc
-    for key, spec in members.items():
-        assert check_scale_level_name(key)
-    # check that dtype is uniform
-    assert len(set(a.dtype for a in members.values())) == 1
-    # check that dimensionality is uniform
-    assert len(set(len(a.shape) for a in members.values())) == 1
-    return members
-
-
-def check_scale_level_name(name: str) -> bool:
-    """
-    Check if the input follows the pattern `s$INT`, i.e., check if the input is
-    a string that starts with "s", followed by a string representation of an integer,
-    and nothing else.
-
-    If validation passes, this function returns `True`.
-    If validation fails, it returns `False`.
-
-    Parameters
-    ----------
-
-    name: str
-            The name to check.
-
-    Returns
-    -------
-
-    `True` if `name` is valid, `False` otherwise.
-    """
-    valid = True
-    if name.startswith("s"):
-        try:
-            int(name.split("s")[-1])
-        except ValueError:
-            valid = False
-    else:
-        valid = False
-    return valid
-
-
 class Group(N5GroupSpec):
     """
     A `GroupSpec` representing the structure of a N5 group with
     neuroglancer-compatible structure and metadata.
 
     Attributes
     ----------
 
     attributes : GroupMetadata
             The metadata required to convey to neuroglancer that this group represents a
             multiscale image.
-    members : Dict[str, Union[GroupSpec, ArraySpec]]
+    members : Dict[str, ArraySpec | GroupSpec]
             The members of this group. Arrays must be consistent with the `scales` attribute
             in `attributes`.
 
     """
 
     attributes: GroupMetadata
-    members: Annotated[dict[str, ArraySpec], AfterValidator(check_members)]
+    members: dict[str, Array | GroupSpec]
+
+    @classmethod
+    def from_arrays(
+        cls: Type[Self],
+        *,
+        arrays: Sequence[NDArray[Any]],
+        paths: Sequence[str],
+        axes: Sequence[str],
+        scales: Sequence[Sequence[float]],
+        units: Sequence[str],
+        chunks: tuple[int, ...] | tuple[tuple[int, ...]] | Literal["auto"] = "auto",
+        compressor: Codec | None | Literal["auto"] = "auto",
+        dimension_order: Literal["C", "F"],
+    ) -> Self:
+        """
+        Create a Neuroglancer / N5 multiscale group from a collection of array-like objects and
+        spatial metadata. This group should be stored in the N5 format.
+
+        Parameters
+        ----------
+        arrays: Sequence[NDArray[Any]]
+            A sequence of arrays that define a multiscale image.
+        paths: Sequence[str]
+            The names of the arrays in storage.
+        axes: Sequence[str]
+            The names of the dimensions of the multiscale image.
+        scales: Sequence[Sequence[float]]
+            The scaling transformation for each array in the multiscale image.
+        units: Sequence[str]
+            The units associated with each dimension of the multiscale image.
+        chunks: tuple[int, ...] | tuple[tuple[int, ...], ...] | Literal["auto"] = "auto"
+            The chunks to use for the Zarr arrays.
+        compressor: Codec | None | Literal["auto"] = "auto"
+            The compressor to use for the Zarr arrays.
+        dimension_order: Literal["C", "F"]
+            The dimension order to use when interpreting dimensional attributes like `axes`,
+            `scales` and `units`. Neuroglancer / N5 metadata iterates array axes in F order, but
+            Python-native tools like `zarr-python` tends to iterate array axes in C order. Because
+            the class being constructed here uses N5 metadata wrapped in a Python library, there is
+            a risk of confusion about the order in which axes will be iterated, in particular when
+            handling `scales` and `axes` metadata. The `dimension_order` parameter explicitly
+            denotes whether the `axes` parameter, and the elements of the `scales` parameter, are
+            to be interpreted as mapping to the dimensions of the data in F order or C order. Note
+            that `dimension_order` has no effect on the `chunks` parameter, since that is managed
+            entirely by Zarr.
+        """
+
+        if dimension_order == "C":
+            # this will reverse the order of axes, units, and scales before writing metadata
+            indexer = slice(-1, None, -1)
+        else:
+            # this preserves the order of axes, units, and scales before writing metadata
+            indexer = slice(None)
+
+        axes_parsed = tuple(axes[indexer])
+        scales_parsed = tuple(tuple(s)[indexer] for s in scales)
+        units_parsed = tuple(units[indexer])
+
+        scale_ratios = tuple(
+            tuple(int(a // b) for a, b in zip(scale, scales_parsed[0])) for scale in scales_parsed
+        )
+
+        attributes = GroupMetadata(
+            axes=axes_parsed,
+            units=units_parsed,
+            scales=scale_ratios,
+            pixelResolution=PixelResolution(unit=units_parsed[0], dimensions=scales_parsed[0]),
+        )
+        members = {
+            path: Array.from_array(
+                attributes=ArrayMetadata(
+                    pixelResolution=PixelResolution(dimensions=scale, unit=units_parsed[0])
+                ),
+                array=array,
+                chunks=chunks,
+                compressor=compressor,
+            )
+            for path, array, scale in zip(paths, arrays, scales_parsed)
+        }
+        return cls(members=members, attributes=attributes)
 
     @model_validator(mode="after")
-    def check_scales(self: "Group"):
+    def check_scales(self: Self):
         scales = self.attributes.scales
         members = self.members
 
         for level in range(len(scales)):
             name_expected = f"s{level}"
             if name_expected not in members:
                 raise ValueError(
-                    f"Expected to find {name_expected} in `members` but it is missing. "
-                    f"members[{name_expected}] should be an array."
+                    f"Expected an array called {name_expected} in `members`, but it is missing. "
                 )
-            elif not isinstance(members[name_expected], ArraySpec):
+            if not isinstance(members[name_expected], ArraySpec):
                 raise ValueError(
-                    f"members[{name_expected}] should be an array. Got {type(members[name_expected])} instead."
+                    f"Expected an array called {name_expected} in `members`. Got {type(members[name_expected])} instead."
                 )
 
         return self
```

### Comparing `cellmap_schemas-0.6.0/src/cellmap_schemas/n5_wrap.py` & `cellmap_schemas-0.7.0/src/cellmap_schemas/n5_wrap.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.6.0/PKG-INFO` & `cellmap_schemas-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap-schemas
-Version: 0.6.0
+Version: 0.7.0
 Summary: Schemas for data used by the Cellmap project team at Janelia Research Campus.
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

