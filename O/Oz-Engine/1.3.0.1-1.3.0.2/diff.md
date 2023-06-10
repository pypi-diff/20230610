# Comparing `tmp/Oz-Engine-1.3.0.1.tar.gz` & `tmp/Oz_Engine-1.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Oz-Engine-1.3.0.1.tar", last modified: Sat Jun 10 09:46:30 2023, max compression
+gzip compressed data, was "Oz_Engine-1.3.0.2.tar", last modified: Sat Jun 10 10:38:58 2023, max compression
```

## Comparing `Oz-Engine-1.3.0.1.tar` & `Oz_Engine-1.3.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.805392 Oz-Engine-1.3.0.1/
--rw-rw-rw-   0        0        0    35823 2023-02-15 15:44:32.000000 Oz-Engine-1.3.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.797882 Oz-Engine-1.3.0.1/Oz-Engine/
--rw-rw-rw-   0        0        0       19 2023-06-10 09:44:23.000000 Oz-Engine-1.3.0.1/Oz-Engine/__init__.py
--rw-rw-rw-   0        0        0    25352 2023-06-08 16:57:22.000000 Oz-Engine-1.3.0.1/Oz-Engine/main.py
-drwxrwxrwx   0        0        0        0 2023-06-10 09:46:30.803880 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/
--rw-rw-rw-   0        0        0      349 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-10 09:46:30.000000 Oz-Engine-1.3.0.1/Oz_Engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      349 2023-06-10 09:46:30.805392 Oz-Engine-1.3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1791 2023-02-27 20:06:32.000000 Oz-Engine-1.3.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-10 09:46:30.806401 Oz-Engine-1.3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      446 2023-06-10 09:46:00.000000 Oz-Engine-1.3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:38:58.591859 Oz_Engine-1.3.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-02-15 15:44:32.000000 Oz_Engine-1.3.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-10 10:38:58.584860 Oz_Engine-1.3.0.2/Oz_Engine/
+-rw-rw-rw-   0        0        0       19 2023-06-10 09:44:23.000000 Oz_Engine-1.3.0.2/Oz_Engine/__init__.py
+-rw-rw-rw-   0        0        0    25352 2023-06-08 16:57:22.000000 Oz_Engine-1.3.0.2/Oz_Engine/main.py
+drwxrwxrwx   0        0        0        0 2023-06-10 10:38:58.590860 Oz_Engine-1.3.0.2/Oz_Engine.egg-info/
+-rw-rw-rw-   0        0        0      349 2023-06-10 10:38:58.000000 Oz_Engine-1.3.0.2/Oz_Engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-06-10 10:38:58.000000 Oz_Engine-1.3.0.2/Oz_Engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 10:38:58.000000 Oz_Engine-1.3.0.2/Oz_Engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-10 10:38:58.000000 Oz_Engine-1.3.0.2/Oz_Engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      349 2023-06-10 10:38:58.590860 Oz_Engine-1.3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2023-06-10 09:49:25.000000 Oz_Engine-1.3.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-10 10:38:58.591859 Oz_Engine-1.3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      446 2023-06-10 10:38:18.000000 Oz_Engine-1.3.0.2/setup.py
```

### Comparing `Oz-Engine-1.3.0.1/LICENSE` & `Oz_Engine-1.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Oz-Engine-1.3.0.1/Oz-Engine/main.py` & `Oz_Engine-1.3.0.2/Oz_Engine/main.py`

 * *Files identical despite different names*

### Comparing `Oz-Engine-1.3.0.1/README.md` & `Oz_Engine-1.3.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 It can be used to make games in:
 * **Terminal**  
 * **Discord** 
 * [**Microbit**](https://github.com/menitoon/Oz-Engine-Microbit-version)
 * **Any matrix-led screen**
 
 
-![](https://thumbs.gfycat.com/ScientificTatteredCardinal-size_restricted.gif)  ![](https://thumbs.gfycat.com/AcclaimedAlienatedGiraffe-size_restricted.gif)  
+![](https://thumbs.gfycat.com/ScientificTatteredCardinal-size_restricted.gif) 
+![](https://thumbs.gfycat.com/AcclaimedAlienatedGiraffe-size_restricted.gif)  
+![](https://cdn.discordapp.com/attachments/1075772045142528060/1113350382400319508/2023-05-31_07-38-59.gif)
 
+_Games like **[Connect-4](https://github.com/menitoon/Connect-4-with-Oz-Engine), [Snake](https://github.com/menitoon/Snake-Microbit-with-Oz-Engine) and [Conway's Game of Life](https://github.com/menitoon/Conway-s-Game-of-Life-with-Oz-Engine)** have been made in Oz-Engine._
 
 ## Features
 
 * Sprites
 * Handling Collision 
 * Calling Groups 
 * Camera Support
```

