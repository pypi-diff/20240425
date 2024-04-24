# Comparing `tmp/hslog-1.8.0.tar.gz` & `tmp/hslog-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hslog-1.8.0.tar", last modified: Wed Apr  8 19:30:56 2020, max compression
+gzip compressed data, was "dist/hslog-1.9.0.tar", last modified: Tue Jun  9 21:51:49 2020, max compression
```

## Comparing `hslog-1.8.0.tar` & `hslog-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-08 19:30:56.000000 hslog-1.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      657 2020-04-08 19:30:56.000000 hslog-1.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3676 2020-04-08 19:30:38.000000 hslog-1.8.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      657 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-08 19:30:56.000000 hslog-1.8.0/hslog/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/player.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9713 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/export.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25443 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4225 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/tokens.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5512 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/packets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-04-08 19:30:38.000000 hslog-1.8.0/hslog/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      685 2020-04-08 19:30:56.000000 hslog-1.8.0/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)       62 2020-04-08 19:30:38.000000 hslog-1.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-09 21:51:49.000000 hslog-1.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      657 2020-06-09 21:51:49.000000 hslog-1.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3676 2020-06-09 21:51:31.000000 hslog-1.9.0/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      657 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      306 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-09 21:51:49.000000 hslog-1.9.0/hslog/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5940 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/player.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10007 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/export.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25848 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4342 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/tokens.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5731 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/packets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      118 2020-06-09 21:51:31.000000 hslog-1.9.0/hslog/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      685 2020-06-09 21:51:49.000000 hslog-1.9.0/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)       62 2020-06-09 21:51:31.000000 hslog-1.9.0/setup.py
```

### Comparing `hslog-1.8.0/PKG-INFO` & `hslog-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hslog
-Version: 1.8.0
+Version: 1.9.0
 Summary: Hearthstone Power.log parser
 Home-page: https://github.com/HearthSim/python-hslog/
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 License: UNKNOWN
 Download-URL: https://github.com/HearthSim/python-hslog/tarball/master
 Description: UNKNOWN
```

### Comparing `hslog-1.8.0/README.md` & `hslog-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hslog-1.8.0/hslog.egg-info/PKG-INFO` & `hslog-1.9.0/hslog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hslog
-Version: 1.8.0
+Version: 1.9.0
 Summary: Hearthstone Power.log parser
 Home-page: https://github.com/HearthSim/python-hslog/
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 License: UNKNOWN
 Download-URL: https://github.com/HearthSim/python-hslog/tarball/master
 Description: UNKNOWN
```

### Comparing `hslog-1.8.0/hslog/player.py` & `hslog-1.9.0/hslog/player.py`

 * *Files identical despite different names*

### Comparing `hslog-1.8.0/hslog/export.py` & `hslog-1.9.0/hslog/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 			packets.SendChoices: self.handle_send_choices,
 			packets.ChosenEntities: self.handle_chosen_entities,
 			packets.Options: self.handle_options,
 			packets.Option: self.handle_option,
 			packets.SendOption: self.handle_send_option,
 			packets.ResetGame: self.handle_reset_game,
 			packets.SubSpell: self.handle_sub_spell,
+			packets.CachedTagForDormantChange: self.handle_cached_tag_for_dormant_change
 		}
 
 	def export(self):
 		for packet in self.packet_tree:
 			self.export_packet(packet)
 		return self
 
@@ -92,14 +93,17 @@
 	def handle_reset_game(self, packet):
 		pass
 
 	def handle_sub_spell(self, packet):
 		for p in packet.packets:
 			self.export_packet(p)
 
+	def handle_cached_tag_for_dormant_change(self, packet):
+		pass
+
 
 class CompositeExporter(BaseExporter):
 	"""Exporter implementation that broadcasts packets to configured child exporters
 
 	Use this class to compose multiple exporters in order to do a single pass over a
 	configured packet tree. Note:
 
@@ -179,14 +183,18 @@
 		for exporter in self.exporters:
 			exporter.handle_reset_game(packet)
 
 	def handle_sub_spell(self, packet):
 		for exporter in self.exporters:
 			exporter.handle_sub_spell(packet)
 
+	def handle_cached_tag_for_dormant_change(self, packet):
+		for exporter in self.exporters:
+			exporter.handle_cached_tag_for_dormant_change(packet)
+
 
 class EntityTreeExporter(BaseExporter):
 	game_class = Game
 	player_class = Player
 	card_class = Card
 
 	class EntityNotFound(Exception):
```

### Comparing `hslog-1.8.0/hslog/parser.py` & `hslog-1.9.0/hslog/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,19 @@
 			regex, callback = tokens.META_DATA_RE, self.meta_data
 		elif opcode == "RESET_GAME":
 			regex, callback = tokens.RESET_GAME_RE, self.reset_game
 		elif opcode == "SUB_SPELL_START":
 			regex, callback = tokens.SUB_SPELL_START_RE, self.sub_spell_start
 		elif opcode == "SUB_SPELL_END":
 			regex, callback = tokens.SUB_SPELL_END_RE, self.sub_spell_end
+		elif opcode == "CACHED_TAG_FOR_DORMANT_CHANGE":
+			regex, callback = (
+				tokens.CACHED_TAG_FOR_DORMANT_CHANGE_RE,
+				self.cached_tag_for_dormant_change
+			)
 		else:
 			raise NotImplementedError(data)
 
 		sre = regex.match(data)
 		if not sre:
 			logging.warning("[%s] Could not correctly parse %r", ts, data)
 			return
@@ -354,14 +359,22 @@
 			logging.warning("[%s] Orphaned SUB_SPELL_END detected", ts)
 			return self.current_block
 		self.current_block.end()
 		sub_spell = self.current_block
 		self.current_block = self.current_block.parent
 		return sub_spell
 
+	def cached_tag_for_dormant_change(self, ts, e, tag, value):
+		id = self.parse_entity_id(e)
+		tag, value = parse_tag(tag, value)
+
+		packet = packets.CachedTagForDormantChange(ts, id, tag, value)
+		self.register_packet(packet)
+		return packet
+
 
 class OptionsHandler:
 	def __init__(self):
 		super(OptionsHandler, self).__init__()
 		self._option_packet = None
 		self._options_packet = None
 		self._suboption_packet = None
```

### Comparing `hslog-1.8.0/hslog/tokens.py` & `hslog-1.9.0/hslog/tokens.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 CHANGE_ENTITY_RE = re.compile(r"CHANGE_ENTITY - Updating Entity=%s CardID=(\w+)$" % _E)
 DEF_CHANGE = "DEF CHANGE"
 TAG_CHANGE_RE = re.compile(r"TAG_CHANGE Entity=%s tag=(\w+) value=(\w+) ?(%s)?" % (_E, DEF_CHANGE))
 META_DATA_RE = re.compile(r"META_DATA - Meta=(\w+) Data=%s InfoCount=(\d+)" % _E)
 RESET_GAME_RE = re.compile(r"RESET_GAME$")
 SUB_SPELL_START_RE = re.compile(r"SUB_SPELL_START - SpellPrefabGUID=([\w:.]+) Source=(\d+) TargetCount=(\d+)$")
 SUB_SPELL_END_RE = re.compile(r"SUB_SPELL_END$")
+CACHED_TAG_FOR_DORMANT_CHANGE_RE = re.compile(r"CACHED_TAG_FOR_DORMANT_CHANGE Entity=%s tag=(\w+) value=(\w+)" % _E)
 
 # Message details
 TAG_VALUE_RE = re.compile(r"tag=(\w+) value=(\w+)")
 METADATA_INFO_RE = re.compile(r"Info\[(\d+)\] = %s" % _E)
 SUB_SPELL_START_SOURCE_RE = re.compile(r"Source = %s" % _E)
 SUB_SPELL_START_TARGETS_RE = re.compile(r"Targets\[(\d+)\] = %s" % _E)
```

### Comparing `hslog-1.8.0/hslog/utils.py` & `hslog-1.9.0/hslog/utils.py`

 * *Files identical despite different names*

### Comparing `hslog-1.8.0/hslog/packets.py` & `hslog-1.9.0/hslog/packets.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,7 +265,17 @@
 	def __repr__(self):
 		return "%s(spell_prefab_guid=%r, source=%r)" % (
 			self.__class__.__name__, self.spell_prefab_guid, self.source
 		)
 
 	def end(self):
 		self.ended = True
+
+
+class CachedTagForDormantChange(Packet):
+	power_type = PowerType.CACHED_TAG_FOR_DORMANT_CHANGE
+
+	def __init__(self, ts, entity, tag, value):
+		self.ts = ts
+		self.entity = entity
+		self.tag = tag
+		self.value = value
```

### Comparing `hslog-1.8.0/setup.cfg` & `hslog-1.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hslog
-version = 1.8.0
+version = 1.9.0
 description = Hearthstone Power.log parser
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hslog/
 download_url = https://github.com/HearthSim/python-hslog/tarball/master
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

