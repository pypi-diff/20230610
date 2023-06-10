# Comparing `tmp/textalloc-0.0.5.tar.gz` & `tmp/textalloc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-0.0.5.tar", last modified: Sat Mar  4 21:42:37 2023, max compression
+gzip compressed data, was "textalloc-0.0.6.tar", last modified: Sat Jun 10 07:41:33 2023, max compression
```

## Comparing `textalloc-0.0.5.tar` & `textalloc-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-03-04 21:42:37.425732 textalloc-0.0.5/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.0.5/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6356 2023-03-04 21:42:37.423543 textalloc-0.0.5/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     5784 2023-03-04 21:05:04.000000 textalloc-0.0.5/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      719 2023-03-04 21:32:25.000000 textalloc-0.0.5/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2023-03-04 21:42:37.426937 textalloc-0.0.5/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-03-04 21:42:37.140581 textalloc-0.0.5/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-03-04 21:42:37.270341 textalloc-0.0.5/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     7582 2023-03-04 19:43:04.000000 textalloc-0.0.5/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     3671 2023-02-14 19:18:58.000000 textalloc-0.0.5/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     5520 2023-02-14 19:18:58.000000 textalloc-0.0.5/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9003 2023-02-14 19:18:58.000000 textalloc-0.0.5/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-03-04 21:42:37.397541 textalloc-0.0.5/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6356 2023-03-04 21:42:37.000000 textalloc-0.0.5/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2023-03-04 21:42:37.000000 textalloc-0.0.5/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2023-03-04 21:42:37.000000 textalloc-0.0.5/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       22 2023-03-04 21:42:37.000000 textalloc-0.0.5/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2023-03-04 21:42:37.000000 textalloc-0.0.5/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-06-10 07:41:33.195928 textalloc-0.0.6/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-0.0.6/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6686 2023-06-10 07:41:33.194351 textalloc-0.0.6/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6114 2023-06-10 07:36:59.000000 textalloc-0.0.6/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      719 2023-06-10 07:40:41.000000 textalloc-0.0.6/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2023-06-10 07:41:33.196929 textalloc-0.0.6/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-06-10 07:41:32.931625 textalloc-0.0.6/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-06-10 07:41:33.065024 textalloc-0.0.6/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8847 2023-06-10 07:34:43.000000 textalloc-0.0.6/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     3890 2023-03-20 21:16:27.000000 textalloc-0.0.6/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6245 2023-03-20 21:46:25.000000 textalloc-0.0.6/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9916 2023-03-20 20:46:54.000000 textalloc-0.0.6/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2023-06-10 07:41:33.173258 textalloc-0.0.6/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6686 2023-06-10 07:41:32.000000 textalloc-0.0.6/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2023-06-10 07:41:32.000000 textalloc-0.0.6/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2023-06-10 07:41:32.000000 textalloc-0.0.6/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       22 2023-06-10 07:41:32.000000 textalloc-0.0.6/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2023-06-10 07:41:32.000000 textalloc-0.0.6/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-0.0.5/LICENSE` & `textalloc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-0.0.5/PKG-INFO` & `textalloc-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,42 +71,49 @@
     x-coordinates of all scattered points.
 y_scatter: (array-like), default None
     y-coordinates of all scattered points.
 x_lines: (array-like), default None
     x-coordinates of all lines in plot.
 y_lines: (array-like), default None
     y-coordinates of all lines in plot.
+scatter_sizes: (array-like), default None
+    sizes of all scattered objects in plot list of 1d arrays/lists.
+text_scatter_sizes: (array-like), default None
+    sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (int), default 10
     Size of text.
-margin: (float), default 0.01
+margin: (float), default 0.0
     Parameter for margins between objects.
     Increase for larger margins to points and lines.
     Given in proportion of ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
-max_distance: (float), default 0.07
+max_distance: (float), default 0.2
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
 linecolor: (str), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
-nbr_candidates: (int), default 100
+nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (str), default "k"
     Color code of the text.
+seed: (int), default 0
+    seeds order of text allocations.
+**kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The focus in this implementation is on speed and allocating as many text-boxes as possible into the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
```

### Comparing `textalloc-0.0.5/README.md` & `textalloc-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -56,42 +56,49 @@
     x-coordinates of all scattered points.
 y_scatter: (array-like), default None
     y-coordinates of all scattered points.
 x_lines: (array-like), default None
     x-coordinates of all lines in plot.
 y_lines: (array-like), default None
     y-coordinates of all lines in plot.
+scatter_sizes: (array-like), default None
+    sizes of all scattered objects in plot list of 1d arrays/lists.
+text_scatter_sizes: (array-like), default None
+    sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (int), default 10
     Size of text.
-margin: (float), default 0.01
+margin: (float), default 0.0
     Parameter for margins between objects.
     Increase for larger margins to points and lines.
     Given in proportion of ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
-max_distance: (float), default 0.07
+max_distance: (float), default 0.2
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
 linecolor: (str), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
-nbr_candidates: (int), default 100
+nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (str), default "k"
     Color code of the text.
+seed: (int), default 0
+    seeds order of text allocations.
+**kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The focus in this implementation is on speed and allocating as many text-boxes as possible into the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
```

### Comparing `textalloc-0.0.5/pyproject.toml` & `textalloc-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `textalloc-0.0.5/src/textalloc/__init__.py` & `textalloc-0.0.6/src/textalloc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,58 +11,70 @@
     x: Union[np.ndarray, List[float]],
     y: Union[np.ndarray, List[float]],
     text_list: List[str],
     x_scatter: Union[np.ndarray, List[float]] = None,
     y_scatter: Union[np.ndarray, List[float]] = None,
     x_lines: List[Union[np.ndarray, List[float]]] = None,
     y_lines: List[Union[np.ndarray, List[float]]] = None,
+    scatter_sizes: List[Union[np.ndarray, List[float]]] = None,
+    text_scatter_sizes: List[Union[np.ndarray, List[float]]] = None,
     textsize: int = 10,
-    margin: float = 0.01,
-    min_distance: float = 0.015,
-    max_distance: float = 0.07,
+    margin: float = 0.008,
+    min_distance: float = 0.013,
+    max_distance: float = 0.2,
     verbose: bool = False,
     draw_lines: bool = True,
     linecolor: str = "r",
     draw_all: bool = True,
-    nbr_candidates: int = 100,
+    nbr_candidates: int = 200,
     linewidth: float = 1,
     textcolor: str = "k",
+    seed: int = 0,
+    **kwargs,
 ):
     """Main function of allocating text-boxes in matplotlib plot
 
     Args:
         fig (_type_): matplotlib figure used for rendering textbox-sizes.
         ax (_type_): matplotlib axes used for plotting.
         x (Union[np.ndarray, List[float]]): x-coordinates of texts 1d array/list.
         y (Union[np.ndarray, List[float]]): y-coordinates of texts 1d array/list.
         text_list (List[str]): list of texts.
         x_scatter (Union[np.ndarray, List[float]], optional): x-coordinates of all scattered points in plot 1d array/list. Defaults to None.
         y_scatter (Union[np.ndarray, List[float]], optional): y-coordinates of all scattered points in plot 1d array/list. Defaults to None.
         x_lines (List[Union[np.ndarray, List[float]]], optional): x-coordinates of all lines in plot list of 1d arrays/lists. Defaults to None.
         y_lines (List[Union[np.ndarray, List[float]]], optional): y-coordinates of all lines in plot list of 1d arrays/lists. Defaults to None.
+        scatter_sizes (List[Union[np.ndarray, List[float]]], optional): sizes of all scattered objects in plot list of 1d arrays/lists. Defaults to None.
+        text_scatter_sizes (List[Union[np.ndarray, List[float]]], optional): sizes of text scattered objects in plot list of 1d arrays/lists. Defaults to None.
         textsize (int, optional): size of text. Defaults to 10.
-        margin (float, optional): parameter for margins between objects. Increase for larger margins to points and lines. Defaults to 0.01.
+        margin (float, optional): parameter for margins between objects. Increase for larger margins to points and lines. Defaults to 0.0.
         min_distance (float, optional): parameter for min distance between text and origin. Defaults to 0.015.
-        max_distance (float, optional): parameter for max distance between text and origin. Defaults to 0.07.
+        max_distance (float, optional): parameter for max distance between text and origin. Defaults to 0.2.
         verbose (bool, optional): prints progress using tqdm. Defaults to False.
         draw_lines (bool, optional): draws lines from original points to textboxes. Defaults to True.
         linecolor (str, optional): color code of the lines between points and text-boxes. Defaults to "r".
         draw_all (bool, optional): Draws all texts after allocating as many as possible despit overlap. Defaults to True.
-        nbr_candidates (int, optional): Sets the number of candidates used. Defaults to 0.
+        nbr_candidates (int, optional): Sets the number of candidates used. Defaults to 200.
         linewidth (float, optional): width of line. Defaults to 1.
         textcolor (str, optional): color code of the text. Defaults to "k".
+        seed (int, optional): seeds order of text allocations. Defaults to 0.
+        **kwargs (): kwargs for the plt.text() call.
     """
     t0 = time.time()
     xlims = ax.get_xlim()
     ylims = ax.get_ylim()
 
     # Ensure good inputs
     assert len(x) == len(y)
     x = np.array(x)
     y = np.array(y)
+    if scatter_sizes is not None:
+        scatter_sizes = np.array(scatter_sizes)
+    if text_scatter_sizes is not None:
+        text_scatter_sizes = np.array(text_scatter_sizes)
     if x_scatter is not None:
         assert y_scatter is not None
     if y_scatter is not None:
         assert x_scatter is not None
         assert len(y_scatter) == len(x_scatter)
         x_scatter = np.array(x_scatter)
         y_scatter = np.array(y_scatter)
@@ -74,14 +86,25 @@
             [len(x_line) == len(y_line) for x_line, y_line in zip(x_lines, y_lines)]
         )
         x_lines = [np.array(x_line) for x_line in x_lines]
         y_lines = [np.array(y_line) for y_line in y_lines]
     assert min_distance <= max_distance
     assert min_distance >= margin
 
+    # Seed
+    if seed > 0:
+        randinds = np.arange(x.shape[0])
+        np.random.seed(seed)
+        np.random.shuffle(randinds)
+        text_list = [text_list[i] for i in randinds]
+        x = x[randinds]
+        y = y[randinds]
+        if text_scatter_sizes is not None:
+            text_scatter_sizes = text_scatter_sizes[randinds]
+
     # Create boxes in original plot
     if verbose:
         print("Creating boxes")
     original_boxes = []
     for x_coord, y_coord, s in tqdm(zip(x, y, text_list), disable=not verbose):
         ann = ax.text(x_coord, y_coord, s, size=textsize)
         box = ax.transData.inverted().transform(
@@ -110,14 +133,16 @@
         min_distance,
         max_distance,
         verbose,
         nbr_candidates,
         draw_all,
         scatter_xy=scatterxy,
         lines_xyxy=lines_xyxy,
+        scatter_sizes=scatter_sizes,
+        text_scatter_sizes=text_scatter_sizes,
     )
 
     # Plot once again
     if verbose:
         print("Plotting")
     if draw_lines:
         for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
@@ -125,19 +150,21 @@
                 x_coord, y_coord, w, h, x[ind], y[ind]
             )
             if x_near is not None:
                 ax.plot(
                     [x[ind], x_near], [y[ind], y_near], linewidth=linewidth, c=linecolor
                 )
     for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
-        ax.text(x_coord, y_coord, s, size=textsize, c=textcolor)
+        ax.text(x_coord, y_coord, s, size=textsize, c=textcolor, **kwargs)
 
     if draw_all:
         for ind in overlapping_boxes_inds:
-            ax.text(x[ind], y[ind], text_list[ind], size=textsize, c=textcolor)
+            ax.text(
+                x[ind], y[ind], text_list[ind], size=textsize, c=textcolor, **kwargs
+            )
 
     if verbose:
         print(f"Finished in {time.time()-t0}s")
 
 
 def find_nearest_point_on_box(
     xmin: float, ymin: float, w: float, h: float, x: float, y: float
```

### Comparing `textalloc-0.0.5/src/textalloc/candidates.py` & `textalloc-0.0.6/src/textalloc/candidates.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,37 @@
     x: float,
     y: float,
     xmindistance: float,
     ymindistance: float,
     xmaxdistance: float,
     ymaxdistance: float,
     nbr_candidates: int,
+    scatter_size: float,
 ) -> np.ndarray:
     """Generates 36 candidate boxes
 
     Args:
         w (float): width of box
         h (float): height of box
         x (float): xmin of box
         y (float): ymin of box
         xmindistance (float): fraction of the x-dimension to use as margins for text bboxes
         ymindistance (float): fraction of the y-dimension to use as margins for text bboxes
         xmaxdistance (float): fraction of the x-dimension to use as max distance for text bboxes
         ymaxdistance (float): fraction of the y-dimension to use as max distance for text bboxes
         nbr_candidates (int): nbr of candidates to use. If <1 or >36 uses all 36
+        scatter_size (float): size of scattered text objects.
 
     Returns:
         np.ndarray: candidate boxes array
     """
+    xmindistance += scatter_size
+    ymindistance += scatter_size
+    xmaxdistance += scatter_size
+    ymaxdistance += scatter_size
     candidates = np.array(
         [
             [
                 x + xmindistance,
                 y + ymindistance,
                 x + w + xmindistance,
                 y + h + ymindistance,
```

### Comparing `textalloc-0.0.5/src/textalloc/non_overlapping_boxes.py` & `textalloc-0.0.6/src/textalloc/non_overlapping_boxes.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,25 +7,27 @@
     non_overlapping_with_boxes,
     inside_plot,
 )
 from tqdm import tqdm
 
 
 def get_non_overlapping_boxes(
-    original_boxes: np.ndarray,
+    original_boxes: list,
     xlims: Tuple[float, float],
     ylims: Tuple[float, float],
     margin: float,
     min_distance: float,
     max_distance: float,
     verbose: bool,
     nbr_candidates: int,
     draw_all: bool,
-    scatter_xy: np.ndarray = None,
-    lines_xyxy: np.ndarray = None,
+    scatter_xy: np.ndarray,
+    lines_xyxy: np.ndarray,
+    scatter_sizes: np.ndarray,
+    text_scatter_sizes: np.ndarray,
 ) -> Tuple[List[Tuple[float, float, float, float, str, int]], List[int]]:
     """Finds boxes that do not have an overlap with any other objects.
 
     Args:
         original_boxes (np.ndarray): original boxes containing texts.
         xlims (Tuple[float, float]): x-limits of plot gotten from ax.get_ylim()
         ylims (Tuple[float, float]): y-limits of plot gotten from ax.get_ylim()
@@ -33,14 +35,16 @@
         min_distance (float): parameter for max distance between text and origin.
         max_distance (float): parameter for max distance between text and origin.
         verbose (bool): prints progress using tqdm.
         nbr_candidates (int): Sets the number of candidates used.
         draw_all (bool): Draws all texts after allocating as many as possible despit overlap.
         scatter_xy (np.ndarray, optional): 2d array of scattered points in plot.
         lines_xyxy (np.ndarray, optional): 2d array of line segments in plot.
+        scatter_sizes (array-like): array of object sizes with centers in scatter_xy.
+        text_scatter_sizes (array-like): array of object sizes with centers in text objects.
 
     Returns:
         Tuple[List[Tuple[float, float, float, float, str, int]], List[int]]: data of non-overlapping boxes and indices of overlapping boxes.
     """
     xmin_bound, xmax_bound = xlims
     ymin_bound, ymax_bound = ylims
 
@@ -49,38 +53,51 @@
     xmindistance = (xmax_bound - xmin_bound) * min_distance
     ymindistance = (ymax_bound - ymin_bound) * min_distance
     xmaxdistance = (xmax_bound - xmin_bound) * max_distance
     ymaxdistance = (ymax_bound - ymin_bound) * max_distance
 
     box_arr = np.zeros((0, 4))
     non_overlapping_boxes = []
+    has_text_scatter_sizes = text_scatter_sizes is not None
+    if has_text_scatter_sizes:
+        assert len(text_scatter_sizes) == len(original_boxes)
+    if scatter_sizes is not None and scatter_xy is not None:
+        assert len(scatter_sizes) == scatter_xy.shape[0]
 
     # Iterate original boxes and find ones that do not overlap by creating multiple candidates
     non_overlapping_boxes = []
     overlapping_boxes_inds = []
     for i, box in tqdm(enumerate(original_boxes), disable=not verbose):
         x_original, y_original, w, h, s = box
+        text_scatter_size = 0
+        if has_text_scatter_sizes:
+            text_scatter_size = text_scatter_sizes[i]
         candidates = generate_candidates(
             w,
             h,
             x_original,
             y_original,
             xmindistance,
             ymindistance,
             xmaxdistance,
             ymaxdistance,
-            nbr_candidates=nbr_candidates,
+            nbr_candidates,
+            scatter_size=text_scatter_size,
         )
 
         # Check for overlapping
         if scatter_xy is None:
             non_op = np.zeros((candidates.shape[0],)) == 0
         else:
             non_op = non_overlapping_with_points(
-                scatter_xy, candidates, xmargin, ymargin
+                scatter_xy,
+                candidates,
+                xmargin,
+                ymargin,
+                scatter_sizes,
             )
         if lines_xyxy is None:
             non_ol = np.zeros((candidates.shape[0],)) == 0
         else:
             non_ol = non_overlapping_with_lines(
                 lines_xyxy, candidates, xmargin, ymargin
             )
```

### Comparing `textalloc-0.0.5/src/textalloc/overlap_functions.py` & `textalloc-0.0.6/src/textalloc/overlap_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 import numpy as np
 
 
 def non_overlapping_with_points(
-    scatter_xy: np.ndarray, candidates: np.ndarray, xmargin: float, ymargin: float
+    scatter_xy: np.ndarray,
+    candidates: np.ndarray,
+    xmargin: float,
+    ymargin: float,
+    scatter_sizes,
 ) -> np.ndarray:
     """Finds candidates not overlapping with points.
 
     Args:
         scatter_xy (np.ndarray): Array of shape (N,2) containing coordinates for all scatter-points
         candidates (np.ndarray): Array of shape (K,4) with K candidate boxes
         xmargin (float): fraction of the x-dimension to use as margins for text boxes
         ymargin (float): fraction of the y-dimension to use as margins for text boxes
 
     Returns:
         np.ndarray: Boolean array of shape (K,) with True for non-overlapping candidates with points
     """
-    return np.invert(
-        np.bitwise_or.reduce(
-            np.bitwise_and(
-                candidates[:, 0][:, None] - xmargin < scatter_xy[:, 0],
+    if scatter_sizes is None:
+        return np.invert(
+            np.bitwise_or.reduce(
                 np.bitwise_and(
-                    candidates[:, 2][:, None] + xmargin > scatter_xy[:, 0],
+                    candidates[:, 0][:, None] - xmargin < scatter_xy[:, 0],
                     np.bitwise_and(
-                        candidates[:, 1][:, None] - ymargin < scatter_xy[:, 1],
-                        candidates[:, 3][:, None] + ymargin > scatter_xy[:, 1],
+                        candidates[:, 2][:, None] + xmargin > scatter_xy[:, 0],
+                        np.bitwise_and(
+                            candidates[:, 1][:, None] - ymargin < scatter_xy[:, 1],
+                            candidates[:, 3][:, None] + ymargin > scatter_xy[:, 1],
+                        ),
                     ),
                 ),
-            ),
-            axis=1,
+                axis=1,
+            )
+        )
+    else:
+        return np.invert(
+            np.bitwise_or.reduce(
+                np.bitwise_and(
+                    candidates[:, 0][:, None] - (xmargin + scatter_sizes)
+                    < scatter_xy[:, 0],
+                    np.bitwise_and(
+                        candidates[:, 2][:, None] + (xmargin + scatter_sizes)
+                        > scatter_xy[:, 0],
+                        np.bitwise_and(
+                            candidates[:, 1][:, None] - (ymargin + scatter_sizes)
+                            < scatter_xy[:, 1],
+                            candidates[:, 3][:, None] + (ymargin + scatter_sizes)
+                            > scatter_xy[:, 1],
+                        ),
+                    ),
+                ),
+                axis=1,
+            )
         )
-    )
 
 
 def non_overlapping_with_lines(
     lines_xyxy: np.ndarray, candidates: np.ndarray, xmargin: float, ymargin: float
 ) -> np.ndarray:
     """Finds candidates not overlapping with lines
```

### Comparing `textalloc-0.0.5/src/textalloc.egg-info/PKG-INFO` & `textalloc-0.0.6/src/textalloc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 0.0.5
+Version: 0.0.6
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -71,42 +71,49 @@
     x-coordinates of all scattered points.
 y_scatter: (array-like), default None
     y-coordinates of all scattered points.
 x_lines: (array-like), default None
     x-coordinates of all lines in plot.
 y_lines: (array-like), default None
     y-coordinates of all lines in plot.
+scatter_sizes: (array-like), default None
+    sizes of all scattered objects in plot list of 1d arrays/lists.
+text_scatter_sizes: (array-like), default None
+    sizes of text scattered objects in plot list of 1d arrays/lists.
 textsize: (int), default 10
     Size of text.
-margin: (float), default 0.01
+margin: (float), default 0.0
     Parameter for margins between objects.
     Increase for larger margins to points and lines.
     Given in proportion of ax dimensions (0-1)
 min_distance: (float), default 0.015
     Parameter for min distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
-max_distance: (float), default 0.07
+max_distance: (float), default 0.2
     Parameter for max distance from textbox to
     its plotted position.
     Given in proportion of ax dimensions (0-1)
 verbose: (bool), default False
     prints progress using tqdm.
 draw_lines: (bool), default True
     draws lines from original points to textboxes.
 linecolor: (str), default "r"
     Color code of the lines between points and text-boxes.
 draw_all: (bool), default True
     Draws all texts after allocating as many as possible despite overlap.
-nbr_candidates: (int), default 100
+nbr_candidates: (int), default 200
     Sets the number of candidates used.
 linewidth: (float), default 1
     Width of line between textbox and it's origin.
 textcolor: (str), default "k"
     Color code of the text.
+seed: (int), default 0
+    seeds order of text allocations.
+**kwargs: (), kwargs for the plt.text() call.
 ```
 # Implementation and speed
 
 The focus in this implementation is on speed and allocating as many text-boxes as possible into the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
```

