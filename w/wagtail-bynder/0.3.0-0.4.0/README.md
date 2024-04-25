# Comparing `tmp/wagtail_bynder-0.3.0.tar.gz` & `tmp/wagtail_bynder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_bynder-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtail_bynder-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtail_bynder-0.3.0.tar` & `wagtail_bynder-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2643 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1495 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/LICENSE
--rw-r--r--   0        0        0    13052 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/README.md
--rw-r--r--   0        0        0     1836 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      916 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/__init__.py
--rw-r--r--   0        0        0       22 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/__version__.py
--rw-r--r--   0        0        0      149 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/apps.py
--rw-r--r--   0        0        0      516 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/blocks.py
--rw-r--r--   0        0        0      161 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/exceptions.py
--rw-r--r--   0        0        0     9277 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/base.py
--rw-r--r--   0        0        0      336 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_documents.py
--rw-r--r--   0        0        0      324 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_images.py
--rw-r--r--   0        0        0      325 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_videos.py
--rw-r--r--   0        0        0      400 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_documents.py
--rw-r--r--   0        0        0     1033 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_images.py
--rw-r--r--   0        0        0      386 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_videos.py
--rw-r--r--   0        0        0     1791 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/middleware.py
--rw-r--r--   0        0        0    15692 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/models.py
--rw-r--r--   0        0        0   976618 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js
--rw-r--r--   0        0        0     1190 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js
--rw-r--r--   0        0        0     1289 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js
--rw-r--r--   0        0        0      171 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser.js
--rw-r--r--   0        0        0     2563 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js
--rw-r--r--   0        0        0     1214 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js
--rw-r--r--   0        0        0     1190 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js
--rw-r--r--   0        0        0      532 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html
--rw-r--r--   0        0        0      515 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html
--rw-r--r--   0        0        0        0 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templatetags/__init__.py
--rw-r--r--   0        0        0      311 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templatetags/bynder_tags.py
--rw-r--r--   0        0        0     1971 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/__init__.py
--rw-r--r--   0        0        0     2472 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/document.py
--rw-r--r--   0        0        0     2372 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/image.py
--rw-r--r--   0        0        0     1845 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/mixins.py
--rw-r--r--   0        0        0     2186 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/video.py
--rw-r--r--   0        0        0     2333 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/wagtail_hooks.py
--rw-r--r--   0        0        0     1535 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/widgets.py
--rw-r--r--   0        0        0    14663 1970-01-01 00:00:00.000000 wagtail_bynder-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2643 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1495 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/LICENSE
+-rw-r--r--   0        0        0    13052 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/README.md
+-rw-r--r--   0        0        0     1835 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      916 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/__version__.py
+-rw-r--r--   0        0        0      149 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/apps.py
+-rw-r--r--   0        0        0      516 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/blocks.py
+-rw-r--r--   0        0        0      161 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/exceptions.py
+-rw-r--r--   0        0        0     9277 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/base.py
+-rw-r--r--   0        0        0      336 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/refresh_bynder_documents.py
+-rw-r--r--   0        0        0      324 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/refresh_bynder_images.py
+-rw-r--r--   0        0        0      325 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/refresh_bynder_videos.py
+-rw-r--r--   0        0        0      400 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/update_stale_documents.py
+-rw-r--r--   0        0        0     1033 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/update_stale_images.py
+-rw-r--r--   0        0        0      386 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/update_stale_videos.py
+-rw-r--r--   0        0        0     1791 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/middleware.py
+-rw-r--r--   0        0        0    17836 2024-04-25 15:27:17.828183 wagtail_bynder-0.4.0/src/wagtail_bynder/models.py
+-rw-r--r--   0        0        0   976618 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js
+-rw-r--r--   0        0        0     1190 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js
+-rw-r--r--   0        0        0     1289 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js
+-rw-r--r--   0        0        0      171 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/video-chooser.js
+-rw-r--r--   0        0        0     2563 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js
+-rw-r--r--   0        0        0     1214 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js
+-rw-r--r--   0        0        0     1190 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js
+-rw-r--r--   0        0        0      532 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html
+-rw-r--r--   0        0        0      515 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html
+-rw-r--r--   0        0        0        0 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/templatetags/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/templatetags/bynder_tags.py
+-rw-r--r--   0        0        0     1971 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/utils.py
+-rw-r--r--   0        0        0        0 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/views/__init__.py
+-rw-r--r--   0        0        0     2472 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/views/document.py
+-rw-r--r--   0        0        0     2372 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/views/image.py
+-rw-r--r--   0        0        0     1845 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/views/mixins.py
+-rw-r--r--   0        0        0     2186 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/views/video.py
+-rw-r--r--   0        0        0     2333 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/wagtail_hooks.py
+-rw-r--r--   0        0        0     1535 2024-04-25 15:27:17.836182 wagtail_bynder-0.4.0/src/wagtail_bynder/widgets.py
+-rw-r--r--   0        0        0    14662 1970-01-01 00:00:00.000000 wagtail_bynder-0.4.0/PKG-INFO
```

### Comparing `wagtail_bynder-0.3.0/CONTRIBUTING.md` & `wagtail_bynder-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/LICENSE` & `wagtail_bynder-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/README.md` & `wagtail_bynder-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/pyproject.toml` & `wagtail_bynder-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -15,27 +15,27 @@
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Framework :: Django",
-    "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Framework :: Wagtail",
     "Framework :: Wagtail :: 4",
     "Framework :: Wagtail :: 5",
+    "Framework :: Wagtail :: 6",
 ]
 
 dynamic = ["version"]
 requires-python = ">=3.11"
 dependencies = [
-    "Django>=3.2",
-    "Wagtail>=4.1",
+    "Django>=4.2",
+    "Wagtail>=5.2",
     "bynder-sdk>=1.1.5,<2.0"
 ]
 
 [project.optional-dependencies]
 testing = [
     "dj-database-url>=2.1.0,<3.0",
     "wagtail_factories>=4.1.0,<5.0",
```

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/__init__.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/blocks.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/base.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_images.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/management/commands/update_stale_images.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/middleware.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/middleware.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/models.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,18 +91,23 @@
             or self.bynder_last_modified
             >= datetime.fromisoformat(asset_data["dateModified"])
         )
 
     def update_from_asset_data(
         self,
         asset_data: dict[str, Any],
+        **kwargs,
     ) -> None:
         """
         Update this object (without saving) to reflect values in `asset_data`,
         which is a representation of the related asset from the Bynder API.
+
+        NOTE: Although this base implementation does nothing with them currently,
+        for compatibility reasons, ``**kwargs`` should always be accepted by all
+        implementations of this method.
         """
         self.title = asset_data.get("name", self.title)
         self.copyright = asset_data.get("copyright", self.copyright)
         self.description = asset_data.get("description", self.description)
         self.collection = self.get_target_collection(asset_data)
         self.bynder_last_modified = asset_data["dateModified"]
         self.is_archived = bool(asset_data.get("archive", 0))
@@ -122,17 +127,25 @@
     class Meta:
         abstract = True
 
     @staticmethod
     def extract_file_source(asset_data: dict[str, Any]) -> str:
         raise NotImplementedError
 
-    def update_from_asset_data(self, asset_data: dict[str, Any]) -> None:
-        super().update_from_asset_data(asset_data)
-        if not self.file or self.asset_file_has_changed(asset_data):
+    def update_from_asset_data(
+        self, asset_data: dict[str, Any], *, force_download: bool = False, **kwargs
+    ) -> None:
+        """
+        Overrides ``BynderAssetMixin.update_from_asset_data()`` to explicitly
+        handle the ``force_download`` option that can be provided by management
+        commands, and to initiate downloading of the source file when it has
+        changed in some way.
+        """
+        super().update_from_asset_data(asset_data, **kwargs)
+        if force_download or not self.file or self.asset_file_has_changed(asset_data):
             self.update_file(asset_data)
 
     def asset_file_has_changed(self, asset_data: dict[str, Any]) -> bool:
         source_url = self.extract_file_source(asset_data)
         filename = utils.filename_from_url(source_url)
         return (
             self.source_filename != filename
@@ -170,32 +183,52 @@
 
     class Meta(AbstractImage.Meta):
         abstract = True
 
     def save(self, *args, **kwargs):
         if getattr(self, "_file_changed", False):
             self._set_image_file_metadata()
+        if self.pk and (
+            getattr(self, "_file_changed", False)
+            or getattr(self, "_focal_point_changed", False)
+        ):
+            # wagtail.images.forms.BaseImageForm usually takes care of this when
+            # updating via the UI. But, if updating objects directly, we must
+            # delete stale renditions ourselves.
+            self.renditions.all().delete()
         super().save(*args, **kwargs)
 
     def update_from_asset_data(
-        self,
-        asset_data: dict[str, Any],
+        self, asset_data: dict[str, Any], *, force_download: bool = False, **kwargs
     ) -> None:
+        """
+        Overrides ``BynderAssetWithFileMixin.update_from_asset_data()`` to
+        handle conversion of focal points to focal areas.
+        """
+
         # Update the file and other field values without saving the changes
-        super().update_from_asset_data(asset_data)
+        super().update_from_asset_data(
+            asset_data, force_download=force_download, **kwargs
+        )
 
         # Update the focal area if a focus point is set
+        current_focal_point = self.get_focal_point()
+        self._focal_point_changed = False
         focus_point = asset_data.get("activeOriginalFocusPoint")
         if focus_point:
             self.set_focal_area_from_focus_point(
                 int(focus_point["x"]),
                 int(focus_point["y"]),
                 int(asset_data["height"]),
                 int(asset_data["width"]),
             )
+            self._focal_point_changed = (
+                current_focal_point is None
+                or self.get_focal_point() != current_focal_point
+            )
 
     def asset_file_has_changed(self, asset_data: dict[str, Any]) -> bool:
         return (
             super().asset_file_has_changed(asset_data)
             or (self.original_height or 0) != int(asset_data["height"])
             or (self.original_width or 0) != int(asset_data["width"])
         )
@@ -205,15 +238,15 @@
         self.original_height = int(asset_data["height"])
         return super().update_file(asset_data)
 
     def set_focal_area_from_focus_point(
         self, x: int, y: int, original_height: int, original_width: int
     ) -> None:
         """
-        Using the provided center-point coordinates, generate a
+        Using the provided focus point coordinates, generate a
         2D focal area for the downloaded image.
         """
         if x < 0 or y < 0 or x > original_width or y > original_height:
             raise ValueError(
                 "Focus point coordinates must be inside the original image bounds"
             )
 
@@ -224,19 +257,29 @@
             x = math.floor(x / scale)
             y = math.floor(y / scale)
 
         # Set the centre point
         self.focal_point_x = x
         self.focal_point_y = y
 
+        # Draw a rectangle around the centre point
         # For the width, span outwards until we hit the left or right bounds
-        self.focal_point_width = min(x, self.width - x) * 2
+        rect_width = min(x, self.width - x) * 2
+        # Restrict rectangle width to 40% of the image height
+        rect_width = min(rect_width, math.floor(self.width * 0.4))
 
         # For the height, span outwards until we hit the top or bottom bounds
-        self.focal_point_height = min(y, self.height - y) * 2
+        rect_height = min(y, self.height - y) * 2
+        # Restrict rectangle height to 40% of the image height
+        rect_height = min(rect_height, math.floor(self.height * 0.4))
+
+        # Use the shortest side to make a square
+        width = min(rect_width, rect_height)
+        self.focal_point_width = width
+        self.focal_point_height = width
 
     @staticmethod
     def extract_file_source(asset_data: dict[str, Any]) -> str:
         # For images, we store and use the source derivative filename,
         # because the 'original' isn't always present
         asset_id = asset_data["id"]
         key = getattr(settings, "BYNDER_IMAGE_SOURCE_THUMBNAIL_NAME", "WagtailSource")
@@ -370,15 +413,21 @@
         if not self.fallback_source_url:
             return ""
         return guess_type(self.fallback_source_url)[0]
 
     def update_from_asset_data(
         self,
         asset_data: dict[str, Any],
+        **kwargs,
     ) -> None:
+        """
+        Overrides ``BynderAssetMixin.update_from_asset_data()`` to handle
+        setting of video-specific field values.
+        """
+
         primary_derivative_name = getattr(
             settings, "BYNDER_VIDEO_PRIMARY_DERIVATIVE_NAME", "WebPrimary"
         )
         fallback_derivative_name = getattr(
             settings, "BYNDER_VIDEO_FALLBACK_DERIVATIVE_NAME", "WebFallback"
         )
         poster_image_derivative_name = getattr(
@@ -413,8 +462,8 @@
                 f"for this asset are: {list(thumbnails.keys())}"
             ) from e
 
         self.original_filesize = int(asset_data["fileSize"])
         self.original_width = int(asset_data["width"])
         self.original_height = int(asset_data["height"])
 
-        super().update_from_asset_data(asset_data)
+        super().update_from_asset_data(asset_data, **kwargs)
```

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js` & `wagtail_bynder-0.4.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html` & `wagtail_bynder-0.4.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html` & `wagtail_bynder-0.4.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/utils.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/views/document.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/views/document.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/views/image.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/views/image.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/views/mixins.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/views/video.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/views/video.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/wagtail_hooks.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/src/wagtail_bynder/widgets.py` & `wagtail_bynder-0.4.0/src/wagtail_bynder/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.3.0/PKG-INFO` & `wagtail_bynder-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-bynder
-Version: 0.3.0
+Version: 0.4.0
 Summary: Wagtail integration with Bynder, a Digital Asset Management System
 Keywords: Wagtail,Django,Bynder,DAMS,digital asset management
 Author-email: Andy Babic  <andy.babic@torchbox.com>
 Maintainer-email: Andy Babic <andy.babic@torchbox.com>, Dan Braghis <dan.braghis@torchbox.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -12,22 +12,22 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0
 Classifier: Framework :: Wagtail
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
-Requires-Dist: Django>=3.2
-Requires-Dist: Wagtail>=4.1
+Classifier: Framework :: Wagtail :: 6
+Requires-Dist: Django>=4.2
+Requires-Dist: Wagtail>=5.2
 Requires-Dist: bynder-sdk>=1.1.5,<2.0
 Requires-Dist: dj-database-url>=2.1.0,<3.0 ; extra == "testing"
 Requires-Dist: wagtail_factories>=4.1.0,<5.0 ; extra == "testing"
 Requires-Dist: responses>=0.24,<1 ; extra == "testing"
 Requires-Dist: coverage>=7.0,<8.0 ; extra == "testing"
 Requires-Dist: freezegun>=1.1,<2 ; extra == "testing"
 Project-URL: Changelog, https://github.com/torchbox/wagtail-bynder/blob/main/CHANGELOG.md
```

