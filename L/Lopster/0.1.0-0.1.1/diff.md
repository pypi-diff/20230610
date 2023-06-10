# Comparing `tmp/Lopster-0.1.0.tar.gz` & `tmp/Lopster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.1.0.tar", last modified: Sat Jun 10 06:59:56 2023, max compression
+gzip compressed data, was "Lopster-0.1.1.tar", last modified: Sat Jun 10 07:42:29 2023, max compression
```

## Comparing `Lopster-0.1.0.tar` & `Lopster-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 06:59:56.046046 Lopster-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-10 06:59:56.014802 Lopster-0.1.0/Lopster/
--rw-rw-rw-   0        0        0     8022 2023-06-10 06:59:00.000000 Lopster-0.1.0/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 06:59:56.046046 Lopster-0.1.0/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-10 06:59:55.000000 Lopster-0.1.0/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-06-10 06:59:55.000000 Lopster-0.1.0/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 06:59:55.000000 Lopster-0.1.0/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 06:59:55.000000 Lopster-0.1.0/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 06:59:55.000000 Lopster-0.1.0/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-10 06:59:56.046046 Lopster-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-10 06:59:56.046046 Lopster-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-10 06:59:49.000000 Lopster-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.232725 Lopster-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.217155 Lopster-0.1.1/Lopster/
+-rw-rw-rw-   0        0        0     8833 2023-06-10 07:42:07.000000 Lopster-0.1.1/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 07:42:29.232725 Lopster-0.1.1/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 07:42:29.000000 Lopster-0.1.1/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-10 07:42:29.232725 Lopster-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-10 07:42:29.232725 Lopster-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-10 07:42:27.000000 Lopster-0.1.1/setup.py
```

### Comparing `Lopster-0.1.0/Lopster/__init__.py` & `Lopster-0.1.1/Lopster/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -135,14 +135,37 @@
         text.append("func update = " +
                     inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
         text.append("init @x @y @h @w @speed @update\n")
         text.append(";")
 
         return "".join(text)
 
+class Sprite(Enemy):
+    def __init__(self, _x, _y, _h, _w, src, size, _update, speed):
+        super().__init__(_x, _y, _h, _w, _update)
+        self.speed = speed
+        self.src = src
+        self.size = size
+        self.srcList = []
+        self.count = 0
+
+    def Animation(self, srcList):
+        self.srcList = srcList
+        self.count = 0
+
+    def draw(self, window):
+        window.blit(pygame.transform.scale(pygame.image.load(self.src), self.size), (self.x, self.y))
+
+    def anim(self, window):
+        if self.count >= len(self.srcList):
+            self.count = 0
+        else:
+            pygame.time.delay(self.speed)
+            window.blit(pygame.transform.scale(pygame.image.load(self.srcList[self.count]), self.size), (self.x, self.y))
+            self.count += 1
 
 class Text(Enemy):
     def __init__(self, _x, _y, _h, _w, _update):
         super().__init__(_x, _y, _h, _w, _update)
 
     def draw(self, window, fontName, fontSize, text, color):
         font = pygame.font.Font(fontName, fontSize)
```

