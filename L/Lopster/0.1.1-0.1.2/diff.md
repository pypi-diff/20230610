# Comparing `tmp/Lopster-0.1.1.tar.gz` & `tmp/Lopster-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.1.1.tar", last modified: Sat Jun 10 07:42:29 2023, max compression
+gzip compressed data, was "Lopster-0.1.2.tar", last modified: Sat Jun 10 08:06:15 2023, max compression
```

## Comparing `Lopster-0.1.1.tar` & `Lopster-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.232725 Lopster-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.217155 Lopster-0.1.1/Lopster/
--rw-rw-rw-   0        0        0     8833 2023-06-10 07:42:07.000000 Lopster-0.1.1/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.232725 Lopster-0.1.1/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-10 07:42:29.232725 Lopster-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-10 07:42:29.232725 Lopster-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-10 07:42:27.000000 Lopster-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.086931 Lopster-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.055672 Lopster-0.1.2/Lopster/
+-rw-rw-rw-   0        0        0    10302 2023-06-10 08:04:38.000000 Lopster-0.1.2/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 08:06:15.086931 Lopster-0.1.2/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 08:06:14.000000 Lopster-0.1.2/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-10 08:06:15.086931 Lopster-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-10 08:06:15.086931 Lopster-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-10 08:02:52.000000 Lopster-0.1.2/setup.py
```

### Comparing `Lopster-0.1.1/Lopster/__init__.py` & `Lopster-0.1.2/Lopster/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     def visible(self, typ):
         self.typ = typ
 
     def cash(self):
         text = []
 
         text.append("Enemy\n")
-        text.append("x = " + self.x + "\n")
-        text.append("y = " + self.y + "\n")
-        text.append("h = " + self.h + "\n")
-        text.append("w = " + self.w + "\n")
+        text.append("x = " + str(self.x) + "\n")
+        text.append("y = " + str(self.y) + "\n")
+        text.append("h = " + str(self.h) + "\n")
+        text.append("w = " + str(self.w) + "\n")
         text.append("func update = " +
                     inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @update\n")
         text.append(";")
 
         return "".join(text)
 
@@ -159,14 +159,30 @@
         if self.count >= len(self.srcList):
             self.count = 0
         else:
             pygame.time.delay(self.speed)
             window.blit(pygame.transform.scale(pygame.image.load(self.srcList[self.count]), self.size), (self.x, self.y))
             self.count += 1
 
+    def cash(self):
+        text = []
+
+        text.append("Player\n")
+        text.append("x = " + str(self.x) + "\n")
+        text.append("y = " + str(self.y) + "\n")
+        text.append("h = " + str(self.h) + "\n")
+        text.append("w = " + str(self.w) + "\n")
+        text.append("src = " + self.src + "\n")
+        text.append("speed = " + str(self.speed) + "\n")
+        text.append("size = " + str(self.size) + "\n")
+        text.append("func update = " +
+                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
+        text.append("init @x @y @h @w @src @size @speed @update\n")
+        text.append(";")
+
 class Text(Enemy):
     def __init__(self, _x, _y, _h, _w, _update):
         super().__init__(_x, _y, _h, _w, _update)
 
     def draw(self, window, fontName, fontSize, text, color):
         font = pygame.font.Font(fontName, fontSize)
         _text = font.render(text, True, color)
@@ -237,44 +253,59 @@
 #         self.src = src
 #
 #     def cash(self):
 #         text = []
 #         for obj in Enemy._object:
 #             text.append(obj.cash())
 #
-#
 #         with open(self.src, "w") as file:
 #             file.write("\n".join(text))
 #
 #     def casher(self):
 #         with open(self.src, "r") as file:
 #             texts = file.read().split(";")
 #
 #             i = 0
-#             while i<len(texts):
+#             while i < len(texts):
 #                 text = texts[i].split("\n")
 #
-#                 y = 0
+#                 variables = {}
+#                 functions = {}
+#
+#                 for line in text:
+#                     line = line.strip()
+#                     if not line:
+#                         continue
+#
+#                     if line.startswith("["):
+#                         class_name = line[1:-1]
+#                         instance_name = text[text.index(line) + 1].strip()
+#                         variables[instance_name] = {}
+#
+#                     elif line.startswith("dec"):
+#                         parts = line.split(" ")
+#                         function_name = parts[1]
+#                         function_body = " ".join(parts[2:])
 #
-#                 while y < len(text):
-#                     line = text[y].replace("^\s+", "").split(" ")
-#                     var = dict()
-#                     com = line[0]
-#                     if com == "func":
-#                         pass
-#                     else:
-#                         if len(line) == 1:
-#                             pass
-#                         else:
-#                             if line[1] == "=":
-#                                 var[com] = " ".join(line[2:len(line)])
+#                         functions[function_name] = eval(function_body, variables)
+#
+#                     elif line.startswith("init"):
+#                         parts = line.split(" ")
+#                         instance_name = parts[1]
+#                         arguments = parts[2:]
+#
+#                         instance_variables = variables[instance_name]
+#                         for i, argument in enumerate(arguments):
+#                             if argument.startswith("@"):
+#                                 variable_name = argument[1:]
+#                                 argument_value = variables[variable_name]
 #                             else:
-#                                 print("Unknown value '"+com+"' in cache '"+self.src+"'")
-#                     y += 1
-#                     print(var)
+#                                 argument_value = eval(argument, variables)
+#                             instance_variables[f"arg{i+1}"] = argument_value
+#
 #                 i += 1
 
 class RunLopster:
     _fps = 16
 
     def __init__(self, window_size, title, icon, update, fps):
         self._window_size = window_size
@@ -313,8 +344,8 @@
                     obj.update(window, obj)
 
             pygame.display.update()
 
         pygame.quit()
 
 
-__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
+__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster', 'Sprite']
```

