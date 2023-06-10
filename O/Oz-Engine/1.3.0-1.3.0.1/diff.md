# Comparing `tmp/Oz-Engine-1.3.0.tar.gz` & `tmp/Oz-Engine-1.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oz-Engine-1.3.0.tar", last modified: Mon May 29 13:31:58 2023, max compression
+gzip compressed data, was "Oz-Engine-1.3.0.1.tar", last modified: Sat Jun 10 09:46:30 2023, max compression
```

## Comparing `Oz-Engine-1.3.0.tar` & `Oz-Engine-1.3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 13:31:58.869176 Oz-Engine-1.3.0/
--rw-rw-rw-   0        0        0    35823 2023-02-15 15:44:32.000000 Oz-Engine-1.3.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-29 13:31:58.862175 Oz-Engine-1.3.0/Oz-Engine/
--rw-rw-rw-   0        0        0       11 2023-05-29 09:16:11.000000 Oz-Engine-1.3.0/Oz-Engine/__init__.py
--rw-rw-rw-   0        0        0    25126 2023-05-09 18:46:03.000000 Oz-Engine-1.3.0/Oz-Engine/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:31:58.868174 Oz-Engine-1.3.0/Oz_Engine.egg-info/
--rw-rw-rw-   0        0        0      347 2023-05-29 13:31:58.000000 Oz-Engine-1.3.0/Oz_Engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-05-29 13:31:58.000000 Oz-Engine-1.3.0/Oz_Engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 13:31:58.000000 Oz-Engine-1.3.0/Oz_Engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 13:31:58.000000 Oz-Engine-1.3.0/Oz_Engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      347 2023-05-29 13:31:58.869176 Oz-Engine-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1791 2023-02-27 20:06:32.000000 Oz-Engine-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 13:31:58.869176 Oz-Engine-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      444 2023-05-29 13:25:38.000000 Oz-Engine-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.805392 Oz-Engine-1.3.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-02-15 15:44:32.000000 Oz-Engine-1.3.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.797882 Oz-Engine-1.3.0.1/Oz-Engine/
+-rw-rw-rw-   0        0        0       19 2023-06-10 09:44:23.000000 Oz-Engine-1.3.0.1/Oz-Engine/__init__.py
+-rw-rw-rw-   0        0        0    25352 2023-06-08 16:57:22.000000 Oz-Engine-1.3.0.1/Oz-Engine/main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.803880 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      349 2023-06-10 09:46:30.805392 Oz-Engine-1.3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1791 2023-02-27 20:06:32.000000 Oz-Engine-1.3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 09:46:30.806401 Oz-Engine-1.3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-06-10 09:46:00.000000 Oz-Engine-1.3.0.1/setup.py
```

### Comparing `Oz-Engine-1.3.0/LICENSE` & `Oz-Engine-1.3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Oz-Engine-1.3.0/Oz-Engine/main.py` & `Oz-Engine-1.3.0.1/Oz-Engine/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class Canvas:
     """
     Object that can store sprites in it to be rendered
     """
 
-    __slots__ = "void", "sprite_names", "sprite_names_dict", "sprite_tree", "sprite_position_dict", "sprite_group_dict", "group_tree", "camera_name_dict", "camera_tree", "structure_tree" ,"structure_dict"
+    __slots__ = "void", "sprite_names", "sprite_names_dict", "sprite_tree", "sprite_position_dict", "sprite_group_dict", "group_tree", "camera_name_dict", "camera_tree", "structure_tree", "structure_dict"
 
     def __init__(self, void):
         ''' Characters that fills the canvas when nothing is rendered on a tile. '''
         self.void = void
         '''List that contains every reference of each sprite that is linked to the canvas in question '''
         self.sprite_tree = set()
         '''List that contains every groups that exists'''
@@ -84,14 +84,15 @@
         for todo_sprite in sprite_to_call:
             func = getattr(todo_sprite, method_to_call)
             func(*args)
 
     def get_structure(self, name):
         return self.structure_dict[name]
 
+
 class Sprite:
     """
     Object that can be used to fill the canvas
     """
 
     __slots__ = "canvas_owner", "char", "position", "name", "group"
 
@@ -103,15 +104,14 @@
             name: str,
             group=None,
     ):
         self.register_info(canvas_owner, char, position, name, group)
 
     def register_info(self, canvas_owner: object, char: str, position: dict, name: str, group=None):
 
-
         '''Character that represents the sprite when rendered.'''
         self.char = char
         '''dict that has two element "x" and "y" it tells where to render the sprite.'''
         self.position = position
         '''Name of the sprite that can be used to get reference from it using the "get_sprite" method throught a "Canvas" object.'''
         self.name = name
         '''Canvas that the sprite is associated to.'''
@@ -138,24 +138,21 @@
             canvas_owner.group_tree.add(group)
 
         canvas_owner.sprite_group_dict[group].append(self)
         self.define_cameras_render_cache()
 
     def define_cameras_render_cache(self):
 
-
         for todo_camera in self.canvas_owner.camera_tree:
             # updates yourself to the render cache of camera
 
             render_position = self.get_render_position(todo_camera)
 
-
             if todo_camera.is_renderable(render_position):
 
-
                 # if can be rendered
                 # update key
                 if todo_camera.row_render_dict.get(render_position["y"]) == None:
                     todo_camera.row_render_dict[render_position["y"]] = {}
 
                 if todo_camera.row_render_dict[render_position["y"]].get(render_position["x"]) == None:
                     todo_camera.row_render_dict[render_position["y"]][render_position["x"]] = []
@@ -169,15 +166,14 @@
         for todo_camera in self.canvas_owner.camera_tree:
             self.update_camera_render_cache(todo_camera)
 
     def update_camera_render_cache(self, camera: object):
 
         render_position = self.get_render_position(camera)
 
-
         if camera.is_renderable(render_position):
 
             # remove sprite reference
             # to update reference
             # only if was rendered before
             if camera.last_sprite_cache_dict.get(self) != None:
 
@@ -193,15 +189,14 @@
                     # if no sprite is rendered at this position in this line remove the position of the line from "row_render_dict"
                     del camera.row_render_dict[sprite_path["y"]][sprite_path["x"]]
 
                     # if no sprite is rendered at this line remove the line entirely
                     if camera.row_render_dict[sprite_path["y"]] == {}:
                         del camera.row_render_dict[sprite_path["y"]]
 
-
             if camera.row_render_dict.get(render_position["y"]) == None:
                 camera.row_render_dict[render_position["y"]] = {}
 
             if camera.row_render_dict[render_position["y"]].get(render_position["x"]) == None:
                 camera.row_render_dict[render_position["y"]][render_position["x"]] = []
 
             camera.row_render_dict[render_position["y"]][render_position["x"]].append(self)
@@ -242,18 +237,16 @@
             # delete group if no one is in it.
             del self.canvas_owner.sprite_group_dict[self.group]
             self.canvas_owner.group_tree.remove(self.group)
 
         # delete render cache in all cameras that are linked
         for todo_camera in self.canvas_owner.camera_tree:
 
-
             if self in todo_camera.last_sprite_cache_dict:
 
-
                 if todo_camera.last_sprite_cache_dict[self] != {}:
                     sprite_path = todo_camera.last_sprite_cache_dict[self]
                     sprite_row_list = todo_camera.row_render_dict[sprite_path["y"]][sprite_path["x"]]
                     sprite_row_list.remove(self)
 
                     if sprite_row_list == []:
                         # if no sprite is rendered at this position in this line remove the position of the line from "row_render_dict"
@@ -382,18 +375,17 @@
 
     def change_position(self, x_val: int = 0, y_val: int = 0):
 
         self.position["x"] += x_val
         self.position["y"] += y_val
         self.update_all_cameras_render_cache()
 
-
     def get_render_position(self, camera):
 
-        return {"x" : self.position["x"] + camera.position["x"], "y" : self.position["y"] + camera.position["y"]}
+        return {"x": self.position["x"] + camera.position["x"], "y": self.position["y"] + camera.position["y"]}
 
 
 class Camera:
     """
     Object that can render a part of a canvas at a given position with a given size using " render() "
     """
 
@@ -411,26 +403,24 @@
         self.name = name
         '''last cache of every sprite'''
         self.last_sprite_cache_dict = {}
         '''Dictionary that contain "y" as a key and a list filled with Dictionaries that are like this : "x" as a key and a sprite reference as a value
             so :  {"y" : {"x" : sprite_reference_here} '''
         self.row_render_dict = {}
 
-
         if size == [0, 0]:
             warn(
                 f''' size of camera : "{name}" isn't defined so it will most likely not work.\n please define a valid size.'''
             )
 
-        self.canvas_owner.camera_tree.append(self)
+        self.canvas_owner.camera_tree.add(self)
         self.canvas_owner.camera_name_dict[self.name] = self
 
     def is_renderable(self, position):
 
-
         return position["x"] >= 0 and position["x"] < self.size["x"] and position[
             "y"] >= 0 and position["y"] < self.size["y"]
 
     def render(self, is_string=True):
         """
         Returns the rendered canvas as a string if "is_string" is true else as a 2D-list
         """
@@ -444,48 +434,57 @@
         number_of_row_to_render = len(self.row_render_dict)
         last_row = 0
 
         if len(rows) == 0:
             # nothing to render
             canvas = line * self.size["y"]
             return canvas
+        else:
+            last_row = rows[0]
 
-        canvas += line * (rows[0] - 1)  # adds line before the first one
+        canvas += line * (rows[0])  # adds line before the first one
 
         for todo_row in rows:
 
             number_to_fill_up = todo_row - 1 - last_row
+
             if number_to_fill_up > 0:
                 canvas += line * number_to_fill_up
             del number_to_fill_up
             last_row = todo_row
 
             x_to_render_line = list(self.row_render_dict[todo_row].keys())
             x_to_render_line.sort()
             render_line = ""
             sprites_to_render = len(x_to_render_line)
+            items_rendered = 0  # also includes void
+
+            # todo_line is the character position that gets rendered
 
             for todo_line in x_to_render_line:
 
                 # fill up with "void" until something to render
-                number_to_fill_up = abs((len(render_line) - todo_line))
+                number_to_fill_up = (todo_line - items_rendered)
                 if number_to_fill_up > 0:
                     # if there is something that can be filled up
                     render_line += self.canvas_owner.void * number_to_fill_up
+                    items_rendered += number_to_fill_up
 
                 del number_to_fill_up
 
                 row_dict = self.row_render_dict[todo_row]
                 render_line += row_dict[todo_line][0].char
+                items_rendered += 1
                 sprites_to_render -= 1
 
                 if sprites_to_render == 0:
                     # if nothing else to render on this line we fill up the line with "void"
-                    number_to_fill_up = (self.size["x"] - len(render_line))
+                    number_to_fill_up = self.size["x"] - (todo_line + 1)
                     render_line += self.canvas_owner.void * number_to_fill_up + "\n"
+                    items_rendered += number_to_fill_up
                     canvas += render_line
                     del number_to_fill_up
                     break
 
             number_of_row_to_render -= 1
             if number_of_row_to_render <= 0:
                 # prob not here
@@ -553,18 +552,18 @@
     def kill(self):
         self.canvas_owner.camera_tree.remove(self)
         del self.canvas_owner.camera_name_dict[self.name]
         del self
 
 
 class Structure(Sprite):
-
     __slots__ = "canvas_owner", "structure", "position", "name", "group", "is_space_empty", "structure_sprite_tree"
 
-    def __init__(self, canvas_owner : object, structure : io.TextIOWrapper , position, name, group=None, is_space_empty=True):
+    def __init__(self, canvas_owner: object, structure: io.TextIOWrapper, position, name, group=None,
+                 is_space_empty=True):
 
         self.canvas_owner = canvas_owner
         self.position = position
         self.group = group
         self.is_space_empty = is_space_empty
         self.name = name
 
@@ -574,48 +573,41 @@
 
         if name in canvas_owner.structure_tree:
             self.name = f"@{name}{str(id(self))}"
 
         canvas_owner.structure_tree.add(self.name)
         canvas_owner.structure_dict[self.name] = self
 
-
         todo = 0
         lines = structure.readlines()
 
         for y in range(len(lines)):
 
             line_length = len(lines[todo])
             todo += 1
             for x in range(line_length):
                 char = lines[y][x]
 
-
                 if char != "\n":
 
-                    if not (is_space_empty == True  and char == " "):
-
-                        structure_sprite = StructureSprite(canvas_owner, char, {"x" : x, "y" : y}, "struc", self)
-
-
+                    if not (is_space_empty == True and char == " "):
+                        structure_sprite = StructureSprite(canvas_owner, char, {"x": x, "y": y}, "struc", self)
 
     def update_all_sprite_child(self):
         for todo_child_sprite in self.structure_sprite_tree:
             todo_child_sprite.update_all_cameras_render_cache()
 
     def set_x(self, value: int):
         self.position["x"] = value
         self.update_all_sprite_child()
 
-
     def change_x(self, value: int):
         self.position["x"] += value
         self.update_all_sprite_child()
 
-
     def set_y(self, value: int):
         self.position["y"] = value
         self.update_all_sprite_child()
 
     def change_y(self, value: int):
         self.position["y"] += value
         self.update_all_sprite_child()
@@ -625,45 +617,43 @@
         self.update_all_cameras_render_cache()
 
     def change_position(self, x_val: int = 0, y_val: int = 0):
         self.position["x"] += x_val
         self.position["y"] += y_val
         self.update_all_cameras_render_cache()
 
-
     def kill(self):
 
         for todo_child_sprite in self.structure_sprite_tree:
-
             todo_child_sprite.kill()
 
         del self
-class StructureSprite(Sprite):
 
 
-        __slots__ = "canvas_owner", "char", "position", "name", "group" , "structure_owner"
+class StructureSprite(Sprite):
+    __slots__ = "canvas_owner", "char", "position", "name", "group", "structure_owner"
 
-        def __init__(
-                self,
-                canvas_owner: object,
-                char: str,
-                position: dict,
-                name: str,
-                structure_owner: object,
-                group=None
-
-        ):
-            self.structure_owner = structure_owner
-            self.register_info(canvas_owner, char, position, name, group)
-            self.structure_owner.structure_sprite_tree.append(self)
+    def __init__(
+            self,
+            canvas_owner: object,
+            char: str,
+            position: dict,
+            name: str,
+            structure_owner: object,
+            group=None
 
+    ):
+        self.structure_owner = structure_owner
+        self.register_info(canvas_owner, char, position, name, group)
+        self.structure_owner.structure_sprite_tree.add(self)
 
-        def get_render_position(self, camera):
+    def get_render_position(self, camera):
+        return {"x": self.position["x"] + camera.position["x"] + self.structure_owner.position["x"],
+                "y": self.position["y"] + camera.position["y"] + self.structure_owner.position["y"]}
 
-            return {"x" : self.position["x"]  + camera.position["x"] + self.structure_owner.position["x"], "y" : self.position["y"] + camera.position["y"] + self.structure_owner.position["y"] }
 
 def critic_test(size, amount, time_mid, is_print=True):
     canvas = Canvas("0")
     camera = Camera(canvas, {"x": size, "y": size}, {"x": 0, "y": 0}, "camera")
 
     for i in range(amount):
         s1 = Sprite(canvas, "0", {"x": i, "y": 0}, "s1")
```

### Comparing `Oz-Engine-1.3.0/README.md` & `Oz-Engine-1.3.0.1/README.md`

 * *Files identical despite different names*

