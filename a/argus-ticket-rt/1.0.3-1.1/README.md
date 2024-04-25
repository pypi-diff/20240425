# Comparing `tmp/argus_ticket_rt-1.0.3-py3-none-any.whl.zip` & `tmp/argus_ticket_rt-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 4327 bytes, number of entries: 4
--rw-r--r--  2.0 unx     8060 b- defN 23-Mar-29 08:43 argus_ticket_rt.py
-?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     3991 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.0.3.dist-info/METADATA
-?rw-r--r--  2.0 unx      305 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.0.3.dist-info/RECORD
-4 files, 12437 bytes uncompressed, 3735 bytes compressed:  70.0%
+Zip file size: 4329 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     8160 b- defN 24-Apr-25 11:58 argus_ticket_rt.py
+-rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4072 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      299 b- defN 16-Jan-01 00:00 argus_ticket_rt-1.1.dist-info/RECORD
+4 files, 12612 bytes uncompressed, 3749 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
 Filename: argus_ticket_rt.py
 Comment: 
 
-Filename: argus_ticket_rt-1.0.3.dist-info/WHEEL
+Filename: argus_ticket_rt-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: argus_ticket_rt-1.0.3.dist-info/METADATA
+Filename: argus_ticket_rt-1.1.dist-info/METADATA
 Comment: 
 
-Filename: argus_ticket_rt-1.0.3.dist-info/RECORD
+Filename: argus_ticket_rt-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## argus_ticket_rt.py

```diff
@@ -15,15 +15,15 @@
     TicketPluginException,
     TicketSettingsException,
 )
 
 LOG = logging.getLogger(__name__)
 
 
-__version__ = "1.0.3"
+__version__ = "1.1"
 __all__ = [
     "RequestTrackerPlugin",
 ]
 
 
 class RequestTrackerPlugin(TicketPlugin):
     @classmethod
@@ -149,19 +149,21 @@
                 LOG.exception(permission_error)
                 raise TicketCreationException(permission_error)
             unexpected_error = (
                 f"Request Tracker: An unexpected response was encountered: {e.message}."
             )
             LOG.exception(unexpected_error)
             raise TicketCreationException(unexpected_error)
-
         except rt_exceptions.NotFoundError:
             queue_error = f"Request Tracker: No queue with the name {queue} can be found. Please check and update the setting 'TICKET_INFORMATION'."
             LOG.exception(queue_error)
             raise TicketSettingsException(queue_error)
+        except Exception as e:
+            LOG.exception(e)
+            raise TicketPluginException(e)
 
         custom_fields, missing_fields = cls.get_custom_fields(
             ticket_information=ticket_information,
             serialized_incident=serialized_incident,
         )
         body = cls.create_html_body(
             serialized_incident={
```

## Comparing `argus_ticket_rt-1.0.3.dist-info/METADATA` & `argus_ticket_rt-1.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: argus_ticket_rt
-Version: 1.0.3
+Version: 1.1
 Summary: Allow argus-server to create tickets in Request Tracker
 Author-email: Johanna England <johanna.england@sikt.no>
 Maintainer-email: Johanna England <johanna.england@sikt.no>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Dist: argus-server>=1.11
+Requires-Dist: argus-server>=1.15
 Requires-Dist: rt>=3.0
 Requires-Dist: tox ; extra == "test"
 Requires-Dist: coverage ; extra == "test"
 Project-URL: Home, https://github.com/Uninett/argus_ticket_rt
 Project-URL: Issues, https://github.com/Uninett/argus_ticket_rt/issues
 Provides-Extra: test
 
@@ -30,14 +30,15 @@
 This is a plugin to create tickets in Request Tracker from [Argus](https://github.com/Uninett/argus-server)
 
 The API supported is RT V2. RT 4.4 needs [RT::Extension::REST2](https://github.com/bestpractical/rt-extension-rest2)
 to support V2, while RT 5.0.0 and later has the support included.
 
 ## Settings
 
+* `TICKET_PLUGIN` must be set to `"argus_ticket_rt.RequestTrackerPlugin"`
 * `TICKET_ENDPOINT`: Link to instance, absolute URL
 * `TICKET_AUTHENTICATION_SECRET`: Standard username/password or token:
 
     ```
     {
         "username": username,
         "password": password
```

