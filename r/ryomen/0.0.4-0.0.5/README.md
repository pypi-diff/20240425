# Comparing `tmp/ryomen-0.0.4.tar.gz` & `tmp/ryomen-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryomen-0.0.4.tar", last modified: Tue Apr 23 23:02:40 2024, max compression
+gzip compressed data, was "ryomen-0.0.5.tar", last modified: Wed Apr 24 18:36:51 2024, max compression
```

## Comparing `ryomen-0.0.4.tar` & `ryomen-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.149716 ryomen-0.0.4/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1064 2024-04-16 15:51:46.000000 ryomen-0.0.4/LICENSE
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5654 2024-04-23 23:02:40.149616 ryomen-0.0.4/PKG-INFO
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.147634 ryomen-0.0.4/ryomen/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       31 2024-04-15 17:56:53.000000 ryomen-0.0.4/ryomen/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    22085 2024-04-23 22:57:56.000000 ryomen-0.0.4/ryomen/main.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.148735 ryomen-0.0.4/ryomen.egg-info/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5654 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/PKG-INFO
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      226 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/SOURCES.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/dependency_links.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        7 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/top_level.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.4/ryomen.egg-info/zip-safe
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-23 23:02:40.150035 ryomen-0.0.4/setup.cfg
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.4/setup.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.148985 ryomen-0.0.4/tests/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     8560 2024-04-17 20:42:38.000000 ryomen-0.0.4/tests/test_ryomen.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-24 18:36:51.442601 ryomen-0.0.5/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1064 2024-04-16 15:51:46.000000 ryomen-0.0.5/LICENSE
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5888 2024-04-24 18:36:51.442685 ryomen-0.0.5/PKG-INFO
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-24 18:36:51.440993 ryomen-0.0.5/ryomen/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       31 2024-04-15 17:56:53.000000 ryomen-0.0.5/ryomen/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    24253 2024-04-24 17:29:01.000000 ryomen-0.0.5/ryomen/main.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-24 18:36:51.442052 ryomen-0.0.5/ryomen.egg-info/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5888 2024-04-24 18:36:51.000000 ryomen-0.0.5/ryomen.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      226 2024-04-24 18:36:51.000000 ryomen-0.0.5/ryomen.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-24 18:36:51.000000 ryomen-0.0.5/ryomen.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        7 2024-04-24 18:36:51.000000 ryomen-0.0.5/ryomen.egg-info/top_level.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.5/ryomen.egg-info/zip-safe
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-24 18:36:51.443080 ryomen-0.0.5/setup.cfg
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.5/setup.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-24 18:36:51.442316 ryomen-0.0.5/tests/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     8561 2024-04-24 15:16:35.000000 ryomen-0.0.5/tests/test_ryomen.py
```

### Comparing `ryomen-0.0.4/LICENSE` & `ryomen-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ryomen-0.0.4/PKG-INFO` & `ryomen-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -155,14 +155,21 @@
     
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
 ### Change Log
+
+
+#### 0.0.5
+    - fixed bug with duplicate indices being shown, leading to redundant behaviro
+    - added support for zarr arrays, as they do not implement a flip method or support negative indexing
+    - refactored for readability
+
 #### 0.0.4
     - padding now works with pure indexing, for reflections. Tested up to 3D with numpy. 
 
 
 #### 0.0.3
     - First working version
```

### Comparing `ryomen-0.0.4/ryomen/main.py` & `ryomen-0.0.5/ryomen/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,23 +33,26 @@
 
     def __iter__(self) -> Iterator:
         ...
 
     def __next__(self) -> TensorLike:
         ...
 
+    def __mul__(self, other) -> TensorLike:
+        ...
+
     def size(self) -> Shape:
         ...
 
     def flip(self, dim: int) -> TensorLike:
         ...
 
 
 def _get_next_slice(
-    ind: List[int], c: List[int], o: List[int], shape: Shape, pad: bool
+        ind: List[int], c: List[int], o: List[int], shape: Shape, pad: bool
 ) -> Tuple[Index, List[int]]:
     """
     given a current index ind, a crop c, overlap o, and image shape
     calculate the next index of a crop such that all tiles of the image are eventually
     covered
 
     :param ind: list of the current coordinate pos
@@ -72,73 +75,88 @@
         else:
             ind[i] = -o[i] if pad else 0
             i += 1
     return tuple(indices), ind
 
 
 def _nd_generator(
-    crop, overlap, shape, pad: bool
+        crop: List[int], overlap: List[int], shape: Shape, pad: bool
 ) -> Generator[Tuple[Index, Sequence[int]], None, None]:
     """ so cursed """
     assert len(crop) == len(overlap)
 
     # In the weird case where an overlap is larger than a crop, we should fail here...
     for c, o in zip(crop, overlap):
         if not c > o * 2:
             raise ValueError(f"Crop Size must be larger than overlap * 2. {c=} !> {o=} * 2")
 
     # init a list of zeros as the "first" crop location
     x = [-o if pad else 0 for _, o in zip(crop, overlap)]
     assert len(shape) >= len(crop)
 
+    # We cache all previous indices here, as the cost of looking this up
+    # is presumably less than the cost of re-running the expensive fn
+    previously_yeilded = []
+
     # copy because lists are mutable and we need to mutate it in this scope but not the higher one...
     shape = copy(list(shape))
 
     # Leading dimensions are allowed, therefore we pop off all leading dimensions until the shape
     # and crop shape are the same!
     while len(shape) > len(crop):
         shape.pop(0)
 
     ind, x = _get_next_slice(x, crop, overlap, shape, pad)
     while not all((a + c) > b + (o * pad) for a, b, c, o in zip(x, shape, crop, overlap)):
-        yield ind, x
+        if str(ind) not in previously_yeilded:
+            previously_yeilded.append(str(ind))
+            yield ind, x
+
         ind, x = _get_next_slice(x, crop, overlap, shape, pad)
-    yield ind, x
+
+    if str(ind) not in previously_yeilded:
+        previously_yeilded.append(str(ind))
+        yield ind, x
 
     ind, x = _get_next_slice(x, crop, overlap, shape, pad)
-    yield ind, x
+    if str(ind) not in previously_yeilded:
+        previously_yeilded.append(str(ind))
+        yield ind, x
 
 
 def default_colate(x: Sequence[TensorLike]) -> TensorLike | Sequence[TensorLike]:
     return x
 
 
 def default_progress_bar(x: Iterator | Generator) -> Any:
     return x
 
 
 class Slicer:
     def __init__(
-        self,
-        image: TensorLike,
-        crop_size: Sequence[int],
-        overlap: Sequence[int],
-        batch_size: int = 1,
-        pad: bool = False,
-        output_transform: Callable[[TensorLike], TensorLike] = lambda x: x,
-        collate: Callable[
-            [Sequence[TensorLike]], TensorLike | Sequence[TensorLike]
-        ] = default_colate,
-        progress_bar: Callable[[Iterator | Generator], Any] = default_progress_bar,
+            self,
+            image: TensorLike,
+            crop_size: Sequence[int],
+            overlap: Sequence[int],
+            batch_size: int = 1,
+            pad: bool = False,
+            output_transform: Callable[[TensorLike], TensorLike] = lambda x: x,
+            collate: Callable[
+                [Sequence[TensorLike]], TensorLike | Sequence[TensorLike]
+            ] = default_colate,
+            progress_bar: Callable[[Iterator | Generator], Any] = default_progress_bar,
     ):
         """
-        BioCropper is a generic cropping utility for separating up large microscopy images into smaller,
-        equal sized, sub crops. It works on any array type as long as that array has the methods __getitem__(), size(),
-        and a class variable: size. Tested Array types include: numpy.ndarray, torch.Tensor, zarr.Array
+        Ryomen is a generic cropping utility for separating up large microscopy images into smaller,
+        equal sized, sub crops.
 
+        Ryomen works with any generic array type, as long as it implements the following methods: __getitem__,
+        __setitem__, __iter__, and __size__. Furthermore, the array type must support either a flip method, or
+        support negative indexing, and must implement a parameter shape. These criteria basically fit all
+        numpy-like arrays. Tested array libraries include zarr, numpy, and pytorch.
 
         Basic Usage:
 
         >>> import numpy as np
         >>> from ryomen import Slicer
         >>> image = np.random.randn((3, 100, 100, 100))  # A large, 3D array with a color channel
         >>> # image.shape is [B, C, X, Y, Z]
@@ -204,51 +222,75 @@
         self.__can_pad = (
             False  # Default, is changed to value of pad after suitable checks
         )
         self.__support_negative_strides = (
             False  # Default, is changed to true after suitable checks
         )
 
-        # Check that all of the nasty inputs are handled...
+        # Zarr arrays dont have a flip method, or support negative indices. However,
+        # after one indexing, they turn into numpy arrays which DO support negative
+        # indices. To keep no dependencies, we do not type check, however
+        # if it looks like a duck...
+        self.__probably_a_zarr_array = False
+
+        # Check that all of the inputs are legitimate...
         self._check_validity()
 
         # Adjust crop size such that we can return images smaller than crop size.
         # This is silent and might be confusing. The user should never have to access the crop size after creation.
+        self._adjust_crop_size()
+
+        # Here we check if we can pad the image with indexing. We require negative indexing support, an implement flip
+        # method, or it to be a zarr array
+        self._able_to_pad(pad)
 
+    def _adjust_crop_size(self):
+        """
+        checks if user supplied crop size is larger than the image. If so, modifies the crop
+        size to fit entire image all at once.
+        """
         self.__user_defined_crop_larger_than_image = False
         image_shape = self.__image.shape
 
         for i, size in enumerate(self.__crop_size):
             if (
-                not self.__crop_size[i]
-                < image_shape[i + len(image_shape) - len(self.__crop_size)]
+                    not self.__crop_size[i]
+                        < image_shape[i + len(image_shape) - len(self.__crop_size)]
             ):
                 self.__user_defined_crop_larger_than_image = True
 
             self.__crop_size[i] = (
                 self.__crop_size[i]
                 if self.__crop_size[i]
-                < image_shape[i + len(image_shape) - len(self.__crop_size)]
+                   < image_shape[i + len(image_shape) - len(self.__crop_size)]
                 else image_shape[i + len(image_shape) - len(self.__crop_size)]
             )
 
-        try:
+    def _able_to_pad(self, pad: bool):
+        """ checks for negative indexing support, or a flip method. Ugly implementation! """
+        try:  # test for negative stride
             self.__image[0:1:-1, ...]  # can flip with negative indices
             self.__support_negative_strides = True
             self.__can_pad = pad
 
-        except:
-            if not hasattr(self.__image, "flip"):
-
-                raise RuntimeError(
-                    "Your image array does not implement a flip method or support negative strides. Therefore, padding is not supported."
-                )
-            else:
+        except:  # Bare except is bad. I dont think its a big deal here though. Dont know error a priori
+            try:
+                self.__image[0:1, ...][::-1, ...]
+                self.__probably_a_zarr_array = True
                 self.__can_pad = pad
 
+            except:
+                if not hasattr(self.__image, "flip"):
+
+                    raise RuntimeError(
+                        "Your image array does not implement a flip method or support negative strides. Therefore, padding is not supported."
+                    )
+                else:
+                    self.__can_pad = pad
+
     def _check_validity(self):
         """ simply checks the validity of all inputs """
 
         if not hasattr(self.__image, "size"):
             raise ValueError(
                 f"Input array of type {type(self.__image)} does not have the method: size"
             )
@@ -315,48 +357,74 @@
         if self.__batch_size > n:
             raise RuntimeError(
                 "requested batch size is greater than the entirety of the image cropped. "
                 f"All crops collated would result in {n} batches. {n} < {self.__batch_size}"
             )
 
     def __iter__(
-        self,
+            self,
     ) -> Generator[
         Tuple[
             TensorLike | Sequence[TensorLike],
             Index | Sequence[Index],
             Index | Sequence[Index],
         ],
         None,
         None,
     ]:
+        """
+        Creates a generator which yields a TensorLike Crop, Source Indices, and Destination Indices
+        """
         image_shape: Shape = self.__image.shape  # C, X, Y, Z
 
         output_cache = []
         for ind, xyz in self.__progress_bar(
-            _nd_generator(self.__crop_size, self.__overlap, image_shape, self.__can_pad)
+                _nd_generator(self.__crop_size, self.__overlap, image_shape, self.__can_pad)
         ):
 
+
             # _nd_generator returns a list of slices
-            source = self._source()
-            destination = self._destination(
+            source: Index = self._get_source_index()
+            destination: Index = self._get_destination_index(
                 tuple(a.start for a in ind if isinstance(a, slice)), image_shape
             )
-            crop = self._index_image_with_pad(tuple(ind))
+            crop: TensorLike = self._index_image_with_pad(tuple(ind))
             output_cache.append((self.__output_fn(crop), source, destination))
 
             # If we've added more to the output cache than the batch size, we flush the batch away
             if len(output_cache) == self.__batch_size:
                 yield self._flush_output(output_cache)
 
         if len(output_cache) > 0:
             yield self._flush_output(output_cache)
 
+    def _get_source_index(self) -> Index:
+        """ returns indices of the crop excluding overlap """
+        source = [Ellipsis]
+        for o, s in zip(self.__overlap, self.__crop_size):
+            source += [slice(o, -o if o != 0 else s)]
+        return tuple(source)
+
+    def _get_destination_index(self, xyz: Sequence[int], shape: Shape) -> Index:
+        """
+        returns the indicies necessary to place the non-overlaping region of the image into a new tensor
+        """
+        shape = list(shape)
+        while len(shape) > len(self.__crop_size):
+            shape.pop(0)
+
+        destination: Sequence[EllipsisType | slice] = [Ellipsis]
+        for a, c, o, s in zip(xyz, self.__crop_size, self.__overlap, shape):
+            a = a if a + c < s + (self.__can_pad * o) else s - c + (self.__can_pad * o)
+            destination += [slice(a + o, (a + c) - o, 1)]
+
+        return tuple(destination)
+
     def _flush_output(
-        self, output_cache
+            self, output_cache
     ) -> Tuple[
         TensorLike | Sequence[TensorLike],
         Index | Sequence[Index],
         Index | Sequence[Index],
     ]:
         """ pop off the cache and convert to images, sources, and destinations """
         output = []
@@ -367,16 +435,16 @@
             [t for t, s, d in output]
         )
 
         sources: List[Index] = [tuple(s) for t, s, d in output]
         destinations: List[Index] = [tuple(d) for t, s, d in output]
 
         if (
-            isinstance(images, list)
-            and len(images) == len(sources) == len(destinations) == 1
+                isinstance(images, list)
+                and len(images) == len(sources) == len(destinations) == 1
         ):
             return images[0], sources[0], destinations[0]
 
         else:
             return images, sources, destinations
 
     def __len__(self):
@@ -392,25 +460,42 @@
                         pad=self.__can_pad,
                     )
                 )
             )
         return self.__N
 
     @staticmethod
-    def minmax(a: slice, m: int) -> slice:
+    def _minmax(a: slice, m: int) -> slice:
+        """ clamps a slice between 0 and m """
 
         if a.start < 0:
             delta = abs(a.start)
             a = slice(a.start + delta, a.stop + delta, a.step)
         elif a.stop > m:
             delta = abs(a.stop - m)
             a = slice(a.start - delta, a.stop - delta, a.step)
 
         return slice(min(max(a.start, 0), m), min(max(a.stop, 0), m), a.step)
 
+    def _flip_array(self, array: TensorLike, index: int):
+        """ handes flipping a zarr array """
+        if self.__probably_a_zarr_array and self.__can_pad:
+            ind = []
+            for i, s in enumerate(array.shape):
+                if i == index:
+                    ind.append(slice(s, None, -1))
+                else:
+                    ind.append(slice(0, None, 1))
+
+            return array[tuple(ind)]
+        elif not self.__support_negative_strides:  # can flip...
+            return array.flip(index)
+        else:
+            RuntimeError('unknown error. cannot flip or not a zarr array')
+
     def _index_image_with_pad(self, index: Index) -> TensorLike:
         """
         Terrible function to index the image, and through indexing alone, pads the image with reflections. It
         should do this in N Dimensions, but was an absolute nightmare to code, and there are so many edge cases. Ive
         tried my best to handle as many as possible, but innevitably some may fall through thte cracks.
         :param index:
         :return:
@@ -449,120 +534,77 @@
             [0 for _ in self.__crop_size],
             c=self.__crop_size,
             o=self.__overlap,
             shape=shape,
             pad=False,
         )
 
-        output_array = (self.__image[_output_index] / float("inf")) + 1
+        output_array = self.__image[_output_index] * 0  # zeros the array
         first_access = False
         n_leading_dimensions = len(shape) - len(self.__crop_size)
         for i, (ind, s, o) in enumerate(zip(modified_index, shape, self.__overlap)):
             pad = None
             other = None
 
             padding_source: SliceList = [Ellipsis]
             other_source: SliceList = [Ellipsis]
             padding_destination: SliceList = [Ellipsis]
             other_destination: SliceList = [Ellipsis]
 
+            has_padded = False
+
             # Padding on the left
             if ind.start < 0:
+                has_padded = True
                 for d, (current_slice, c) in enumerate(
-                    zip(modified_index, self.__crop_size)
+                        zip(modified_index, self.__crop_size)
                 ):
                     x = c if first_access else shape[d + n_leading_dimensions]
                     if i + n_leading_dimensions != d:
-                        padding_source.append(self.minmax(current_slice, c if first_access else x))
-                        other_source.append(self.minmax(current_slice, c if first_access else x))
+                        padding_source.append(self._minmax(current_slice, c if first_access else x))
+                        other_source.append(self._minmax(current_slice, c if first_access else x))
                         padding_destination.append(slice(0, c, 1))
                         other_destination.append(slice(0, c, 1))
                     else:
                         padding_source.append(
                             slice(abs(ind.start) - 1, None, -1)
                             if self.__support_negative_strides
                             else slice(0, abs(ind.start), 1)
                         )
                         padding_destination.append(slice(0, abs(ind.start), 1))
                         other_source.append(slice(0, ind.stop, 1))
                         other_destination.append(slice(abs(ind.start), None, 1))
 
-                to_acces = output_array if first_access else self.__image
-                if self.__support_negative_strides:
-                    pad = to_acces[tuple(padding_source)]
-                else:
-                    pad = to_acces[tuple(padding_source)].flip(
-                        i + len(shape) - len(self.__crop_size)
-                    )
-
-                other = to_acces[tuple(other_source)]
-
-            if pad is not None:
-                try:
-                    output_array[tuple(other_destination)] = other
-                    output_array[tuple(padding_destination)] = pad
-                except:
-                    pass
-                    raise RuntimeError
-                first_access = True
-
             # Padding on the right
             elif ind.stop > s:
+                has_padded = True
                 for d, (current_slice, c) in enumerate(
-                    zip(modified_index, self.__crop_size)
+                        zip(modified_index, self.__crop_size)
                 ):
                     x = c if first_access else shape[d + n_leading_dimensions]
                     if i + len(shape) - len(self.__crop_size) != d:
-                        padding_source.append(self.minmax(current_slice, x))
-                        other_source.append(self.minmax(current_slice, x))
+                        padding_source.append(self._minmax(current_slice, x))
+                        other_source.append(self._minmax(current_slice, x))
                         padding_destination.append(slice(0, c, 1))
                         other_destination.append(slice(0, c, 1))
                     else:
-
                         padding_source.append(
                             slice(x, -(ind.stop - s) - 1, -1)
                             if self.__support_negative_strides
                             else slice(-(ind.stop - s), x, 1)
                         )
                         other_source.append(slice(ind.stop - s if first_access else current_slice.start, x))
                         padding_destination.append(slice(-(ind.stop - s), c, 1))
                         other_destination.append(slice(0, -(ind.stop - s), 1))
 
-                    to_acces = output_array if first_access else self.__image
-                    if self.__support_negative_strides:
-                        pad = to_acces[tuple(padding_source)]
-                    else:
-                        pad = to_acces[tuple(padding_source)].flip(
-                            i + len(shape) - len(self.__crop_size)
-                        )
-
-                    other = to_acces[tuple(other_source)]
+            if has_padded:
+                to_access = output_array if first_access else self.__image
+                pad = deepcopy(to_access[tuple(padding_source)])
+                if not self.__support_negative_strides:
+                    pad = self._flip_array(pad, i + len(shape) - len(self.__crop_size))
+                other = deepcopy(to_access[tuple(other_source)])
 
-                if pad is not None:
-                    output_array[tuple(other_destination)] = other
-                    output_array[tuple(padding_destination)] = pad
+                output_array[tuple(other_destination)] = other
+                output_array[tuple(padding_destination)] = pad
+                first_access = True
 
-                    first_access = True
-        pass
         return output_array
-
-    def _source(self) -> Index:
-        """ returns indices of the crop excluding overlap """
-        source = [Ellipsis]
-        for o, s in zip(self.__overlap, self.__crop_size):
-            source += [slice(o, -o if o != 0 else s)]
-        return tuple(source)
-
-    def _destination(self, xyz: Sequence[int], shape: Shape) -> Index:
-        """
-        returns the indicies to place the non-overlaping region of the image into a new tensor
-        """
-        shape = list(shape)
-        while len(shape) > len(self.__crop_size):
-            shape.pop(0)
-
-        destination: Sequence[EllipsisType | slice] = [Ellipsis]
-        for a, c, o, s in zip(xyz, self.__crop_size, self.__overlap, shape):
-            a = a if a + c < s + (self.__can_pad * o) else s - c + (self.__can_pad * o)
-            destination += [slice(a + o, (a + c) - o, 1)]
-
-        return tuple(destination)
```

### Comparing `ryomen-0.0.4/ryomen.egg-info/PKG-INFO` & `ryomen-0.0.5/ryomen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.4
+Version: 0.0.5
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -155,14 +155,21 @@
     
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
 ### Change Log
+
+
+#### 0.0.5
+    - fixed bug with duplicate indices being shown, leading to redundant behaviro
+    - added support for zarr arrays, as they do not implement a flip method or support negative indexing
+    - refactored for readability
+
 #### 0.0.4
     - padding now works with pure indexing, for reflections. Tested up to 3D with numpy. 
 
 
 #### 0.0.3
     - First working version
```

### Comparing `ryomen-0.0.4/tests/test_ryomen.py` & `ryomen-0.0.5/tests/test_ryomen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 from ryomen.main import Slicer, _nd_generator
 import numpy as np
 
 
+
 def test_that_nd_gen_finishes():
     max = 10000
     counter = 0
     for ind, xyz in _nd_generator(
         crop=[10, 10, 10], overlap=[2, 2, 2], shape=(100, 100, 10), pad=False
     ):
         counter += 1
```

