# Comparing `tmp/pygame_magics-0.4.0.tar.gz` & `tmp/pygame_magics-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_magics-0.4.0.tar", last modified: Wed Apr 24 18:44:21 2024, max compression
+gzip compressed data, was "pygame_magics-0.5.0.tar", last modified: Wed Apr 24 20:12:41 2024, max compression
```

## Comparing `pygame_magics-0.4.0.tar` & `pygame_magics-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.544132 pygame_magics-0.4.0/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 18:44:21.543893 pygame_magics-0.4.0/PKG-INFO
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541042 pygame_magics-0.4.0/pygame_magics/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:21:17.000000 pygame_magics-0.4.0/pygame_magics/__init__.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541978 pygame_magics-0.4.0/pygame_magics/camera/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 16:50:43.000000 pygame_magics-0.4.0/pygame_magics/camera/__init__.py
--rw-r--r--   0 senya      (501) staff       (20)     2795 2024-04-24 17:55:58.000000 pygame_magics-0.4.0/pygame_magics/camera/camera.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.543527 pygame_magics-0.4.0/pygame_magics/entities/
--rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:40.000000 pygame_magics-0.4.0/pygame_magics/entities/__init__.py
--rw-r--r--   0 senya      (501) staff       (20)      820 2024-04-24 17:55:59.000000 pygame_magics-0.4.0/pygame_magics/entities/enemy.py
--rw-r--r--   0 senya      (501) staff       (20)      619 2024-04-24 18:42:39.000000 pygame_magics-0.4.0/pygame_magics/entities/experience_orb.py
--rw-r--r--   0 senya      (501) staff       (20)     3212 2024-04-24 18:39:32.000000 pygame_magics-0.4.0/pygame_magics/entities/magic_bolt.py
--rw-r--r--   0 senya      (501) staff       (20)     1992 2024-04-24 18:39:32.000000 pygame_magics-0.4.0/pygame_magics/entities/player.py
--rw-r--r--   0 senya      (501) staff       (20)     2950 2024-04-24 18:44:00.000000 pygame_magics-0.4.0/pygame_magics/entities/setup_m.py
-drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 18:44:21.541721 pygame_magics-0.4.0/pygame_magics.egg-info/
--rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/PKG-INFO
--rw-r--r--   0 senya      (501) staff       (20)      494 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/SOURCES.txt
--rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/dependency_links.txt
--rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/requires.txt
--rw-r--r--   0 senya      (501) staff       (20)       14 2024-04-24 18:44:21.000000 pygame_magics-0.4.0/pygame_magics.egg-info/top_level.txt
--rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 18:44:21.544184 pygame_magics-0.4.0/setup.cfg
--rw-r--r--   0 senya      (501) staff       (20)      879 2024-04-24 18:44:19.000000 pygame_magics-0.4.0/setup.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 20:12:41.531616 pygame_magics-0.5.0/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 20:12:41.531448 pygame_magics-0.5.0/PKG-INFO
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 20:12:41.528950 pygame_magics-0.5.0/pygame_magics/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:21:17.000000 pygame_magics-0.5.0/pygame_magics/__init__.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 20:12:41.529871 pygame_magics-0.5.0/pygame_magics/camera/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 16:50:43.000000 pygame_magics-0.5.0/pygame_magics/camera/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)     3383 2024-04-24 20:08:36.000000 pygame_magics-0.5.0/pygame_magics/camera/camera.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 20:12:41.531211 pygame_magics-0.5.0/pygame_magics/entities/
+-rw-r--r--   0 senya      (501) staff       (20)        0 2024-04-24 17:05:40.000000 pygame_magics-0.5.0/pygame_magics/entities/__init__.py
+-rw-r--r--   0 senya      (501) staff       (20)      725 2024-04-24 19:28:54.000000 pygame_magics-0.5.0/pygame_magics/entities/enemy.py
+-rw-r--r--   0 senya      (501) staff       (20)      551 2024-04-24 19:48:05.000000 pygame_magics-0.5.0/pygame_magics/entities/experience_orb.py
+-rw-r--r--   0 senya      (501) staff       (20)     3738 2024-04-24 19:48:05.000000 pygame_magics-0.5.0/pygame_magics/entities/magic_bolt.py
+-rw-r--r--   0 senya      (501) staff       (20)     1378 2024-04-24 20:12:35.000000 pygame_magics-0.5.0/pygame_magics/entities/player.py
+-rw-r--r--   0 senya      (501) staff       (20)      647 2024-04-24 20:12:35.000000 pygame_magics-0.5.0/pygame_magics/entities/player_stats.py
+-rw-r--r--   0 senya      (501) staff       (20)     3637 2024-04-24 20:00:09.000000 pygame_magics-0.5.0/pygame_magics/entities/samples.py
+-rw-r--r--   0 senya      (501) staff       (20)      294 2024-04-24 20:12:35.000000 pygame_magics-0.5.0/pygame_magics/entities/singleton.py
+drwxr-xr-x   0 senya      (501) staff       (20)        0 2024-04-24 20:12:41.529640 pygame_magics-0.5.0/pygame_magics.egg-info/
+-rw-r--r--   0 senya      (501) staff       (20)      699 2024-04-24 20:12:41.000000 pygame_magics-0.5.0/pygame_magics.egg-info/PKG-INFO
+-rw-r--r--   0 senya      (501) staff       (20)      569 2024-04-24 20:12:41.000000 pygame_magics-0.5.0/pygame_magics.egg-info/SOURCES.txt
+-rw-r--r--   0 senya      (501) staff       (20)        1 2024-04-24 20:12:41.000000 pygame_magics-0.5.0/pygame_magics.egg-info/dependency_links.txt
+-rw-r--r--   0 senya      (501) staff       (20)        7 2024-04-24 20:12:41.000000 pygame_magics-0.5.0/pygame_magics.egg-info/requires.txt
+-rw-r--r--   0 senya      (501) staff       (20)       14 2024-04-24 20:12:41.000000 pygame_magics-0.5.0/pygame_magics.egg-info/top_level.txt
+-rw-r--r--   0 senya      (501) staff       (20)       38 2024-04-24 20:12:41.531658 pygame_magics-0.5.0/setup.cfg
+-rw-r--r--   0 senya      (501) staff       (20)      880 2024-04-24 20:08:36.000000 pygame_magics-0.5.0/setup.py
```

### Comparing `pygame_magics-0.4.0/PKG-INFO` & `pygame_magics-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_magics
-Version: 0.4.0
+Version: 0.5.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame_magics-0.4.0/pygame_magics/camera/camera.py` & `pygame_magics-0.5.0/pygame_magics/camera/camera.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 class CameraGroup(pygame.sprite.Group):
 
     def __init__(self, map_x, map_y, field_img, size_coefficient=1):
         """
             https://github.com/clear-code-projects/Pygame-Cameras
             https://www.youtube.com/watch?v=u7LPRqrzry8
+            :param map_x: map width
+            :param map_y: map height
+            :param field_img: image of a map
+            :param size_coefficient: coefficient of resizing
         """
         super().__init__()
         self.display_surface = pygame.display.get_surface()
 
         self.ground_surf = pygame.image.load(field_img)
         self.ground_surf = pygame.transform.scale(self.ground_surf, (self.ground_surf.get_width() * size_coefficient,
                                                                      self.ground_surf.get_height() * size_coefficient))
@@ -20,18 +24,28 @@
         self.map_y = map_y
 
         self.offset = pygame.math.Vector2(800, 300)
         self.half_w = self.display_surface.get_size()[0] // 2
         self.half_h = self.display_surface.get_size()[1] // 2
 
     def center_target_camera(self, target):
+        """
+        it centralizes player on camera
+        :param target: player
+        :return:
+        """
         self.offset.x = target.rect.centerx - self.half_w
         self.offset.y = target.rect.centery - self.half_h
 
     def round_walk_effect(self, target):
+        """
+        it makes that player goes round
+        :param target: player
+        :return:
+        """
         min_x = self.offset.x - self.half_w
         max_x = self.offset.x + self.half_w
         min_y = self.offset.y - self.half_h
         max_y = self.offset.y + self.half_h
 
         if target.rect.right < min_x:
             target.rect.right = min_x
@@ -51,27 +65,36 @@
             self.offset.x = self.map_x
         if self.offset.y < -self.map_y:
             self.offset.y = -self.map_y
         elif self.offset.y > self.map_y:
             self.offset.y = self.map_y
 
     def map_draw(self):
+        """
+        draw map
+        :return:
+        """
         ground_offset = self.ground_rect.topleft - self.offset
         self.display_surface.blit(self.ground_surf, ground_offset)
 
     def custom_draw(self, *args):
+        """
+        the most important function where it mest ne sprite group to be shown
+        :param args: group sprites
+        :return:
+        """
         player = args[0]
         groups = args[1:]
 
         self.map_draw()
 
         self.center_target_camera(player)
         self.round_walk_effect(player)
 
         all_sprites = []
         for group in groups:
             all_sprites.extend(group.sprites())
-        all_sprites.append(player)  # Add the player sprite
+        all_sprites.append(player)
 
         for sprite in sorted(all_sprites, key=lambda x: x.rect.centery):
             offset_pos = sprite.rect.topleft - self.offset
             self.display_surface.blit(sprite.image, offset_pos)
```

### Comparing `pygame_magics-0.4.0/pygame_magics/entities/enemy.py` & `pygame_magics-0.5.0/pygame_magics/entities/experience_orb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import pygame
 
 
-class Enemy(pygame.sprite.Sprite):
-    def __init__(self, pos, image, image_size, speed, health, group):
+class ExperienceOrb(pygame.sprite.Sprite):
+    def __init__(self, pos, image, size, group):
+        """
+        sprites of experience orbs
+        :param pos: position
+        :param image: its image
+        :param size: its size
+        :param group: group in what object is
+        """
         super().__init__(group)
         self.original_image = pygame.image.load(image).convert_alpha()
-        self.image = pygame.transform.scale(self.original_image, image_size)
+        self.image = pygame.transform.scale(self.original_image, size)
         self.rect = self.image.get_rect()
         self.rect.center = pos
-        self.speed = speed
-        self.hp = health
-
-    def lost_hp(self, amount_hp):
-        self.hp -= amount_hp
-
-    def update(self, player):
-        direction_vector = pygame.math.Vector2(player.rect.center) - pygame.math.Vector2(self.rect.center)
-        direction_vector.normalize_ip()
-        self.rect.move_ip(direction_vector * self.speed)
-        # if pygame.sprite.collide_rect(self, player):
-        #     PlayerStats().health -= 1
```

### Comparing `pygame_magics-0.4.0/pygame_magics/entities/magic_bolt.py` & `pygame_magics-0.5.0/pygame_magics/entities/magic_bolt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 from math import degrees, cos, sin, atan2
 
 import pygame
 
 
 class MagicBoltBullet(pygame.sprite.Sprite):
     def __init__(self, pos, image, angle, damage, size, speed, delay, group):
+        """
+        fires a bullet
+        :param pos: position of player
+        :param image: image of bullet
+        :param angle: angle in which it fires
+        :param damage: amount of damage
+        :param size: bullet size
+        :param speed: bullet speed
+        :param delay: delay in time
+        :param group: group of all bullets
+        """
         super().__init__(group)
         self.original_image = (pygame.image.load(image).
                                convert_alpha())
         orig_size = self.original_image.get_size()
         self.image = pygame.transform.scale(pygame.transform.rotate(self.original_image, degrees(angle)),
                                             (orig_size[0] * size, orig_size[1] * size))
         self.rect = self.image.get_rect()
@@ -31,17 +42,27 @@
                 if enemy.hp <= 0:
                     enemy.remove()
                     enemy.kill()
 
 
 class MagicBolt:
     def __init__(self, player_pos):
+        """
+        :param player_pos: player position
+        """
         self.player_pos = player_pos
 
     def spawn_magic_bolt(self, magic_bolt_group, player, n, nearest_enemy_func):
+        """
+        :param magic_bolt_group: Sprite Group for magic bolt
+        :param player: player sprite
+        :param n: level of magic bolt
+        :param nearest_enemy_func: function which will give example of nearest enemy
+        :return:
+        """
         amount = 1
         damage = 10
         size = 1
         speed = 1
         if n >= 2:
             amount += 1
         if n >= 3:
@@ -63,29 +84,28 @@
                 enemy_rect = enemy_rect.rect.center
                 player_rect = player.rect.center
                 angle = atan2((enemy_rect[1] - player_rect[1]), (enemy_rect[0] - player_rect[0]))
                 delay = 20 * j
                 MagicBoltBullet(self.player_pos, angle, damage, size, speed, delay, magic_bolt_group)
 
     def stop_fire(self, magic_bolt_group, enemies):
+        """
+        deletes all instances of class
+        :param magic_bolt_group: magic bolt group
+        :param enemies: enemy group
+        :return:
+        """
         for sprite in magic_bolt_group.sprites():
             sprite.remove()
             sprite.kill()
             sprite.update(enemies)
 
     def update(self, player_position, magic_bolt_group):
+        """
+        you should implement something new here
+        :param player_position: player position
+        :param magic_bolt_group: magic bolt group
+        :return:
+        """
         self.player_pos = player_position
         self.spawn_magic_bolt(magic_bolt_group)
 
-
-# def create_enemy():
-#     Enemy(player.rect.center + pygame.math.Vector2(
-#         (-1) * randint(1, 2) * screen.get_width() * 1.5,
-#         (-1) * randint(1, 2) * screen.get_height() * 1.5), enemy_group)
-
-
-# def get_nearest_enemy():
-#     arr = []
-#     for enemy in enemy_group.sprites():
-#         delta = sqrt((enemy.rect.centerx - player.rect.centerx) ** 2 + (enemy.rect.centery - player.rect.centery) ** 2)
-#         arr.append((delta, enemy))
-#     return min(arr, key=lambda x: x[0])[1] if arr else 0
```

### Comparing `pygame_magics-0.4.0/pygame_magics.egg-info/PKG-INFO` & `pygame_magics-0.5.0/pygame_magics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-magics
-Version: 0.4.0
+Version: 0.5.0
 Summary: Magic survival funcs
 Home-page: https://github.com/MCtop4ik/pygame-magics
 Author: MCtop4ik
 Author-email: senyaza@mail.ru
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygame_magics-0.4.0/setup.py` & `pygame_magics-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+
 from setuptools import setup, find_packages
 
 setup(
     name='pygame_magics',
-    version='0.4.0',
+    version='0.5.0',
     author='MCtop4ik',
     author_email='senyaza@mail.ru',
     description='Magic survival funcs',
     long_description='Hyper grest library for magic survival',
     long_description_content_type='text/markdown',
     url='https://github.com/MCtop4ik/pygame-magics',
     packages=find_packages(),
```

