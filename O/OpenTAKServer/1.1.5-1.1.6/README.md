# Comparing `tmp/opentakserver-1.1.5.tar.gz` & `tmp/opentakserver-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.5.tar", max compression
+gzip compressed data, was "opentakserver-1.1.6.tar", max compression
```

## Comparing `opentakserver-1.1.5.tar` & `opentakserver-1.1.6.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.5/LICENSE
--rw-r--r--   0        0        0      128 2024-04-21 21:15:38.770557 opentakserver-1.1.5/opentakserver/__init__.py
--rw-r--r--   0        0        0    11215 2024-04-21 19:26:51.392701 opentakserver-1.1.5/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.5/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    46981 2024-04-21 19:26:51.393698 opentakserver-1.1.5/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.5/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26684 2024-04-21 19:26:51.394711 opentakserver-1.1.5/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.5/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4580 2024-04-21 19:26:51.395692 opentakserver-1.1.5/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.5/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.5/opentakserver/ca_config.py
--rw-r--r--   0        0        0    21470 2024-04-21 21:10:51.114412 opentakserver-1.1.5/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.5/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10751 2024-04-21 19:26:51.397701 opentakserver-1.1.5/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34945 2024-04-21 19:26:51.398683 opentakserver-1.1.5/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     4114 2024-04-21 19:26:51.399789 opentakserver-1.1.5/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.5/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      393 2024-04-17 03:09:51.512546 opentakserver-1.1.5/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.5/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.5/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.5/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.5/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.5/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.5/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.5/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.5/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.5/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.5/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.5/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.5/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.5/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.5/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.5/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.5/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.5/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.5/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.5/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.5/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.5/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.5/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.5/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.5/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.5/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.5/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.5/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.5/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.5/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.5/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.5/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.5/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-04-21 21:15:38.759586 opentakserver-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.5/README.md
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.6/LICENSE
+-rw-r--r--   0        0        0      125 2024-04-25 01:30:38.930304 opentakserver-1.1.6/opentakserver/__init__.py
+-rw-r--r--   0        0        0    11359 2024-04-25 01:28:40.559208 opentakserver-1.1.6/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.6/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    46981 2024-04-25 01:28:32.326084 opentakserver-1.1.6/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.6/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26684 2024-04-21 19:26:51.394711 opentakserver-1.1.6/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.6/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4580 2024-04-21 19:26:51.395692 opentakserver-1.1.6/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.6/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.6/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    21365 2024-04-25 01:28:40.561201 opentakserver-1.1.6/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.6/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10751 2024-04-21 19:26:51.397701 opentakserver-1.1.6/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34945 2024-04-25 01:28:32.328083 opentakserver-1.1.6/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     4153 2024-04-25 01:28:40.562199 opentakserver-1.1.6/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.6/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      377 2024-04-25 01:28:32.330072 opentakserver-1.1.6/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.6/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.6/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.6/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.6/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.6/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.6/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.6/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.6/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.6/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.6/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.6/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.6/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.6/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.6/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.6/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.6/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1427 2024-04-25 01:28:32.332068 opentakserver-1.1.6/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.6/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.6/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.6/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.6/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.6/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.6/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.6/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-04-16 19:41:24.153676 opentakserver-1.1.6/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.6/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.6/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.6/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.6/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.6/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.6/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0      524 2024-04-25 01:28:40.558211 opentakserver-1.1.6/opentakserver/PasswordValidator.py
+-rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.6/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1679 2024-04-25 01:30:38.918295 opentakserver-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2073 2024-04-11 21:18:43.687758 opentakserver-1.1.6/README.md
+-rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 opentakserver-1.1.6/PKG-INFO
```

### Comparing `opentakserver-1.1.5/LICENSE` & `opentakserver-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/app.py` & `opentakserver-1.1.6/opentakserver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import eventlet
 try:
     eventlet.monkey_patch()
 except BaseException as e:
     print("Failed to monkey_patch(): {}".format(e))
 
+from opentakserver.PasswordValidator import PasswordValidator
+
 import platform
 import requests
 from sqlalchemy import insert
 import sqlite3
 from opentakserver.models.Icon import Icon
 
 import yaml
@@ -107,15 +109,15 @@
     except sqlalchemy.exc.InvalidRequestError:
         pass
 
     from opentakserver.models.user import User
     from opentakserver.models.role import Role
 
     user_datastore = SQLAlchemyUserDatastore(db, User, Role, WebAuthn)
-    app.security = Security(app, user_datastore, mail_util_cls=EmailValidator)
+    app.security = Security(app, user_datastore, mail_util_cls=EmailValidator, password_util_cls=PasswordValidator)
 
     mail.init_app(app)
     with app.app_context():
         db.create_all()
 
 
 def setup_logging(app):
@@ -284,8 +286,9 @@
             logger.error("Failed to enable Mumble authentication: {}".format(e))
             logger.error(traceback.format_exc())
     else:
         logger.info("Mumble authentication handler disabled")
 
     app.start_time = datetime.now()
 
-    socketio.run(app, host="127.0.0.1", port=app.config.get("OTS_LISTENER_PORT"), debug=app.config.get("DEBUG"), log_output=app.config.get("DEBUG"))
+    socketio.run(app, host=app.config.get("OTS_LISTENER_ADDRESS"), port=app.config.get("OTS_LISTENER_PORT"),
+                 debug=app.config.get("DEBUG"), log_output=app.config.get("DEBUG"))
```

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/api.py` & `opentakserver-1.1.6/opentakserver/blueprints/api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/config.py` & `opentakserver-1.1.6/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/marti.py` & `opentakserver-1.1.6/opentakserver/blueprints/marti.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.6/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.6/opentakserver/blueprints/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.6/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/ca_config.py` & `opentakserver-1.1.6/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/certificate_authority.py` & `opentakserver-1.1.6/opentakserver/certificate_authority.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,14 @@
             self.logger.debug(command)
 
             exit_code = subprocess.call(command, shell=True)
 
             if exit_code:
                 raise Exception("Failed to create ca.pem. Exit code {}".format(exit_code))
 
-            # os.chmod(os.path.join(self.app.config.get("OTS_CA_FOLDER"), "ca-do-not-share.key"), 1411)
-
             command = ('openssl x509 -in {} -addtrust clientAuth -addtrust serverAuth -setalias {} -out {}'
                        .format(os.path.join(self.app.config.get("OTS_CA_FOLDER"), "ca.pem"),
                                self.app.config.get("OTS_CA_NAME"),
                                os.path.join(self.app.config.get("OTS_CA_FOLDER"), "ca-trusted.pem")))
 
             self.logger.debug(command)
```

### Comparing `opentakserver-1.1.5/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.6/opentakserver/controllers/client_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.6/opentakserver/controllers/cot_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/defaultconfig.py` & `opentakserver-1.1.6/opentakserver/defaultconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class DefaultConfig:
     SECRET_KEY = secrets.token_hex()
     DEBUG = False
 
     OTS_DATA_FOLDER = os.path.join(Path.home(), 'ots')
+    OTS_LISTENER_ADDRESS = "127.0.0.1"
     OTS_LISTENER_PORT = 8081  # OTS will listen for HTTP requests on this port. Nginx will listen on ports 80, 443,
                               # 8080, 8443, and 8446 and proxy requests to OTS_LISTENER_PORT
     OTS_MARTI_HTTP_PORT = 8080
     OTS_MARTI_HTTPS_PORT = 8443
     OTS_ENABLE_TCP_STREAMING_PORT = True
     OTS_TCP_STREAMING_PORT = 8088
     OTS_SSL_STREAMING_PORT = 8089
```

### Comparing `opentakserver-1.1.5/opentakserver/EmailValidator.py` & `opentakserver-1.1.6/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.6/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.6/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Alert.py` & `opentakserver-1.1.6/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/CasEvac.py` & `opentakserver-1.1.6/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Certificate.py` & `opentakserver-1.1.6/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.6/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.6/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/CoT.py` & `opentakserver-1.1.6/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/DataPackage.py` & `opentakserver-1.1.6/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/EUD.py` & `opentakserver-1.1.6/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/GeoChat.py` & `opentakserver-1.1.6/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Icon.py` & `opentakserver-1.1.6/opentakserver/models/Icon.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import base64
-from dataclasses import dataclass
-
-from opentakserver.extensions import db
-from sqlalchemy import Integer, String, LargeBinary
-from sqlalchemy.orm import Mapped, mapped_column, relationship
-
-
-@dataclass
-class Icon(db.Model):
-    __tablename__ = "icons"
-
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    iconset_uid: Mapped[str] = mapped_column(String, nullable=True)
-    filename: Mapped[str] = mapped_column(String, nullable=True)
-    groupName: Mapped[str] = mapped_column(String, nullable=True)
-    type2525b: Mapped[str] = mapped_column(String, nullable=True)
-    useCnt: Mapped[int] = mapped_column(Integer, nullable=True)
-    bitmap: Mapped[bytes] = mapped_column(LargeBinary, nullable=True)
-    shadow: Mapped[bytes] = mapped_column(LargeBinary, nullable=True)
-    markers = relationship("Marker", back_populates="icon")
-
-    def serialize(self):
-        return {
-            'iconset_uid': self.iconset_uid,
-            'filename': self.filename,
-            'groupName': self.groupName,
-            'type2525b': self.type2525b,
-            'useCnt': self.useCnt,
-            'bitmap': 'data:image/png;base64,{}'.format(base64.b64encode(self.bitmap).decode('utf-8')) if self.bitmap else None,
-            'shadow': 'data:image/png;base64,{}'.format(base64.b64encode(self.shadow).decode('utf-8')) if self.shadow else None
-        }
-
-    def to_json(self):
-        return self.serialize()
+import base64
+from dataclasses import dataclass
+
+from opentakserver.extensions import db
+from sqlalchemy import Integer, String, LargeBinary
+from sqlalchemy.orm import Mapped, mapped_column, relationship
+
+
+@dataclass
+class Icon(db.Model):
+    __tablename__ = "icons"
+
+    id: Mapped[int] = mapped_column(Integer, primary_key=True)
+    iconset_uid: Mapped[str] = mapped_column(String, nullable=True)
+    filename: Mapped[str] = mapped_column(String, nullable=True)
+    groupName: Mapped[str] = mapped_column(String, nullable=True)
+    type2525b: Mapped[str] = mapped_column(String, nullable=True)
+    useCnt: Mapped[int] = mapped_column(Integer, nullable=True)
+    bitmap: Mapped[bytes] = mapped_column(LargeBinary, nullable=True)
+    shadow: Mapped[bytes] = mapped_column(LargeBinary, nullable=True)
+    markers = relationship("Marker", back_populates="icon")
+
+    def serialize(self):
+        return {
+            'iconset_uid': self.iconset_uid,
+            'filename': self.filename,
+            'groupName': self.groupName,
+            'type2525b': self.type2525b,
+            'useCnt': self.useCnt,
+            'bitmap': 'data:image/png;base64,{}'.format(base64.b64encode(self.bitmap).decode('utf-8')) if self.bitmap else None,
+            'shadow': 'data:image/png;base64,{}'.format(base64.b64encode(self.shadow).decode('utf-8')) if self.shadow else None
+        }
+
+    def to_json(self):
+        return self.serialize()
```

### Comparing `opentakserver-1.1.5/opentakserver/models/Marker.py` & `opentakserver-1.1.6/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Point.py` & `opentakserver-1.1.6/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/RBLine.py` & `opentakserver-1.1.6/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/Team.py` & `opentakserver-1.1.6/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/user.py` & `opentakserver-1.1.6/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.6/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/VideoStream.py` & `opentakserver-1.1.6/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/models/ZMIST.py` & `opentakserver-1.1.6/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.6/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.6/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.6/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/opentakserver/SocketServer.py` & `opentakserver-1.1.6/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/pyproject.toml` & `opentakserver-1.1.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-[tool.poetry]
-name = "OpenTAKServer"
-version = "1.1.5"
-description = "A server for ATAK, WinTAK, and iTAK"
-authors = ["OpenTAKServer <opentakserver@gmail.com>"]
-readme = "README.md"
-license = "GPL-3.0-or-later"
-repository = "https://github.com/brian7704/OpenTAKServer"
-documentation = "https://docs.opentakserver.io"
-
-[tool.poetry.dependencies]
-adsbxcot = "6.0.4"
-beautifulsoup4 = "4.12.3"
-colorlog = "6.8.2"
-datetime = "5.3"
-ffmpeg-python = "0.2.0"
-flask = "3.0.2"
-flask-apscheduler = "1.13.1"
-flask-cors = "4.0.0"
-Flask-Security-Too = {version="5.4.3", extras=["common", "mfa"]}
-flask-socketio = "5.3.6"
-flask-sqlalchemy = "3.1.1"
-eventlet = "0.35.2"
-gevent = "23.9.1"
-lastversion = "*"
-lxml = "5.1.0"
-pika = "1.3.2"
-poetry-dynamic-versioning = {version = "1.2.0", extras = ["plugin"]}
-psutil = "5.9.8"
-pygc = "1.3.0"
-PyJWT = "2.8.0"
-pytak = "6.3.2"
-pytest = "7.4.4"
-pytest-cov = "4.1.0"
-python = "^3.10"
-python-socketio = {extras = ["client", "websocket_client", "asyncio_client"], version = "5.10.0"}
-pyOpenSSL = "23.3.0"
-pyotp = "2.9.0"
-PyYAML = "6.0.1"
-sqlalchemy = "2.0.28"
-sqlalchemy-utils = "0.41.1"
-tldextract = "5.1.2"
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "semver"
-dirty = true
-pattern = "((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
-
-[tool.poetry-dynamic-versioning.files."opentakserver/__init__.py"]
-persistent-substitution = true
-initial-content = """
-  # These version placeholders will be replaced later during substitution.
-  __version__ = "0.0.0"
-  __version_tuple__ = (0, 0, 0)
-"""
-
-[build-system]
-requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
-build-backend = "poetry_dynamic_versioning.backend"
+[tool.poetry]
+name = "OpenTAKServer"
+version = "1.1.6"
+description = "A server for ATAK, WinTAK, and iTAK"
+authors = ["OpenTAKServer <opentakserver@gmail.com>"]
+readme = "README.md"
+license = "GPL-3.0-or-later"
+repository = "https://github.com/brian7704/OpenTAKServer"
+documentation = "https://docs.opentakserver.io"
+
+[tool.poetry.dependencies]
+adsbxcot = "6.0.4"
+beautifulsoup4 = "4.12.3"
+colorlog = "6.8.2"
+datetime = "5.3"
+ffmpeg-python = "0.2.0"
+flask = "3.0.2"
+flask-apscheduler = "1.13.1"
+flask-cors = "4.0.0"
+Flask-Security-Too = {version="5.4.3", extras=["common", "mfa"]}
+flask-socketio = "5.3.6"
+flask-sqlalchemy = "3.1.1"
+eventlet = "0.35.2"
+gevent = "23.9.1"
+lastversion = "*"
+lxml = "5.1.0"
+pika = "1.3.2"
+poetry-dynamic-versioning = {version = "1.2.0", extras = ["plugin"]}
+psutil = "5.9.8"
+pygc = "1.3.0"
+PyJWT = "2.8.0"
+pytak = "6.3.2"
+pytest = "7.4.4"
+pytest-cov = "4.1.0"
+python = "^3.10"
+python-socketio = {extras = ["client", "websocket_client", "asyncio_client"], version = "5.10.0"}
+pyOpenSSL = "23.3.0"
+pyotp = "2.9.0"
+PyYAML = "6.0.1"
+sqlalchemy = "2.0.28"
+sqlalchemy-utils = "0.41.1"
+tldextract = "5.1.2"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "semver"
+dirty = false
+pattern = "((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
+
+[tool.poetry-dynamic-versioning.files."opentakserver/__init__.py"]
+persistent-substitution = true
+initial-content = """
+  # These version placeholders will be replaced later during substitution.
+  __version__ = "0.0.0"
+  __version_tuple__ = (0, 0, 0)
+"""
+
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `opentakserver-1.1.5/README.md` & `opentakserver-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.5/PKG-INFO` & `opentakserver-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenTAKServer
-Version: 1.1.5
+Version: 1.1.6
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

