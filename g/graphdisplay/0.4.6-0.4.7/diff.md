# Comparing `tmp/graphdisplay-0.4.6.tar.gz` & `tmp/graphdisplay-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.6.tar", last modified: Thu Jun  1 13:51:08 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.7.tar", last modified: Sat Jun 10 17:54:28 2023, max compression
```

## Comparing `graphdisplay-0.4.6.tar` & `graphdisplay-0.4.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.300131 graphdisplay-0.4.6/
--rw-rw-rw-   0        0        0     1088 2023-05-07 07:45:49.000000 graphdisplay-0.4.6/LICENSE
--rw-rw-rw-   0        0        0     6818 2023-06-01 13:51:08.299134 graphdisplay-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     6146 2023-06-01 11:38:53.000000 graphdisplay-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.278190 graphdisplay-0.4.6/graphdisplay/
--rw-rw-rw-   0        0        0      101 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/about_win_manager.py
--rw-rw-rw-   0        0        0     5199 2023-06-01 13:50:58.000000 graphdisplay-0.4.6/graphdisplay/general_config.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.292153 graphdisplay-0.4.6/graphdisplay/graphs/
--rw-rw-rw-   0        0        0       24 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/graphs/__init__.py
--rw-rw-rw-   0        0        0    23057 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/graphs/graph.py
--rw-rw-rw-   0        0        0     7686 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/json_manager.py
--rw-rw-rw-   0        0        0    36268 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.293150 graphdisplay-0.4.6/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/store/__init__.py
--rw-rw-rw-   0        0        0    17294 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/tools_win_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.298137 graphdisplay-0.4.6/graphdisplay/trees/
--rw-rw-rw-   0        0        0       88 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/auto_balance_tree.py
--rw-rw-rw-   0        0        0     3253 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/binary_search_tree.py
--rw-rw-rw-   0        0        0     6197 2023-06-01 13:39:52.000000 graphdisplay-0.4.6/graphdisplay/trees/binary_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:51:08.290157 graphdisplay-0.4.6/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     6818 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 13:51:08.000000 graphdisplay-0.4.6/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 13:51:08.300131 graphdisplay-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1763 2023-06-01 13:48:37.000000 graphdisplay-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.533296 graphdisplay-0.4.7/
+-rw-rw-rw-   0        0        0     1088 2023-05-07 07:45:49.000000 graphdisplay-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0     8112 2023-06-10 17:54:28.532298 graphdisplay-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     7440 2023-06-10 17:53:37.000000 graphdisplay-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.489007 graphdisplay-0.4.7/graphdisplay/
+-rw-rw-rw-   0        0        0     1390 2023-06-10 15:20:24.000000 graphdisplay-0.4.7/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     2364 2023-06-10 08:53:32.000000 graphdisplay-0.4.7/graphdisplay/about_win_manager.py
+-rw-rw-rw-   0        0        0     5241 2023-06-10 09:54:24.000000 graphdisplay-0.4.7/graphdisplay/general_config.py
+-rw-rw-rw-   0        0        0    39051 2023-06-10 15:58:23.000000 graphdisplay-0.4.7/graphdisplay/graphdisplay.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.514615 graphdisplay-0.4.7/graphdisplay/graphs/
+-rw-rw-rw-   0        0        0       24 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/graphs/__init__.py
+-rw-rw-rw-   0        0        0    23060 2023-06-07 15:39:55.000000 graphdisplay-0.4.7/graphdisplay/graphs/graph.py
+-rw-rw-rw-   0        0        0    12487 2023-06-10 16:08:07.000000 graphdisplay-0.4.7/graphdisplay/json_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.515612 graphdisplay-0.4.7/graphdisplay/store/
+-rw-rw-rw-   0        0        0        0 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/store/__init__.py
+-rw-rw-rw-   0        0        0    19130 2023-06-10 10:09:26.000000 graphdisplay-0.4.7/graphdisplay/tools_win_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.531299 graphdisplay-0.4.7/graphdisplay/trees/
+-rw-rw-rw-   0        0        0       88 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/__init__.py
+-rw-rw-rw-   0        0        0     3612 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-rw-   0        0        0     3159 2023-06-10 13:54:50.000000 graphdisplay-0.4.7/graphdisplay/trees/binary_search_tree.py
+-rw-rw-rw-   0        0        0     6197 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/binary_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.507631 graphdisplay-0.4.7/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     8112 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 17:54:28.533296 graphdisplay-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1763 2023-06-10 15:14:59.000000 graphdisplay-0.4.7/setup.py
```

### Comparing `graphdisplay-0.4.6/LICENSE` & `graphdisplay-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.6/PKG-INFO` & `graphdisplay-0.4.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.6
+Version: 0.4.7
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -33,89 +33,127 @@
 
 ## 📐Método de uso
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
 Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
-asignatura, por lo que también son importables.
-Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón. 
-Junto con el grafo, el resto de argumentos son los siguientes: 
-+ graph: es el objeto de tipo grafo/árbol que se va a representar **ES MUY IMPORTANTE** que éste sea implementado en base al código base de la asignatura. Si alguno
-de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la implementación de grafos que viene por defecto con el paquete.
-+ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos.
+asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
+**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
+o utilizar la implementación de grafos que viene por defecto con el paquete.
+Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
+gestiona el almacenado de grafos.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-```python
-from graphdisplay import GraphGUI, Graph
 
-g = Graph([1, 2, 3])
-g.addEdge(1, 2)
-g.addEdge(2, 3)
++ Para representar el siguiente grafo:
 
-# Para representar el grafo con todos los valores por defecto
-GraphGUI(g)
-
-# Para ajustar el radio de los nodos a 32, y el tema a 'dark'
-GraphGUI(g, node_radius=32, theme='dark')
-```
-Ejemplo con árboles binarios de búsqueda:
-```python
-from graphdisplay import GraphGUI, BinarySearchTree
-from random import randint
-
-tree = BinarySearchTree()
-for _ in range(80):
-    tree.insert(randint(1, 1000))
-   
-GraphGUI(tree)
-```
+     <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png' width='25%'/>
+    
+    Se podría disponer del siguiente código:
+    ```python
+    from graphdisplay import GraphGUI, Graph
+    
+    # Implementaremos el grafo de la siguiente imagen:
+    # https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png
+    
+    labels = ['A', 'B', 'C', 'D', 'E']
+    g = Graph(labels)
+    
+    g.addEdge('A', 'C', 12)  # A->(12)C
+    g.addEdge('A', 'D', 60)  # A->(60)D
+    g.addEdge('B', 'A', 10)  # B->(10)A
+    g.addEdge('C', 'B', 20)  # C->(20)B
+    g.addEdge('C', 'D', 32)  # C->(32)D
+    g.addEdge('E', 'A', 7)   # E->(7)A
+    
+    # Para representar el grafo 
+    if __name__ == "__main__":
+        GraphGUI(g)
+    ```
+
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/9210f5d4-4903-45ea-9bb8-e625890adac3' width='30%'/>
+  
++ Ejemplo con árboles binarios de búsqueda:
+
+    Para representar el siguiente árbol:
+
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1418ef2c-3215-4d88-93ce-3d1c67c4a58e' width='70%'/>
+    
+    Se dispondría del siguiente código:
+    ```python
+    from graphdisplay import GraphGUI, BinarySearchTree
+    
+    labels = [12, 4, 16, 2, 10, 14, 19, 1, 8, 13, 18, 20, 6, 24]
+    tree = BinarySearchTree()
+    for i in labels:
+        tree.insert(i)
+       
+    # Para representar el árbol
+    if __name__ == "__main__":
+        GraphGUI(tree)
+    ```
+    
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1e87b61d-d6fd-4635-bdf0-136509250de7' width='60%'/>
 
 ## ⚡️Funcionalidades
 Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
 éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
 instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
 Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
-después poder cargarlo en cualquier momento.
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
+después poder cargarlo (file>load) en cualquier momento.
 
 Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
 al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
 Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
 issue #16
+
+
 ## 🎯Ejemplos de uso
 
-Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
 from graphdisplay import GraphGUI, Graph
 
-labels = ['A', 'B', 'C', 'D', 'E']
-g = Graph(labels)
-
-# Now, we add the edges
-g.addEdge('A', 'C', 12)  # A->(12)C
-g.addEdge('A', 'D', 60)  # A->(60)D
-g.addEdge('B', 'A', 10)  # B->(10)A
-g.addEdge('C', 'B', 20)  # C->(20)B
-g.addEdge('C', 'D', 32)  # C->(32)D
-g.addEdge('E', 'A', 7)   # E->(7)A
-g.addEdge('A', 'E', 50)  # A->(50)E
-```
+my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
+my_gragph.addEdge('A', 'B', 4)
+my_gragph.addEdge('B', 'C', 8)
+my_gragph.addEdge('C', 'A', 100)
+my_gragph.addEdge('D', 'E', 7)
+my_gragph.addEdge('E', 'F', 10)
+my_gragph.addEdge('F', 'G', 5)
+my_gragph.addEdge('G', 'Z', 6)
+my_gragph.addEdge('A', 'H', 2)
+my_gragph.addEdge('B', 'I', 3)
+my_gragph.addEdge('C', 'J', 4)
+my_gragph.addEdge('D', 'K', 5)
+my_gragph.addEdge('E', 'L', 6)
+my_gragph.addEdge('F', 'D', 3)
+my_gragph.addEdge('G', 'H', 9)
+my_gragph.addEdge('H', 'Z', 2)
+my_gragph.addEdge('I', 'J', 1)
+my_gragph.addEdge('J', 'A', 6)
+my_gragph.addEdge('K', 'L', 5)
+my_gragph.addEdge('L', 'M', 4)
+my_gragph.addEdge('M', 'H', 3)
+my_gragph.addEdge('N', 'O', 2)
+my_gragph.addEdge('O', 'P', 1)
+my_gragph.addEdge('P', 'Q', 7)
+my_gragph.addEdge('H', 'A', 20)
+my_gragph.addEdge('K', 'B', 7)
+my_gragph.addEdge('H', 'N', 9)
+my_gragph.addEdge('Q', 'D', 40)
 
-Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
-
-```python
+if __name__ == "__main__":
     GraphGUI(g)
 ```
-Y nos mostrará la ventana:
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/0abc6d79-120e-470f-8d9b-7035e38def40" width="400" height="400">
 
-Sabiendo cómo instanciar grafos y reorganiando un poco los vértices, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 25, theme="la gran ola")`
+Y nos mostrará la ventana (reordenando los vértices):
 
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/a1edfcbf-4cec-4b08-98c6-709b87b7892d" width="800" height="500">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
 
 De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
 
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/3afa798a-28c3-4c6f-9357-8d849018dfa5" width="1000" height="480">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
```

### Comparing `graphdisplay-0.4.6/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.7/graphdisplay/about_win_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,23 +29,25 @@
         self.canvas.create_text(0, 147, text="An open source proyect made", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.canvas.create_text(0, 165, text="by and for students!", font=("Courier", 13),
                                 fill=self.__graphgui._AUTHOR_NAME_COLOR)
         self.running = True
         i = 0
         self.turtle.color(self.__graphgui._VERTEX_COLOR)
-        while self.running and i<92:
-            if i % 2 == 0:
-                self.turtle.penup()
-            else:
-                self.turtle.pendown()
-            if self.running:
+        try:
+            while self.running and i<92:
+                if i % 2 == 0:
+                    self.turtle.penup()
+                else:
+                    self.turtle.pendown()
                 self.turtle.forward(i + 1 + 5)
                 self.turtle.right(91)
-            i += 1
+                i += 1
+        except tk.TclError:
+            pass
 
     def __on_close(self):
         self.running = False
         self.destroy()
 
     def __open_github(self):
         webbrowser.open("https://github.com/seniorbeto/graphdisplay")
```

### Comparing `graphdisplay-0.4.6/graphdisplay/general_config.py` & `graphdisplay-0.4.7/graphdisplay/general_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-VERSION = '0.4.6'
+VERSION = '0.4.7'
 DEFAULT_SCR_WIDTH = 600
 DEFAULT_SCR_HEIGHT = 600
+DEFAULT_NODE_RADIUS = 25
+DEFAULT_THEME = 'BROWN'
 BUTTON_HEIGHT = 30
 BUTTON_WIDTH = 60
 XMARGEN = 7
 YMARGEN = 7
 THEMES = {
     "BROWN":{
         "BUTTON_COLOR": "#ede4cc",
         "SELECTED_VERTEX_COLOR": "#c2baa7",
         "VERTEX_COLOR": "#e3d7c5",
         "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
         "FRAME_COLOR": "#87715f",
         "AUTHOR_NAME_COLOR": "#301d05"
     },
+    "LIGHT":{
+        "BUTTON_COLOR": "#a6a6a6",
+        "SELECTED_VERTEX_COLOR": "#b3b3b3",
+        "VERTEX_COLOR": "#bfbdbd",
+        "BACKGROUND_CANVAS_COLOR": "#d4d3d2",
+        "FRAME_COLOR": "#b3b3b3",
+        "AUTHOR_NAME_COLOR": "#454545"
+    },
     "BLUE":{
         "BUTTON_COLOR": "#b7e7e8",
         "VERTEX_COLOR": "#a7d6fc",
         "SELECTED_VERTEX_COLOR": "#91b9ba",
         "BACKGROUND_CANVAS_COLOR": "#b5d9f7",
         "FRAME_COLOR": "#6aaade",
         "AUTHOR_NAME_COLOR": "#0b2d47"
     },
     "DARK":{
         "BUTTON_COLOR": "#6a6a7d",
         "SELECTED_VERTEX_COLOR": "#8d8da6",
         "VERTEX_COLOR": "#7d7d96",
         "BACKGROUND_CANVAS_COLOR": "#404147",
         "FRAME_COLOR": "#272729",
-        "AUTHOR_NAME_COLOR": "#c0c0f0"
-    },
-    "JESUSFUCKINGCHRIST":{
-        "BUTTON_COLOR": "#fffb00",
-        "SELECTED_VERTEX_COLOR": "#fffb00",
-        "VERTEX_COLOR": "#fffb00",
-        "BACKGROUND_CANVAS_COLOR": "#fffb00",
-        "FRAME_COLOR": "#fffb00",
-        "AUTHOR_NAME_COLOR": "#000000"
+        "AUTHOR_NAME_COLOR": "#7c7c9c"
     },
     "PURPLE":{
         "BUTTON_COLOR": "#f2c8fa",
         "SELECTED_VERTEX_COLOR": "#bf97c7",
         "VERTEX_COLOR": "#e7cdf7",
         "BACKGROUND_CANVAS_COLOR": "#e4c3fa",
         "FRAME_COLOR": "#d899f7",
@@ -64,31 +66,31 @@
     },
     "UBUNTU":{
         "BUTTON_COLOR": "#b35625",
         "SELECTED_VERTEX_COLOR": "#FFFFFF",
         "VERTEX_COLOR": "#d45102",
         "BACKGROUND_CANVAS_COLOR": "#404040",
         "FRAME_COLOR": "#303030",
-        "AUTHOR_NAME_COLOR": "#FFFFFF"
+        "AUTHOR_NAME_COLOR": "#b35625"
     },
     "LA NOCHE ESTRELLADA":{
         "BUTTON_COLOR": "#9bafaa",
         "SELECTED_VERTEX_COLOR": "#aed4eb",
         "VERTEX_COLOR": "#8fadbf",
         "BACKGROUND_CANVAS_COLOR": "#557491",
         "FRAME_COLOR": "#242d34",
         "AUTHOR_NAME_COLOR": "#d5bc6a"
     },
     "LA GRAN OLA":{
         "BUTTON_COLOR": "#a6a49b",
         "SELECTED_VERTEX_COLOR": "#d5bc6a",
-        "VERTEX_COLOR": "#e7e2d2",
+            "VERTEX_COLOR": "#e7e2d2",
         "BACKGROUND_CANVAS_COLOR": "#8599a4",
         "FRAME_COLOR": "#4a5f79",
-        "AUTHOR_NAME_COLOR": "#d5bc6a"
+        "AUTHOR_NAME_COLOR": "#2d3a4a"
     },
     "ANTARTICA":{
         "BUTTON_COLOR": "#9BA4B5",
         "SELECTED_VERTEX_COLOR": "#becde8",
         "VERTEX_COLOR": "#9BA4B5",
         "BACKGROUND_CANVAS_COLOR": "#394867",
         "FRAME_COLOR": "#212A3E",
@@ -96,15 +98,15 @@
     },
     "BREAKING BAD":{
         "BUTTON_COLOR": "#F7E1AE",
         "SELECTED_VERTEX_COLOR": "#b3a37f",
         "VERTEX_COLOR": "#F7E1AE",
         "BACKGROUND_CANVAS_COLOR": "#617A55",
         "FRAME_COLOR": "#3d4d36",
-        "AUTHOR_NAME_COLOR": "#F7E1AE"
+        "AUTHOR_NAME_COLOR": "#000000"
     },
     "SOFT":{
         "BUTTON_COLOR": "#E4D0D0",
         "SELECTED_VERTEX_COLOR": "#a89d9d",
         "VERTEX_COLOR": "#E4D0D0",
         "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
         "FRAME_COLOR": "#867070",
```

### Comparing `graphdisplay-0.4.6/graphdisplay/graphs/graph.py` & `graphdisplay-0.4.7/graphdisplay/graphs/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Ofitial graph implementation for Data Structures and Algorithms subject at Carlos III university of Madrid
+Official graph implementation for Data Structures and Algorithms subject at Carlos III university of Madrid
 
     - min_number_edges function implemented by Raúl Aguilar Arroyo (https://github.com/Ragarr)
     - transpose and is_strongly_connected functions implemented by Alberto Penas Díaz (https://github.com/seniorbeto)
       and Natalia Rodriguez Navarro (https://github.com/NataaNK)
 """
 import math
 
@@ -37,19 +37,19 @@
         if start not in self._vertices.keys():
             print(start, ' does not exist!')
             return
         if end not in self._vertices.keys():
             print(end, ' does not exist!')
             return
 
-        # adds to the end of the list of neigbours for start
+        # adds to the end of the list of neighbours for start
         self._vertices[start].append(AdjacentVertex(end, weight))
 
         if self._directed == False:
-            # adds to the end of the list of neigbours for end
+            # adds to the end of the list of neighbours for end
             self._vertices[end].append(AdjacentVertex(start, weight))
 
     def containsEdge(self, start, end):
         if start not in self._vertices.keys():
             print(start, ' does not exist!')
             return 0
         if end not in self._vertices.keys():
```

### Comparing `graphdisplay-0.4.6/graphdisplay/json_manager.py` & `graphdisplay-0.4.7/graphdisplay/json_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 import tkinter as tk
 from tkinter import messagebox
 from datetime import datetime
+from .general_config import *
 
 class JsonManager:
     def __init__(self, parent, graphgui):
         self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
 
         self.graphgui = graphgui
         self.__parent = parent
@@ -15,14 +16,28 @@
 
         try:
             with open(self.__JSON_SAVE_DIR + '../permanent.json', "r", encoding="utf-8", newline="") as file:
                 self.__permanent = json.load(file)
         except FileNotFoundError:
             self.__permanent = {}
 
+        try:
+            with open(self.__JSON_SAVE_DIR + '../win_config.json', "r", encoding="utf-8", newline="") as file:
+                self._config = json.load(file)
+        except FileNotFoundError:
+            self._config = {
+                'node_radius': DEFAULT_NODE_RADIUS,
+                'theme': DEFAULT_THEME
+            }
+            self.update_main_config()
+
+    def update_main_config(self):
+        with open(self.__JSON_SAVE_DIR + '../win_config.json', "w", encoding="utf-8", newline="") as file:
+            json.dump(self._config, file, indent=4)
+
     def update_permanent(self):
         with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
             json.dump(self.__permanent, file, indent=4)
 
     def delete_permanent(self, name: str):
         del self.__permanent[name]
         os.remove(self.__JSON_SAVE_DIR + name + '.json')
@@ -51,14 +66,102 @@
 
     def generate_load_window(self):
         LoadWindow(self.__parent, self)
 
     def generate_delete_window(self):
         DeleteWindow(self.__parent, self)
 
+    def generate_config_window(self):
+        ConfigWindow(self.__parent, self)
+
+class ConfigWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Config")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._FRAME_COLOR)
+
+        # Node configuration frame
+        self.__node_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
+        self.__node_frame.pack(padx=7, pady=7, expand=True)
+
+        # Theme configuration frame
+        self.__theme_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
+        self.__theme_frame.pack(padx=7, pady=7, expand=True)
+
+        # Node radius label
+        text_label = tk.Label(self.__node_frame,
+                              text="Node radius:",
+                              bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13))
+        text_label.place(x=5, y=7)
+
+        # Node radius Scale widget
+        self.__node_scale = tk.Scale(self.__node_frame,
+                                     from_=10,
+                                     to=100,
+                                     orient=tk.HORIZONTAL,
+                                     bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
+                                     troughcolor=self.__manager.graphgui._FRAME_COLOR,
+                                     highlightthickness=0,
+                                     length=150,
+                                     sliderlength=20)
+        self.__node_scale.set(self.__manager._config['node_radius'])
+        self.__node_scale.place(x=150, y=0)
+
+        # Theme label
+        text_label = tk.Label(self.__theme_frame,
+                                text="Theme:",
+                                bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
+                                font=("Courier", 13))
+        text_label.place(x=5, y=7)
+
+         # Theme Selection widget
+        self.__theme_selection = tk.StringVar(self)
+        self.__theme_selection.set(self.__manager._config['theme'])
+        self.__theme_option_menu = tk.OptionMenu(self.__theme_frame, self.__theme_selection, *THEMES)
+        self.__theme_option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR, bd=0, highlightthickness=0)
+        self.__theme_option_menu.place(x=150, y=9)
+
+        # Button frame
+        self.__button_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
+        self.__button_frame.pack(padx=7, pady=7, expand=True)
+
+        # Apply button
+        self.__apply_button = tk.Button(self.__button_frame,
+                                        text="Apply",
+                                        bg=self.__manager.graphgui._BUTTON_COLOR,
+                                        bd=0,
+                                        command=self.__apply__settings)
+        self.__apply_button.place(width=BUTTON_WIDTH,
+                                  height=BUTTON_HEIGHT,
+                                  x=160 - BUTTON_WIDTH / 2,
+                                  y=7)
+
+
+    def __apply__settings(self):
+        new_node_radius = self.__node_scale.get()
+        new_theme = self.__theme_selection.get()
+        self.__manager._config['node_radius'] = new_node_radius
+        self.__manager._config['theme'] = new_theme
+        self.__manager.update_main_config()
+
+        # Change the GUI theme
+        self.__manager.graphgui._theme = new_theme
+        self.__manager.graphgui.set_colors(new_theme)
+
+        # Change the node radius
+        self.__manager.graphgui.set_node_radius(new_node_radius)
+
+        # Update the GUI
+        current_position = self.__manager.graphgui.get_current_position()
+        self.__manager.graphgui.display_reset(current_position)
+
+
 class DeleteWindow(tk.Toplevel):
     def __init__(self, root, json_manager: JsonManager):
         super().__init__(root)
         self.title("Delete save")
         self.geometry("200x100")
         self.resizable(False, False)
         self.__manager = json_manager
@@ -172,13 +275,16 @@
     confirmation = input("WARNING: eliminating store. Do you want to proceed? [Y/N]: ")
     if confirmation == "Y":
         path = os.getcwd()
 
         if os.path.exists(os.path.join(path, "permanent.json")):
             os.remove(os.path.join(path, "permanent.json"))
 
+        if os.path.exists(os.path.join(path, "win_config.json")):
+            os.remove(os.path.join(path, "win_config.json"))
+
         store_path = os.path.join(path, "store/")
 
         for file in os.listdir(store_path):
             if file.endswith(".json"):
                 removing = os.path.join(store_path, file)
                 os.remove(removing)
```

### Comparing `graphdisplay-0.4.6/graphdisplay/main.py` & `graphdisplay-0.4.7/graphdisplay/graphdisplay.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,126 +7,109 @@
 import tkinter as tk
 import math
 import copy
 import time
 import queue
 import platform
 import multiprocessing as mp
+from typing import Any
 
 # Modules
 from .json_manager import JsonManager
 from .about_win_manager import AboutWindow
 from .tools_win_manager import ToolWindow
 from .graphs import Graph
 from .trees import AVLTree, BinarySearchTree
+from .trees.binary_tree import BinaryNode
 from .general_config import *
 
+class Node: ...
+class Edge: ...
+
+
+# Decorator builtin function for measure time
+def measure_time(func):
+    def wrapper(*args, **kwargs):
+        start = time.time()
+        func(*args, **kwargs)
+        print(f"\nFunction {func.__name__} Finished in: {time.time() - start}\n")
+    return wrapper
 
-class GraphGUI:
-    """
-    Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
-    :param graph: The graph/tree to be displayed.
-    :param node_radius: The radius of the nodes.
-    :param scr_width: The width of the window.
-    :param scr_height: The height of the window.
-    :param theme: color scheme of the node display.
-    """
 
-    # Using a instance-counter will determine how many GraphGUI objects are wanted
+class GraphGUI:
+    # Using an instance-counter will determine how many GraphGUI objects are wanted
     instance = 0
 
-    def __new__(cls, graph, node_radius: int = 30, theme: str = 'BROWN'):
+    def __new__(cls, graph: Any):
         GraphGUI.instance += 1
         if GraphGUI.instance > 5:
             raise Exception("For safety reasons, only five instances of GraphGUI can be created")
 
         # Generate multiprocessing
 
         if platform.system() == "Linux":
-            mp.Process(target=cls._generate, args=(graph,
-                                                    GraphGUI.instance,
-                                                    node_radius,
-                                                    theme)).start()
+            mp.Process(target=cls._generate, args=(graph, GraphGUI.instance)).start()
         else:
             try:
-                pid = mp.Process(target=cls._generate, args=(graph,
-                                                             GraphGUI.instance,
-                                                             node_radius,
-                                                             theme))
+                pid = mp.Process(target=cls._generate, args=(graph, GraphGUI.instance))
                 pid.start()
             except RecursionError:
                 print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "For how GraphGUI works, high-demanding recursion trees are"
                                                                  " not supported. Sorry for the inconvenience. ")
             except RuntimeError:
 
                 # For how multiprocessing works in python, it doesn't allow generating multiple processes
                 # without using a "if __name__ == "__main__":" statement. By implementing a try/expect, we
                 # can temporarily deal with this issue. Nevertheless, by doing this, there is a high chance
                 # to run into code-duplication and zombie processes generations.
 
                 print('\n'+'\033[93m'+"WARNING:"+'\033[0m'+" it is highly recommended to run the program inside a\n\n"
                       "     if __name__ == \"__main__\":\n\n"
                       "statement in order to avoid issues and duplicated processes.\n"
-                      "For more information please consider visiting the proyect \n"
+                      "For more information please consider visiting the project \n"
                       "documentation at: https://github.com/seniorbeto/graphdisplay\n")
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def __setattr__(self, name, value):
         return setattr(self.instance, name, value)
 
     @staticmethod
-    def _generate(graph, instance, node_radius, theme):
-        GraphGUI.__GraphGUI(graph, instance, node_radius, theme)
+    def _generate(graph, instance):
+        GraphGUI.__GraphGUI(graph, instance)
 
     class __GraphGUI:
-        def __init__(self, graph, instance, node_radius: int = 40, theme: str = 'BROWN'):
-            """
-            Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
-            The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
-            to create the GraphGUI object at the end of the program.
-            :param graph: The graph to be displayed
-            :param node_radius: The radius of the nodes (default 40)
-            :param scr_width: The width of the window (default 600)
-            :param scr_height: The height of the window (default 600)
-            """
-
+        def __init__(self, graph, instance):
             # Begin time measurement
             start = time.time()
 
-            # Parameter validation
-            if type(node_radius) != int:
-                raise TypeError("The parameter node_radius must be an integer")
-            if node_radius < 10 or node_radius > 100:
-                raise ValueError("The parameter node_radius must be a value between 10 and 100")
+            # Create the main window
+            self.root = tk.Tk()
+
+            # Create the json manager
+            self.json_manager = JsonManager(self.root, self)
 
             self.__ACTUAL_INSTANCE = instance
             self._graph = graph
-            self.__node_radius = node_radius
+            self.__node_radius = self.json_manager._config['node_radius']
             self.__scr_width = DEFAULT_SCR_WIDTH
             self.__scr_height = DEFAULT_SCR_WIDTH
             self.__XMARGIN = XMARGEN
             self.__YMARGIN = YMARGEN
-            self._theme = theme.upper()
-            self.nodes = []
+            self._theme = self.json_manager._config['theme']
+            self.nodes = {}
             self.edges = []
             self.__canvas_node_relation = {}
-            try:
-                self._BACKGROUND_CANVAS_COLOR = THEMES[theme.upper()]['BACKGROUND_CANVAS_COLOR']
-                self._BUTTON_COLOR = THEMES[theme.upper()]['BUTTON_COLOR']
-                self._SELECTED_VERTEX_COLOR = THEMES[theme.upper()]['SELECTED_VERTEX_COLOR']
-                self._FRAME_COLOR = THEMES[theme.upper()]['FRAME_COLOR']
-                self._VERTEX_COLOR = THEMES[theme.upper()]['VERTEX_COLOR']
-                self._AUTHOR_NAME_COLOR = THEMES[theme.upper()]['AUTHOR_NAME_COLOR']
-            except KeyError:
-                raise ValueError("The theme must be one of the following: " + str(list(THEMES.keys())))
+
+            # Set the color theme
+            self.set_colors(self._theme)
 
             # We will transform the graph type into our own prototype, so that future changes are easier
-            # to implement. Beyond this point, code will be implemented based on this prototypes.
+            # to implement. Beyond this point, code will be implemented based on these prototypes.
             try:
                 self.__tree_root = graph._root
                 self._is_tree = True
 
                 vertices = list(self.__levelorder(self.__tree_root).keys())
                 if type(graph) == AVLTree:
                     self._graph = AVLTree()
@@ -142,43 +125,36 @@
                 vertices = list(graph._vertices.keys())
                 self._graph = Graph(vertices)
 
                 for vertex in graph._vertices:
                     for adj in graph._vertices[vertex]:
                         self._graph.addEdge(vertex, adj._vertex, adj._weight)
 
-            # Create the main window
-            self.root = tk.Tk()
+            # Configure main window
             self.root.title('GraphGUI')
             self.root.geometry(f"{self.__scr_width}x{self.__scr_height}")
             self.root.configure(bg=self._FRAME_COLOR, border=0)
 
-            # Button Frame
-            self.button_frame = tk.Frame(self.root, bg=self._FRAME_COLOR,
-                                         height=self.__YMARGIN + BUTTON_HEIGHT)
-            self.button_frame.pack(fill='x', side='bottom')
-
             # Canvas Frame
             self.__canvas_frame = tk.Frame(self.root, bg=self._BACKGROUND_CANVAS_COLOR)
             self.__canvas_frame.pack(expand=1, fill='both', pady=self.__YMARGIN, padx=self.__XMARGIN)
 
             # Closing protocol
             self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
 
             # Canvas creation and placement
             self.canvas = tk.Canvas(self.__canvas_frame, bg=self._BACKGROUND_CANVAS_COLOR, bd=0,
                                     width=self.__scr_width - self.__XMARGIN * 2,
                                     height=self.__scr_height - self.__YMARGIN * 2 - BUTTON_HEIGHT)
             self.canvas.pack(fill='both', expand=1)
 
-            # Buttons display
-            self.__display_buttons()
+            # Menu display ( Experimental )
+            self.__menu_display()
 
             # Main display
-            self.json_manager = JsonManager(self.root, self)
             data = self.json_manager.get_data('__last_store_'+str(self.__ACTUAL_INSTANCE))
             self.__display(data)
             if data:
                 actual_scr_width = data['Screen_dimensions'][0]
                 actual_scr_height = data['Screen_dimensions'][1]
                 self.root.geometry(f'{actual_scr_width}x{actual_scr_height}')
 
@@ -187,361 +163,349 @@
             if self._is_tree and platform.system() != "Linux":
                 self.canvas.tag_bind("movil", "<Button-3>", self.on_press_left)
             self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
             self.selected_node = None
 
             # End time measurement
             end = time.time()
-            print("Displayed in:", round(end-start, 4))
+            print("\nDisplayed in:", round(end-start, 4))
+            print()
 
             # Main display protocol
             self.root.mainloop()
 
-        def __display_buttons(self):
-            # Reset button
-            self.reset_button = tk.Button(self.button_frame,
-                                          text="Reset",
-                                          bg=self._BUTTON_COLOR,
-                                          command=self.display_reset,
-                                          bd=0)
-            self.reset_button.place(x = self.__XMARGIN,
-                                    y = 0,
-                                    width=BUTTON_WIDTH,
-                                    height=BUTTON_HEIGHT)
-
-            # Load button
-            self.load_button = tk.Button(self.button_frame,
-                                         text="Load",
-                                         bg=self._BUTTON_COLOR,
-                                         command=self.__call_manager_load,
-                                         bd=0)
-            self.load_button.place(x=self.__XMARGIN + BUTTON_WIDTH + self.__XMARGIN,
-                                   y=0,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
-
-            # Save button
-            self.save_button = tk.Button(self.button_frame,
-                                         text="Save",
-                                         bg=self._BUTTON_COLOR,
-                                         command=self.__call_manager_save,
-                                         bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 2,
-                                   y=0,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
-
-            # Delete button
-            self.save_button = tk.Button(self.button_frame,
-                                         text="Delete",
-                                         bg=self._BUTTON_COLOR,
-                                         command=self.__call_manager_delete, bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 3,
-                                   y=0,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
-
-            # Tools button
-            self.save_button = tk.Button(self.button_frame,
-                                         text="Tools",
-                                         bg=self._BUTTON_COLOR,
-                                         command=self.__call_tools_window, bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 4,
-                                   y=0,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
-
-            # About button
-            self.save_button = tk.Button(self.button_frame,
-                                         text="About",
-                                         bg=self._BUTTON_COLOR,
-                                         command=self.__call_about_window, bd=0)
-            self.save_button.place(x=self.__XMARGIN + (BUTTON_WIDTH + self.__XMARGIN) * 5,
-                                   y=0,
-                                   width=BUTTON_WIDTH,
-                                   height=BUTTON_HEIGHT)
+        def set_colors(self, theme: str) -> None:
+            """Set the color theme for the GUI"""
+            try:
+                self._BACKGROUND_CANVAS_COLOR = THEMES[theme.upper()]['BACKGROUND_CANVAS_COLOR']
+                self._BUTTON_COLOR = THEMES[theme.upper()]['BUTTON_COLOR']
+                self._SELECTED_VERTEX_COLOR = THEMES[theme.upper()]['SELECTED_VERTEX_COLOR']
+                self._FRAME_COLOR = THEMES[theme.upper()]['FRAME_COLOR']
+                self._VERTEX_COLOR = THEMES[theme.upper()]['VERTEX_COLOR']
+                self._AUTHOR_NAME_COLOR = THEMES[theme.upper()]['AUTHOR_NAME_COLOR']
+            except KeyError:
+                raise ValueError("The theme must be one of the following: " + str(list(THEMES.keys())))
+
+        def __menu_display(self) -> None:
+            """It creates the menu bar and its options"""
+            self.__main_menu = tk.Menu(self.root)
+            self.root.config(menu=self.__main_menu)
+
+            self.__file_menu = tk.Menu(self.__main_menu, tearoff=False)
+            self.__main_menu.add_cascade(label='File', menu=self.__file_menu)
+
+            self.__file_menu.add_command(label='Save', command=self.__call_manager_save)
+            self.__file_menu.add_command(label='Reset', command=self.display_reset)
+            self.__file_menu.add_command(label='Load', command=self.__call_manager_load)
+            self.__file_menu.add_command(label='Delete', command=self.__call_manager_delete)
 
-        def __call_tools_window(self):
+            self.__main_menu.add_command(label='Tools', command=self.__call_tools_window)
+
+            self.__main_menu.add_command(label='About', command=self.__call_about_window)
+
+            self.__main_menu.add_command(label='Config', command=self.__call_manager_config)
+
+        def __call_tools_window(self) -> None:
             """Generator of ToolWindow"""
             ToolWindow(self.root, self)
 
-        def __call_about_window(self):
+        def __call_about_window(self) -> None:
             """Generator of AboutWindow"""
             AboutWindow(self.root, self)
 
-        def __call_manager_delete(self):
+        def __call_manager_config(self) -> None:
+            """Generator of ConfigWindow"""
+            self.json_manager.generate_config_window()
+
+        def __call_manager_delete(self) -> None:
             """Generator of Delete Window"""
             if not self._is_tree:
                 self.json_manager.generate_delete_window()
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
-        def __call_manager_load(self):
+        def __call_manager_load(self) -> None:
             """Generator of Load Window"""
             if not self._is_tree:
                 new_position = self.json_manager.generate_load_window()
                 if new_position:
                     self.display_reset(new_position)
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
-        def __call_manager_save(self):
+        def __call_manager_save(self) -> None:
             """Generator of Save Window"""
             if not self._is_tree:
-                curr_pos = {}
-                actual_scr_width = self.root.winfo_width()
-                actual_scr_height = self.root.winfo_height()
-                curr_pos['Screen_dimensions'] = (actual_scr_width, actual_scr_height)
-                for node in self.nodes:
-                    curr_pos[node.id] = (node.pos_x, node.pos_y)
+                curr_pos = self.get_current_position()
                 self.json_manager.generate_save_window(curr_pos)
             else:
                 tk.messagebox.showerror("Error", "This function is not yet available for trees")
 
-        def display_reset(self, new_data: dict = None):
+        def get_current_position(self) -> dict:
+            """Returns the current position of the nodes in the canvas"""
+            curr_pos = {}
+            actual_scr_width = self.root.winfo_width()
+            actual_scr_height = self.root.winfo_height()
+            curr_pos['Screen_dimensions'] = (actual_scr_width, actual_scr_height)
+            for node in self.nodes:
+                curr_pos[node] = (self.nodes[node].pos_x, self.nodes[node].pos_y)
+            return curr_pos
+
+        def display_reset(self, new_data: dict = None) -> None:
             """
             Sets the main display to default by deleting all objects in canvas and displaying them
             in the position stored in new_data.
             """
+            if new_data:
+                actual_scr_width = new_data['Screen_dimensions'][0]
+                actual_scr_height = new_data['Screen_dimensions'][1]
+                self.root.geometry(f'{actual_scr_width}x{actual_scr_height}')
             self.canvas.delete("all")
+            self.root.config(bg=self._FRAME_COLOR)
+            self.canvas.config(bg=self._BACKGROUND_CANVAS_COLOR)
             self.__display(new_data)
 
-        def __display(self, data: dict = None):
+        def __display(self, data: dict = None) -> None:
             """
-            Main display for all nodes in the canvas. Whose position is determined in "data".
+            Main display for all nodes in the canvas, whose position is determined in "data".
             If data is None, the default display will be showed. This is, in case of a simple graph,
             the first vertex in the middle of the screen and the rest surrounding it in a polygon shape.
             In case of a tree, it is always display in a tree-like structure.
 
             This function also checks if some node position has been stored outside the frames of the window,
             in which case will correct.
             """
             # First, we store the actual dimensions of the screen
             if data:
                 actual_scr_width = data['Screen_dimensions'][0]
                 actual_scr_height = data['Screen_dimensions'][1]
             else:
                 actual_scr_width = self.root.winfo_width()
                 actual_scr_height = self.root.winfo_height()
+                if actual_scr_height == 1 and actual_scr_width == 1:
+                    actual_scr_width = DEFAULT_SCR_WIDTH
+                    actual_scr_height = DEFAULT_SCR_HEIGHT
 
-            # Now, we will restrict the screen to the canvas dimensions
-            actual_scr_width -= self.__XMARGIN * 2
-            actual_scr_height -= self.__YMARGIN * 2 + BUTTON_HEIGHT
 
             if not self._is_tree:
                 # Preparation for the nodes display
-                scr_center = ((actual_scr_width - 14) // 2, (actual_scr_height - 30) // 2)
+                scr_center = ((actual_scr_width - (self.__XMARGIN*2)) // 2, (actual_scr_height - (self.__YMARGIN*2)) // 2)
                 display_radius = min(actual_scr_width - 30 - self.__node_radius, actual_scr_height - 14 - self.__node_radius) // 2 - self.__node_radius - 10
                 arch_angle = 360 / len(self._graph._vertices)
                 first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
 
                 # Display the nodes
-                self.nodes = []
+                self.nodes = {}
                 i = 0
                 angle = 0
                 for vertex in self._graph._vertices:
                     # The first vertex will be displayed in the screen center
                     if i == 0:
                         if data and str(vertex) in data and \
                                 data[str(vertex)][0] < actual_scr_width and \
                                 data[str(vertex)][1] < actual_scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
-                            self.nodes.append(
-                                Node(self.canvas,
+                            node = Node(self.canvas,
                                      self.__node_radius,
                                      data[str(vertex)][0],
                                      data[str(vertex)][1],
                                      text=vertex,
-                                     bg=self._VERTEX_COLOR))
+                                     bg=self._VERTEX_COLOR)
+                            self.nodes[vertex] = node
                         else:
-                            self.nodes.append(
-                                Node(self.canvas,
+                            node = Node(self.canvas,
                                      self.__node_radius,
                                      first_node_pos[0],
                                      first_node_pos[1],
                                      text=vertex,
-                                     bg=self._VERTEX_COLOR))
+                                     bg=self._VERTEX_COLOR)
+                            self.nodes[vertex] = node
                     else:
                         # Those vertices that are not the first, will surround the screen center, scrolling
                         # around an imaginary circumference.
                         if data and str(vertex) in data and \
                                 data[str(vertex)][0] < actual_scr_width and \
                                 data[str(vertex)][1] < actual_scr_height - 30 and \
                                 data[str(vertex)][0] + self.__node_radius*2 > 0 and \
                                 data[str(vertex)][1] + self.__node_radius*2 > 0:
-                            self.nodes.append(
-                                Node(self.canvas,
+                            node = Node(self.canvas,
                                      self.__node_radius,
                                      data[str(vertex)][0],
                                      data[str(vertex)][1],
                                      text=vertex,
-                                     bg=self._VERTEX_COLOR))
+                                     bg=self._VERTEX_COLOR)
+                            self.nodes[vertex] = node
                         else:
-                            self.nodes.append(Node(self.canvas,
+                            node = Node(self.canvas,
                                                    self.__node_radius,
                                                    int(scr_center[0] - self.__node_radius - display_radius * math.sin(
                                                        math.radians(angle))),
                                                    int(scr_center[1] - self.__node_radius - display_radius * math.cos(
                                                        math.radians(angle))),
-                                                   text=vertex, bg=self._VERTEX_COLOR))
+                                                   text=vertex, bg=self._VERTEX_COLOR)
+                            self.nodes[vertex] = node
                     i += 1
                     angle += arch_angle
+                    # We will store each canvas TAGorID with each associated node object in order
+                    # to reduce movement complexity to O(1) so that every time we want to look for a node
+                    # having its canvas TAGorID, we can do it in O(1) time.
+                    self.__canvas_node_relation[node.circle] = node
+                    self.__canvas_node_relation[node.text] = node
 
                 # Create the edges
                 i = 0
                 self.edges = []
                 for vertex in self._graph._vertices:
                     for adj in self._graph._vertices[vertex]:
-                        for node in self.nodes:
-                            if node.id == adj._vertex:
-                                self.edges.append(Edge(self.canvas,
-                                                       self.nodes[i],
-                                                       node,
-                                                       adj._weight,
-                                                       window_color=self._BACKGROUND_CANVAS_COLOR))
-                                node.asociated_edges_IN.append(self.edges[-1])
-                                self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
+                        node = self.nodes[adj._vertex]
+                        self.edges.append(Edge(self.canvas,
+                                               self.nodes[vertex],
+                                               node,
+                                               adj._weight,
+                                               window_color=self._BACKGROUND_CANVAS_COLOR,
+                                               text_color=self._AUTHOR_NAME_COLOR))
                     i += 1
 
                 # While displaying the edges, we first have to check if it is needed to display the weight
-                # in an edge side (instead of the center) in case that to vertices are pointing to each other,
-                # since this would result in an overlap between those to weights
+                # in an edge side (instead of the center) in case that two vertices are pointing to each other,
+                # since this would result in an overlap between those two weights.
                 if self._graph._directed:
                     for edge in self.edges:
                         edge_start_node = edge.start_node
                         edge_end_node = edge.end_node
                         found = False
-                        for i in edge_start_node.asociated_edges_IN:
+                        for i in edge_start_node.associated_edges_IN:
                             if i.start_node == edge_end_node:
                                 found = True
-                                edge.overlaped = True
+                                edge.overlapped = True
                                 edge.show()
                                 break
                         if not found:
                             edge.show()
                 else:
                     for edge in self.edges:
                         edge.show()
 
             elif self._is_tree:
-                # The tree display is slightly more complicated (it was a complete nightmare for a one man job
-                # to be honest). For information on how it works, please consider visiting: #TODO
-                self.nodes = []
+                # The tree display is slightly more complicated  For information, please consider visiting: #TODO
+                self.nodes = {}
                 self.edges = []
-                root_position = ((actual_scr_width - self.__node_radius*2) // 2, self.__YMARGIN + 33)
-                self.nodes.append(Node(self.canvas,
+                root_position = ((actual_scr_width - self.__node_radius*2) // 2, self.__YMARGIN + 3)
+                root_node = Node(self.canvas,
                                        self.__node_radius,
                                        root_position[0],
                                        root_position[1],
                                        text=self._graph._root.elem,
-                                       bg=self._VERTEX_COLOR))
+                                       bg=self._VERTEX_COLOR)
+                self.nodes[self._graph._root.elem] = root_node
+                # We will store each canvas TAGorID with each associated node object in order
+                # to reduce movement complexity to O(1) so that every time we want to look for a node
+                # having its canvas TAGorID, we can do it in O(1) time.
+                self.__canvas_node_relation[root_node.circle] = root_node
+                self.__canvas_node_relation[root_node.text] = root_node
 
                 # We display the rest of the nodes in a tree-like structure by
                 # dividing the screen in levels and displaying the nodes in each level
                 level_order = self.__levelorder(self._graph._root)
                 levels = max(level_order.values()) + 1
-                level_height = (actual_scr_height - self.__YMARGIN - 60) // levels
+                level_height = (actual_scr_height - self.__YMARGIN*2 - self.__node_radius) // levels
+                level_list = []
+                for _ in range(levels):
+                    level_list.append([])
+                for node in level_order:
+                    level_list[level_order[node]].append(node)
 
                 # We determine how many nodes are in each level
                 last_nodes = [self._graph._root.elem]
                 for i in range(levels - 1):
                     if i != 0:
                         last_nodes = nodes_in_level
-                    nodes_in_level = []
-                    for node in level_order:
-                        if level_order[node] == i + 1:
-                            nodes_in_level.append(node)
+                    nodes_in_level = level_list[i+1]
 
                     level_grid = 2**(i + 1)
 
                     # We determine the x_axis of each node in the level
                     x_axis = (actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2)) // level_grid
-                    x_axis_counter = 0
 
                     final_nodes = nodes_in_level + last_nodes
                     final_nodes.sort()
                     for node in last_nodes:
                         # We look for the position x of the father
-                        for aux in self.nodes:
-                            if node == aux.id:
-                                position_x = aux.pos_x
-                                father_node = aux
-                                break
-                        relative = last_nodes.index(node) + 1
+                        position_x = self.nodes[node].pos_x
+                        father_node: Node = self.nodes[node]
+
+                        # We look for the children of the current node
                         children_left, children_right = self.__get_children(node)
+
                         if children_left or children_left == 0:
                             final_position_x = position_x - x_axis // 2
                             if final_position_x <= self.__XMARGIN + 5:
                                 final_position_x = self.__XMARGIN + 5
+
                             new_node = Node(self.canvas,
                                             self.__node_radius,
                                             final_position_x,
                                             root_position[1] + level_height*(level_order[children_left]),
                                             text=children_left,
                                             bg=self._VERTEX_COLOR)
-                            self.nodes.append(new_node)
+                            self.nodes[children_left] = new_node
+                            self.__canvas_node_relation[new_node.circle] = new_node
+                            self.__canvas_node_relation[new_node.text] = new_node
                             new_edge = Edge(self.canvas,
                                             father_node,
                                             new_node,
                                             None,
-                                            window_color=self._BACKGROUND_CANVAS_COLOR)
+                                            window_color=self._BACKGROUND_CANVAS_COLOR,
+                                            text_color=self._AUTHOR_NAME_COLOR)
                             new_edge.show()
                             self.edges.append(new_edge)
-                            new_node.asociated_edges_IN.append(new_edge)
-                            father_node.asociated_edges_OUT.append(new_edge)
 
                         if children_right or children_right == 0:
                             final_position_x = position_x + x_axis // 2
                             if final_position_x >= actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5:
                                 final_position_x = actual_scr_width - (self.__XMARGIN * 2) - (self.__node_radius * 2) - 5
 
                             new_node = Node(self.canvas,
                                             self.__node_radius,
                                             final_position_x,
                                             root_position[1] + level_height*(level_order[children_right]),
                                             text=children_right,
                                             bg=self._VERTEX_COLOR)
-                            self.nodes.append(new_node)
+                            self.nodes[children_right] = new_node
+                            self.__canvas_node_relation[new_node.circle] = new_node
+                            self.__canvas_node_relation[new_node.text] = new_node
                             new_edge = Edge(self.canvas,
                                             father_node,
                                             new_node,
                                             None,
-                                            window_color=self._BACKGROUND_CANVAS_COLOR)
+                                            window_color=self._BACKGROUND_CANVAS_COLOR,
+                                            text_color=self._AUTHOR_NAME_COLOR)
                             new_edge.show()
                             self.edges.append(new_edge)
-                            new_node.asociated_edges_IN.append(new_edge)
-                            father_node.asociated_edges_OUT.append(new_edge)
-
-            # We will store each canvas TAGorID with each associated node object in order
-            # to reduce movement complexity to O(1)
-            self.__canvas_node_relation = {}
-            for node in self.nodes:
-                self.__canvas_node_relation[node.circle] = node
-                self.__canvas_node_relation[node.text] = node
 
         def __get_children(self, elem) -> tuple:
             """returns a tuple with the children of node with element = elem"""
             node = self.__search_node(elem)
             return node.left.elem if node.left else None, node.right.elem if node.right else None
 
-        def __search_node(self, elem):
+        def __search_node(self, elem) -> BinaryNode:
             """returns the node with the given element"""
             return self.__search_node_aux(self._graph._root, elem)
 
-        def __search_node_aux(self, node, elem):
+        def __search_node_aux(self, node: BinaryNode, elem) -> BinaryNode:
             """returns the node with the given element"""
             if node == None:
                 return None
             if node.elem == elem:
                 return node
             else:
                 return self.__search_node_aux(node.left, elem) or self.__search_node_aux(node.right, elem)
 
-        def __levelorder(self, node) -> dict:
+        def __levelorder(self, node: BinaryNode) -> dict:
             """
             returns a dictionary with the level order of the tree and the height of each node
             """
             register = {}
             q = queue.Queue()
             q.put(node)  # enqueue: we save the root
             register[node.elem] = 0
@@ -554,137 +518,250 @@
                     register[current.left.elem] = value + 1
                 if current.right != None:
                     q.put(current.right)
                     register[current.right.elem] = value + 1
 
             return register
 
-        def __on_closing(self):
+        def __on_closing(self) -> None:
             """Store the current data at closing protocol"""
             data = {}
             actual_scr_width = self.root.winfo_width()
             actual_scr_height = self.root.winfo_height()
             data['Screen_dimensions'] = (actual_scr_width, actual_scr_height)
             for node in self.nodes:
-                data[node.id] = (node.pos_x, node.pos_y)
+                data[node] = (self.nodes[node].pos_x, self.nodes[node].pos_y)
             self.json_manager.save_data('__last_store_'+str(self.__ACTUAL_INSTANCE), data)
+            self.json_manager.update_main_config()
             self.root.destroy()
 
-        def on_press_left(self, event):
+        def on_press_left(self, event: tk.Event) -> None:
             """
             If, in a tree, a node is left-clicked, it will generate a display of the subtree
             """
             if self._is_tree:
                 node = self.canvas.find_withtag(tk.CURRENT)
-                for nd in self.nodes:
-                    if nd.circle == node[0] or nd.text == node[0]:
-                        root = self.__search_node(nd.id)
-                        vertices = self.__levelorder(root)
-                        new_tree = copy.copy(self._graph)
-                        new_tree.remove_all()
-                        for i in list(vertices.keys()):
-                            new_tree.insert(i)
-                GraphGUI(new_tree,
-                         self.__node_radius,
-                         self._theme)
+                node_obj = self.__canvas_node_relation[node[0]]
+                root = self.__search_node(node_obj.id)
+                vertices = self.__levelorder(root)
+                new_tree = copy.copy(self._graph)
+                new_tree.remove_all()
+                for i in list(vertices.keys()):
+                    new_tree.insert(i)
+                GraphGUI(new_tree)
 
-        def on_press(self, event):
+        def on_press(self, event: tk.Event) -> None:
             """Right mouse click protocol"""
             # Store the node if it has been right-clicked
             node = self.canvas.find_withtag(tk.CURRENT)
             self.selected_node = (node, event.x, event.y)
 
-        def move(self, event):
+        def move(self, event: tk.Event) -> Node:
             """
             It moves a node if it has been selected on the right mouse click protocol. After moving it, it updates
-            automatically all edges attached to the node.
+            automatically all edges attached to the node. Returns the node that has been moved.
             """
             x, y = event.x, event.y
             node, x0, y0 = self.selected_node
             node_obj = self.__canvas_node_relation[node[0]]
             self.canvas.move(node_obj.circle, x - x0, y - y0)
             self.canvas.move(node_obj.text, x - x0, y - y0)
             node_obj.pos_x += x - x0
             node_obj.pos_y += y - y0
-            for edge in node_obj.asociated_edges_IN:
+            for edge in node_obj.associated_edges_IN:
                 edge.update_position()
-            for edge in node_obj.asociated_edges_OUT:
+            for edge in node_obj.associated_edges_OUT:
                 edge.update_position()
             self.selected_node = (node, x, y)
 
+            return node_obj
+
+        def set_node_radius(self, value) -> None:
+            self.__node_radius = value
+
 class Node:
-    def __init__(self, canvas: tk.Canvas, radius:int, posx: int, posy: int, text: str, bg: str = "white"):
-        self.asociated_edges_IN = []
-        self.asociated_edges_OUT = []
-        self.canvas = canvas
-        self.id = text
-        self.radius = radius
-        self.pos_x = posx
-        self.pos_y = posy
-        self.circle = canvas.create_oval(self.pos_x, self.pos_y, self.pos_x + self.radius*2, self.pos_y + self.radius*2, fill=bg, width=2,)
-        self.text = canvas.create_text(self.pos_x + self.radius, self.pos_y + self.radius, text=text)
-        canvas.addtag_enclosed("movil", self.pos_x - 3, self.pos_y - 3, self.pos_x + self.radius * 2 + 3, self.pos_y + self.radius * 2 + 3)
+    """
+    Node class representing a vertex in the graph or tree GUI. It stores the canvas object of the node, the radius,
+    the position, the text and all the edges associated to it (dividing them into two list so that it can be determined
+    which of those vertices are pointing IN or OUT of the vertex).
+
+    :param canvas: tkinter canvas object
+    :param radius: radius of the node
+    :param posx: x position of the node
+    :param posy: y position of the node
+    :param text: text shown in the node
+    :param bg: background color of the node
+    """
+    def __init__(self, canvas: tk.Canvas,
+                 radius: int,
+                 posx: int,
+                 posy: int,
+                 text: str,
+                 bg: str = "white"):
+
+        if type(canvas) != tk.Canvas:
+            raise TypeError("canvas must be a tkinter canvas object")
+        if type(radius) != int or radius < 0:
+            raise TypeError("radius must be a positive integer")
+        if type(posx) != int:
+            raise TypeError("posx must be a positive integer")
+        if type(posy) != int:
+            raise TypeError("posy must be a positive integer")
+
+        self.associated_edges_IN = []
+        self.associated_edges_OUT = []
+        self.__canvas = canvas
+        self.__id = text
+        self.__radius = radius
+        self.__pos_x = posx
+        self.__pos_y = posy
+        self.__circle = self.__canvas.create_oval(self.__pos_x, self.__pos_y, self.__pos_x + self.__radius*2, self.__pos_y + self.__radius*2, fill=bg, width=2,)
+        self.__text = self.__canvas.create_text(self.__pos_x + self.__radius, self.__pos_y + self.__radius, text=self.__id)
+        self.__canvas.addtag_enclosed("movil", self.__pos_x - 3, self.__pos_y - 3, self.__pos_x + self.__radius * 2 + 3, self.__pos_y + self.__radius * 2 + 3)
 
-    def terminate(self):
+    def terminate(self) -> None:
         for edge in self.asociated_edges_IN:
             edge.terminate()
         for edge in self.asociated_edges_OUT:
             edge.terminate()
-        self.canvas.delete(self.circle)
-        self.canvas.delete(self.text)
+        self.__canvas.delete(self.__circle)
+        self.__canvas.delete(self.__text)
+
+    def __str__(self):
+        return 'Node: ' + str(self.__id)
+
+    @property
+    def id(self):
+        return self.__id
+
+    @property
+    def pos_x(self):
+        return self.__pos_x
+
+    @pos_x.setter
+    def pos_x(self, value):
+        self.__pos_x = value
+
+    @property
+    def pos_y(self):
+        return self.__pos_y
+
+    @pos_y.setter
+    def pos_y(self, value):
+        self.__pos_y = value
+
+    @property
+    def circle(self):
+        return self.__circle
+
+    @property
+    def text(self):
+        return self.__text
+
+    @property
+    def radius(self):
+        return self.__radius
 
 class Edge:
-    def __init__(self, canvas: tk.Canvas, start: Node, end: Node, weight: int = 1, overlaped: bool = False, window_color: str = "white"):
-        self.canvas = canvas
-        self.overlaped = overlaped
-        self.start_node = start
-        self.end_node = end
-        self.weight = weight
-        self.window_color = window_color
-        self.start = self.__calculate_start(start, end)
-        self.end = self.__calculate_end(start, end)
+    """
+    Class representing an edge between two nodes that have been already created in the canvas of the GraphGUI.
+    The weight of the edge will be shown in the middle of the edge. The overlapped parameter is used to
+    determine if the edge will be overlapped by the nodes or not, if it is, the weight will be shown in the rightmost
+    side of the edge. The window_color parameter is used to determine the background color of the weight canvas label.
+
+    :param canvas: tkinter canvas object
+    :param start: Node object
+    :param end: Node object
+    :param weight: weight of the edge. If it is None, it will be shown as an empty edge
+    :param overlapped: boolean value to determine if the edge will be overlapped by the nodes or not
+    :param window_color: background color of the weight canvas label
+    :param text_color: text color of the weight canvas label
+    """
+    def __init__(self, canvas: tk.Canvas,
+                 start: Node,
+                 end: Node,
+                 weight: int = 1,
+                 overlapped: bool = False,
+                 window_color: str = "white",
+                 text_color: str = "black"):
+
+        if type(canvas) != tk.Canvas:
+            raise TypeError("canvas must be a tkinter canvas object")
+        if type(start) != Node or type(end) != Node:
+            raise TypeError("start and end must be Node objects")
+
+        self.__canvas = canvas
+        self.overlapped = overlapped
+        self.__start_node = start
+        self.__end_node = end
+        self.__weight = weight
+        self.__window_color = window_color
+        self.__text_color = text_color
+        self.__start = self.__calculate_start(start, end)
+        self.__end = self.__calculate_end(start, end)
+
+        if self not in self.__end_node.associated_edges_IN:
+            self.__end_node.associated_edges_IN.append(self)
+        if self not in self.__start_node.associated_edges_OUT:
+            self.__start_node.associated_edges_OUT.append(self)
+
+    def __str__(self):
+        return 'Edge: ' + str(self.__start_node.id) + ' -> ' + str(self.__end_node.id)
 
-    def update_position(self):
+    def update_position(self) -> None:
+        """Updates the position of the edge by recalculating the start and end node position"""
         self.__recalculate()
-        self.canvas.coords(self.line, self.start[0], self.start[1], self.end[0], self.end[1])
-        if self.weight:
-            if not self.overlaped:
-                self.canvas.coords(self.window, (self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2)
+        self.__canvas.coords(self.line, self.__start[0], self.__start[1], self.__end[0], self.__end[1])
+        if self.__weight:
+            if not self.overlapped:
+                self.__canvas.coords(self.window, (self.__start[0] + self.__end[0]) // 2, (self.__start[1] + self.__end[1]) // 2)
             else:
-                self.canvas.coords(self.window, self.start[0] * 0.2 + self.end[0] * 0.8, self.start[1] * 0.2 + self.end[1] * 0.8)
+                self.__canvas.coords(self.window, self.__start[0] * 0.2 + self.__end[0] * 0.8, self.__start[1] * 0.2 + self.__end[1] * 0.8)
 
-    def terminate(self):
-        self.canvas.delete(self.line)
-        if self.weight:
-            self.canvas.delete(self.window)
-
-    def show(self):
-        self.line = self.canvas.create_line(self.start[0],
-                                            self.start[1],
-                                            self.end[0],
-                                            self.end[1],
+    def terminate(self) -> None:
+        """Deletes the edge from the canvas and removes it from the asociated edges of the start and end nodes"""
+        self.__canvas.delete(self.line)
+        if self.__weight:
+            self.__canvas.delete(self.window)
+
+        if self in self.__end_node.associated_edges_IN:
+            self.__end_node.associated_edges_IN.remove(self)
+        if self in self.__start_node.associated_edges_OUT:
+            self.__start_node.associated_edges_OUT.remove(self)
+
+    def show(self) -> None:
+        """Displays the edge in the canvas"""
+        self.line = self.__canvas.create_line(self.__start[0],
+                                            self.__start[1],
+                                            self.__end[0],
+                                            self.__end[1],
                                             arrow=tk.LAST,
                                             width=1.5)
-        if self.weight:
-            if not self.overlaped:
-                self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2,
-                                                        (self.start[1] + self.end[1]) // 2,
-                                                        window=tk.Label(self.canvas,
-                                                                        bg=self.window_color,
-                                                                        text=str(self.weight)))
+        if self.__weight:
+            if not self.overlapped:
+                self.window = self.__canvas.create_window((self.__start[0] + self.__end[0]) // 2,
+                                                        (self.__start[1] + self.__end[1]) // 2,
+                                                        window=tk.Label(self.__canvas,
+                                                                        bg=self.__window_color,
+                                                                        text=str(self.__weight),
+                                                                        font=("Arial", 13),
+                                                                        fg=self.__text_color))
             else:
-                self.window = self.canvas.create_window((self.start[0] * 0.2 + self.end[0] * 0.8),
-                                                        (self.start[1] * 0.2 + self.end[1] * 0.8),
-                                                        window=tk.Label(self.canvas,
-                                                                        bg=self.window_color,
-                                                                        text=str(self.weight)))
-
-    def __recalculate(self):
-        self.start = self.__calculate_start(self.start_node, self.end_node)
-        self.end = self.__calculate_end(self.start_node, self.end_node)
+                self.window = self.__canvas.create_window((self.__start[0] * 0.2 + self.__end[0] * 0.8),
+                                                        (self.__start[1] * 0.2 + self.__end[1] * 0.8),
+                                                        window=tk.Label(self.__canvas,
+                                                                        bg=self.__window_color,
+                                                                        text=str(self.__weight),
+                                                                        font=("Arial", 13),
+                                                                        fg=self.__text_color))
+
+    def __recalculate(self) -> None:
+        """Recalculates the start and end position of the edge"""
+        self.__start = self.__calculate_start(self.__start_node, self.__end_node)
+        self.__end = self.__calculate_end(self.__start_node, self.__end_node)
 
     def __calculate_start(self, start: Node, end: Node) -> tuple:
         """
         It calculates the initial position of the arrow that connects the nodes "start" and "end"
         :param start: Node
         :param end: Node
         :return: tuple with the initial position of the arrow
@@ -722,9 +799,34 @@
         x = x2 - x1
         y = y2 - y1
         edge_angle = math.atan2(y, x) * (180.0 / math.pi)
         x = math.cos(math.radians(edge_angle)) * end.radius
         y = math.sin(math.radians(edge_angle)) * end.radius
         return  (center_end[0] - int(x), center_end[1] - int(y))
 
+    @property
+    def start_node(self):
+        return self.__start_node
+
+    @property
+    def end_node(self):
+        return self.__end_node
+
+    @property
+    def weight(self):
+        return self.__weight
+
+    @property
+    def window_color(self):
+        return self.__window_color
+
+    @property
+    def start(self):
+        return self.__start
+
+    @property
+    def end(self):
+        return self.__end
+
+
 if __name__ == "__main__":
     pass
```

### Comparing `graphdisplay-0.4.6/graphdisplay/tools_win_manager.py` & `graphdisplay-0.4.7/graphdisplay/tools_win_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,51 @@
             self.__create_minimum_path_frame()
             #self.__create_tree_convert_frame()
         else:
             self.__create_preorder_frame()
             self.__create_postorder_frame()
             self.__create_inorder_frame()
             self.__create_levelorder_frame()
+            self.__create_speed_frame()
+
+    def __create_speed_frame(self):
+        self.__speed_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=40,
+                                        width=500)
+        self.__speed_frame.pack(padx=7, pady=7)
+
+        text_label = tk.Label(self.__speed_frame,
+                              text="Animation speed",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=12)
+
+        self.__speed_scale = tk.Scale(self.__speed_frame,
+                                      from_=0.1,
+                                      to=1,
+                                      resolution=0.1,
+                                      highlightthickness=0,
+                                      orient=tk.HORIZONTAL,
+                                      bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                      bd=0,
+                                      length=150)
+        self.__speed_scale.place(x = 300, y = 0)
 
     def __create_inorder_frame(self):
         self.__inorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__inorder_frame.pack(padx=7, pady=7)
 
         text_label = tk.Label(self.__inorder_frame,
                               text="Inorder traversal",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=30)
 
         go_button = tk.Button(self.__inorder_frame,
                               text="Play",
                               command=self.__inorder_press_play,
                               bg=self.__gui._BUTTON_COLOR,
                               bd=0)
@@ -51,34 +77,35 @@
 
     def __inorder_press_play(self):
         self.__running_inorder = True
         self.__reset_colors()
         gui_tree: AVLTree = self.__gui._graph
         inorder_list = gui_tree.inorder_list()
 
+        hold = self.__speed_scale.get()
         for i in inorder_list:
-            for nd in self.__gui.nodes:
-                if nd.id == i and self.__running_inorder:
-                    self.__gui.canvas.itemconfigure(nd.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    self.__gui.canvas.update()
-                    time.sleep(0.1)
-                    break
-            if not self.__running_inorder:
+            if self.__running_inorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
                 break
 
     def __create_levelorder_frame(self):
         self.__levelorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__levelorder_frame.pack(padx=7, pady=7)
 
         text_label = tk.Label(self.__levelorder_frame,
                               text="Level order traversal",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=30)
 
         go_button = tk.Button(self.__levelorder_frame,
                               text="Play",
                               command=self.__levelorder_press_play,
                               bg=self.__gui._BUTTON_COLOR,
                               bd=0)
@@ -93,34 +120,35 @@
 
     def __levelorder_press_play(self):
         self.__running_levelorder = True
         self.__reset_colors()
         gui_tree: AVLTree = self.__gui._graph
         levelorder_list = gui_tree.levelorder_list()
 
+        hold = self.__speed_scale.get()
         for i in levelorder_list:
-            for nd in self.__gui.nodes:
-                if nd.id == i and self.__running_levelorder:
-                    self.__gui.canvas.itemconfigure(nd.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    self.__gui.canvas.update()
-                    time.sleep(0.1)
-                    break
-            if not self.__running_levelorder:
+            if self.__running_levelorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
                 break
 
     def __create_preorder_frame(self):
         self.__preorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__preorder_frame.pack(padx=7, pady=7)
 
         text_label = tk.Label(self.__preorder_frame,
                               text="Preorder traversal",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=30)
 
         go_button = tk.Button(self.__preorder_frame,
                               text="Play",
                               command=self.__preorder_press_play,
                               bg=self.__gui._BUTTON_COLOR,
                               bd=0)
@@ -135,34 +163,35 @@
 
     def __preorder_press_play(self):
         self.__running_preorder = True
         self.__reset_colors()
         gui_tree: AVLTree = self.__gui._graph
         preorder_list = gui_tree.preorder_list()
 
+        hold = self.__speed_scale.get()
         for i in preorder_list:
-            for nd in self.__gui.nodes:
-                if nd.id == i and self.__running_preorder:
-                    self.__gui.canvas.itemconfigure(nd.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    self.__gui.canvas.update()
-                    time.sleep(0.1)
-                    break
-            if not self.__running_preorder:
+            if self.__running_preorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
                 break
 
     def __create_postorder_frame(self):
         self.__postorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__postorder_frame.pack(padx=7, pady=7)
 
         text_label = tk.Label(self.__postorder_frame,
                               text="Postorder traversal",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=30)
 
         go_button = tk.Button(self.__postorder_frame,
                               text="Play",
                               command=self.__postorder_press_play,
                               bg=self.__gui._BUTTON_COLOR,
                               bd=0)
@@ -177,59 +206,62 @@
 
     def __postorder_press_play(self):
         self.__running_postorder = True
         self.__reset_colors()
         gui_tree: AVLTree = self.__gui._graph
         postorder_list = gui_tree.postorder_list()
 
+        hold = self.__speed_scale.get()
         for i in postorder_list:
-            for nd in self.__gui.nodes:
-                if nd.id == i and self.__running_postorder:
-                    self.__gui.canvas.itemconfigure(nd.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    self.__gui.canvas.update()
-                    time.sleep(0.1)
-                    break
-            if not self.__running_postorder:
+            if self.__running_postorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
                 break
 
     def __create_djistra_frame(self):
         self.__djistra_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__djistra_frame.pack(padx=7, pady=7)
 
         # Djistra text
         text_label = tk.Label(self.__djistra_frame,
-                              text="Djistra",
+                              text="Dijkstra",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=30)
 
         # First node entry
         self.first_node_entry_djis = tk.Entry(self.__djistra_frame)
         self.first_node_entry_djis.place(height=BUTTON_HEIGHT,
                                width=BUTTON_WIDTH,
                                y=35,
                                x=170)
         first_entry_text = tk.Label(self.__djistra_frame,
                                     text="First Node",
                                     bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13))
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
         first_entry_text.place(x=150, y=10)
 
         # Second node entry
         self.second_node_entry_djis = tk.Entry(self.__djistra_frame)
         self.second_node_entry_djis.place(height=BUTTON_HEIGHT,
                                width=BUTTON_WIDTH,
                                y=35,
                                x=240 + BUTTON_WIDTH)
         first_entry_text = tk.Label(self.__djistra_frame,
                                     text="Second Node",
                                     bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13))
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
         first_entry_text.place(x=275, y=10)
 
         # Go button
         go_button = tk.Button(self.__djistra_frame,
                               text="Show Path",
                               command=self.__djistra_press,
                               bg=self.__gui._BUTTON_COLOR,
@@ -249,59 +281,62 @@
             return
         elif second_node not in list(gui_graph._vertices.keys()):
             print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
             return
 
         min_path = gui_graph.minimum_path(first_node, second_node)
         if len(min_path[0]) >= 2:
-            for node in self.__gui.nodes:
-                if node.id in min_path[0] and self.__djistra_running:
-                    if node.id == first_node or node.id == second_node:
-                        self.__gui.canvas.itemconfigure(node.circle,
-                                                        fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    else:
-                        self.__gui.canvas.itemconfigure(node.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
+            for node in min_path[0]:
+                if node == first_node or node == second_node:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+                else:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
         else:
             print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
 
     def __create_minimum_path_frame(self):
         self.__minimum_path_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
         self.__minimum_path_frame.pack(padx=7, pady=7)
 
         # Djistra text
         text_label = tk.Label(self.__minimum_path_frame,
                               text="Minimum Edge \nPath",
                               bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
+                              font=("Courier", 13),
+                                fg=self.__gui._AUTHOR_NAME_COLOR)
         text_label.place(x=5, y=20)
 
         # First node entry
         self.first_node_entry_min = tk.Entry(self.__minimum_path_frame)
         self.first_node_entry_min.place(height=BUTTON_HEIGHT,
                                width=BUTTON_WIDTH,
                                y=35,
                                x=170)
         first_entry_text = tk.Label(self.__minimum_path_frame,
                                     text="First Node",
                                     bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13))
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
         first_entry_text.place(x=150, y=10)
 
         # Second node entry
         self.second_node_entry_min = tk.Entry(self.__minimum_path_frame)
         self.second_node_entry_min.place(height=BUTTON_HEIGHT,
                                width=BUTTON_WIDTH,
                                y=35,
                                x=240 + BUTTON_WIDTH)
         first_entry_text = tk.Label(self.__minimum_path_frame,
                                     text="Second Node",
                                     bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13))
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
         first_entry_text.place(x=275, y=10)
 
         # Go button
         go_button = tk.Button(self.__minimum_path_frame,
                               text="Show Path",
                               command=self.__minpath_press,
                               bg=self.__gui._BUTTON_COLOR,
@@ -320,21 +355,21 @@
             return
         elif second_node not in list(gui_graph._vertices.keys()):
             print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
             return
 
         min_path = gui_graph.min_number_edges(first_node, second_node)
         if len(min_path) >= 2:
-            for node in self.__gui.nodes:
-                if node.id in min_path:
-                    if node.id == first_node or node.id == second_node:
-                        self.__gui.canvas.itemconfigure(node.circle,
-                                                        fill=self.__gui._SELECTED_VERTEX_COLOR)
-                    else:
-                        self.__gui.canvas.itemconfigure(node.circle, fill=self.__gui._SELECTED_VERTEX_COLOR)
+            for node in min_path:
+                if node == first_node or node == second_node:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+                else:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
         else:
             print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
 
     def __create_tree_convert_frame(self):
         self.__tree_convert_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
                                         height=80,
                                         width=500)
@@ -364,15 +399,15 @@
             # WORK IN PROGRESS... CHECK OUT SOON ;)
             ...
         else:
             print("ERROR: graph cannot be converted into a binary tree")
 
     def __reset_colors(self):
         for node in self.__gui.nodes:
-            self.__gui.canvas.itemconfigure(node.circle, fill=self.__gui._VERTEX_COLOR)
+            self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle, fill=self.__gui._VERTEX_COLOR)
 
     def __reset_all_traversal(self):
         self.__djistra_running = False
         self.__running_postorder = False
         self.__running_preorder = False
         self.__running_levelorder = False
         self.__running_inorder = False
```

### Comparing `graphdisplay-0.4.6/graphdisplay/trees/auto_balance_tree.py` & `graphdisplay-0.4.7/graphdisplay/trees/auto_balance_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.6/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.7/graphdisplay/trees/binary_search_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self._root = self._insert(self._root, elem)
 
     def _insert(self, node: BinaryNode, elem: object) -> BinaryNode:
         if node is None:
             return BinaryNode(elem)
 
         if node.elem == elem:
-            print('Error: elem already exist ', elem)
             return node
 
         if elem < node.elem:
             node.left = self._insert(node.left, elem)
         else:
             # elem>node.elem
             node.right = self._insert(node.right, elem)
@@ -53,15 +52,14 @@
         # update the root with the new subtree after remove elem
         self._root = self._remove(self._root, elem)
 
     def _remove(self, node: BinaryNode, elem: object) -> BinaryNode:
         """It recursively searches the node. When the node is
         found, the node has to be removed"""
         if node is None:
-            print(elem, ' not found')
             return node
 
         if elem < node.elem:
             node.left = self._remove(node.left, elem)
         elif elem > node.elem:
             node.right = self._remove(node.right, elem)
         else:
```

### Comparing `graphdisplay-0.4.6/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.7/graphdisplay/trees/binary_tree.py`

 * *Files identical despite different names*

### Comparing `graphdisplay-0.4.6/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.7/graphdisplay.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.4.6
+Version: 0.4.7
 Summary: Librería para representar grafos visualmente
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz (@seniorbeto)
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -33,89 +33,127 @@
 
 ## 📐Método de uso
 
 Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
 tkinter y math (que muchas veces vienen instaladas por defecto en python). 
 
 Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
-asignatura, por lo que también son importables.
-Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón. 
-Junto con el grafo, el resto de argumentos son los siguientes: 
-+ graph: es el objeto de tipo grafo/árbol que se va a representar **ES MUY IMPORTANTE** que éste sea implementado en base al código base de la asignatura. Si alguno
-de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA) o utilizar la implementación de grafos que viene por defecto con el paquete.
-+ node_radius: el radio de cada vértice del grafo, por defecto es 40 y puede tomar cualquier valor entero entre 10 y 100
-+ theme: el tema de la ventana, por defecto es 'brown' y no voy a mencionarlos todos porque hay muchos.
+asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
+**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
+o utilizar la implementación de grafos que viene por defecto con el paquete.
+Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
+gestiona el almacenado de grafos.
 
 Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-```python
-from graphdisplay import GraphGUI, Graph
 
-g = Graph([1, 2, 3])
-g.addEdge(1, 2)
-g.addEdge(2, 3)
++ Para representar el siguiente grafo:
 
-# Para representar el grafo con todos los valores por defecto
-GraphGUI(g)
-
-# Para ajustar el radio de los nodos a 32, y el tema a 'dark'
-GraphGUI(g, node_radius=32, theme='dark')
-```
-Ejemplo con árboles binarios de búsqueda:
-```python
-from graphdisplay import GraphGUI, BinarySearchTree
-from random import randint
-
-tree = BinarySearchTree()
-for _ in range(80):
-    tree.insert(randint(1, 1000))
-   
-GraphGUI(tree)
-```
+     <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png' width='25%'/>
+    
+    Se podría disponer del siguiente código:
+    ```python
+    from graphdisplay import GraphGUI, Graph
+    
+    # Implementaremos el grafo de la siguiente imagen:
+    # https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png
+    
+    labels = ['A', 'B', 'C', 'D', 'E']
+    g = Graph(labels)
+    
+    g.addEdge('A', 'C', 12)  # A->(12)C
+    g.addEdge('A', 'D', 60)  # A->(60)D
+    g.addEdge('B', 'A', 10)  # B->(10)A
+    g.addEdge('C', 'B', 20)  # C->(20)B
+    g.addEdge('C', 'D', 32)  # C->(32)D
+    g.addEdge('E', 'A', 7)   # E->(7)A
+    
+    # Para representar el grafo 
+    if __name__ == "__main__":
+        GraphGUI(g)
+    ```
+
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/9210f5d4-4903-45ea-9bb8-e625890adac3' width='30%'/>
+  
++ Ejemplo con árboles binarios de búsqueda:
+
+    Para representar el siguiente árbol:
+
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1418ef2c-3215-4d88-93ce-3d1c67c4a58e' width='70%'/>
+    
+    Se dispondría del siguiente código:
+    ```python
+    from graphdisplay import GraphGUI, BinarySearchTree
+    
+    labels = [12, 4, 16, 2, 10, 14, 19, 1, 8, 13, 18, 20, 6, 24]
+    tree = BinarySearchTree()
+    for i in labels:
+        tree.insert(i)
+       
+    # Para representar el árbol
+    if __name__ == "__main__":
+        GraphGUI(tree)
+    ```
+    
+    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1e87b61d-d6fd-4635-bdf0-136509250de7' width='60%'/>
 
 ## ⚡️Funcionalidades
 Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
 éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
 instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
 Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón save y nombrando el guardado) para
-después poder cargarlo en cualquier momento.
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
+después poder cargarlo (file>load) en cualquier momento.
 
 Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
 al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
 Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
 issue #16
+
+
 ## 🎯Ejemplos de uso
 
-Para instanciar un grafo de tipo diccionario, se debe hacer de la siguiente manera: 
 
 ```python
 from graphdisplay import GraphGUI, Graph
 
-labels = ['A', 'B', 'C', 'D', 'E']
-g = Graph(labels)
-
-# Now, we add the edges
-g.addEdge('A', 'C', 12)  # A->(12)C
-g.addEdge('A', 'D', 60)  # A->(60)D
-g.addEdge('B', 'A', 10)  # B->(10)A
-g.addEdge('C', 'B', 20)  # C->(20)B
-g.addEdge('C', 'D', 32)  # C->(32)D
-g.addEdge('E', 'A', 7)   # E->(7)A
-g.addEdge('A', 'E', 50)  # A->(50)E
-```
+my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
+my_gragph.addEdge('A', 'B', 4)
+my_gragph.addEdge('B', 'C', 8)
+my_gragph.addEdge('C', 'A', 100)
+my_gragph.addEdge('D', 'E', 7)
+my_gragph.addEdge('E', 'F', 10)
+my_gragph.addEdge('F', 'G', 5)
+my_gragph.addEdge('G', 'Z', 6)
+my_gragph.addEdge('A', 'H', 2)
+my_gragph.addEdge('B', 'I', 3)
+my_gragph.addEdge('C', 'J', 4)
+my_gragph.addEdge('D', 'K', 5)
+my_gragph.addEdge('E', 'L', 6)
+my_gragph.addEdge('F', 'D', 3)
+my_gragph.addEdge('G', 'H', 9)
+my_gragph.addEdge('H', 'Z', 2)
+my_gragph.addEdge('I', 'J', 1)
+my_gragph.addEdge('J', 'A', 6)
+my_gragph.addEdge('K', 'L', 5)
+my_gragph.addEdge('L', 'M', 4)
+my_gragph.addEdge('M', 'H', 3)
+my_gragph.addEdge('N', 'O', 2)
+my_gragph.addEdge('O', 'P', 1)
+my_gragph.addEdge('P', 'Q', 7)
+my_gragph.addEdge('H', 'A', 20)
+my_gragph.addEdge('K', 'B', 7)
+my_gragph.addEdge('H', 'N', 9)
+my_gragph.addEdge('Q', 'D', 40)
 
-Si queremos mostrar la pantalla, basta con instanciar un objeto de tipo GraphGUI, pasándole como argumento el grafo que queremos mostrar: 
-
-```python
+if __name__ == "__main__":
     GraphGUI(g)
 ```
-Y nos mostrará la ventana:
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/0abc6d79-120e-470f-8d9b-7035e38def40" width="400" height="400">
 
-Sabiendo cómo instanciar grafos y reorganiando un poco los vértices, podemos ahora representar objetos algo más complicados ajustando un poco los parámetros de la instancia GraphGUI. En este caso: `GraphGUI(my_gragph, 25, theme="la gran ola")`
+Y nos mostrará la ventana (reordenando los vértices):
 
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/a1edfcbf-4cec-4b08-98c6-709b87b7892d" width="800" height="500">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
 
 De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
 
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/3afa798a-28c3-4c6f-9357-8d849018dfa5" width="1000" height="480">
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
```

### Comparing `graphdisplay-0.4.6/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.7/graphdisplay.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 LICENSE
 README.md
 setup.py
 graphdisplay/__init__.py
 graphdisplay/about_win_manager.py
 graphdisplay/general_config.py
+graphdisplay/graphdisplay.py
 graphdisplay/json_manager.py
-graphdisplay/main.py
 graphdisplay/tools_win_manager.py
 graphdisplay.egg-info/PKG-INFO
 graphdisplay.egg-info/SOURCES.txt
 graphdisplay.egg-info/dependency_links.txt
 graphdisplay.egg-info/top_level.txt
 graphdisplay/graphs/__init__.py
 graphdisplay/graphs/graph.py
```

### Comparing `graphdisplay-0.4.6/setup.py` & `graphdisplay-0.4.7/setup.py`

 * *Files identical despite different names*

