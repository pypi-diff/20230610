# Comparing `tmp/pygameHat-1.1.2.1.tar.gz` & `tmp/pygameHat-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.1.2.1.tar", last modified: Thu May 11 18:56:08 2023, max compression
+gzip compressed data, was "pygameHat-1.1.3.tar", last modified: Sat Jun 10 17:40:24 2023, max compression
```

## Comparing `pygameHat-1.1.2.1.tar` & `pygameHat-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.837662 pygameHat-1.1.2.1/
--rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      545 2023-05-11 18:56:08.837662 pygameHat-1.1.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.677611 pygameHat-1.1.2.1/pygameHat/
--rw-rw-rw-   0        0        0    43862 2023-05-11 18:55:01.000000 pygameHat-1.1.2.1/pygameHat/__init__.py
--rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.2.1/pygameHat/pygameHat.py
-drwxrwxrwx   0        0        0        0 2023-05-11 18:56:08.787607 pygameHat-1.1.2.1/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      545 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 18:56:07.000000 pygameHat-1.1.2.1/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 18:56:08.844658 pygameHat-1.1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-05-11 18:54:47.000000 pygameHat-1.1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:40:24.304538 pygameHat-1.1.3/
+-rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-06-10 17:40:24.305543 pygameHat-1.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-10 17:40:24.160511 pygameHat-1.1.3/pygameHat/
+-rw-rw-rw-   0        0        0    44187 2023-06-10 17:39:23.000000 pygameHat-1.1.3/pygameHat/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.3/pygameHat/pygameHat.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:40:24.293588 pygameHat-1.1.3/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-06-10 17:40:21.000000 pygameHat-1.1.3/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-06-10 17:40:22.000000 pygameHat-1.1.3/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 17:40:21.000000 pygameHat-1.1.3/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-10 17:40:21.000000 pygameHat-1.1.3/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 17:40:22.000000 pygameHat-1.1.3/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 17:40:24.312619 pygameHat-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-06-10 17:40:11.000000 pygameHat-1.1.3/setup.py
```

### Comparing `pygameHat-1.1.2.1/PKG-INFO` & `pygameHat-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.2.1
+Version: 1.1.3
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.2.1/pygameHat/__init__.py` & `pygameHat-1.1.3/pygameHat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pygame, sys, time, base64, os, json
 
 #pygame initialization
-version = "Beta 1.1.2.1"
+version = "Beta 1.1.3"
 print(f"\nAdditional hello from pygameHat {version} :D")
 print("\nThis version may not be compatible with older versions")
 
 pygame.init()
 pygame.font.init()
 try:
     pygame.mixer.init()
@@ -33,14 +33,18 @@
         pass
     def is_colliding(self, object):
         pass
     def on_destroy(self):
         pass
     def on_alarm(self, alarm):
         pass
+    def on_create(self):
+        pass
+    def on_signal(self, signal):
+        pass
 
 
     def add_timer(self, time, name):
         self.active_timers[name] = time
     
     def decrement_active_timers(self):
         dead_timers = []
@@ -57,26 +61,23 @@
 class Room:
     def __init__(self, background=(50, 50, 50), layers={"default": []}, instances=[]):
         self.background = background
         self.layers = layers
         self.instances = instances
 
 class Sprite:
-    def __init__(self, index, spritesheet_data=(1, 1), speed=60, collision=False, offset="upper-left", looping=True, size=None):
+    def __init__(self, index, spritesheet_data=(1, 1), speed=60, collision=False, offset="upper-left", looping=True):
         if type(index) == type(pygame.Surface((0, 0))):
             self.index = index
         else:
             self.index = pygame.image.load(index).convert_alpha()
 
         self.speed = speed
         self.x_frames, self.y_frames = spritesheet_data
 
-        if size:
-            resize_sprite(self, size)
-
         self.x_size, self.y_size = self.index.get_width()/(self.x_frames), self.index.get_height()/(self.y_frames)
         
         self.x_frames -= 1
         self.y_frames -= 1
 
         self.current_x_frame = 0
         self.current_y_frame = 0
@@ -329,14 +330,15 @@
     monitor.blit(pygame.font.Font(None, 100).render("(=OwO=)", True, (3, 252, 48)), (100, 150))
     pygame.display.flip()
 
 def add_object_instance(object, layer, position="default"):
     if position != "default":
         object.x, object.y = position
     current_room.layers[layer].append(object)
+    object.on_create()
     return object
 
 def find_object_by_class(object, multiple=False):
     found_objects = []
 
     for layer in current_room.layers:
         for instance in current_room.layers[layer]:
@@ -379,14 +381,17 @@
 
     if object.sprite and object.sprite.collision:
         object_shape = object.sprite.update_collision_shape_position(object.x, object.y)
 
         if object_shape.collidepoint((pointX, pointY)):
             return object
 
+def collide_mouse(object):
+    return collide_point(get_mouse_position(), object)
+
 def screen_position_to_ingame_position(position):
     pX, pY = position
     rSX, rSY = Settings.room_size
     sSX, sSY = screen_size
 
     tSX = sSX/rSX
     tSY = sSY/rSY
@@ -433,14 +438,26 @@
     screen.blit(font.font.render(text, True, color, bg_color), (x-camera.x, y-camera.y))
 
 def change_room(room):
     global current_room, changed_room
     current_room = room
     changed_room = True
 
+def send_signal(signal):
+    for layer in current_room.layers:
+        for instance in current_room.layers[layer]:
+            instance.on_signal(signal)
+
+
+def fill_background():
+    if type(current_room.background) == Sprite:
+        draw_sprite(current_room.background, 0, 0)
+    else:
+        screen.fill(current_room.background)
+
 
 def start():
     timeB = 0
     last_input = None
     last_input_released = None
     console_text = ""
     global delta_time, current_time
@@ -479,18 +496,15 @@
             elif event.type == pygame.MOUSEBUTTONUP:
                 last_input_released = event.button
             
             elif event.type == pygame.VIDEORESIZE:
                 screen_size = (event.w, event.h)
 
         #background                
-        if type(current_room.background) == Sprite:
-            draw_sprite(current_room.background, 0, 0)
-        else:
-            screen.fill(current_room.background)
+        fill_background()
     
         #object handling
         try:
             for layer in current_room.layers:
                 for instance in current_room.layers[layer]:
                     #object drawing and processing
                     if instance.visible:
```

### Comparing `pygameHat-1.1.2.1/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.3/pygameHat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.2.1
+Version: 1.1.3
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.2.1/setup.py` & `pygameHat-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.2.1'
+VERSION = '1.1.3'
 DESCRIPTION = 'Pygame game-making engine'
 
 # Setting up
 setup(
     name="pygameHat",
     version=VERSION,
     author="Wojciech Błajda",
```

