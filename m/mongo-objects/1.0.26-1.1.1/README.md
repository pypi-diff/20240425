# Comparing `tmp/mongo_objects-1.0.26.tar.gz` & `tmp/mongo_objects-1.1.1.tar.gz`

## Comparing `mongo_objects-1.0.26.tar` & `mongo_objects-1.1.1.tar`

### file list

```diff
@@ -1,23 +1,32 @@
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/requirements.txt
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/docs/source/conf.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/docs/source/index.rst
--rw-r--r--   0        0        0    30788 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/conftest.py
--rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_proxy_combo.py
--rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/buildProject
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/runTests
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/setupPythonVenv
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/updateRequirements
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/.hgignore
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/README.rst
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/pyproject.toml
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/PKG-INFO
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoDictProxy.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoListProxy.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoSingleProxy.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/MongoUserDict.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/customization.rst
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/quickstart.rst
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/docs/source/sample.rst
+-rw-r--r--   0        0        0    33028 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/src/mongo_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    41395 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tests/test_proxy_combo.py
+-rwxr-xr-x   0        0        0     1326 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/buildProject
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/runTests
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/setupPythonVenv
+-rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/tools/updateRequirements
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/README.rst
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 mongo_objects-1.1.1/PKG-INFO
```

### Comparing `mongo_objects-1.0.26/requirements.txt` & `mongo_objects-1.1.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 alabaster==0.7.16
 attrs==23.2.0
 Babel==2.14.0
-backports.tarfile==1.1.0
+backports.tarfile==1.1.1
 build==1.2.1
 cattrs==23.2.3
 certifi==2024.2.2
 charset-normalizer==3.3.2
 dnspython==2.6.1
-docutils==0.21.1
+docutils==0.21.2
 esbonio==0.16.4
 idna==3.7
 imagesize==1.4.1
 importlib_metadata==7.1.0
 iniconfig==2.0.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
@@ -22,32 +22,34 @@
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mdurl==0.1.2
 more-itertools==10.2.0
 nh3==0.2.17
 packaging==24.0
 pkginfo==1.10.0
-platformdirs==4.2.0
-pluggy==1.4.0
+platformdirs==4.2.1
+pluggy==1.5.0
 pygls==1.3.1
 Pygments==2.17.2
-pymongo==4.6.3
+pymongo==4.7.0
 pyproject_hooks==1.0.0
 PySocks==1.7.1
 pyspellchecker==0.8.1
 pytest==8.1.1
 readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
+setuptools==69.5.1
 snowballstemmer==2.2.0
 Sphinx==7.3.7
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
 twine==5.0.0
 urllib3==2.2.1
+wheel==0.43.0
 zipp==3.18.1
```

### Comparing `mongo_objects-1.0.26/docs/source/conf.py` & `mongo_objects-1.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/src/mongo_objects.py` & `mongo_objects-1.1.1/src/mongo_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
 class MongoUserDict( UserDict ):
     # Subclasses can provide a collection name and a MongoDb database connection
     # as a class attribute OR override collection() to return the correct collection object
     collection_name = None
     database = None
 
+    # If object_version is non-None, find() and find_one() by default restrict queries
+    # to documents with the current object_version
+    # This enables a type of schema versioning.
+    object_version = None
+
     # The character sequence used to separate the document ID from proxy subdocument keys
     # This may be overriden but it is the user's responsibility to guarantee that this
     # sequence will never appear in any ID or subdoc key.
     # Since the default IDs and subdoc keys are hex, 'g' is a safe separator
     subdoc_key_sep = 'g'
 
 
@@ -58,14 +63,35 @@
         self.readonly = readonly
 
         # Authorize creating this object prior to returning to the user
         if not self.authorize_init():
             raise MongoObjectAuthFailed
 
 
+    @classmethod
+    def add_object_version_filter( cls, filter, object_version ):
+        '''Implement automatic object version filtering for find() and find_one()
+        The command-line object-version affects if and how to implement
+        object version filtering.'''
+        if cls.object_version is not None:
+            # False suppresses automatic object_version filtering
+            if object_version is False:
+                pass
+            # None (the default) filters the query to the current class object version
+            elif object_version is None:
+                filter = dict(filter)
+                filter['_objver'] = cls.object_version
+
+            # Any other value filters object version to that value
+            else:
+                filter = dict(filter)
+                filter['_objver'] = object_version
+        return filter
+
+
     # Authorization hooks()
     # The user may call these hooks to authorize various CRUD operations
     def authorize_init( self ):
         '''Called after the document object is initialized but
         before it is returned to the user.
         If the return value is not truthy, an exception is raised.'''
         return True
@@ -115,40 +141,51 @@
             if not self.authorize_delete():
                 raise MongoObjectAuthFailed
             self.collection().find_one_and_delete( { '_id' : ObjectId( self['_id'] ) } )
             del self['_id']
 
 
     @classmethod
-    def find( cls, filter={}, projection=None, readonly=False, **kwargs ):
+    def find( cls, filter={}, projection=None, readonly=None, object_version=None, **kwargs ):
         '''Return matching documents as instances of this class'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
-        # if a projection is provided, force the resulting object to be read-only
-        readonly = readonly or projection is not None
+        # if readonly is None, by default force queries with a projection to be read-only
+        # otherwise, accept the (presumably boolean) value provided by the user
+        if readonly is None:
+            readonly = projection is not None
+
+        # automatically filter by object version if requested
+        if cls.object_version is not None:
+            filter = cls.add_object_version_filter( filter, object_version )
 
         for doc in cls.collection().find( filter, projection, **kwargs ):
-            print( "STEP 4" )
             obj = cls(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, no_match=None, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=None, object_version=None, no_match=None, **kwargs ):
         '''Return a single matching document as an instance of this class or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
-        # if a projection is provided, force the resulting object to be read-only
-        readonly = readonly or projection is not None
+        # if readonly is None, by default force queries with a projection to be read-only
+        # otherwise, accept the (presumably boolean) value provided by the user
+        if readonly is None:
+            readonly = projection is not None
+
+        # automatically filter by object version if requested
+        if cls.object_version is not None:
+            filter = cls.add_object_version_filter( filter, object_version )
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
             obj = cls(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 return obj
@@ -223,61 +260,74 @@
         1) Documents without an _id are inserted into the database; MongoDB will assign the ID
         2) If force is set, document will be saved regardless of update time or even if it exists.
            This is useful for upserting document from another database.
         3) Otherwise, only a document with this _id and _updated timestamp will be replaced.
            This protects against overwriting documents that have been updated elsewhere.
         '''
 
+        # internal class to note if a metadata field has added and had no original value
+        class NewFieldAdded( object ):
+            pass
+
         # authorize saving this document
         if not self.authorize_save():
             raise MongoObjectAuthFailed
 
         # refuse to save a read-only document
         if self.readonly:
             raise MongoObjectReadOnly( f"Can't save readonly object {type(self)} at {id(self)}" )
 
+        # Use a dictionary to record original metadata in case they need to be rolled back
+        # These metadata values should never be None, so during rollback we remove any values
+        # for which get() returned None.
+        original_metadata = {}
+
         # set updated timestamp
-        # Note the original value in case we need to roll back
-        added_updated = '_updated' not in self
-        original_updated = self.get('_updated')
+        original_metadata['_updated'] = self.get('_updated')
         self['_updated'] = self.utcnow()
 
         # add created timestamp if it doesn't exist
-        # set flag in case we need to roll back
-        added_created = '_created' not in self
-        self.setdefault( '_created', self['_updated'] )
+        if '_created' not in self:
+            original_metadata['_created'] = None
+            self['_created'] = self['_updated']
+
+        # add object version if provided
+        if self.object_version is not None:
+            original_metadata['_objver'] = self.get('_objver')
+            self['_objver'] = self.object_version
 
         try:
             # if the document has never been written to the database, write it now and record the ID
             if '_id' not in self:
                 result = self.collection().insert_one( self.data )
                 self['_id'] = result.inserted_id
 
             # Force-save a document regardless of timestamp
             elif force:
                 result = self.collection().replace_one( { '_id' : self['_id'] }, self.data, upsert=True )
 
             # Otherwise, only update a document with the same updated timestamp as our in-memory object
             else:
                 result = self.collection().find_one_and_replace(
-                    { '_id' : self['_id'], '_updated' : original_updated },
+                    { '_id' : self['_id'], '_updated' : original_metadata['_updated'] },
                     self.data,
                     return_document=ReturnDocument.AFTER )
 
                 # on failure, we assume the document has been updated elsewhere and raise an exception
                 assert result is not None, f"document {self.id()} already updated"
 
-        # on any error roll back _updated and _created to the original value or remove if we added them
+        # on any error roll back to the original metadata
         except Exception as e:
-            if added_created:
-                del self['_created']
-            if added_updated:
-                del self['_updated']
-            else:
-                self['_updated'] = original_updated
+            for (k, v) in original_metadata.items():
+                # If the original value is None, assume we added the field and should remove it
+                if v is None:
+                    del self[k]
+                # Otherwise, restore the original value
+                else:
+                    self[k] = v
             raise(e)
 
 
     @classmethod
     def split_id( cls, subdoc_id ):
         '''Split a subdocument ID into its component document ID and one or more subdocument keys.'''
         return subdoc_id.split( cls.subdoc_key_sep )
@@ -320,15 +370,15 @@
                 assert cls.subclass_key not in cls.subclass_map, f"duplicate subclass_key for {type(cls)}"
                 cls.subclass_map[ cls.subclass_key ] = cls
         except Exception as e:
             raise Exception( 'PolymorphicMongoUserDict(): unable to register subclass' ) from e
 
 
     @classmethod
-    def find( cls, filter={}, projection=None, readonly=False, **kwargs ):
+    def find( cls, filter={}, projection=None, readonly=None, **kwargs ):
         '''Return matching documents as appropriate subclass instances'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
@@ -337,15 +387,15 @@
             obj = cls.instantiate(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, no_match=None, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=None, no_match=None, **kwargs ):
         '''Return a single matching document as the appropriate subclass or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
```

### Comparing `mongo_objects-1.0.26/tests/test_MongoDictProxy.py` & `mongo_objects-1.1.1/tests/test_MongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_MongoListProxy.py` & `mongo_objects-1.1.1/tests/test_MongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_MongoSingleProxy.py` & `mongo_objects-1.1.1/tests/test_MongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_MongoUserDict.py` & `mongo_objects-1.1.1/tests/test_MongoUserDict.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,14 +50,185 @@
     for x in sampleData:
         obj = MMUD(x)
         obj.save()
     return MMUD
 
 
 
+@pytest.fixture( scope='class' )
+def getVersionedPopulatedMMUDClass( getMMUDClass, sampleData ):
+    '''Like getPopulatedMMUDClass except each document is saved
+    with a different version number.
+
+    MMUD is left with the final object version number.'''
+
+    MMUD = getMMUDClass
+
+    # for each entry in the sampleData, save it to the collection configured in MMUD
+    for (ver, x) in enumerate( sampleData ):
+        MMUD.object_version = ver+1
+        obj = MMUD(x)
+        obj.save()
+    return MMUD
+
+
+
+class TestVersioning:
+    '''Test how various function perform with object versioning'''
+
+    def test_find_all_current_version( self, getVersionedPopulatedMMUDClass ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # There should only be one document at the current version (the default query)
+        result = list( MMUD.find() )
+        assert len( result ) == 1
+        assert result[0]['_objver'] == MMUD.object_version
+
+
+    def test_find_all_specified_version( self, getVersionedPopulatedMMUDClass ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # There should only be one document at version 1
+        result = list( MMUD.find( object_version=1 ) )
+        assert len( result ) == 1
+        assert result[0]['_objver'] == 1
+
+
+    def test_find_all_versioning_suppressed( self, getVersionedPopulatedMMUDClass, sampleData ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # All documents should be returned if object versioning is suppressed
+        result = list( MMUD.find( object_version=False ) )
+        assert len( result ) == len( sampleData )
+
+
+    def test_find_all_nonexistent_version( self, getVersionedPopulatedMMUDClass ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # Nothing should be returned at a non-existent version
+        result = list( MMUD.find( object_version=10000000 ) )
+        assert len( result ) == 0
+
+
+    def test_find_one_current_version( self, getVersionedPopulatedMMUDClass, sampleData ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # There should only be one document at the current version (the default query)
+        matches = 0
+        for doc in sampleData:
+            filter = dict( doc )
+            result = MMUD.find_one( filter )
+            if result is not None:
+                assert result['_objver'] == MMUD.object_version
+                matches += 1
+
+        assert matches == 1
+
+
+    def test_find_one_specified_version( self, getVersionedPopulatedMMUDClass, sampleData ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # There should only be one document at version 1
+        matches = 0
+        for doc in sampleData:
+            filter = dict( doc )
+            result = MMUD.find_one( filter, object_version=1 )
+            if result is not None:
+                assert result['_objver'] == 1
+                matches += 1
+
+        assert matches == 1
+
+
+    def test_find_one_versioning_suppressed( self, getVersionedPopulatedMMUDClass, sampleData ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # Any document may be returned if object versioning is suppressed
+        for doc in sampleData:
+            filter = dict( doc )
+            assert MMUD.find_one( filter, object_version=False ) is not None
+
+
+    def test_find_one_nonexistent_version( self, getVersionedPopulatedMMUDClass, sampleData ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # None should be returned at a non-existent version for any document
+        for doc in sampleData:
+            filter = dict( doc )
+            assert MMUD.find_one( filter, object_version=10000000 ) is None
+
+
+
+class TestVersionedSave:
+
+    def test_save_version( self, getVersionedPopulatedMMUDClass ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # Create an empty object
+        obj = MMUD( {} )
+        assert '_objver' not in obj
+
+        # save the object and verify the version was added to the document
+        obj.save()
+        assert obj['_objver'] == MMUD.object_version
+
+        # load the data from the database and check the version
+        obj2 = MMUD.load_by_id( obj.id() )
+        assert obj2['_objver'] == MMUD.object_version
+
+
+
+class TestVersionedSaveException:
+
+    def test_save_version_exception( self, getVersionedPopulatedMMUDClass ):
+        MMUD = getVersionedPopulatedMMUDClass
+
+        # verify there is a current object version
+        assert MMUD.object_version is not None
+
+        # Create an invalid object; BSON dictionary keys must be strings
+        obj = MMUD( { 1 : "not valid BSON"} )
+        assert '_objver' not in obj
+
+        # saving the object will raise an exceptionsave the object and verify the version was added to the document
+        with pytest.raises( Exception ):
+            obj.save()
+
+        # verify that the object version was removed during rollback
+        assert '_objver' not in obj
+
+
+
 class TestSave:
     '''Test various permutations of MongoUserDict.save()
     Other functionality is tested in a separate class'''
 
     def test_save( self, getMMUDClass, sampleData ):
         '''Verify a basic dictionary is saved properly.
         Confirm original object is updated with time and ID
@@ -108,39 +279,41 @@
         # make sure the database object as the exact same data as the in-memory object
         assert len( set( obj.keys() ).symmetric_difference( doc.keys() ) ) == 0, "missing keys"
         for key in obj.keys():
             assert doc[key] == obj[key]
 
 
     def test_save_exception_1( self, getMMUDClass ):
-        '''Test that an exception saving a new document removes _created and _updated timestamps'''
+        '''Test that an exception saving a new document removes _created, _updated timestamps'''
         MMUD = getMMUDClass
 
         # count documents
         count =  MMUD.collection().count_documents( {} )
 
         # Create an empty document
         obj = MMUD()
         assert '_created' not in obj
         assert '_updated' not in obj
+        assert '_objver' not in obj
 
         # Create an exception
         # MongoDB keys must be strings, so use an integer to create the exception
         obj[1] = "This document can't be saved."
 
         # Raise the exception
         with pytest.raises( Exception ):
             obj.save()
 
         # verify that nothing was saved
         assert MMUD.collection().count_documents( {} ) == count
 
-        # verify that _created and _updated were removed
+        # verify that _created and _updated were removed; _objver won't have been added anyway
         assert '_created' not in obj
         assert '_updated' not in obj
+        assert '_objver' not in obj
 
 
     def test_save_exception_2( self, getMMUDClass ):
         '''Test that an exception saving a previously saved document leaves the _updated timestamp unchanged'''
         MMUD = getMMUDClass
 
         # count documents
@@ -395,29 +568,87 @@
                 return False
 
         # verify initializing a document without authorization produces an exception
         with pytest.raises( mongo_objects.MongoObjectAuthFailed ):
             obj = LocalMMUD( sampleData[0] )
 
 
+    def test_add_object_version( self ):
+        '''Verify add_object_version adds the correct filter
+        The original filter should be left intact.'''
+        class LocalClass( mongo_objects.MongoUserDict ):
+            object_version = 5
+
+        # object_version = False never adds a filter
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, False )
+        assert len(filter) == 0
+        assert len(result) == 0
+
+        # object_version = None adds a filter for the current object version
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, None )
+        assert len(filter) == 0
+        assert result == { '_objver' : 5 }
+
+        # object_version = Value adds a filter for the current value
+        # With no class object version, nothing will happen
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, 10 )
+        assert len(filter) == 0
+        assert result == { '_objver' : 10 }
+
+
+    def test_add_object_version_empty( self ):
+        '''Verify add_object_version() if the class has no object version
+        Since the class has no object version, no filter should be
+        added under any circumstances'''
+        class LocalClass( mongo_objects.MongoUserDict ):
+            pass
+
+        # object_version = False never adds a filter
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, False )
+        assert len(filter) == 0
+        assert len(result) == 0
+
+        # object_version = None adds a filter for the current object version
+        # With no class object version, nothing will happen
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, None )
+        assert len(filter) == 0
+        assert len(result) == 0
+
+        # object_version = Value adds a filter for the current value
+        # With no class object version, nothing will happen
+        filter = {}
+        result = LocalClass.add_object_version_filter( filter, 10 )
+        assert len(filter) == 0
+        assert len(result) == 0
+
+
     def test_collection( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
         assert isinstance( MMUD.collection(), Collection )
 
 
     def test_find_all( self, getPopulatedMMUDClass, sampleData ):
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = list( MMUD.find() )
 
         # verify that we found all the entries
         assert len( result ) == len( sampleData )
         assert len( result ) == MMUD.collection().count_documents( {} )
 
         # verify type and data present
-        # since no projection was used and readonly wasn't provided,
+        # since no projection was used and readonly wasn't True,
         # verify object is not marked readonly
         for x in result:
             assert isinstance( x, MMUD )
             assert '_id' in x
             assert '_created' in x
             assert '_updated' in x
             assert 'name' in x
@@ -430,91 +661,137 @@
             set( [ x['name'] for x in result] ).symmetric_difference(
                  [ y['name'] for y in sampleData ] )
             ) == 0
 
 
     def test_find_none( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = list( MMUD.find( { 'not-a-field' : 'wont-match-anything' } ) )
 
         # verify that we found nothing
         assert len( result ) == 0
 
 
     def test_find_single( self, getPopulatedMMUDClass, sampleData ):
         '''Use a filter to find a single record, in this case, the first sample by name'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = list( MMUD.find( { 'name' : sampleData[0]['name'] } ) )
 
         # verify that we found a single entry
         assert len( result ) == 1
 
-        # since no projection was used and readonly wasn't provided,
+        # since no projection was used and readonly wasn't True,
         # verify object is not marked readonly
         assert result[0].readonly is False
 
 
     def test_find_projection_1( self, getPopulatedMMUDClass ):
         '''Test find() with a "positive" projection'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         for x in MMUD.find( {}, { 'amount' : True } ):
             assert '_id' in x
             assert '_created' not in x
             assert '_updated' not in x
             assert 'amount' in x
             assert 'name' not in x
             assert x.readonly is True
 
 
     def test_find_projection_2( self, getPopulatedMMUDClass ):
         '''Test find() with a "positive" projection but suppress _id'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         for x in MMUD.find( {}, { '_id' : False, 'name' : True } ):
             assert '_id' not in x
             assert '_created' not in x
             assert '_updated' not in x
             assert 'amount' not in x
             assert 'name' in x
             assert x.readonly is True
 
 
     def test_find_projection_3( self, getPopulatedMMUDClass ):
         '''Test find() with a "negative" projection'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         for x in MMUD.find( {}, { 'amount' : False } ):
             assert '_id' in x
             assert '_created' in x
             assert '_updated' in x
             assert 'amount' not in x
             assert 'name' in x
             assert x.readonly is True
 
 
     def test_find_projection_4( self, getPopulatedMMUDClass ):
         '''Test find() with a "negative" projection and suppress _id'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         for x in MMUD.find( {}, { '_id' : False, 'name' : False } ):
             assert '_id' not in x
             assert '_created' in x
             assert '_updated' in x
             assert 'amount' in x
             assert 'name' not in x
             assert x.readonly is True
 
 
+    def test_find_projection_5( self, getPopulatedMMUDClass ):
+        '''Test find() with a "negative" projection with readonly forced to False'''
+        MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
+        # Verify projection produced the proper key set
+        # Also confirm object is not marked readonly
+        for x in MMUD.find( {}, { '_id' : False, 'name' : False }, readonly=False ):
+            assert '_id' not in x
+            assert '_created' in x
+            assert '_updated' in x
+            assert 'amount' in x
+            assert 'name' not in x
+            assert x.readonly is False
+
+
     def test_find_readonly( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = list( MMUD.find( readonly=True ) )
 
         # verify all objects are marked readonly
         for x in result:
             assert x.readonly is True
 
 
@@ -561,110 +838,159 @@
         assert len( diff ) == 1
         assert diff[0] == ids[0]
 
 
     def test_find_one( self, getPopulatedMMUDClass ):
         '''Test returning a single (random) object'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = MMUD.find_one()
         assert isinstance( result, MMUD )
         assert '_id' in result
         assert '_created' in result
         assert '_updated' in result
         assert 'amount' in result
         assert 'name' in result
         assert result.readonly is False
 
 
     def test_find_one_none( self, getPopulatedMMUDClass ):
         '''Verify a non-matching filter produces a None result'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' } )
 
         # verify that we found nothing
         assert result is None
 
 
     def test_find_one_none_custom_return( self, getPopulatedMMUDClass ):
         '''Verify a non-matching filter produces our custom "no_match" result'''
         MMUD = getPopulatedMMUDClass
 
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         class EmptyResponse( object ):
             pass
 
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' }, no_match=EmptyResponse() )
 
         assert isinstance( result, EmptyResponse )
 
 
     def test_find_one_filter( self, getPopulatedMMUDClass, sampleData ):
         '''Use a filter to find a specific single record, in this case, the third sample by name'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         result = MMUD.find_one( { 'name' : sampleData[2]['name'] } )
 
         # verify that we found the right record
         assert result['name'] == sampleData[2]['name']
 
 
     def test_find_one_projection_1( self, getPopulatedMMUDClass ):
         '''Test find() with a "positive" projection'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         result = MMUD.find_one( {}, { 'amount' : True } )
         assert '_id' in result
         assert '_created' not in result
         assert '_updated' not in result
         assert 'amount' in result
         assert 'name' not in result
         assert result.readonly is True
 
 
     def test_find_one_projection_2( self, getPopulatedMMUDClass ):
         '''Test find() with a "positive" projection but suppress _id'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         result = MMUD.find_one( {}, { '_id' : False, 'name' : True } )
         assert '_id' not in result
         assert '_created' not in result
         assert '_updated' not in result
         assert 'amount' not in result
         assert 'name' in result
         assert result.readonly is True
 
 
     def test_find_one_projection_3( self, getPopulatedMMUDClass ):
         '''Test find() with a "negative" projection'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         result = MMUD.find_one( {}, { 'amount' : False } )
         assert '_id' in result
         assert '_created' in result
         assert '_updated' in result
         assert 'amount' not in result
         assert 'name' in result
         assert result.readonly is True
 
 
     def test_find_one_projection_4( self, getPopulatedMMUDClass ):
         '''Test find() with a "negative" projection and suppress _id'''
         MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
         # Verify projection produced the proper key set
         # Also confirm object is marked readonly
         result = MMUD.find_one( {}, { '_id' : False, 'name' : False } )
         assert '_id' not in result
         assert '_created' in result
         assert '_updated' in result
         assert 'amount' in result
         assert 'name' not in result
         assert result.readonly is True
 
 
+    def test_find_one_projection_5( self, getPopulatedMMUDClass ):
+        '''Test find() with a "negative" projection with readonly forced to False'''
+        MMUD = getPopulatedMMUDClass
+
+        # verify that this is an unversioned test
+        assert MMUD.object_version is None
+
+        # Verify projection produced the proper key set
+        # Also confirm object is not marked readonly
+        result = MMUD.find_one( {}, { '_id' : False, 'name' : False }, readonly=False )
+        assert '_id' not in result
+        assert '_created' in result
+        assert '_updated' in result
+        assert 'amount' in result
+        assert 'name' not in result
+        assert result.readonly is False
+
+
     def test_find_one_readonly( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
         result = MMUD.find_one( readonly=True )
 
         # verify object are marked readonly
         result.readonly is True
 
@@ -814,15 +1140,15 @@
         # id() is just the string version of the MongoDB _id value
         assert result.id() == str( result['_id'] )
 
 
     def test_id_new_object( self, getMMUDClass ):
         MMUD = getMMUDClass
 
-        # new object don't have an _id value yet
+        # new objects don't have an _id value yet
         # so id() will raise an exception
         obj = MMUD( {} )
         with pytest.raises( Exception ):
             obj.id()
 
 
     def test_load_by_id_bson( self, getPopulatedMMUDClass ):
```

### Comparing `mongo_objects-1.0.26/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.1.1/tests/test_PolymorphicMongoDictProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.1.1/tests/test_PolymorphicMongoListProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_PolymorphicMongoSingleProxy.py` & `mongo_objects-1.1.1/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_PolymorphicMongoUserDict.py` & `mongo_objects-1.1.1/tests/test_PolymorphicMongoUserDict.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tests/test_proxy_combo.py` & `mongo_objects-1.1.1/tests/test_proxy_combo.py`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tools/buildProject` & `mongo_objects-1.1.1/tools/buildProject`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,40 @@
 PROJECT_DIR=$(pwd)
 
 # activate the project virtual environment
 source ${PROJECT_DIR}/venv/bin/activate
 echo "activating virtual environment"
 
 # make sure there are no uncommitted changes
-if [[ $(hg status | wc -l ) -gt 0 ]]
+if [[ $(git status --porcelain | wc -l ) -gt 0 ]]
 then
 echo "Project contains uncommitted changes; aborting build"
-hg status
-#exit -1
+git status
+exit -1
 fi
 
-# upgrade all packages
-pip install --upgrade $(pip freeze | awk -F= '{print $1}')
+# verify that the current HEAD has a tag
+VERSION=$(git describe --abbrev=0 --exact-match)
+if [[ -z "${VERSION}" ]]
+then
+echo "No git tag found for HEAD"
+git log -n 1
+exit -1
+
+elif [[ "v${VERSION#v}" != "${VERSION}" ]]
+then
+echo "Tag ${VERSION} is not a version tag"
+exit -1
+fi
 
 # create version file
-echo "__version__ = \"1.0.$(hg log --rev tip --template '{rev}')\"" > src/__about__.py
+echo "__version__ = \"${VERSION}\"" > src/__about__.py
+
+# upgrade all packages
+pip install --upgrade $(pip freeze | awk -F= '{print $1}')
 
 # remove previous artifacts
 rm -rf ./dist 2> /dev/null
 
 # build project distribution
 if python3 -m build
 then
```

### Comparing `mongo_objects-1.0.26/tools/runTests` & `mongo_objects-1.1.1/tools/runTests`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/tools/setupPythonVenv` & `mongo_objects-1.1.1/tools/setupPythonVenv`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.26/README.rst` & `mongo_objects-1.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 
 Documents are returned as UserDict subclasses:
 
 * convenient pass-through to ``find()`` and ``find_one()``
 * convenient ``load_by_id()`` to locate documents by ObjectId
 * smart ``save()`` function to insert, upsert or replace documents as appropriate
 * automatically record document creation and update times
+* track separate object schema versions
 * support polymorphic user objects loaded from the same collection
 
 Subdocuments are accessed through dictionary proxy objects:
 
 * returned as their own classes independent of the parent MongoDB document class
 * data access is proxied back to the parent so no separate database access is performed
 * subdocuments have their own unique URL-safe ID useful for loading the data
 * subdocuments can be grouped in either dictionary or list containers
-* polymorphic subdocuments are supported within same container
-* using subdocuments avoids "JOIN-like" additional database queries
+* polymorphic subdocuments are supported within the same container
+* using subdocuments avoids "JOIN-like" additional database queries across collections
 
 
 Example
 =======
 
 Imagine an event ticketing system with a single MongoDB collection containing documents like the following::
 
@@ -63,15 +64,15 @@
 MongoUserDict
 -------------
 
 ``mongo_objects`` allows us to create our own class for viewing these event documents::
 
     class Event( mongo_objects.MongoUserDict ):
 
-        db = ...     # set your MongoDB database object here
+        db = ...     # provide your MongoDB database object here
         collection_name = 'events'
 
         def isFuture( self ):
             return self['date'] >= datetime.utcnow()
 
 Loop through all events::
 
@@ -138,7 +139,19 @@
         'name' : 'Student Ticket',
         'desc' : 'For our student friends',
         'cost' : 50,
         'quantity' : 25,
     } )
 
 
+Credits
+-------
+
+Development sponsored by `Headwaters Entrepreneurs Pte Ltd <https://headwaters.com.sg>`_.
+
+Originally developed by `Frontier Tech Team LLC <https://frontiertechteam.com>`_
+for the `Wasted Minutes <https://wasted-minutes.com>`_ ™️ language study tool.
+
+
+License
+-------
+mongo_objects is made available to the community under the "MIT License".
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mongo_objects-1.0.26/pyproject.toml` & `mongo_objects-1.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,28 +6,33 @@
 
 [project]
 name = "mongo_objects"
 authors = [
   { name="Jonathan Lindstrom", email="lindstrom.j@headwaters.com.sg" },
 ]
 classifiers = [
+    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pymongo",
 ]
 description = "Access MongoDB documents and subdocuments through user-defined UserDict and proxy objects."
 dynamic = ["version"]
+keywords = ["Mongo", "MongoDB", "pymongo"]
+license = {text = "MIT License"}
 readme = "README.rst"
 requires-python = ">=3.8"
 
 [project.urls]
-Homepage = "https://headwaters.com.sg/pycon-2023"
+Homepage = "https://github.com/lindstrom-j/mongo_objects"
+Documentation = "https://mongo-objects.headwaters.com.sg/en/latest/"
+Issues = "https://github.com/lindstrom-j/mongo_objects/issues"
 
 [tool.hatch.version]
 path = "src/__about__.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/mongo_objects.py"]
```

