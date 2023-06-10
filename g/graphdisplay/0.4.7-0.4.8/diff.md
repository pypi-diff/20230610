# Comparing `tmp/graphdisplay-0.4.7.tar.gz` & `tmp/graphdisplay-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.4.7.tar", last modified: Sat Jun 10 17:54:28 2023, max compression
+gzip compressed data, was "graphdisplay-0.4.8.tar", last modified: Sat Jun 10 19:41:49 2023, max compression
```

## Comparing `graphdisplay-0.4.7.tar` & `graphdisplay-0.4.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.533296 graphdisplay-0.4.7/
--rw-rw-rw-   0        0        0     1088 2023-05-07 07:45:49.000000 graphdisplay-0.4.7/LICENSE
--rw-rw-rw-   0        0        0     8112 2023-06-10 17:54:28.532298 graphdisplay-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     7440 2023-06-10 17:53:37.000000 graphdisplay-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.489007 graphdisplay-0.4.7/graphdisplay/
--rw-rw-rw-   0        0        0     1390 2023-06-10 15:20:24.000000 graphdisplay-0.4.7/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     2364 2023-06-10 08:53:32.000000 graphdisplay-0.4.7/graphdisplay/about_win_manager.py
--rw-rw-rw-   0        0        0     5241 2023-06-10 09:54:24.000000 graphdisplay-0.4.7/graphdisplay/general_config.py
--rw-rw-rw-   0        0        0    39051 2023-06-10 15:58:23.000000 graphdisplay-0.4.7/graphdisplay/graphdisplay.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.514615 graphdisplay-0.4.7/graphdisplay/graphs/
--rw-rw-rw-   0        0        0       24 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/graphs/__init__.py
--rw-rw-rw-   0        0        0    23060 2023-06-07 15:39:55.000000 graphdisplay-0.4.7/graphdisplay/graphs/graph.py
--rw-rw-rw-   0        0        0    12487 2023-06-10 16:08:07.000000 graphdisplay-0.4.7/graphdisplay/json_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.515612 graphdisplay-0.4.7/graphdisplay/store/
--rw-rw-rw-   0        0        0        0 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/store/__init__.py
--rw-rw-rw-   0        0        0    19130 2023-06-10 10:09:26.000000 graphdisplay-0.4.7/graphdisplay/tools_win_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.531299 graphdisplay-0.4.7/graphdisplay/trees/
--rw-rw-rw-   0        0        0       88 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/__init__.py
--rw-rw-rw-   0        0        0     3612 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/auto_balance_tree.py
--rw-rw-rw-   0        0        0     3159 2023-06-10 13:54:50.000000 graphdisplay-0.4.7/graphdisplay/trees/binary_search_tree.py
--rw-rw-rw-   0        0        0     6197 2023-06-01 13:39:52.000000 graphdisplay-0.4.7/graphdisplay/trees/binary_tree.py
-drwxrwxrwx   0        0        0        0 2023-06-10 17:54:28.507631 graphdisplay-0.4.7/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     8112 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      590 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 17:54:28.000000 graphdisplay-0.4.7/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 17:54:28.533296 graphdisplay-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1763 2023-06-10 15:14:59.000000 graphdisplay-0.4.7/setup.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1067 2023-05-06 20:46:34.000000 graphdisplay-0.4.8/LICENSE
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7299 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/README.md
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.912483 graphdisplay-0.4.8/graphdisplay/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1344 2023-06-10 19:16:02.000000 graphdisplay-0.4.8/graphdisplay/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     2309 2023-06-08 08:28:47.000000 graphdisplay-0.4.8/graphdisplay/about_win_manager.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     5079 2023-06-10 19:41:48.000000 graphdisplay-0.4.8/graphdisplay/general_config.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    38219 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/graphdisplay.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    11353 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/graphdisplay.pyi
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/graphs/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       24 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/graphs/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    22482 2023-06-07 15:32:37.000000 graphdisplay-0.4.8/graphdisplay/graphs/graph.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    12198 2023-06-10 18:55:10.000000 graphdisplay-0.4.8/graphdisplay/json_manager.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/store/
+-rw-rw-r--   0 beto      (1000) beto      (1000)        0 2023-05-06 20:46:34.000000 graphdisplay-0.4.8/graphdisplay/store/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)    18712 2023-06-08 08:22:05.000000 graphdisplay-0.4.8/graphdisplay/tools_win_manager.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/graphdisplay/trees/
+-rw-rw-r--   0 beto      (1000) beto      (1000)       87 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/trees/__init__.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3524 2023-05-14 22:04:49.000000 graphdisplay-0.4.8/graphdisplay/trees/auto_balance_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     3068 2023-06-10 19:31:00.000000 graphdisplay-0.4.8/graphdisplay/trees/binary_search_tree.py
+-rw-rw-r--   0 beto      (1000) beto      (1000)     6026 2023-05-28 11:58:14.000000 graphdisplay-0.4.8/graphdisplay/trees/binary_tree.py
+drwxrwxr-x   0 beto      (1000) beto      (1000)        0 2023-06-10 19:41:49.912483 graphdisplay-0.4.8/graphdisplay.egg-info/
+-rw-rw-r--   0 beto      (1000) beto      (1000)     7953 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/PKG-INFO
+-rw-rw-r--   0 beto      (1000) beto      (1000)      620 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)        1 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       13 2023-06-10 19:41:49.000000 graphdisplay-0.4.8/graphdisplay.egg-info/top_level.txt
+-rw-rw-r--   0 beto      (1000) beto      (1000)       38 2023-06-10 19:41:49.916483 graphdisplay-0.4.8/setup.cfg
+-rw-rw-r--   0 beto      (1000) beto      (1000)     1763 2023-06-10 19:40:18.000000 graphdisplay-0.4.8/setup.py
```

### Comparing `graphdisplay-0.4.7/LICENSE` & `graphdisplay-0.4.8/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 seniorbeto
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 seniorbeto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `graphdisplay-0.4.7/PKG-INFO` & `graphdisplay-0.4.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-Metadata-Version: 2.1
-Name: graphdisplay
-Version: 0.4.7
-Summary: Librería para representar grafos visualmente
-Home-page: https://github.com/seniorbeto
-Author: Alberto Penas Díaz (@seniorbeto)
-Author-email: albertopenasdiaz@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
-  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
-  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
-</p>
-
-## 💡Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
-
-## ⚡️¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## 📐Método de uso
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
-asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
-Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
-**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
-de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
-o utilizar la implementación de grafos que viene por defecto con el paquete.
-Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
-gestiona el almacenado de grafos.
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-
-+ Para representar el siguiente grafo:
-
-     <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png' width='25%'/>
-    
-    Se podría disponer del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, Graph
-    
-    # Implementaremos el grafo de la siguiente imagen:
-    # https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png
-    
-    labels = ['A', 'B', 'C', 'D', 'E']
-    g = Graph(labels)
-    
-    g.addEdge('A', 'C', 12)  # A->(12)C
-    g.addEdge('A', 'D', 60)  # A->(60)D
-    g.addEdge('B', 'A', 10)  # B->(10)A
-    g.addEdge('C', 'B', 20)  # C->(20)B
-    g.addEdge('C', 'D', 32)  # C->(32)D
-    g.addEdge('E', 'A', 7)   # E->(7)A
-    
-    # Para representar el grafo 
-    if __name__ == "__main__":
-        GraphGUI(g)
-    ```
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/9210f5d4-4903-45ea-9bb8-e625890adac3' width='30%'/>
-  
-+ Ejemplo con árboles binarios de búsqueda:
-
-    Para representar el siguiente árbol:
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1418ef2c-3215-4d88-93ce-3d1c67c4a58e' width='70%'/>
-    
-    Se dispondría del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, BinarySearchTree
-    
-    labels = [12, 4, 16, 2, 10, 14, 19, 1, 8, 13, 18, 20, 6, 24]
-    tree = BinarySearchTree()
-    for i in labels:
-        tree.insert(i)
-       
-    # Para representar el árbol
-    if __name__ == "__main__":
-        GraphGUI(tree)
-    ```
-    
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1e87b61d-d6fd-4635-bdf0-136509250de7' width='60%'/>
-
-## ⚡️Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
-después poder cargarlo (file>load) en cualquier momento.
-
-Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
-al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
-Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
-issue #16
-
-
-## 🎯Ejemplos de uso
-
-
-```python
-from graphdisplay import GraphGUI, Graph
-
-my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
-my_gragph.addEdge('A', 'B', 4)
-my_gragph.addEdge('B', 'C', 8)
-my_gragph.addEdge('C', 'A', 100)
-my_gragph.addEdge('D', 'E', 7)
-my_gragph.addEdge('E', 'F', 10)
-my_gragph.addEdge('F', 'G', 5)
-my_gragph.addEdge('G', 'Z', 6)
-my_gragph.addEdge('A', 'H', 2)
-my_gragph.addEdge('B', 'I', 3)
-my_gragph.addEdge('C', 'J', 4)
-my_gragph.addEdge('D', 'K', 5)
-my_gragph.addEdge('E', 'L', 6)
-my_gragph.addEdge('F', 'D', 3)
-my_gragph.addEdge('G', 'H', 9)
-my_gragph.addEdge('H', 'Z', 2)
-my_gragph.addEdge('I', 'J', 1)
-my_gragph.addEdge('J', 'A', 6)
-my_gragph.addEdge('K', 'L', 5)
-my_gragph.addEdge('L', 'M', 4)
-my_gragph.addEdge('M', 'H', 3)
-my_gragph.addEdge('N', 'O', 2)
-my_gragph.addEdge('O', 'P', 1)
-my_gragph.addEdge('P', 'Q', 7)
-my_gragph.addEdge('H', 'A', 20)
-my_gragph.addEdge('K', 'B', 7)
-my_gragph.addEdge('H', 'N', 9)
-my_gragph.addEdge('Q', 'D', 40)
-
-if __name__ == "__main__":
-    GraphGUI(g)
-```
-
-Y nos mostrará la ventana (reordenando los vértices):
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
-
-De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
+Metadata-Version: 2.1
+Name: graphdisplay
+Version: 0.4.8
+Summary: Librería para representar grafos visualmente
+Home-page: https://github.com/seniorbeto
+Author: Alberto Penas Díaz (@seniorbeto)
+Author-email: albertopenasdiaz@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
+  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
+  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
+</p>
+
+## 💡Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
+
+## ⚡️¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## 📐Método de uso
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
+asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
+**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
+o utilizar la implementación de grafos que viene por defecto con el paquete.
+Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
+gestiona el almacenado de grafos.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+
++ Para representar el siguiente grafo:
+
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
+
+## ⚡️Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
+después poder cargarlo (file>load) en cualquier momento.
+
+Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
+al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
+Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
+issue #16
+
+
+## 🎯Ejemplos de uso
+
+
+```python
+from graphdisplay import GraphGUI, Graph
+
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
+
+if __name__ == "__main__":
+    GraphGUI(g)
+```
+
+Y nos mostrará la ventana (reordenando los vértices):
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
+
+De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
```

### Comparing `graphdisplay-0.4.7/README.md` & `graphdisplay-0.4.8/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-<p align="center">
-  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
-  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
-  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
-</p>
-
-## 💡Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
-
-## ⚡️¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## 📐Método de uso
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
-asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
-Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
-**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
-de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
-o utilizar la implementación de grafos que viene por defecto con el paquete.
-Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
-gestiona el almacenado de grafos.
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-
-+ Para representar el siguiente grafo:
-
-     <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png' width='25%'/>
-    
-    Se podría disponer del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, Graph
-    
-    # Implementaremos el grafo de la siguiente imagen:
-    # https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png
-    
-    labels = ['A', 'B', 'C', 'D', 'E']
-    g = Graph(labels)
-    
-    g.addEdge('A', 'C', 12)  # A->(12)C
-    g.addEdge('A', 'D', 60)  # A->(60)D
-    g.addEdge('B', 'A', 10)  # B->(10)A
-    g.addEdge('C', 'B', 20)  # C->(20)B
-    g.addEdge('C', 'D', 32)  # C->(32)D
-    g.addEdge('E', 'A', 7)   # E->(7)A
-    
-    # Para representar el grafo 
-    if __name__ == "__main__":
-        GraphGUI(g)
-    ```
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/9210f5d4-4903-45ea-9bb8-e625890adac3' width='30%'/>
-  
-+ Ejemplo con árboles binarios de búsqueda:
-
-    Para representar el siguiente árbol:
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1418ef2c-3215-4d88-93ce-3d1c67c4a58e' width='70%'/>
-    
-    Se dispondría del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, BinarySearchTree
-    
-    labels = [12, 4, 16, 2, 10, 14, 19, 1, 8, 13, 18, 20, 6, 24]
-    tree = BinarySearchTree()
-    for i in labels:
-        tree.insert(i)
-       
-    # Para representar el árbol
-    if __name__ == "__main__":
-        GraphGUI(tree)
-    ```
-    
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1e87b61d-d6fd-4635-bdf0-136509250de7' width='60%'/>
-
-## ⚡️Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
-después poder cargarlo (file>load) en cualquier momento.
-
-Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
-al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
-Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
-issue #16
-
-
-## 🎯Ejemplos de uso
-
-
-```python
-from graphdisplay import GraphGUI, Graph
-
-my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
-my_gragph.addEdge('A', 'B', 4)
-my_gragph.addEdge('B', 'C', 8)
-my_gragph.addEdge('C', 'A', 100)
-my_gragph.addEdge('D', 'E', 7)
-my_gragph.addEdge('E', 'F', 10)
-my_gragph.addEdge('F', 'G', 5)
-my_gragph.addEdge('G', 'Z', 6)
-my_gragph.addEdge('A', 'H', 2)
-my_gragph.addEdge('B', 'I', 3)
-my_gragph.addEdge('C', 'J', 4)
-my_gragph.addEdge('D', 'K', 5)
-my_gragph.addEdge('E', 'L', 6)
-my_gragph.addEdge('F', 'D', 3)
-my_gragph.addEdge('G', 'H', 9)
-my_gragph.addEdge('H', 'Z', 2)
-my_gragph.addEdge('I', 'J', 1)
-my_gragph.addEdge('J', 'A', 6)
-my_gragph.addEdge('K', 'L', 5)
-my_gragph.addEdge('L', 'M', 4)
-my_gragph.addEdge('M', 'H', 3)
-my_gragph.addEdge('N', 'O', 2)
-my_gragph.addEdge('O', 'P', 1)
-my_gragph.addEdge('P', 'Q', 7)
-my_gragph.addEdge('H', 'A', 20)
-my_gragph.addEdge('K', 'B', 7)
-my_gragph.addEdge('H', 'N', 9)
-my_gragph.addEdge('Q', 'D', 40)
-
-if __name__ == "__main__":
-    GraphGUI(g)
-```
-
-Y nos mostrará la ventana (reordenando los vértices):
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
-
-De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
+<p align="center">
+  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
+  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
+  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
+</p>
+
+## 💡Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
+
+## ⚡️¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## 📐Método de uso
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
+asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
+**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
+o utilizar la implementación de grafos que viene por defecto con el paquete.
+Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
+gestiona el almacenado de grafos.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+
++ Para representar el siguiente grafo:
+
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
+
+## ⚡️Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
+después poder cargarlo (file>load) en cualquier momento.
+
+Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
+al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
+Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
+issue #16
+
+
+## 🎯Ejemplos de uso
+
+
+```python
+from graphdisplay import GraphGUI, Graph
+
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
+
+if __name__ == "__main__":
+    GraphGUI(g)
+```
+
+Y nos mostrará la ventana (reordenando los vértices):
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
+
+De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
```

### Comparing `graphdisplay-0.4.7/graphdisplay/about_win_manager.py` & `graphdisplay-0.4.8/graphdisplay/about_win_manager.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import tkinter as tk
-import turtle
-import webbrowser
-from .general_config import *
-
-class AboutWindow(tk.Toplevel):
-    def __init__(self, root, graphgui):
-        super().__init__(root)
-        self.__graphgui = graphgui
-        self.title("About")
-        self.geometry("400x430")
-        self.resizable(False, False)
-        self.configure(bg=self.__graphgui._FRAME_COLOR, width=400, height=430)
-        self.protocol("WM_DELETE_WINDOW", self.__on_close)
-
-        buton = tk.Button(self, text="Contribute", bg=self.__graphgui._BUTTON_COLOR, command=self.__open_github, bd=0)
-        buton.pack(side=tk.BOTTOM)
-
-        self.canvas = tk.Canvas(self, width=400, height=400, bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
-        self.canvas.pack()
-        self.turtle = turtle.RawTurtle(self.canvas, visible=False)
-        self.canvas.configure(bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
-        self.turtle.speed(0)
-        self.canvas.create_text(0, -100, text="by @seniorbeto",
-                                fill=self.__graphgui._AUTHOR_NAME_COLOR, font=("Courier", 15))
-        text = "GraphDisplay v"+VERSION
-        self.canvas.create_text(0, -150, text=text, font=("Courier", 20),
-                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
-        self.canvas.create_text(0, 147, text="An open source proyect made", font=("Courier", 13),
-                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
-        self.canvas.create_text(0, 165, text="by and for students!", font=("Courier", 13),
-                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
-        self.running = True
-        i = 0
-        self.turtle.color(self.__graphgui._VERTEX_COLOR)
-        try:
-            while self.running and i<92:
-                if i % 2 == 0:
-                    self.turtle.penup()
-                else:
-                    self.turtle.pendown()
-                self.turtle.forward(i + 1 + 5)
-                self.turtle.right(91)
-                i += 1
-        except tk.TclError:
-            pass
-
-    def __on_close(self):
-        self.running = False
-        self.destroy()
-
-    def __open_github(self):
-        webbrowser.open("https://github.com/seniorbeto/graphdisplay")
-
-    def __open_twitter(self):
+import tkinter as tk
+import turtle
+import webbrowser
+from .general_config import *
+
+class AboutWindow(tk.Toplevel):
+    def __init__(self, root, graphgui):
+        super().__init__(root)
+        self.__graphgui = graphgui
+        self.title("About")
+        self.geometry("400x430")
+        self.resizable(False, False)
+        self.configure(bg=self.__graphgui._FRAME_COLOR, width=400, height=430)
+        self.protocol("WM_DELETE_WINDOW", self.__on_close)
+
+        buton = tk.Button(self, text="Contribute", bg=self.__graphgui._BUTTON_COLOR, command=self.__open_github, bd=0)
+        buton.pack(side=tk.BOTTOM)
+
+        self.canvas = tk.Canvas(self, width=400, height=400, bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
+        self.canvas.pack()
+        self.turtle = turtle.RawTurtle(self.canvas, visible=False)
+        self.canvas.configure(bg=self.__graphgui._BACKGROUND_CANVAS_COLOR)
+        self.turtle.speed(0)
+        self.canvas.create_text(0, -100, text="by @seniorbeto",
+                                fill=self.__graphgui._AUTHOR_NAME_COLOR, font=("Courier", 15))
+        text = "GraphDisplay v"+VERSION
+        self.canvas.create_text(0, -150, text=text, font=("Courier", 20),
+                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
+        self.canvas.create_text(0, 147, text="An open source proyect made", font=("Courier", 13),
+                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
+        self.canvas.create_text(0, 165, text="by and for students!", font=("Courier", 13),
+                                fill=self.__graphgui._AUTHOR_NAME_COLOR)
+        self.running = True
+        i = 0
+        self.turtle.color(self.__graphgui._VERTEX_COLOR)
+        try:
+            while self.running and i<92:
+                if i % 2 == 0:
+                    self.turtle.penup()
+                else:
+                    self.turtle.pendown()
+                self.turtle.forward(i + 1 + 5)
+                self.turtle.right(91)
+                i += 1
+        except tk.TclError:
+            pass
+
+    def __on_close(self):
+        self.running = False
+        self.destroy()
+
+    def __open_github(self):
+        webbrowser.open("https://github.com/seniorbeto/graphdisplay")
+
+    def __open_twitter(self):
         webbrowser.open("https://twitter.com/seniorbeto__")
```

### Comparing `graphdisplay-0.4.7/graphdisplay/general_config.py` & `graphdisplay-0.4.8/graphdisplay/general_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-VERSION = '0.4.7'
-DEFAULT_SCR_WIDTH = 600
-DEFAULT_SCR_HEIGHT = 600
-DEFAULT_NODE_RADIUS = 25
-DEFAULT_THEME = 'BROWN'
-BUTTON_HEIGHT = 30
-BUTTON_WIDTH = 60
-XMARGEN = 7
-YMARGEN = 7
-THEMES = {
-    "BROWN":{
-        "BUTTON_COLOR": "#ede4cc",
-        "SELECTED_VERTEX_COLOR": "#c2baa7",
-        "VERTEX_COLOR": "#e3d7c5",
-        "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
-        "FRAME_COLOR": "#87715f",
-        "AUTHOR_NAME_COLOR": "#301d05"
-    },
-    "LIGHT":{
-        "BUTTON_COLOR": "#a6a6a6",
-        "SELECTED_VERTEX_COLOR": "#b3b3b3",
-        "VERTEX_COLOR": "#bfbdbd",
-        "BACKGROUND_CANVAS_COLOR": "#d4d3d2",
-        "FRAME_COLOR": "#b3b3b3",
-        "AUTHOR_NAME_COLOR": "#454545"
-    },
-    "BLUE":{
-        "BUTTON_COLOR": "#b7e7e8",
-        "VERTEX_COLOR": "#a7d6fc",
-        "SELECTED_VERTEX_COLOR": "#91b9ba",
-        "BACKGROUND_CANVAS_COLOR": "#b5d9f7",
-        "FRAME_COLOR": "#6aaade",
-        "AUTHOR_NAME_COLOR": "#0b2d47"
-    },
-    "DARK":{
-        "BUTTON_COLOR": "#6a6a7d",
-        "SELECTED_VERTEX_COLOR": "#8d8da6",
-        "VERTEX_COLOR": "#7d7d96",
-        "BACKGROUND_CANVAS_COLOR": "#404147",
-        "FRAME_COLOR": "#272729",
-        "AUTHOR_NAME_COLOR": "#7c7c9c"
-    },
-    "PURPLE":{
-        "BUTTON_COLOR": "#f2c8fa",
-        "SELECTED_VERTEX_COLOR": "#bf97c7",
-        "VERTEX_COLOR": "#e7cdf7",
-        "BACKGROUND_CANVAS_COLOR": "#e4c3fa",
-        "FRAME_COLOR": "#d899f7",
-        "AUTHOR_NAME_COLOR": "#6d1aa3"
-    },
-    "GREEN":{
-        "BUTTON_COLOR": "#B5FFC7",
-        "SELECTED_VERTEX_COLOR": "#05331F",
-        "VERTEX_COLOR": "#A1FDB3",
-        "BACKGROUND_CANVAS_COLOR": "#BFFFCF",
-        "FRAME_COLOR": "#80FF99",
-        "AUTHOR_NAME_COLOR": "#05331F"
-    },
-    "DARKGREEN":{
-        "BUTTON_COLOR": "#173F2D",
-        "SELECTED_VERTEX_COLOR": "#05331F",
-        "VERTEX_COLOR": "#215C41",
-        "BACKGROUND_CANVAS_COLOR": "#163623",
-        "FRAME_COLOR": "#0C2B1A",
-        "AUTHOR_NAME_COLOR": "#FFFFFF"
-    },
-    "UBUNTU":{
-        "BUTTON_COLOR": "#b35625",
-        "SELECTED_VERTEX_COLOR": "#FFFFFF",
-        "VERTEX_COLOR": "#d45102",
-        "BACKGROUND_CANVAS_COLOR": "#404040",
-        "FRAME_COLOR": "#303030",
-        "AUTHOR_NAME_COLOR": "#b35625"
-    },
-    "LA NOCHE ESTRELLADA":{
-        "BUTTON_COLOR": "#9bafaa",
-        "SELECTED_VERTEX_COLOR": "#aed4eb",
-        "VERTEX_COLOR": "#8fadbf",
-        "BACKGROUND_CANVAS_COLOR": "#557491",
-        "FRAME_COLOR": "#242d34",
-        "AUTHOR_NAME_COLOR": "#d5bc6a"
-    },
-    "LA GRAN OLA":{
-        "BUTTON_COLOR": "#a6a49b",
-        "SELECTED_VERTEX_COLOR": "#d5bc6a",
-            "VERTEX_COLOR": "#e7e2d2",
-        "BACKGROUND_CANVAS_COLOR": "#8599a4",
-        "FRAME_COLOR": "#4a5f79",
-        "AUTHOR_NAME_COLOR": "#2d3a4a"
-    },
-    "ANTARTICA":{
-        "BUTTON_COLOR": "#9BA4B5",
-        "SELECTED_VERTEX_COLOR": "#becde8",
-        "VERTEX_COLOR": "#9BA4B5",
-        "BACKGROUND_CANVAS_COLOR": "#394867",
-        "FRAME_COLOR": "#212A3E",
-        "AUTHOR_NAME_COLOR": "#83764F"
-    },
-    "BREAKING BAD":{
-        "BUTTON_COLOR": "#F7E1AE",
-        "SELECTED_VERTEX_COLOR": "#b3a37f",
-        "VERTEX_COLOR": "#F7E1AE",
-        "BACKGROUND_CANVAS_COLOR": "#617A55",
-        "FRAME_COLOR": "#3d4d36",
-        "AUTHOR_NAME_COLOR": "#000000"
-    },
-    "SOFT":{
-        "BUTTON_COLOR": "#E4D0D0",
-        "SELECTED_VERTEX_COLOR": "#a89d9d",
-        "VERTEX_COLOR": "#E4D0D0",
-        "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
-        "FRAME_COLOR": "#867070",
-        "AUTHOR_NAME_COLOR": "#000000"
-    },
-    "TURQUOISE": {
-        "BUTTON_COLOR": "#0E8388",
-        "SELECTED_VERTEX_COLOR": "#b7c4c1",
-        "VERTEX_COLOR": "#83918e",
-        "BACKGROUND_CANVAS_COLOR": "#2E4F4F",
-        "FRAME_COLOR": "#2C3333",
-        "AUTHOR_NAME_COLOR": "#CBE4DE"
-    },
-    "DEEP PURPLE":{
-        "BUTTON_COLOR": "#bdb8ac",
-        "SELECTED_VERTEX_COLOR": "#bdb8ac",
-        "VERTEX_COLOR": "#bdb8ac",
-        "BACKGROUND_CANVAS_COLOR": "#6D5D6E",
-        "FRAME_COLOR": "#4F4557",
-        "AUTHOR_NAME_COLOR": "#F4EEE0"
-    },
-    "THIS ONE IS UGLY":{
-        "BUTTON_COLOR": "#F67280",
-        "SELECTED_VERTEX_COLOR": "#F67280",
-        "VERTEX_COLOR": "#C06C84",
-        "BACKGROUND_CANVAS_COLOR": "#6C5B7B",
-        "FRAME_COLOR": "#355C7D",
-        "AUTHOR_NAME_COLOR": "#F67280"
-    },
-    "FROST": {
-        "BUTTON_COLOR": "#00ADB5",
-        "SELECTED_VERTEX_COLOR": "#13787d",
-        "VERTEX_COLOR": "#00ADB5",
-        "BACKGROUND_CANVAS_COLOR": "#393E46",
-        "FRAME_COLOR": "#222831",
-        "AUTHOR_NAME_COLOR": "#EEEEEE"
-    },
-    "NEKOS": {
-        "BUTTON_COLOR": "#DEFCF9",
-        "VERTEX_COLOR": "#CADEFC",
-        "SELECTED_VERTEX_COLOR": "#DEFCF9",
-        "BACKGROUND_CANVAS_COLOR": "#C3BEF0",
-        "FRAME_COLOR": "#CCA8E9",
-        "AUTHOR_NAME_COLOR": "#DEFCF9"
-    },
-    "VAMPIRE": {
-        "BUTTON_COLOR": "#FF0000",
-        "SELECTED_VERTEX_COLOR": "#FF0000",
-        "VERTEX_COLOR": "#FF0000",
-        "BACKGROUND_CANVAS_COLOR": "#950101",
-        "FRAME_COLOR": "#3D0000",
-        "AUTHOR_NAME_COLOR": "#FF0000"
-    }
+VERSION = '0.4.8'
+DEFAULT_SCR_WIDTH = 600
+DEFAULT_SCR_HEIGHT = 600
+DEFAULT_NODE_RADIUS = 25
+DEFAULT_THEME = 'BROWN'
+BUTTON_HEIGHT = 30
+BUTTON_WIDTH = 60
+XMARGEN = 7
+YMARGEN = 7
+THEMES = {
+    "BROWN":{
+        "BUTTON_COLOR": "#ede4cc",
+        "SELECTED_VERTEX_COLOR": "#c2baa7",
+        "VERTEX_COLOR": "#e3d7c5",
+        "BACKGROUND_CANVAS_COLOR": "#c7b9a5",
+        "FRAME_COLOR": "#87715f",
+        "AUTHOR_NAME_COLOR": "#301d05"
+    },
+    "LIGHT":{
+        "BUTTON_COLOR": "#a6a6a6",
+        "SELECTED_VERTEX_COLOR": "#b3b3b3",
+        "VERTEX_COLOR": "#bfbdbd",
+        "BACKGROUND_CANVAS_COLOR": "#d4d3d2",
+        "FRAME_COLOR": "#b3b3b3",
+        "AUTHOR_NAME_COLOR": "#454545"
+    },
+    "BLUE":{
+        "BUTTON_COLOR": "#b7e7e8",
+        "VERTEX_COLOR": "#a7d6fc",
+        "SELECTED_VERTEX_COLOR": "#91b9ba",
+        "BACKGROUND_CANVAS_COLOR": "#b5d9f7",
+        "FRAME_COLOR": "#6aaade",
+        "AUTHOR_NAME_COLOR": "#0b2d47"
+    },
+    "DARK":{
+        "BUTTON_COLOR": "#6a6a7d",
+        "SELECTED_VERTEX_COLOR": "#8d8da6",
+        "VERTEX_COLOR": "#7d7d96",
+        "BACKGROUND_CANVAS_COLOR": "#404147",
+        "FRAME_COLOR": "#272729",
+        "AUTHOR_NAME_COLOR": "#7c7c9c"
+    },
+    "PURPLE":{
+        "BUTTON_COLOR": "#f2c8fa",
+        "SELECTED_VERTEX_COLOR": "#bf97c7",
+        "VERTEX_COLOR": "#e7cdf7",
+        "BACKGROUND_CANVAS_COLOR": "#e4c3fa",
+        "FRAME_COLOR": "#d899f7",
+        "AUTHOR_NAME_COLOR": "#6d1aa3"
+    },
+    "GREEN":{
+        "BUTTON_COLOR": "#B5FFC7",
+        "SELECTED_VERTEX_COLOR": "#05331F",
+        "VERTEX_COLOR": "#A1FDB3",
+        "BACKGROUND_CANVAS_COLOR": "#BFFFCF",
+        "FRAME_COLOR": "#80FF99",
+        "AUTHOR_NAME_COLOR": "#05331F"
+    },
+    "DARKGREEN":{
+        "BUTTON_COLOR": "#173F2D",
+        "SELECTED_VERTEX_COLOR": "#05331F",
+        "VERTEX_COLOR": "#215C41",
+        "BACKGROUND_CANVAS_COLOR": "#163623",
+        "FRAME_COLOR": "#0C2B1A",
+        "AUTHOR_NAME_COLOR": "#FFFFFF"
+    },
+    "UBUNTU":{
+        "BUTTON_COLOR": "#b35625",
+        "SELECTED_VERTEX_COLOR": "#FFFFFF",
+        "VERTEX_COLOR": "#d45102",
+        "BACKGROUND_CANVAS_COLOR": "#404040",
+        "FRAME_COLOR": "#303030",
+        "AUTHOR_NAME_COLOR": "#b35625"
+    },
+    "LA NOCHE ESTRELLADA":{
+        "BUTTON_COLOR": "#9bafaa",
+        "SELECTED_VERTEX_COLOR": "#aed4eb",
+        "VERTEX_COLOR": "#8fadbf",
+        "BACKGROUND_CANVAS_COLOR": "#557491",
+        "FRAME_COLOR": "#242d34",
+        "AUTHOR_NAME_COLOR": "#d5bc6a"
+    },
+    "LA GRAN OLA":{
+        "BUTTON_COLOR": "#a6a49b",
+        "SELECTED_VERTEX_COLOR": "#d5bc6a",
+            "VERTEX_COLOR": "#e7e2d2",
+        "BACKGROUND_CANVAS_COLOR": "#8599a4",
+        "FRAME_COLOR": "#4a5f79",
+        "AUTHOR_NAME_COLOR": "#2d3a4a"
+    },
+    "ANTARTICA":{
+        "BUTTON_COLOR": "#9BA4B5",
+        "SELECTED_VERTEX_COLOR": "#becde8",
+        "VERTEX_COLOR": "#9BA4B5",
+        "BACKGROUND_CANVAS_COLOR": "#394867",
+        "FRAME_COLOR": "#212A3E",
+        "AUTHOR_NAME_COLOR": "#83764F"
+    },
+    "BREAKING BAD":{
+        "BUTTON_COLOR": "#F7E1AE",
+        "SELECTED_VERTEX_COLOR": "#b3a37f",
+        "VERTEX_COLOR": "#F7E1AE",
+        "BACKGROUND_CANVAS_COLOR": "#617A55",
+        "FRAME_COLOR": "#3d4d36",
+        "AUTHOR_NAME_COLOR": "#000000"
+    },
+    "SOFT":{
+        "BUTTON_COLOR": "#E4D0D0",
+        "SELECTED_VERTEX_COLOR": "#a89d9d",
+        "VERTEX_COLOR": "#E4D0D0",
+        "BACKGROUND_CANVAS_COLOR": "#D5B4B4",
+        "FRAME_COLOR": "#867070",
+        "AUTHOR_NAME_COLOR": "#000000"
+    },
+    "TURQUOISE": {
+        "BUTTON_COLOR": "#0E8388",
+        "SELECTED_VERTEX_COLOR": "#b7c4c1",
+        "VERTEX_COLOR": "#83918e",
+        "BACKGROUND_CANVAS_COLOR": "#2E4F4F",
+        "FRAME_COLOR": "#2C3333",
+        "AUTHOR_NAME_COLOR": "#CBE4DE"
+    },
+    "DEEP PURPLE":{
+        "BUTTON_COLOR": "#bdb8ac",
+        "SELECTED_VERTEX_COLOR": "#bdb8ac",
+        "VERTEX_COLOR": "#bdb8ac",
+        "BACKGROUND_CANVAS_COLOR": "#6D5D6E",
+        "FRAME_COLOR": "#4F4557",
+        "AUTHOR_NAME_COLOR": "#F4EEE0"
+    },
+    "THIS ONE IS UGLY":{
+        "BUTTON_COLOR": "#F67280",
+        "SELECTED_VERTEX_COLOR": "#F67280",
+        "VERTEX_COLOR": "#C06C84",
+        "BACKGROUND_CANVAS_COLOR": "#6C5B7B",
+        "FRAME_COLOR": "#355C7D",
+        "AUTHOR_NAME_COLOR": "#F67280"
+    },
+    "FROST": {
+        "BUTTON_COLOR": "#00ADB5",
+        "SELECTED_VERTEX_COLOR": "#13787d",
+        "VERTEX_COLOR": "#00ADB5",
+        "BACKGROUND_CANVAS_COLOR": "#393E46",
+        "FRAME_COLOR": "#222831",
+        "AUTHOR_NAME_COLOR": "#EEEEEE"
+    },
+    "NEKOS": {
+        "BUTTON_COLOR": "#DEFCF9",
+        "VERTEX_COLOR": "#CADEFC",
+        "SELECTED_VERTEX_COLOR": "#DEFCF9",
+        "BACKGROUND_CANVAS_COLOR": "#C3BEF0",
+        "FRAME_COLOR": "#CCA8E9",
+        "AUTHOR_NAME_COLOR": "#DEFCF9"
+    },
+    "VAMPIRE": {
+        "BUTTON_COLOR": "#FF0000",
+        "SELECTED_VERTEX_COLOR": "#FF0000",
+        "VERTEX_COLOR": "#FF0000",
+        "BACKGROUND_CANVAS_COLOR": "#950101",
+        "FRAME_COLOR": "#3D0000",
+        "AUTHOR_NAME_COLOR": "#FF0000"
+    }
 }
```

### Comparing `graphdisplay-0.4.7/graphdisplay/graphs/graph.py` & `graphdisplay-0.4.8/graphdisplay/graphs/graph.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,578 +1,578 @@
-"""
-Official graph implementation for Data Structures and Algorithms subject at Carlos III university of Madrid
-
-    - min_number_edges function implemented by Raúl Aguilar Arroyo (https://github.com/Ragarr)
-    - transpose and is_strongly_connected functions implemented by Alberto Penas Díaz (https://github.com/seniorbeto)
-      and Natalia Rodriguez Navarro (https://github.com/NataaNK)
-"""
-import math
-
-class AdjacentVertex:
-    """This class allows us to represent a tuple with an adjacent vertex
-    and the weight associated (by default 1, for non-unweighted graphs)"""
-
-    def __init__(self, vertex, weight=None):
-        self._vertex = vertex
-        self._weight = weight
-
-    def __str__(self):
-        if self._weight != None:
-            return '(' + str(self._vertex) + ',' + str(self._weight) + ')'
-        else:
-            return str(self._vertex)
-
-
-class Graph():
-    def __init__(self, vertices, directed=True):
-        """We use a dictionary to represent the graph
-        the dictionary's keys are the vertices
-        The value associated for a given key will be the list of their neighbours.
-        Initially, the list of neighbours is empty"""
-        self._vertices = {}
-        for v in vertices:
-            self._vertices[v] = []
-        self._directed = directed
-
-    def addEdge(self, start, end, weight=None):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return
-
-        # adds to the end of the list of neighbours for start
-        self._vertices[start].append(AdjacentVertex(end, weight))
-
-        if self._directed == False:
-            # adds to the end of the list of neighbours for end
-            self._vertices[end].append(AdjacentVertex(start, weight))
-
-    def containsEdge(self, start, end):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return 0
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return 0
-
-        # we search the AdjacentVertex whose v is end
-        for adj in self._vertices[start]:
-            if adj._vertex == end:
-                if adj._weight != None:
-                    return adj._weight
-                else:
-                    return 1  # unweighted graphs
-        return 0  # does not exist
-
-    def removeEdge(self, start, end):
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!')
-            return
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!')
-            return
-
-        # we must look for the adjacent AdjacentVertex (neighbour)  whose vertex is end, and then remove it
-        for adj in self._vertices[start]:
-            if adj._vertex == end:
-                self._vertices[start].remove(adj)
-        if self._directed == False:
-            # we must also look for the AdjacentVertex (neighbour)  whose vertex is end, and then remove it
-            for adj in self._vertices[end]:
-                if adj._vertex == start:
-                    self._vertices[end].remove(adj)
-
-    def __str__(self):
-        result = ''
-        for v in self._vertices:
-            result += '\n' + str(v) + ':'
-            for adj in self._vertices[v]:
-                result += str(adj) + "  "
-        return result
-
-    def add_vertex(self, vertex: str) -> None:
-        if vertex in self._vertices.keys():
-            print(vertex, ' already exists!')
-            return
-        self._vertices[vertex] = []
-
-    def _dfs(self, vertex: str, visited: dict) -> None:
-        visited[vertex] = True
-        for adj in self._vertices[vertex]:
-            # adj is an object of AdjacentVertex
-            adj_vertex = adj._vertex
-            if not visited[adj_vertex]:
-                self._dfs(adj_vertex, visited)
-
-    def _bfs(self, vertex: str, visited: dict) -> None:
-        queue = [vertex]
-        visited[vertex] = True
-        while len(queue) > 0:
-            u = queue.pop(0)
-            for adj in self._vertices[u]:
-                # remember that adj is an AdjacentVertex
-                if not visited[adj._vertex]:
-                    queue.append(adj._vertex)
-                    visited[adj._vertex] = True
-
-    def non_accessible(self, vertex: str) -> list:
-        """gets a vertex and returns the list of vertices
-        that cannot be reached from vertex, that is, there is no path
-        from vertex to these vertices"""
-        # First, we need to obtain all vertices that can be
-        # reached from vertex. To do this, we can apply
-        # the algorithms of dfs or bfs
-        visited = {}
-        for v1 in self._vertices:
-            visited[v1] = False
-        self._dfs(vertex, visited)
-        # The function _dfs will visit all vertices reachable
-        # from vertex. Therefore, the non-visited vertices
-        # will form the list of non-accessible vertices from vertex
-        result = []  # list with the non-accessible vertices
-        for v1 in self._vertices:
-            if not visited[v1]:
-                result.append(v1)
-
-        return result
-
-    def get_reachable(self, vertex: str, alg: str = '_dfs') -> list:
-        """gets a vertex and returns the list of vertices
-        that can be reached from vertex, that is, there is a path
-        from vertex to these vertices"""
-        # First, we need to obtain all vertices that can be
-        # reached from vertex. To do this, we can apply
-        # the algorithms of dfs or bfs
-        visited = {}
-        for v1 in self._vertices:
-            visited[v1] = False
-        if alg == '_dfs':
-            self._dfs(vertex, visited)
-        else:
-            self._bfs(vertex, visited)
-
-        # The function _dfs will visit all vertices reachable
-        # from vertex. Therefore, the visited vertices
-        # will form the list of accessible vertices from vertex
-        result = []  # list with the accessible vertices
-        for v1 in self._vertices:
-            if visited[v1]:
-                result.append(v1)
-
-        return result
-
-    def _check_bipartite(self, source: str, color: dict) -> bool:
-
-        # Assign first color to source
-        queue = [source]
-        color[source] = 1
-        # similar to bfs
-        while len(queue):
-            u = queue.pop(0)
-            for adj in self._vertices[u]:
-                adj_vertex = adj.vertex
-                if color[adj_vertex] is None:
-                    color[adj_vertex] = 1 - color[u]
-                    queue.append(adj_vertex)
-                elif color[adj_vertex] == color[u]:
-                    return False
-
-        # If we reach here, then all adjacent
-        # vertices can be colored with alternate
-        # color
-        return True
-
-    def check_bipartite(self) -> bool:
-        """ returns True if the graph is bipartite and False eoc
-        A graph is bipartite is a graph whose vertices can be divided
-        into two independent sets, U and V
-        such that every edge (u, v) either connects a vertex
-        from U to V or a vertex from V to U.
-        In other words, for every edge (u, v), either u belongs to U and v to V,
-         or u belongs to V and v to U. We can also say that there is no edge
-         that connects vertices of same set. """
-        color = {}
-        # We use a dictionary color to save the color
-        # assigned to each vertex: 1 means first color (origins)
-        # , 0 means second color (target)
-        for v1 in self._vertices:
-            color[v1] = None
-
-        for v1 in self._vertices:
-            if color[v1] is None:
-                if not self._check_bipartite(v1, color):
-                    return False
-
-        return True
-
-    def _has_cycles_bfs(self, vertex: str, visited: dict) -> bool:
-        """This is function is based on bfs to detect if there is
-        some cycle in the breadth traversal from vertex. It uses the dictionary
-        visited and the parent of the vertices to detect
-        cycle in subgraph reachable from vertex v."""
-
-        # Mark the current vertex as visited
-        queue = [vertex]
-        parents = {}
-        for v1 in self._vertices:
-            parents[v1] = None
-
-        while len(queue) > 0:
-            s = queue.pop(0)
-            visited[s] = True
-            for adj in self._vertices[s]:
-                adj_vertex = adj.vertex
-                if not visited[adj_vertex]:
-                    visited[adj_vertex] = True
-                    queue.append(adj_vertex)
-                    parents[adj_vertex] = s
-                elif parents[s] != adj_vertex:
-                    # if the ajd_vertex has been already visited,
-                    # and it is not the parent of current vertex,
-                    # then there is a cycle
-                    return True
-        return False
-
-    def _has_cycles_dfs(self, vertex: str, visited: dict, parent: str) -> bool:
-        """This is recursive function that uses the dictionary
-        visited and the parent of the vertices to detect
-        cycle in subgraph reachable from vertex v."""
-
-        # Mark the current vertex as visited
-        visited[vertex] = True
-        # Recur for all the vertices
-        # adjacent to this vertex
-        for adj in self._vertices[vertex]:
-            adj_vertex = adj.vertex
-            # If the node is not visited then recurse on it
-            if not visited[adj_vertex]:
-                if self._has_cycles_dfs(adj_vertex, visited, vertex):
-                    return True
-            elif parent != adj_vertex:
-                # if the ajd_vertex has been already visited,
-                # and it is not the parent of current vertex,
-                # then there is a cycle
-                return True
-        print()
-        return False
-
-    def _has_cycles_directed(self, vertex: str, visited: dict, rec_stack: dict) -> bool:
-        """detects a cycle in a directed graph using the
-        dfs alg. Moreover, visited and rec_stack allow us
-        to detect if a vertex has been previously visited."""
-
-        # Mark the current vertex as visited
-        visited[vertex] = True
-        rec_stack[vertex] = True
-        # Recur for all the vertices
-        # adjacent to this vertex
-        for adj in self._vertices[vertex]:
-            adj_vertex = adj._vertex
-            # If the node is not visited then recurse on it
-            if not visited[adj_vertex]:
-                if self._has_cycles_directed(adj_vertex, visited, rec_stack):
-                    return True
-            elif rec_stack[adj_vertex]:
-                return True
-        # The node needs to be popped from
-        # recursion stack before function ends
-        rec_stack[vertex] = False
-        return False
-
-    def has_cycles(self, alg: str = 'dfs') -> bool:
-        """returns True if the graph contains a cycle, False eoc"""
-        visited = {}
-        recursion_stack = {}
-
-        for v1 in self._vertices:
-            visited[v1] = False
-            # we will only use it for directed graphs
-            recursion_stack[v1] = False
-
-        # Call the recursive helper
-        # function to detect cycle in different
-        # DFS trees
-        for v1 in self._vertices:
-            if not visited[v1]:
-                if self._directed:
-                    result = self._has_cycles_directed(v1, visited, recursion_stack)
-                else:
-                    if alg == 'dfs':
-                        result = self._has_cycles_dfs(v1, visited, None)
-                    else:
-                        result = self._has_cycles_bfs(v1, visited)
-
-                if result:
-                    return True
-
-        return False
-
-    def min_distance(self, distances: dict, visited: dict) -> int:
-        """ This function is used from dijkstra.
-        It returns the vertex (index) whose associated value in
-        the dictionary distances is the smallest value. We
-        only consider the set of vertices that have not been visited"""
-        # Initialize minimum distance for next node
-        min_distance = math.inf
-        min_vertex = None
-
-        # returns the vertex with minimum distance from the non-visited vertices
-        for vertex in self._vertices.keys():
-            if distances[vertex] <= min_distance and not visited[vertex]:
-                min_distance = distances[vertex]  # update the new smallest
-                min_vertex = vertex  # update the index of the smallest
-
-        return min_vertex
-
-    def dijkstra(self, origin: object) -> None:
-        visited = {}  # for each vertex (key), the value is a boolean indicating if the vertex has been visited
-        previous = {}  # for each vertex (key), the value is the previous node in the minimum path from origin
-        distances = {}  # for each vertex (key), the value is minimum distance in the minimum path from origin
-
-        # initialize dictionaries
-        for v in self._vertices.keys():
-            visited[v] = False
-            previous[v] = None
-            distances[v] = math.inf
-
-        # The distance from origin to itself is 0
-        distances[origin] = 0
-
-        for _ in range(len(self._vertices)):
-            # pick the non-visited vertex with minimum distance
-            u = self.min_distance(distances, visited)
-            visited[u] = True
-            # get the adjacent vertices of u
-            for adj in self._vertices[u]:
-                i = adj._vertex
-                w = adj._weight
-                # for non-visited vertex, we have to check if its distance is greater than the distance from u
-                if not visited[i] and distances[i] > distances[u] + w:
-                    # we must update because its distance is greater than the new distance
-                    distances[i] = distances[u] + w
-                    previous[i] = u
-
-        # Finally, we print the minimum path from origin to the other vertices
-        #self.print_solution(distances, previous, origin)
-
-        return distances, previous
-
-    def print_solution(self, distances: dict, previous: dict, origin: object):
-        """Both Dijkstra and Bellman-Ford algorithms use this function.
-        For each vertex, the function is able to rebuild the reverse path from i to origin.
-        To do this, the function only needs to read the value associated to the vertex in the dictionary
-        previous until to reach a vertex whouse associated value is None (origin)"""
-        print("Minimum path from ", origin)
-
-        for i in self._vertices.keys():
-            if distances[i] == math.inf:
-                print("There is not path from ", origin, ' to ', i)
-            else:
-                # minimum_path is the list which contains the minimum path from origin to i
-                minimum_path = []
-                prev = previous[i]
-                # this loop helps us to build the path
-                while prev is not None:
-                    minimum_path.insert(0, prev)
-                    prev = previous[prev]
-
-                # we append the last vertex, which is i
-                minimum_path.append(i)
-
-                # we print the path from v to i and the distance
-                print(origin, '->', i, ":", minimum_path, distances[i])
-
-    def bellmanford(self, origin: object) -> None:
-        """Bellman-Ford algorithm for minimum path"""
-        previous = {}
-        distances = {}
-        for v in self._vertices.keys():
-            previous[v] = None
-            distances[v] = math.inf
-        distances[origin] = 0
-
-        for _ in range(len(self._vertices) - 1):
-            for u in self._vertices.keys():
-                # get all adjacent vertices of u
-                for adj in self._vertices[u]:
-                    v = adj.vertex
-                    w = adj.weight
-                    if distances[v] > distances[u] + w:
-                        distances[v] = distances[u] + w
-                        previous[v] = u
-
-        # final review to check if there is a solution, or there is a negative cicle (therefore, there is no solution)
-        for u in self._vertices.keys():
-            for adj in self._vertices[u]:
-                v = adj._vertex
-                w = adj._weight
-                if distances[v] > distances[u] + w:
-                    # There is at least a negative cicle.
-                    print('There is no solution ', origin)
-                    return False
-
-        self.print_solution(distances, previous, origin)
-        return distances, previous
-
-    def minimum_path(self, start: object, end: object) -> list:
-        """ returns a list containing the path from star to end.
-        It also returns the distance of the path. If the path
-        does not exist, it returns an empty list and infinito"""
-        if start not in self._vertices.keys():
-            print(start, ' does not exist!!!')
-            return None, None
-        if end not in self._vertices.keys():
-            print(end, ' does not exist!!!')
-            return None, None
-
-        distances, previous = self.dijkstra(start)
-        if distances[end] == math.inf:
-            return [], math.inf
-
-        result = [end]
-        prev = previous[end]
-        while prev is not None:
-            result.insert(0, prev)
-            prev = previous[prev]
-
-        return result, distances[end]
-
-    def min_number_edges(self, start: str, end: str) -> int:
-        """returns the minimum number of edges from start to end, kind of dijskstra without weights"""
-        visited = {}
-        distances = {}
-        for v in self._vertices.keys():
-            visited[v] = False
-            distances[v] = math.inf
-        distances[start] = 0
-
-        for n in range(len(self._vertices)):
-            current = self.__closer_vertex(visited, distances)
-            visited[current] = True
-
-            for adjV in self._vertices[current]:
-                v = adjV._vertex
-                if visited[v] == False and distances[v] > distances[current] + 1:
-                    distances[v] = distances[current] + 1
-
-        path = []
-        if distances[end] != math.inf:
-            path.insert(0, end)
-            current = end
-            for i in range(distances[end]):
-                posibles = []
-                for vx in distances:
-                    if distances[vx] == distances[end] - 1 - i:
-                        posibles.append(vx)
-                for pos in posibles:
-                    reachable = []
-                    for adj in self._vertices[pos]:
-                        reachable.append(adj._vertex)
-                    if current in reachable:
-                        path.insert(0, pos)
-                        current = pos
-                        break
-        return path
-
-    def __closer_vertex(self, visited, distances):
-        """This function is used by the min_number_edges function."""
-        min = math.inf
-        for vertex in self._vertices.keys():
-            if distances[vertex] <= min and visited[vertex] == False:
-                min = distances[vertex]
-                min_vertex = vertex
-        return min_vertex
-
-    def transpose(self):
-        """ returns a new graph that is the transpose graph of self"""
-        if self._directed and self._vertices != []:
-            nuevos_vertices = []
-            for v in self._vertices:
-                nuevos_vertices.append(v)
-            transpose = Graph(nuevos_vertices)
-            for v in self._vertices:
-                for edge in self._vertices[v]:
-                    transpose.addEdge(edge._vertex, v, edge._weight)
-        else:
-            transpose = self
-
-        return transpose
-
-    def is_strongly_connected(self) -> bool:
-        """ This function checks if the graph is strongly connected.
-        A directed graph is strongly connected when for any pair of vertices
-        u and v, there is always a path from u to v. If the graph is undirected,
-        the function returns True if the graph is connected, that is, there is
-        a path from any vertex to any other vertex in the graph.
-        """
-        if len(self._vertices) == 0:
-            print('ERROR: empty graph')
-            return
-        if len(self._vertices) > 1:
-            for key in list(self._vertices):
-                visitados = [key]
-                running = [key]
-                while len(running) >= 1:
-                    key = running.pop(0)
-                    for edge in self._vertices[key]:
-                        if edge._vertex not in visitados:
-                            visitados.append(edge._vertex)
-                            running.append(edge._vertex)
-                if len(visitados) != len(self._vertices):
-                    return False
-        return True
-
-if __name__ == "__main__":
-    g = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'])
-    g.addEdge('A', 'B', 1)
-    g.addEdge('A', 'C', 5)
-    g.addEdge('A', 'D', 3)
-    g.addEdge('B', 'C', 2)
-    g.addEdge('B', 'E', 1)
-    g.addEdge('C', 'D', 8)
-    g.addEdge('C', 'E', 4)
-    g.addEdge('C', 'F', 6)
-    g.addEdge('D', 'F', 1)
-    g.addEdge('E', 'F', 2)
-    g.addEdge('E', 'G', 3)
-    g.addEdge('F', 'G', 4)
-    g.addEdge('F', 'H', 2)
-    g.addEdge('G', 'H', 1)
-    g.addEdge('G', 'I', 2)
-    g.addEdge('G', 'J', 4)
-    g.addEdge('H', 'J', 3)
-    g.addEdge('I', 'J', 1)
-
-    #g.addEdge('B', 'J', 1)
-
-    my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
-    my_gragph.addEdge('A', 'B', 4)
-    my_gragph.addEdge('B', 'C', 8)
-    my_gragph.addEdge('C', 'A', 100)
-    my_gragph.addEdge('D', 'E', 7)
-    my_gragph.addEdge('E', 'F', 10)
-    my_gragph.addEdge('F', 'G', 5)
-    my_gragph.addEdge('G', 'Z', 6)
-    my_gragph.addEdge('A', 'H', 2)
-    my_gragph.addEdge('B', 'I', 3)
-    my_gragph.addEdge('C', 'J', 4)
-    my_gragph.addEdge('D', 'K', 5)
-    my_gragph.addEdge('E', 'L', 6)
-    my_gragph.addEdge('F', 'D', 3)
-    my_gragph.addEdge('G', 'H', 9)
-    my_gragph.addEdge('H', 'Z', 2)
-    my_gragph.addEdge('I', 'J', 1)
-    my_gragph.addEdge('J', 'A', 6)
-    my_gragph.addEdge('K', 'L', 5)
-    my_gragph.addEdge('L', 'M', 4)
-    my_gragph.addEdge('M', 'H', 3)
-    my_gragph.addEdge('N', 'O', 2)
-    my_gragph.addEdge('O', 'P', 1)
-    my_gragph.addEdge('P', 'Q', 7)
-    my_gragph.addEdge('H', 'A', 20)
-    my_gragph.addEdge('K', 'B', 7)
-    my_gragph.addEdge('H', 'N', 9)
-    my_gragph.addEdge('Q', 'D', 40)
-
-    print(my_gragph.min_number_edges('H', 'P'))
+"""
+Official graph implementation for Data Structures and Algorithms subject at Carlos III university of Madrid
+
+    - min_number_edges function implemented by Raúl Aguilar Arroyo (https://github.com/Ragarr)
+    - transpose and is_strongly_connected functions implemented by Alberto Penas Díaz (https://github.com/seniorbeto)
+      and Natalia Rodriguez Navarro (https://github.com/NataaNK)
+"""
+import math
+
+class AdjacentVertex:
+    """This class allows us to represent a tuple with an adjacent vertex
+    and the weight associated (by default 1, for non-unweighted graphs)"""
+
+    def __init__(self, vertex, weight=None):
+        self._vertex = vertex
+        self._weight = weight
+
+    def __str__(self):
+        if self._weight != None:
+            return '(' + str(self._vertex) + ',' + str(self._weight) + ')'
+        else:
+            return str(self._vertex)
+
+
+class Graph():
+    def __init__(self, vertices, directed=True):
+        """We use a dictionary to represent the graph
+        the dictionary's keys are the vertices
+        The value associated for a given key will be the list of their neighbours.
+        Initially, the list of neighbours is empty"""
+        self._vertices = {}
+        for v in vertices:
+            self._vertices[v] = []
+        self._directed = directed
+
+    def addEdge(self, start, end, weight=None):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return
+
+        # adds to the end of the list of neighbours for start
+        self._vertices[start].append(AdjacentVertex(end, weight))
+
+        if self._directed == False:
+            # adds to the end of the list of neighbours for end
+            self._vertices[end].append(AdjacentVertex(start, weight))
+
+    def containsEdge(self, start, end):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return 0
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return 0
+
+        # we search the AdjacentVertex whose v is end
+        for adj in self._vertices[start]:
+            if adj._vertex == end:
+                if adj._weight != None:
+                    return adj._weight
+                else:
+                    return 1  # unweighted graphs
+        return 0  # does not exist
+
+    def removeEdge(self, start, end):
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!')
+            return
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!')
+            return
+
+        # we must look for the adjacent AdjacentVertex (neighbour)  whose vertex is end, and then remove it
+        for adj in self._vertices[start]:
+            if adj._vertex == end:
+                self._vertices[start].remove(adj)
+        if self._directed == False:
+            # we must also look for the AdjacentVertex (neighbour)  whose vertex is end, and then remove it
+            for adj in self._vertices[end]:
+                if adj._vertex == start:
+                    self._vertices[end].remove(adj)
+
+    def __str__(self):
+        result = ''
+        for v in self._vertices:
+            result += '\n' + str(v) + ':'
+            for adj in self._vertices[v]:
+                result += str(adj) + "  "
+        return result
+
+    def add_vertex(self, vertex: str) -> None:
+        if vertex in self._vertices.keys():
+            print(vertex, ' already exists!')
+            return
+        self._vertices[vertex] = []
+
+    def _dfs(self, vertex: str, visited: dict) -> None:
+        visited[vertex] = True
+        for adj in self._vertices[vertex]:
+            # adj is an object of AdjacentVertex
+            adj_vertex = adj._vertex
+            if not visited[adj_vertex]:
+                self._dfs(adj_vertex, visited)
+
+    def _bfs(self, vertex: str, visited: dict) -> None:
+        queue = [vertex]
+        visited[vertex] = True
+        while len(queue) > 0:
+            u = queue.pop(0)
+            for adj in self._vertices[u]:
+                # remember that adj is an AdjacentVertex
+                if not visited[adj._vertex]:
+                    queue.append(adj._vertex)
+                    visited[adj._vertex] = True
+
+    def non_accessible(self, vertex: str) -> list:
+        """gets a vertex and returns the list of vertices
+        that cannot be reached from vertex, that is, there is no path
+        from vertex to these vertices"""
+        # First, we need to obtain all vertices that can be
+        # reached from vertex. To do this, we can apply
+        # the algorithms of dfs or bfs
+        visited = {}
+        for v1 in self._vertices:
+            visited[v1] = False
+        self._dfs(vertex, visited)
+        # The function _dfs will visit all vertices reachable
+        # from vertex. Therefore, the non-visited vertices
+        # will form the list of non-accessible vertices from vertex
+        result = []  # list with the non-accessible vertices
+        for v1 in self._vertices:
+            if not visited[v1]:
+                result.append(v1)
+
+        return result
+
+    def get_reachable(self, vertex: str, alg: str = '_dfs') -> list:
+        """gets a vertex and returns the list of vertices
+        that can be reached from vertex, that is, there is a path
+        from vertex to these vertices"""
+        # First, we need to obtain all vertices that can be
+        # reached from vertex. To do this, we can apply
+        # the algorithms of dfs or bfs
+        visited = {}
+        for v1 in self._vertices:
+            visited[v1] = False
+        if alg == '_dfs':
+            self._dfs(vertex, visited)
+        else:
+            self._bfs(vertex, visited)
+
+        # The function _dfs will visit all vertices reachable
+        # from vertex. Therefore, the visited vertices
+        # will form the list of accessible vertices from vertex
+        result = []  # list with the accessible vertices
+        for v1 in self._vertices:
+            if visited[v1]:
+                result.append(v1)
+
+        return result
+
+    def _check_bipartite(self, source: str, color: dict) -> bool:
+
+        # Assign first color to source
+        queue = [source]
+        color[source] = 1
+        # similar to bfs
+        while len(queue):
+            u = queue.pop(0)
+            for adj in self._vertices[u]:
+                adj_vertex = adj.vertex
+                if color[adj_vertex] is None:
+                    color[adj_vertex] = 1 - color[u]
+                    queue.append(adj_vertex)
+                elif color[adj_vertex] == color[u]:
+                    return False
+
+        # If we reach here, then all adjacent
+        # vertices can be colored with alternate
+        # color
+        return True
+
+    def check_bipartite(self) -> bool:
+        """ returns True if the graph is bipartite and False eoc
+        A graph is bipartite is a graph whose vertices can be divided
+        into two independent sets, U and V
+        such that every edge (u, v) either connects a vertex
+        from U to V or a vertex from V to U.
+        In other words, for every edge (u, v), either u belongs to U and v to V,
+         or u belongs to V and v to U. We can also say that there is no edge
+         that connects vertices of same set. """
+        color = {}
+        # We use a dictionary color to save the color
+        # assigned to each vertex: 1 means first color (origins)
+        # , 0 means second color (target)
+        for v1 in self._vertices:
+            color[v1] = None
+
+        for v1 in self._vertices:
+            if color[v1] is None:
+                if not self._check_bipartite(v1, color):
+                    return False
+
+        return True
+
+    def _has_cycles_bfs(self, vertex: str, visited: dict) -> bool:
+        """This is function is based on bfs to detect if there is
+        some cycle in the breadth traversal from vertex. It uses the dictionary
+        visited and the parent of the vertices to detect
+        cycle in subgraph reachable from vertex v."""
+
+        # Mark the current vertex as visited
+        queue = [vertex]
+        parents = {}
+        for v1 in self._vertices:
+            parents[v1] = None
+
+        while len(queue) > 0:
+            s = queue.pop(0)
+            visited[s] = True
+            for adj in self._vertices[s]:
+                adj_vertex = adj.vertex
+                if not visited[adj_vertex]:
+                    visited[adj_vertex] = True
+                    queue.append(adj_vertex)
+                    parents[adj_vertex] = s
+                elif parents[s] != adj_vertex:
+                    # if the ajd_vertex has been already visited,
+                    # and it is not the parent of current vertex,
+                    # then there is a cycle
+                    return True
+        return False
+
+    def _has_cycles_dfs(self, vertex: str, visited: dict, parent: str) -> bool:
+        """This is recursive function that uses the dictionary
+        visited and the parent of the vertices to detect
+        cycle in subgraph reachable from vertex v."""
+
+        # Mark the current vertex as visited
+        visited[vertex] = True
+        # Recur for all the vertices
+        # adjacent to this vertex
+        for adj in self._vertices[vertex]:
+            adj_vertex = adj.vertex
+            # If the node is not visited then recurse on it
+            if not visited[adj_vertex]:
+                if self._has_cycles_dfs(adj_vertex, visited, vertex):
+                    return True
+            elif parent != adj_vertex:
+                # if the ajd_vertex has been already visited,
+                # and it is not the parent of current vertex,
+                # then there is a cycle
+                return True
+        print()
+        return False
+
+    def _has_cycles_directed(self, vertex: str, visited: dict, rec_stack: dict) -> bool:
+        """detects a cycle in a directed graph using the
+        dfs alg. Moreover, visited and rec_stack allow us
+        to detect if a vertex has been previously visited."""
+
+        # Mark the current vertex as visited
+        visited[vertex] = True
+        rec_stack[vertex] = True
+        # Recur for all the vertices
+        # adjacent to this vertex
+        for adj in self._vertices[vertex]:
+            adj_vertex = adj._vertex
+            # If the node is not visited then recurse on it
+            if not visited[adj_vertex]:
+                if self._has_cycles_directed(adj_vertex, visited, rec_stack):
+                    return True
+            elif rec_stack[adj_vertex]:
+                return True
+        # The node needs to be popped from
+        # recursion stack before function ends
+        rec_stack[vertex] = False
+        return False
+
+    def has_cycles(self, alg: str = 'dfs') -> bool:
+        """returns True if the graph contains a cycle, False eoc"""
+        visited = {}
+        recursion_stack = {}
+
+        for v1 in self._vertices:
+            visited[v1] = False
+            # we will only use it for directed graphs
+            recursion_stack[v1] = False
+
+        # Call the recursive helper
+        # function to detect cycle in different
+        # DFS trees
+        for v1 in self._vertices:
+            if not visited[v1]:
+                if self._directed:
+                    result = self._has_cycles_directed(v1, visited, recursion_stack)
+                else:
+                    if alg == 'dfs':
+                        result = self._has_cycles_dfs(v1, visited, None)
+                    else:
+                        result = self._has_cycles_bfs(v1, visited)
+
+                if result:
+                    return True
+
+        return False
+
+    def min_distance(self, distances: dict, visited: dict) -> int:
+        """ This function is used from dijkstra.
+        It returns the vertex (index) whose associated value in
+        the dictionary distances is the smallest value. We
+        only consider the set of vertices that have not been visited"""
+        # Initialize minimum distance for next node
+        min_distance = math.inf
+        min_vertex = None
+
+        # returns the vertex with minimum distance from the non-visited vertices
+        for vertex in self._vertices.keys():
+            if distances[vertex] <= min_distance and not visited[vertex]:
+                min_distance = distances[vertex]  # update the new smallest
+                min_vertex = vertex  # update the index of the smallest
+
+        return min_vertex
+
+    def dijkstra(self, origin: object) -> None:
+        visited = {}  # for each vertex (key), the value is a boolean indicating if the vertex has been visited
+        previous = {}  # for each vertex (key), the value is the previous node in the minimum path from origin
+        distances = {}  # for each vertex (key), the value is minimum distance in the minimum path from origin
+
+        # initialize dictionaries
+        for v in self._vertices.keys():
+            visited[v] = False
+            previous[v] = None
+            distances[v] = math.inf
+
+        # The distance from origin to itself is 0
+        distances[origin] = 0
+
+        for _ in range(len(self._vertices)):
+            # pick the non-visited vertex with minimum distance
+            u = self.min_distance(distances, visited)
+            visited[u] = True
+            # get the adjacent vertices of u
+            for adj in self._vertices[u]:
+                i = adj._vertex
+                w = adj._weight
+                # for non-visited vertex, we have to check if its distance is greater than the distance from u
+                if not visited[i] and distances[i] > distances[u] + w:
+                    # we must update because its distance is greater than the new distance
+                    distances[i] = distances[u] + w
+                    previous[i] = u
+
+        # Finally, we print the minimum path from origin to the other vertices
+        #self.print_solution(distances, previous, origin)
+
+        return distances, previous
+
+    def print_solution(self, distances: dict, previous: dict, origin: object):
+        """Both Dijkstra and Bellman-Ford algorithms use this function.
+        For each vertex, the function is able to rebuild the reverse path from i to origin.
+        To do this, the function only needs to read the value associated to the vertex in the dictionary
+        previous until to reach a vertex whouse associated value is None (origin)"""
+        print("Minimum path from ", origin)
+
+        for i in self._vertices.keys():
+            if distances[i] == math.inf:
+                print("There is not path from ", origin, ' to ', i)
+            else:
+                # minimum_path is the list which contains the minimum path from origin to i
+                minimum_path = []
+                prev = previous[i]
+                # this loop helps us to build the path
+                while prev is not None:
+                    minimum_path.insert(0, prev)
+                    prev = previous[prev]
+
+                # we append the last vertex, which is i
+                minimum_path.append(i)
+
+                # we print the path from v to i and the distance
+                print(origin, '->', i, ":", minimum_path, distances[i])
+
+    def bellmanford(self, origin: object) -> None:
+        """Bellman-Ford algorithm for minimum path"""
+        previous = {}
+        distances = {}
+        for v in self._vertices.keys():
+            previous[v] = None
+            distances[v] = math.inf
+        distances[origin] = 0
+
+        for _ in range(len(self._vertices) - 1):
+            for u in self._vertices.keys():
+                # get all adjacent vertices of u
+                for adj in self._vertices[u]:
+                    v = adj.vertex
+                    w = adj.weight
+                    if distances[v] > distances[u] + w:
+                        distances[v] = distances[u] + w
+                        previous[v] = u
+
+        # final review to check if there is a solution, or there is a negative cicle (therefore, there is no solution)
+        for u in self._vertices.keys():
+            for adj in self._vertices[u]:
+                v = adj._vertex
+                w = adj._weight
+                if distances[v] > distances[u] + w:
+                    # There is at least a negative cicle.
+                    print('There is no solution ', origin)
+                    return False
+
+        self.print_solution(distances, previous, origin)
+        return distances, previous
+
+    def minimum_path(self, start: object, end: object) -> list:
+        """ returns a list containing the path from star to end.
+        It also returns the distance of the path. If the path
+        does not exist, it returns an empty list and infinito"""
+        if start not in self._vertices.keys():
+            print(start, ' does not exist!!!')
+            return None, None
+        if end not in self._vertices.keys():
+            print(end, ' does not exist!!!')
+            return None, None
+
+        distances, previous = self.dijkstra(start)
+        if distances[end] == math.inf:
+            return [], math.inf
+
+        result = [end]
+        prev = previous[end]
+        while prev is not None:
+            result.insert(0, prev)
+            prev = previous[prev]
+
+        return result, distances[end]
+
+    def min_number_edges(self, start: str, end: str) -> int:
+        """returns the minimum number of edges from start to end, kind of dijskstra without weights"""
+        visited = {}
+        distances = {}
+        for v in self._vertices.keys():
+            visited[v] = False
+            distances[v] = math.inf
+        distances[start] = 0
+
+        for n in range(len(self._vertices)):
+            current = self.__closer_vertex(visited, distances)
+            visited[current] = True
+
+            for adjV in self._vertices[current]:
+                v = adjV._vertex
+                if visited[v] == False and distances[v] > distances[current] + 1:
+                    distances[v] = distances[current] + 1
+
+        path = []
+        if distances[end] != math.inf:
+            path.insert(0, end)
+            current = end
+            for i in range(distances[end]):
+                posibles = []
+                for vx in distances:
+                    if distances[vx] == distances[end] - 1 - i:
+                        posibles.append(vx)
+                for pos in posibles:
+                    reachable = []
+                    for adj in self._vertices[pos]:
+                        reachable.append(adj._vertex)
+                    if current in reachable:
+                        path.insert(0, pos)
+                        current = pos
+                        break
+        return path
+
+    def __closer_vertex(self, visited, distances):
+        """This function is used by the min_number_edges function."""
+        min = math.inf
+        for vertex in self._vertices.keys():
+            if distances[vertex] <= min and visited[vertex] == False:
+                min = distances[vertex]
+                min_vertex = vertex
+        return min_vertex
+
+    def transpose(self):
+        """ returns a new graph that is the transpose graph of self"""
+        if self._directed and self._vertices != []:
+            nuevos_vertices = []
+            for v in self._vertices:
+                nuevos_vertices.append(v)
+            transpose = Graph(nuevos_vertices)
+            for v in self._vertices:
+                for edge in self._vertices[v]:
+                    transpose.addEdge(edge._vertex, v, edge._weight)
+        else:
+            transpose = self
+
+        return transpose
+
+    def is_strongly_connected(self) -> bool:
+        """ This function checks if the graph is strongly connected.
+        A directed graph is strongly connected when for any pair of vertices
+        u and v, there is always a path from u to v. If the graph is undirected,
+        the function returns True if the graph is connected, that is, there is
+        a path from any vertex to any other vertex in the graph.
+        """
+        if len(self._vertices) == 0:
+            print('ERROR: empty graph')
+            return
+        if len(self._vertices) > 1:
+            for key in list(self._vertices):
+                visitados = [key]
+                running = [key]
+                while len(running) >= 1:
+                    key = running.pop(0)
+                    for edge in self._vertices[key]:
+                        if edge._vertex not in visitados:
+                            visitados.append(edge._vertex)
+                            running.append(edge._vertex)
+                if len(visitados) != len(self._vertices):
+                    return False
+        return True
+
+if __name__ == "__main__":
+    g = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J'])
+    g.addEdge('A', 'B', 1)
+    g.addEdge('A', 'C', 5)
+    g.addEdge('A', 'D', 3)
+    g.addEdge('B', 'C', 2)
+    g.addEdge('B', 'E', 1)
+    g.addEdge('C', 'D', 8)
+    g.addEdge('C', 'E', 4)
+    g.addEdge('C', 'F', 6)
+    g.addEdge('D', 'F', 1)
+    g.addEdge('E', 'F', 2)
+    g.addEdge('E', 'G', 3)
+    g.addEdge('F', 'G', 4)
+    g.addEdge('F', 'H', 2)
+    g.addEdge('G', 'H', 1)
+    g.addEdge('G', 'I', 2)
+    g.addEdge('G', 'J', 4)
+    g.addEdge('H', 'J', 3)
+    g.addEdge('I', 'J', 1)
+
+    #g.addEdge('B', 'J', 1)
+
+    my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
+    my_gragph.addEdge('A', 'B', 4)
+    my_gragph.addEdge('B', 'C', 8)
+    my_gragph.addEdge('C', 'A', 100)
+    my_gragph.addEdge('D', 'E', 7)
+    my_gragph.addEdge('E', 'F', 10)
+    my_gragph.addEdge('F', 'G', 5)
+    my_gragph.addEdge('G', 'Z', 6)
+    my_gragph.addEdge('A', 'H', 2)
+    my_gragph.addEdge('B', 'I', 3)
+    my_gragph.addEdge('C', 'J', 4)
+    my_gragph.addEdge('D', 'K', 5)
+    my_gragph.addEdge('E', 'L', 6)
+    my_gragph.addEdge('F', 'D', 3)
+    my_gragph.addEdge('G', 'H', 9)
+    my_gragph.addEdge('H', 'Z', 2)
+    my_gragph.addEdge('I', 'J', 1)
+    my_gragph.addEdge('J', 'A', 6)
+    my_gragph.addEdge('K', 'L', 5)
+    my_gragph.addEdge('L', 'M', 4)
+    my_gragph.addEdge('M', 'H', 3)
+    my_gragph.addEdge('N', 'O', 2)
+    my_gragph.addEdge('O', 'P', 1)
+    my_gragph.addEdge('P', 'Q', 7)
+    my_gragph.addEdge('H', 'A', 20)
+    my_gragph.addEdge('K', 'B', 7)
+    my_gragph.addEdge('H', 'N', 9)
+    my_gragph.addEdge('Q', 'D', 40)
+
+    print(my_gragph.min_number_edges('H', 'P'))
```

### Comparing `graphdisplay-0.4.7/graphdisplay/json_manager.py` & `graphdisplay-0.4.8/graphdisplay/json_manager.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-import os
-import json
-import tkinter as tk
-from tkinter import messagebox
-from datetime import datetime
-from .general_config import *
-
-class JsonManager:
-    def __init__(self, parent, graphgui):
-        self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
-
-        self.graphgui = graphgui
-        self.__parent = parent
-        self.current_data_id = None
-        self.current_data = None
-
-        try:
-            with open(self.__JSON_SAVE_DIR + '../permanent.json', "r", encoding="utf-8", newline="") as file:
-                self.__permanent = json.load(file)
-        except FileNotFoundError:
-            self.__permanent = {}
-
-        try:
-            with open(self.__JSON_SAVE_DIR + '../win_config.json', "r", encoding="utf-8", newline="") as file:
-                self._config = json.load(file)
-        except FileNotFoundError:
-            self._config = {
-                'node_radius': DEFAULT_NODE_RADIUS,
-                'theme': DEFAULT_THEME
-            }
-            self.update_main_config()
-
-    def update_main_config(self):
-        with open(self.__JSON_SAVE_DIR + '../win_config.json', "w", encoding="utf-8", newline="") as file:
-            json.dump(self._config, file, indent=4)
-
-    def update_permanent(self):
-        with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
-            json.dump(self.__permanent, file, indent=4)
-
-    def delete_permanent(self, name: str):
-        del self.__permanent[name]
-        os.remove(self.__JSON_SAVE_DIR + name + '.json')
-        self.update_permanent()
-
-    def add_permanent(self, name: str):
-        self.__permanent[name] = str(datetime.now())
-        self.update_permanent()
-
-    def get_data(self, file_name: str) -> dict:
-        try:
-            with open(self.__JSON_SAVE_DIR + file_name + '.json', "r", encoding="utf-8", newline="") as file:
-                data = json.load(file)
-        except FileNotFoundError:
-            data = None
-        self.current_data_id = file_name
-        self.current_data = data
-        return data
-
-    def save_data(self, file_name: str, data: dict):
-        with open(self.__JSON_SAVE_DIR + file_name + '.json', "w", encoding="utf-8", newline="") as file:
-            json.dump(data, file, indent=4)
-
-    def generate_save_window(self, current_position: dict):
-        SaveWindow(self.__parent, self, current_position)
-
-    def generate_load_window(self):
-        LoadWindow(self.__parent, self)
-
-    def generate_delete_window(self):
-        DeleteWindow(self.__parent, self)
-
-    def generate_config_window(self):
-        ConfigWindow(self.__parent, self)
-
-class ConfigWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager):
-        super().__init__(root)
-        self.title("Config")
-        self.resizable(False, False)
-        self.__manager = json_manager
-        self.configure(background=self.__manager.graphgui._FRAME_COLOR)
-
-        # Node configuration frame
-        self.__node_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
-        self.__node_frame.pack(padx=7, pady=7, expand=True)
-
-        # Theme configuration frame
-        self.__theme_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
-        self.__theme_frame.pack(padx=7, pady=7, expand=True)
-
-        # Node radius label
-        text_label = tk.Label(self.__node_frame,
-                              text="Node radius:",
-                              bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
-        text_label.place(x=5, y=7)
-
-        # Node radius Scale widget
-        self.__node_scale = tk.Scale(self.__node_frame,
-                                     from_=10,
-                                     to=100,
-                                     orient=tk.HORIZONTAL,
-                                     bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
-                                     troughcolor=self.__manager.graphgui._FRAME_COLOR,
-                                     highlightthickness=0,
-                                     length=150,
-                                     sliderlength=20)
-        self.__node_scale.set(self.__manager._config['node_radius'])
-        self.__node_scale.place(x=150, y=0)
-
-        # Theme label
-        text_label = tk.Label(self.__theme_frame,
-                                text="Theme:",
-                                bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR,
-                                font=("Courier", 13))
-        text_label.place(x=5, y=7)
-
-         # Theme Selection widget
-        self.__theme_selection = tk.StringVar(self)
-        self.__theme_selection.set(self.__manager._config['theme'])
-        self.__theme_option_menu = tk.OptionMenu(self.__theme_frame, self.__theme_selection, *THEMES)
-        self.__theme_option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR, bd=0, highlightthickness=0)
-        self.__theme_option_menu.place(x=150, y=9)
-
-        # Button frame
-        self.__button_frame = tk.Frame(self, bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR, width=320, height=40)
-        self.__button_frame.pack(padx=7, pady=7, expand=True)
-
-        # Apply button
-        self.__apply_button = tk.Button(self.__button_frame,
-                                        text="Apply",
-                                        bg=self.__manager.graphgui._BUTTON_COLOR,
-                                        bd=0,
-                                        command=self.__apply__settings)
-        self.__apply_button.place(width=BUTTON_WIDTH,
-                                  height=BUTTON_HEIGHT,
-                                  x=160 - BUTTON_WIDTH / 2,
-                                  y=7)
-
-
-    def __apply__settings(self):
-        new_node_radius = self.__node_scale.get()
-        new_theme = self.__theme_selection.get()
-        self.__manager._config['node_radius'] = new_node_radius
-        self.__manager._config['theme'] = new_theme
-        self.__manager.update_main_config()
-
-        # Change the GUI theme
-        self.__manager.graphgui._theme = new_theme
-        self.__manager.graphgui.set_colors(new_theme)
-
-        # Change the node radius
-        self.__manager.graphgui.set_node_radius(new_node_radius)
-
-        # Update the GUI
-        current_position = self.__manager.graphgui.get_current_position()
-        self.__manager.graphgui.display_reset(current_position)
-
-
-class DeleteWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager):
-        super().__init__(root)
-        self.title("Delete save")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__manager = json_manager
-        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-
-        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        options = list(self.__manager._JsonManager__permanent.keys())
-        if len(options) > 0:
-            self.__selecion = tk.StringVar(self)
-            self.__selecion.set(options[0])
-            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
-            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__option_menu.pack(side=tk.TOP)
-
-            self.__button = tk.Button(self, text="Delete", command=self.__on_delete, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_delete(self):
-        selection = self.__selecion.get()
-        if selection not in self.__manager._JsonManager__permanent:
-            messagebox.showerror("Error", "The selected save does not exist")
-            self.destroy()
-        self.__manager.delete_permanent(selection)
-        messagebox.showinfo("Confirm", f"Removed : {selection}")
-
-    def __on_cancel(self):
-        self.destroy()
-
-class LoadWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager):
-        super().__init__(root)
-        self.title("Load")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__manager = json_manager
-        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-
-        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        options = list(self.__manager._JsonManager__permanent.keys())
-        if len(options) > 0:
-            self.__selecion = tk.StringVar(self)
-            self.__selecion.set(options[0])
-            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
-            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__option_menu.pack(side=tk.TOP)
-
-            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_load(self):
-        selection = self.__selecion.get()
-        if selection not in self.__manager._JsonManager__permanent:
-            messagebox.showerror("Error", "The selected save does not exist")
-            self.destroy()
-        self.new_position = self.__manager.get_data(selection)
-        self.__manager.graphgui.display_reset(self.new_position)
-
-    def __on_cancel(self):
-        self.destroy()
-
-class SaveWindow(tk.Toplevel):
-    def __init__(self, root, json_manager: JsonManager, graph_position: dict):
-        super().__init__(root)
-        self.title("Save")
-        self.geometry("200x100")
-        self.resizable(False, False)
-        self.__current_position = graph_position
-        self.__manager = json_manager
-        self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__root = root
-        self.bind("<Return>", self.__on_save)
-
-        self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
-        self.__label.pack(side=tk.TOP)
-
-        self.__entry = tk.Entry(self)
-        self.__entry.pack(side=tk.TOP)
-
-        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
-        self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
-
-        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
-        self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
-
-    def __on_save(self, event = None):
-        word = self.__entry.get()
-        word = word.strip()
-        word = word.replace(" ", "_")
-        if word:
-            self.__manager.save_data(word, self.__current_position)
-            self.__manager.add_permanent(word)
-            messagebox.showinfo("Confirmación", f"Guardado : {word}")
-        else:
-            messagebox.showerror("Error", "You must enter a name")
-        self.destroy()
-
-    def __on_cancel(self):
-        self.destroy()
-
-if __name__ == "__main__":
-    confirmation = input("WARNING: eliminating store. Do you want to proceed? [Y/N]: ")
-    if confirmation == "Y":
-        path = os.getcwd()
-
-        if os.path.exists(os.path.join(path, "permanent.json")):
-            os.remove(os.path.join(path, "permanent.json"))
-
-        if os.path.exists(os.path.join(path, "win_config.json")):
-            os.remove(os.path.join(path, "win_config.json"))
-
-        store_path = os.path.join(path, "store/")
-
-        for file in os.listdir(store_path):
-            if file.endswith(".json"):
-                removing = os.path.join(store_path, file)
+import os
+import json
+import tkinter as tk
+from tkinter import messagebox
+from datetime import datetime
+from .general_config import *
+
+class JsonManager:
+    def __init__(self, parent, graphgui):
+        self.__JSON_SAVE_DIR = os.path.join(os.path.dirname(__file__), 'store/')
+
+        self.graphgui = graphgui
+        self.__parent = parent
+        self.current_data_id = None
+        self.current_data = None
+
+        try:
+            with open(self.__JSON_SAVE_DIR + '../permanent.json', "r", encoding="utf-8", newline="") as file:
+                self.__permanent = json.load(file)
+        except FileNotFoundError:
+            self.__permanent = {}
+
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
+    def update_permanent(self):
+        with open(self.__JSON_SAVE_DIR + '../permanent.json', "w", encoding="utf-8", newline="") as file:
+            json.dump(self.__permanent, file, indent=4)
+
+    def delete_permanent(self, name: str):
+        del self.__permanent[name]
+        os.remove(self.__JSON_SAVE_DIR + name + '.json')
+        self.update_permanent()
+
+    def add_permanent(self, name: str):
+        self.__permanent[name] = str(datetime.now())
+        self.update_permanent()
+
+    def get_data(self, file_name: str) -> dict:
+        try:
+            with open(self.__JSON_SAVE_DIR + file_name + '.json', "r", encoding="utf-8", newline="") as file:
+                data = json.load(file)
+        except FileNotFoundError:
+            data = None
+        self.current_data_id = file_name
+        self.current_data = data
+        return data
+
+    def save_data(self, file_name: str, data: dict):
+        with open(self.__JSON_SAVE_DIR + file_name + '.json', "w", encoding="utf-8", newline="") as file:
+            json.dump(data, file, indent=4)
+
+    def generate_save_window(self, current_position: dict):
+        SaveWindow(self.__parent, self, current_position)
+
+    def generate_load_window(self):
+        LoadWindow(self.__parent, self)
+
+    def generate_delete_window(self):
+        DeleteWindow(self.__parent, self)
+
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
+class DeleteWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Delete save")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        options = list(self.__manager._JsonManager__permanent.keys())
+        if len(options) > 0:
+            self.__selecion = tk.StringVar(self)
+            self.__selecion.set(options[0])
+            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__option_menu.pack(side=tk.TOP)
+
+            self.__button = tk.Button(self, text="Delete", command=self.__on_delete, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_delete(self):
+        selection = self.__selecion.get()
+        if selection not in self.__manager._JsonManager__permanent:
+            messagebox.showerror("Error", "The selected save does not exist")
+            self.destroy()
+        self.__manager.delete_permanent(selection)
+        messagebox.showinfo("Confirm", f"Removed : {selection}")
+
+    def __on_cancel(self):
+        self.destroy()
+
+class LoadWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager):
+        super().__init__(root)
+        self.title("Load")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__manager = json_manager
+        self.configure(background=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+
+        self.__label = tk.Label(self, text="Select save:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        options = list(self.__manager._JsonManager__permanent.keys())
+        if len(options) > 0:
+            self.__selecion = tk.StringVar(self)
+            self.__selecion.set(options[0])
+            self.__option_menu = tk.OptionMenu(self, self.__selecion, *options)
+            self.__option_menu.config(bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__option_menu.pack(side=tk.TOP)
+
+            self.__button = tk.Button(self, text="Load", command=self.__on_load, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+            self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+            self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_load(self):
+        selection = self.__selecion.get()
+        if selection not in self.__manager._JsonManager__permanent:
+            messagebox.showerror("Error", "The selected save does not exist")
+            self.destroy()
+        self.new_position = self.__manager.get_data(selection)
+        self.__manager.graphgui.display_reset(self.new_position)
+
+    def __on_cancel(self):
+        self.destroy()
+
+class SaveWindow(tk.Toplevel):
+    def __init__(self, root, json_manager: JsonManager, graph_position: dict):
+        super().__init__(root)
+        self.title("Save")
+        self.geometry("200x100")
+        self.resizable(False, False)
+        self.__current_position = graph_position
+        self.__manager = json_manager
+        self.configure(bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__root = root
+        self.bind("<Return>", self.__on_save)
+
+        self.__label = tk.Label(self, text="Save as:", bg=self.__manager.graphgui._BACKGROUND_CANVAS_COLOR)
+        self.__label.pack(side=tk.TOP)
+
+        self.__entry = tk.Entry(self)
+        self.__entry.pack(side=tk.TOP)
+
+        self.__button = tk.Button(self, text="Save", command=self.__on_save, bg=self.__manager.graphgui._BUTTON_COLOR)
+        self.__button.place(x=0+7, y=100-7-30, width=60, height=30)
+
+        self.__button2 = tk.Button(self, text="Cancel", command=self.__on_cancel, bg=self.__manager.graphgui._BUTTON_COLOR)
+        self.__button2.place(x=200-7-60, y=100-7-30, width=60, height=30)
+
+    def __on_save(self, event = None):
+        word = self.__entry.get()
+        word = word.strip()
+        word = word.replace(" ", "_")
+        if word:
+            self.__manager.save_data(word, self.__current_position)
+            self.__manager.add_permanent(word)
+            messagebox.showinfo("Confirmación", f"Guardado : {word}")
+        else:
+            messagebox.showerror("Error", "You must enter a name")
+        self.destroy()
+
+    def __on_cancel(self):
+        self.destroy()
+
+if __name__ == "__main__":
+    confirmation = input("WARNING: eliminating store. Do you want to proceed? [Y/N]: ")
+    if confirmation == "Y":
+        path = os.getcwd()
+
+        if os.path.exists(os.path.join(path, "permanent.json")):
+            os.remove(os.path.join(path, "permanent.json"))
+
+        if os.path.exists(os.path.join(path, "win_config.json")):
+            os.remove(os.path.join(path, "win_config.json"))
+
+        store_path = os.path.join(path, "store/")
+
+        for file in os.listdir(store_path):
+            if file.endswith(".json"):
+                removing = os.path.join(store_path, file)
                 os.remove(removing)
```

### Comparing `graphdisplay-0.4.7/graphdisplay/tools_win_manager.py` & `graphdisplay-0.4.8/graphdisplay/tools_win_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,419 +1,419 @@
-import tkinter as tk
-import time
-from .general_config import *
-from .graphs import Graph
-from .trees import AVLTree, BinarySearchTree
-
-class ToolWindow(tk.Toplevel):
-    def __init__(self, root, graph):
-        super().__init__(root)
-        #self.geometry("500x500")
-        self.resizable(False, False)
-        self.__gui = graph
-        self.configure(background=self.__gui._FRAME_COLOR)
-        self.protocol("WM_DELETE_WINDOW", self.__on_closing)
-
-        if not self.__gui._is_tree:
-            self.__create_djistra_frame()
-            self.__create_minimum_path_frame()
-            #self.__create_tree_convert_frame()
-        else:
-            self.__create_preorder_frame()
-            self.__create_postorder_frame()
-            self.__create_inorder_frame()
-            self.__create_levelorder_frame()
-            self.__create_speed_frame()
-
-    def __create_speed_frame(self):
-        self.__speed_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=40,
-                                        width=500)
-        self.__speed_frame.pack(padx=7, pady=7)
-
-        text_label = tk.Label(self.__speed_frame,
-                              text="Animation speed",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=12)
-
-        self.__speed_scale = tk.Scale(self.__speed_frame,
-                                      from_=0.1,
-                                      to=1,
-                                      resolution=0.1,
-                                      highlightthickness=0,
-                                      orient=tk.HORIZONTAL,
-                                      bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                      bd=0,
-                                      length=150)
-        self.__speed_scale.place(x = 300, y = 0)
-
-    def __create_inorder_frame(self):
-        self.__inorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__inorder_frame.pack(padx=7, pady=7)
-
-        text_label = tk.Label(self.__inorder_frame,
-                              text="Inorder traversal",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=30)
-
-        go_button = tk.Button(self.__inorder_frame,
-                              text="Play",
-                              command=self.__inorder_press_play,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-        reset_button = tk.Button(self.__inorder_frame,
-                                 text="Reset",
-                                 command=self.__reset_all_traversal,
-                                 bg=self.__gui._BUTTON_COLOR,
-                                 bd=0)
-        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-    def __inorder_press_play(self):
-        self.__running_inorder = True
-        self.__reset_colors()
-        gui_tree: AVLTree = self.__gui._graph
-        inorder_list = gui_tree.inorder_list()
-
-        hold = self.__speed_scale.get()
-        for i in inorder_list:
-            if self.__running_inorder:
-                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
-                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
-                self.__gui.canvas.update()
-                time.sleep(hold)
-            else:
-                break
-
-    def __create_levelorder_frame(self):
-        self.__levelorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__levelorder_frame.pack(padx=7, pady=7)
-
-        text_label = tk.Label(self.__levelorder_frame,
-                              text="Level order traversal",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=30)
-
-        go_button = tk.Button(self.__levelorder_frame,
-                              text="Play",
-                              command=self.__levelorder_press_play,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-        reset_button = tk.Button(self.__levelorder_frame,
-                                 text="Reset",
-                                 command=self.__reset_all_traversal,
-                                 bg=self.__gui._BUTTON_COLOR,
-                                 bd=0)
-        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-    def __levelorder_press_play(self):
-        self.__running_levelorder = True
-        self.__reset_colors()
-        gui_tree: AVLTree = self.__gui._graph
-        levelorder_list = gui_tree.levelorder_list()
-
-        hold = self.__speed_scale.get()
-        for i in levelorder_list:
-            if self.__running_levelorder:
-                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
-                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
-                self.__gui.canvas.update()
-                time.sleep(hold)
-            else:
-                break
-
-    def __create_preorder_frame(self):
-        self.__preorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__preorder_frame.pack(padx=7, pady=7)
-
-        text_label = tk.Label(self.__preorder_frame,
-                              text="Preorder traversal",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=30)
-
-        go_button = tk.Button(self.__preorder_frame,
-                              text="Play",
-                              command=self.__preorder_press_play,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-        reset_button = tk.Button(self.__preorder_frame,
-                              text="Reset",
-                              command=self.__reset_all_traversal,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-    def __preorder_press_play(self):
-        self.__running_preorder = True
-        self.__reset_colors()
-        gui_tree: AVLTree = self.__gui._graph
-        preorder_list = gui_tree.preorder_list()
-
-        hold = self.__speed_scale.get()
-        for i in preorder_list:
-            if self.__running_preorder:
-                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
-                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
-                self.__gui.canvas.update()
-                time.sleep(hold)
-            else:
-                break
-
-    def __create_postorder_frame(self):
-        self.__postorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__postorder_frame.pack(padx=7, pady=7)
-
-        text_label = tk.Label(self.__postorder_frame,
-                              text="Postorder traversal",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=30)
-
-        go_button = tk.Button(self.__postorder_frame,
-                              text="Play",
-                              command=self.__postorder_press_play,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-        reset_button = tk.Button(self.__postorder_frame,
-                              text="Reset",
-                              command=self.__reset_all_traversal,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
-
-    def __postorder_press_play(self):
-        self.__running_postorder = True
-        self.__reset_colors()
-        gui_tree: AVLTree = self.__gui._graph
-        postorder_list = gui_tree.postorder_list()
-
-        hold = self.__speed_scale.get()
-        for i in postorder_list:
-            if self.__running_postorder:
-                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
-                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
-                self.__gui.canvas.update()
-                time.sleep(hold)
-            else:
-                break
-
-    def __create_djistra_frame(self):
-        self.__djistra_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__djistra_frame.pack(padx=7, pady=7)
-
-        # Djistra text
-        text_label = tk.Label(self.__djistra_frame,
-                              text="Dijkstra",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                              fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=30)
-
-        # First node entry
-        self.first_node_entry_djis = tk.Entry(self.__djistra_frame)
-        self.first_node_entry_djis.place(height=BUTTON_HEIGHT,
-                               width=BUTTON_WIDTH,
-                               y=35,
-                               x=170)
-        first_entry_text = tk.Label(self.__djistra_frame,
-                                    text="First Node",
-                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13),
-                                    fg=self.__gui._AUTHOR_NAME_COLOR)
-        first_entry_text.place(x=150, y=10)
-
-        # Second node entry
-        self.second_node_entry_djis = tk.Entry(self.__djistra_frame)
-        self.second_node_entry_djis.place(height=BUTTON_HEIGHT,
-                               width=BUTTON_WIDTH,
-                               y=35,
-                               x=240 + BUTTON_WIDTH)
-        first_entry_text = tk.Label(self.__djistra_frame,
-                                    text="Second Node",
-                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13),
-                                    fg=self.__gui._AUTHOR_NAME_COLOR)
-        first_entry_text.place(x=275, y=10)
-
-        # Go button
-        go_button = tk.Button(self.__djistra_frame,
-                              text="Show Path",
-                              command=self.__djistra_press,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
-
-    def __djistra_press(self):
-        self.__djistra_running = True
-        self.__reset_colors()
-        first_node = self.first_node_entry_djis.get()
-        second_node = self.second_node_entry_djis.get()
-
-        gui_graph: Graph = self.__gui._graph
-
-        if first_node not in list(gui_graph._vertices.keys()):
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "first node not in graph's vertices")
-            return
-        elif second_node not in list(gui_graph._vertices.keys()):
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
-            return
-
-        min_path = gui_graph.minimum_path(first_node, second_node)
-        if len(min_path[0]) >= 2:
-            for node in min_path[0]:
-                if node == first_node or node == second_node:
-                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
-                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
-                else:
-                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
-                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
-        else:
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
-
-    def __create_minimum_path_frame(self):
-        self.__minimum_path_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__minimum_path_frame.pack(padx=7, pady=7)
-
-        # Djistra text
-        text_label = tk.Label(self.__minimum_path_frame,
-                              text="Minimum Edge \nPath",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13),
-                                fg=self.__gui._AUTHOR_NAME_COLOR)
-        text_label.place(x=5, y=20)
-
-        # First node entry
-        self.first_node_entry_min = tk.Entry(self.__minimum_path_frame)
-        self.first_node_entry_min.place(height=BUTTON_HEIGHT,
-                               width=BUTTON_WIDTH,
-                               y=35,
-                               x=170)
-        first_entry_text = tk.Label(self.__minimum_path_frame,
-                                    text="First Node",
-                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13),
-                                    fg=self.__gui._AUTHOR_NAME_COLOR)
-        first_entry_text.place(x=150, y=10)
-
-        # Second node entry
-        self.second_node_entry_min = tk.Entry(self.__minimum_path_frame)
-        self.second_node_entry_min.place(height=BUTTON_HEIGHT,
-                               width=BUTTON_WIDTH,
-                               y=35,
-                               x=240 + BUTTON_WIDTH)
-        first_entry_text = tk.Label(self.__minimum_path_frame,
-                                    text="Second Node",
-                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                    font=("Courier", 13),
-                                    fg=self.__gui._AUTHOR_NAME_COLOR)
-        first_entry_text.place(x=275, y=10)
-
-        # Go button
-        go_button = tk.Button(self.__minimum_path_frame,
-                              text="Show Path",
-                              command=self.__minpath_press,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
-
-    def __minpath_press(self):
-        self.__reset_colors()
-        first_node = self.first_node_entry_min.get()
-        second_node = self.second_node_entry_min.get()
-
-        gui_graph: Graph = self.__gui._graph
-
-        if first_node not in list(gui_graph._vertices.keys()):
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "first node not in graph's vertices")
-            return
-        elif second_node not in list(gui_graph._vertices.keys()):
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
-            return
-
-        min_path = gui_graph.min_number_edges(first_node, second_node)
-        if len(min_path) >= 2:
-            for node in min_path:
-                if node == first_node or node == second_node:
-                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
-                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
-                else:
-                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
-                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
-        else:
-            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
-
-    def __create_tree_convert_frame(self):
-        self.__tree_convert_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                                        height=80,
-                                        width=500)
-        self.__tree_convert_frame.pack(padx=7, pady=7)
-
-        # Tree conversion text
-        text_label = tk.Label(self.__tree_convert_frame,
-                              text="Convert graph into binary tree",
-                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
-                              font=("Courier", 13))
-        text_label.place(x=5, y=30)
-
-        # Go button
-        go_button = tk.Button(self.__tree_convert_frame,
-                              text="Convert",
-                              command=self.__tree_convert_press,
-                              bg=self.__gui._BUTTON_COLOR,
-                              bd=0)
-        go_button.place(x=390, y=30, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
-
-    def __tree_convert_press(self):
-        self.__reset_colors()
-
-        gui_graph: Graph = self.__gui._graph
-
-        if not gui_graph.has_cycles():
-            # WORK IN PROGRESS... CHECK OUT SOON ;)
-            ...
-        else:
-            print("ERROR: graph cannot be converted into a binary tree")
-
-    def __reset_colors(self):
-        for node in self.__gui.nodes:
-            self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle, fill=self.__gui._VERTEX_COLOR)
-
-    def __reset_all_traversal(self):
-        self.__djistra_running = False
-        self.__running_postorder = False
-        self.__running_preorder = False
-        self.__running_levelorder = False
-        self.__running_inorder = False
-        self.__reset_colors()
-
-    def __on_closing(self):
-        self.__reset_all_traversal()
-        self.__reset_colors()
+import tkinter as tk
+import time
+from .general_config import *
+from .graphs import Graph
+from .trees import AVLTree, BinarySearchTree
+
+class ToolWindow(tk.Toplevel):
+    def __init__(self, root, graph):
+        super().__init__(root)
+        #self.geometry("500x500")
+        self.resizable(False, False)
+        self.__gui = graph
+        self.configure(background=self.__gui._FRAME_COLOR)
+        self.protocol("WM_DELETE_WINDOW", self.__on_closing)
+
+        if not self.__gui._is_tree:
+            self.__create_djistra_frame()
+            self.__create_minimum_path_frame()
+            #self.__create_tree_convert_frame()
+        else:
+            self.__create_preorder_frame()
+            self.__create_postorder_frame()
+            self.__create_inorder_frame()
+            self.__create_levelorder_frame()
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
+
+    def __create_inorder_frame(self):
+        self.__inorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__inorder_frame.pack(padx=7, pady=7)
+
+        text_label = tk.Label(self.__inorder_frame,
+                              text="Inorder traversal",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=30)
+
+        go_button = tk.Button(self.__inorder_frame,
+                              text="Play",
+                              command=self.__inorder_press_play,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+        reset_button = tk.Button(self.__inorder_frame,
+                                 text="Reset",
+                                 command=self.__reset_all_traversal,
+                                 bg=self.__gui._BUTTON_COLOR,
+                                 bd=0)
+        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+    def __inorder_press_play(self):
+        self.__running_inorder = True
+        self.__reset_colors()
+        gui_tree: AVLTree = self.__gui._graph
+        inorder_list = gui_tree.inorder_list()
+
+        hold = self.__speed_scale.get()
+        for i in inorder_list:
+            if self.__running_inorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
+                break
+
+    def __create_levelorder_frame(self):
+        self.__levelorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__levelorder_frame.pack(padx=7, pady=7)
+
+        text_label = tk.Label(self.__levelorder_frame,
+                              text="Level order traversal",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=30)
+
+        go_button = tk.Button(self.__levelorder_frame,
+                              text="Play",
+                              command=self.__levelorder_press_play,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+        reset_button = tk.Button(self.__levelorder_frame,
+                                 text="Reset",
+                                 command=self.__reset_all_traversal,
+                                 bg=self.__gui._BUTTON_COLOR,
+                                 bd=0)
+        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+    def __levelorder_press_play(self):
+        self.__running_levelorder = True
+        self.__reset_colors()
+        gui_tree: AVLTree = self.__gui._graph
+        levelorder_list = gui_tree.levelorder_list()
+
+        hold = self.__speed_scale.get()
+        for i in levelorder_list:
+            if self.__running_levelorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
+                break
+
+    def __create_preorder_frame(self):
+        self.__preorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__preorder_frame.pack(padx=7, pady=7)
+
+        text_label = tk.Label(self.__preorder_frame,
+                              text="Preorder traversal",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=30)
+
+        go_button = tk.Button(self.__preorder_frame,
+                              text="Play",
+                              command=self.__preorder_press_play,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+        reset_button = tk.Button(self.__preorder_frame,
+                              text="Reset",
+                              command=self.__reset_all_traversal,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+    def __preorder_press_play(self):
+        self.__running_preorder = True
+        self.__reset_colors()
+        gui_tree: AVLTree = self.__gui._graph
+        preorder_list = gui_tree.preorder_list()
+
+        hold = self.__speed_scale.get()
+        for i in preorder_list:
+            if self.__running_preorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
+                break
+
+    def __create_postorder_frame(self):
+        self.__postorder_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__postorder_frame.pack(padx=7, pady=7)
+
+        text_label = tk.Label(self.__postorder_frame,
+                              text="Postorder traversal",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=30)
+
+        go_button = tk.Button(self.__postorder_frame,
+                              text="Play",
+                              command=self.__postorder_press_play,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=300, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+        reset_button = tk.Button(self.__postorder_frame,
+                              text="Reset",
+                              command=self.__reset_all_traversal,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        reset_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH)
+
+    def __postorder_press_play(self):
+        self.__running_postorder = True
+        self.__reset_colors()
+        gui_tree: AVLTree = self.__gui._graph
+        postorder_list = gui_tree.postorder_list()
+
+        hold = self.__speed_scale.get()
+        for i in postorder_list:
+            if self.__running_postorder:
+                self.__gui.canvas.itemconfigure(self.__gui.nodes[i].circle,
+                                                fill=self.__gui._SELECTED_VERTEX_COLOR)
+                self.__gui.canvas.update()
+                time.sleep(hold)
+            else:
+                break
+
+    def __create_djistra_frame(self):
+        self.__djistra_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__djistra_frame.pack(padx=7, pady=7)
+
+        # Djistra text
+        text_label = tk.Label(self.__djistra_frame,
+                              text="Dijkstra",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                              fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=30)
+
+        # First node entry
+        self.first_node_entry_djis = tk.Entry(self.__djistra_frame)
+        self.first_node_entry_djis.place(height=BUTTON_HEIGHT,
+                               width=BUTTON_WIDTH,
+                               y=35,
+                               x=170)
+        first_entry_text = tk.Label(self.__djistra_frame,
+                                    text="First Node",
+                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
+        first_entry_text.place(x=150, y=10)
+
+        # Second node entry
+        self.second_node_entry_djis = tk.Entry(self.__djistra_frame)
+        self.second_node_entry_djis.place(height=BUTTON_HEIGHT,
+                               width=BUTTON_WIDTH,
+                               y=35,
+                               x=240 + BUTTON_WIDTH)
+        first_entry_text = tk.Label(self.__djistra_frame,
+                                    text="Second Node",
+                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
+        first_entry_text.place(x=275, y=10)
+
+        # Go button
+        go_button = tk.Button(self.__djistra_frame,
+                              text="Show Path",
+                              command=self.__djistra_press,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
+
+    def __djistra_press(self):
+        self.__djistra_running = True
+        self.__reset_colors()
+        first_node = self.first_node_entry_djis.get()
+        second_node = self.second_node_entry_djis.get()
+
+        gui_graph: Graph = self.__gui._graph
+
+        if first_node not in list(gui_graph._vertices.keys()):
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "first node not in graph's vertices")
+            return
+        elif second_node not in list(gui_graph._vertices.keys()):
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
+            return
+
+        min_path = gui_graph.minimum_path(first_node, second_node)
+        if len(min_path[0]) >= 2:
+            for node in min_path[0]:
+                if node == first_node or node == second_node:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+                else:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+        else:
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
+
+    def __create_minimum_path_frame(self):
+        self.__minimum_path_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__minimum_path_frame.pack(padx=7, pady=7)
+
+        # Djistra text
+        text_label = tk.Label(self.__minimum_path_frame,
+                              text="Minimum Edge \nPath",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13),
+                                fg=self.__gui._AUTHOR_NAME_COLOR)
+        text_label.place(x=5, y=20)
+
+        # First node entry
+        self.first_node_entry_min = tk.Entry(self.__minimum_path_frame)
+        self.first_node_entry_min.place(height=BUTTON_HEIGHT,
+                               width=BUTTON_WIDTH,
+                               y=35,
+                               x=170)
+        first_entry_text = tk.Label(self.__minimum_path_frame,
+                                    text="First Node",
+                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
+        first_entry_text.place(x=150, y=10)
+
+        # Second node entry
+        self.second_node_entry_min = tk.Entry(self.__minimum_path_frame)
+        self.second_node_entry_min.place(height=BUTTON_HEIGHT,
+                               width=BUTTON_WIDTH,
+                               y=35,
+                               x=240 + BUTTON_WIDTH)
+        first_entry_text = tk.Label(self.__minimum_path_frame,
+                                    text="Second Node",
+                                    bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                    font=("Courier", 13),
+                                    fg=self.__gui._AUTHOR_NAME_COLOR)
+        first_entry_text.place(x=275, y=10)
+
+        # Go button
+        go_button = tk.Button(self.__minimum_path_frame,
+                              text="Show Path",
+                              command=self.__minpath_press,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=390, y=35, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
+
+    def __minpath_press(self):
+        self.__reset_colors()
+        first_node = self.first_node_entry_min.get()
+        second_node = self.second_node_entry_min.get()
+
+        gui_graph: Graph = self.__gui._graph
+
+        if first_node not in list(gui_graph._vertices.keys()):
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "first node not in graph's vertices")
+            return
+        elif second_node not in list(gui_graph._vertices.keys()):
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "second node not in graph's vertices")
+            return
+
+        min_path = gui_graph.min_number_edges(first_node, second_node)
+        if len(min_path) >= 2:
+            for node in min_path:
+                if node == first_node or node == second_node:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+                else:
+                    self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle,
+                                                    fill=self.__gui._SELECTED_VERTEX_COLOR)
+        else:
+            print('\n' + '\033[91m' + "ERROR: " + '\033[0m' + "there is no path from", first_node, "to", second_node)
+
+    def __create_tree_convert_frame(self):
+        self.__tree_convert_frame = tk.Frame(self, bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                                        height=80,
+                                        width=500)
+        self.__tree_convert_frame.pack(padx=7, pady=7)
+
+        # Tree conversion text
+        text_label = tk.Label(self.__tree_convert_frame,
+                              text="Convert graph into binary tree",
+                              bg=self.__gui._BACKGROUND_CANVAS_COLOR,
+                              font=("Courier", 13))
+        text_label.place(x=5, y=30)
+
+        # Go button
+        go_button = tk.Button(self.__tree_convert_frame,
+                              text="Convert",
+                              command=self.__tree_convert_press,
+                              bg=self.__gui._BUTTON_COLOR,
+                              bd=0)
+        go_button.place(x=390, y=30, height=BUTTON_HEIGHT, width=BUTTON_WIDTH + 30)
+
+    def __tree_convert_press(self):
+        self.__reset_colors()
+
+        gui_graph: Graph = self.__gui._graph
+
+        if not gui_graph.has_cycles():
+            # WORK IN PROGRESS... CHECK OUT SOON ;)
+            ...
+        else:
+            print("ERROR: graph cannot be converted into a binary tree")
+
+    def __reset_colors(self):
+        for node in self.__gui.nodes:
+            self.__gui.canvas.itemconfigure(self.__gui.nodes[node].circle, fill=self.__gui._VERTEX_COLOR)
+
+    def __reset_all_traversal(self):
+        self.__djistra_running = False
+        self.__running_postorder = False
+        self.__running_preorder = False
+        self.__running_levelorder = False
+        self.__running_inorder = False
+        self.__reset_colors()
+
+    def __on_closing(self):
+        self.__reset_all_traversal()
+        self.__reset_colors()
         self.destroy()
```

### Comparing `graphdisplay-0.4.7/graphdisplay/trees/binary_search_tree.py` & `graphdisplay-0.4.8/graphdisplay/trees/binary_search_tree.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-# -*- coding: utf-8 -*-
-
-from .binary_tree import BinaryNode
-from .binary_tree import BinaryTree
-
-
-class BinarySearchTree(BinaryTree):
-
-    def search(self, elem: object) -> BinaryNode:
-        """Returns the node whose elem is elem"""
-        return self._search(self._root, elem)
-
-    def _search(self, node: BinaryNode, elem: object) -> BinaryNode:
-        """Recursive function"""
-        if node is None or node.elem == elem:
-            return node
-        elif elem < node.elem:
-            return self._search(node.left, elem)
-        elif elem > node.elem:
-            return self._search(node.right, elem)
-
-    def insert(self, elem: object) -> None:
-        self._root = self._insert(self._root, elem)
-
-    def _insert(self, node: BinaryNode, elem: object) -> BinaryNode:
-        if node is None:
-            return BinaryNode(elem)
-
-        if node.elem == elem:
-            return node
-
-        if elem < node.elem:
-            node.left = self._insert(node.left, elem)
-        else:
-            # elem>node.elem
-            node.right = self._insert(node.right, elem)
-        return node
-
-    def _minimum_node(self, node: BinaryNode) -> BinaryNode:
-        """returns the  node with the smallest elem
-        in the subtree node.
-        This is the node that is furthest to the left"""
-        min_node = node
-        while min_node.left is not None:
-            min_node = min_node.left
-        return min_node
-
-    def remove_all(self):
-        self._root = None
-
-    def remove(self, elem: object) -> None:
-        # update the root with the new subtree after remove elem
-        self._root = self._remove(self._root, elem)
-
-    def _remove(self, node: BinaryNode, elem: object) -> BinaryNode:
-        """It recursively searches the node. When the node is
-        found, the node has to be removed"""
-        if node is None:
-            return node
-
-        if elem < node.elem:
-            node.left = self._remove(node.left, elem)
-        elif elem > node.elem:
-            node.right = self._remove(node.right, elem)
-        else:
-            # node.elem == elem, node is the node to remove!!!
-            if node.left is None and node.right is None:
-                # Case 1: node is a leave
-                return None
-
-            # Case 2: node only has a child, so the function has to return it
-            if node.left is None:
-                # It only has the right child
-                return node.right
-
-            elif node.right is None:
-                # It only has the left child
-                return node.left
-            else:
-                # Case 3: node.left!=None and node.right!=None
-                # we search the smallest node from its right child
-                successor = self._minimum_node(node.right)
-                # we replace elem with the elem of the successor
-                node.elem = successor.elem
-                # now, we have to remove successor from the right child
-                node.right = self._remove(node.right, successor.elem)
-
-        return node
-
-
-if __name__ == "__main__":
+# -*- coding: utf-8 -*-
+
+from .binary_tree import BinaryNode
+from .binary_tree import BinaryTree
+
+
+class BinarySearchTree(BinaryTree):
+
+    def search(self, elem: object) -> BinaryNode:
+        """Returns the node whose elem is elem"""
+        return self._search(self._root, elem)
+
+    def _search(self, node: BinaryNode, elem: object) -> BinaryNode:
+        """Recursive function"""
+        if node is None or node.elem == elem:
+            return node
+        elif elem < node.elem:
+            return self._search(node.left, elem)
+        elif elem > node.elem:
+            return self._search(node.right, elem)
+
+    def insert(self, elem: object) -> None:
+        self._root = self._insert(self._root, elem)
+
+    def _insert(self, node: BinaryNode, elem: object) -> BinaryNode:
+        if node is None:
+            return BinaryNode(elem)
+
+        if node.elem == elem:
+            return node
+
+        if elem < node.elem:
+            node.left = self._insert(node.left, elem)
+        else:
+            # elem>node.elem
+            node.right = self._insert(node.right, elem)
+        return node
+
+    def _minimum_node(self, node: BinaryNode) -> BinaryNode:
+        """returns the  node with the smallest elem
+        in the subtree node.
+        This is the node that is furthest to the left"""
+        min_node = node
+        while min_node.left is not None:
+            min_node = min_node.left
+        return min_node
+
+    def remove_all(self):
+        self._root = None
+
+    def remove(self, elem: object) -> None:
+        # update the root with the new subtree after remove elem
+        self._root = self._remove(self._root, elem)
+
+    def _remove(self, node: BinaryNode, elem: object) -> BinaryNode:
+        """It recursively searches the node. When the node is
+        found, the node has to be removed"""
+        if node is None:
+            return node
+
+        if elem < node.elem:
+            node.left = self._remove(node.left, elem)
+        elif elem > node.elem:
+            node.right = self._remove(node.right, elem)
+        else:
+            # node.elem == elem, node is the node to remove!!!
+            if node.left is None and node.right is None:
+                # Case 1: node is a leave
+                return None
+
+            # Case 2: node only has a child, so the function has to return it
+            if node.left is None:
+                # It only has the right child
+                return node.right
+
+            elif node.right is None:
+                # It only has the left child
+                return node.left
+            else:
+                # Case 3: node.left!=None and node.right!=None
+                # we search the smallest node from its right child
+                successor = self._minimum_node(node.right)
+                # we replace elem with the elem of the successor
+                node.elem = successor.elem
+                # now, we have to remove successor from the right child
+                node.right = self._remove(node.right, successor.elem)
+
+        return node
+
+
+if __name__ == "__main__":
     pass
```

### Comparing `graphdisplay-0.4.7/graphdisplay/trees/binary_tree.py` & `graphdisplay-0.4.8/graphdisplay/trees/binary_tree.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-# -*- coding: utf-8 -*-
-# Implementation of Binary Tree
-
-import queue
-
-class BinaryNode:
-
-    def __init__(self, elem: object, node_left: 'BinaryNode' = None, node_right: 'BinaryNode' = None) -> None:
-        self.elem = elem
-        self.left = node_left
-        self.right = node_right
-
-    def __eq__(self, other: 'BinaryNode') -> bool:
-        """checks if two nodes (subtrees) are equal o not"""
-        return other is not None and self.elem == other.elem and self.left == other.left and self.right == other.right
-
-    def __str__(self):
-        return str(self.elem)
-
-
-class BinaryTree:
-    def __init__(self) -> None:
-        """creates an empty binary trees
-        I only has an attribute: _root"""
-        self._root = None
-
-    def __eq__(self, other: 'BinaryTree') -> bool:
-        """checks if two binary trees are equal o not"""
-        return other is not None and self._root == other._root
-
-    def size(self) -> int:
-        """Returns the number of nodes"""
-        return self._size(self._root)
-
-    def _size(self, node: BinaryNode) -> int:
-        """return the size of the subtree from node"""
-        if node is None:
-            return 0
-        else:
-            return 1 + self._size(node.left) + self._size(node.right)
-
-    def height(self) -> int:
-        """Returns the height of the trees"""
-        return self._height(self._root)
-
-    def _height(self, node: BinaryNode) -> int:
-        """return the height of node"""
-        if node is None:
-            return -1
-        else:
-            return 1 + max(self._height(node.left), self._height(node.right))
-
-    def preorder(self) -> None:
-        """prints the preorder (root, left, right) traversal of the trees"""
-        # self.draw()
-        print('Preorder traversal: ', end=' ')  # end=' ' avoid the newline
-        self._preorder(self._root)
-        print()
-
-    def _preorder(self, node: BinaryNode) -> None:
-        """prints the preorder (root, left, right) traversal of the subtree
-        than hangs from node"""
-        if node is not None:
-            print(node.elem, end=' ')  # end=' ' avoid new line
-            self._preorder(node.left)
-            self._preorder(node.right)
-
-    def preorder_list(self) -> list:
-        """returns a list with the preorder traversal"""
-        # self.draw()
-        result = []
-        self._preorder_list(self._root, result)
-        return result
-
-    def _preorder_list(self, node: BinaryNode, pre_list: list) -> None:
-        """populates pre_list with the preorder traversal of the subtree node"""
-        if node is not None:
-            pre_list.append(node.elem)
-            self._preorder_list(node.left, pre_list)
-            self._preorder_list(node.right, pre_list)
-
-    def postorder(self) -> None:
-        """prints the postorder (left, right, root)  traversal of the trees"""
-        # self.draw()
-        print('Postorder traversal: ', end=' ')  # end=' ' avoid the newline
-        self._postorder(self._root)
-        print()
-
-    def _postorder(self, node: BinaryNode) -> None:
-        """prints the postorder (left, right, root) traversal of the subtree
-        than hangs from node"""
-        if node is not None:
-            self._postorder(node.left)
-            self._postorder(node.right)
-            print(node.elem, end=' ')  # end=' ' avoid new line
-
-    def postorder_list(self) -> list:
-        """returns a list with the postorder traversal of the trees"""
-        # self.draw()
-        result = []
-        self._postorder_list(self._root, result)
-        return result
-
-    def _postorder_list(self, node: BinaryNode, post_list: list) -> None:
-        """populates post_list with the postorder traversal of the subtree node"""
-        if node is not None:
-            self._postorder_list(node.left, post_list)
-            self._postorder_list(node.right, post_list)
-            post_list.append(node.elem)
-
-    def inorder(self) -> None:
-        """prints the inorder (left, root, right)  traversal of the trees"""
-        # self.draw()
-        print('Inorder traversal: ', end=' ')  # end=' ' avoid the newline
-        self._inorder(self._root)
-        print()
-
-    def _inorder(self, node: BinaryNode) -> None:
-        """prints the inorder (left, root, right) traversal of the subtree
-        than hangs from node"""
-        if node is not None:
-            self._inorder(node.left)
-            print(node.elem, end=' ')  # end=' ' avoid new line
-            self._inorder(node.right)
-
-    def inorder_list(self) -> list:
-        """returns a list with the inorder traversal of the trees"""
-        # self.draw()
-        result = []
-        self._inorder_list(self._root, result)
-        return result
-
-    def _inorder_list(self, node: BinaryNode, in_list: list) -> None:
-        """populates in_list with the inorder traversal of the subtree node"""
-        if node is not None:
-            self._postorder_list(node.left, in_list)
-            in_list.append(node.elem)
-            self._postorder_list(node.right, in_list)
-
-    def levelorder_list(self):
-        """returns a list with the level order traversal of the trees"""
-        levelorder = []
-        q = queue.Queue()
-        q.put(self._root)  # enqueue: we save the root
-
-        while q.empty() == False:
-            current = q.get()  # dequeue
-            levelorder.append(current.elem)
-            if current.left != None:
-                q.put(current.left)
-            if current.right != None:
-                q.put(current.right)
-
-        return levelorder
-
-    def draw(self) -> None:
-        """function to draw a trees. """
-        if self._root:
-            self._draw('', self._root, False)
-        else:
-            print('trees is empty')
-        print('\n\n')
-
-    def _draw(self, prefix: str, node: BinaryNode, is_left: bool) -> None:
-        if node is not None:
-            self._draw(prefix + "     ", node.right, False)
-            print(prefix + "|-- " + str(node.elem))
-            self._draw(prefix + "     ", node.left, True)
-
-
-if __name__ == '__main__':
+# -*- coding: utf-8 -*-
+# Implementation of Binary Tree
+
+import queue
+
+class BinaryNode:
+
+    def __init__(self, elem: object, node_left: 'BinaryNode' = None, node_right: 'BinaryNode' = None) -> None:
+        self.elem = elem
+        self.left = node_left
+        self.right = node_right
+
+    def __eq__(self, other: 'BinaryNode') -> bool:
+        """checks if two nodes (subtrees) are equal o not"""
+        return other is not None and self.elem == other.elem and self.left == other.left and self.right == other.right
+
+    def __str__(self):
+        return str(self.elem)
+
+
+class BinaryTree:
+    def __init__(self) -> None:
+        """creates an empty binary trees
+        I only has an attribute: _root"""
+        self._root = None
+
+    def __eq__(self, other: 'BinaryTree') -> bool:
+        """checks if two binary trees are equal o not"""
+        return other is not None and self._root == other._root
+
+    def size(self) -> int:
+        """Returns the number of nodes"""
+        return self._size(self._root)
+
+    def _size(self, node: BinaryNode) -> int:
+        """return the size of the subtree from node"""
+        if node is None:
+            return 0
+        else:
+            return 1 + self._size(node.left) + self._size(node.right)
+
+    def height(self) -> int:
+        """Returns the height of the trees"""
+        return self._height(self._root)
+
+    def _height(self, node: BinaryNode) -> int:
+        """return the height of node"""
+        if node is None:
+            return -1
+        else:
+            return 1 + max(self._height(node.left), self._height(node.right))
+
+    def preorder(self) -> None:
+        """prints the preorder (root, left, right) traversal of the trees"""
+        # self.draw()
+        print('Preorder traversal: ', end=' ')  # end=' ' avoid the newline
+        self._preorder(self._root)
+        print()
+
+    def _preorder(self, node: BinaryNode) -> None:
+        """prints the preorder (root, left, right) traversal of the subtree
+        than hangs from node"""
+        if node is not None:
+            print(node.elem, end=' ')  # end=' ' avoid new line
+            self._preorder(node.left)
+            self._preorder(node.right)
+
+    def preorder_list(self) -> list:
+        """returns a list with the preorder traversal"""
+        # self.draw()
+        result = []
+        self._preorder_list(self._root, result)
+        return result
+
+    def _preorder_list(self, node: BinaryNode, pre_list: list) -> None:
+        """populates pre_list with the preorder traversal of the subtree node"""
+        if node is not None:
+            pre_list.append(node.elem)
+            self._preorder_list(node.left, pre_list)
+            self._preorder_list(node.right, pre_list)
+
+    def postorder(self) -> None:
+        """prints the postorder (left, right, root)  traversal of the trees"""
+        # self.draw()
+        print('Postorder traversal: ', end=' ')  # end=' ' avoid the newline
+        self._postorder(self._root)
+        print()
+
+    def _postorder(self, node: BinaryNode) -> None:
+        """prints the postorder (left, right, root) traversal of the subtree
+        than hangs from node"""
+        if node is not None:
+            self._postorder(node.left)
+            self._postorder(node.right)
+            print(node.elem, end=' ')  # end=' ' avoid new line
+
+    def postorder_list(self) -> list:
+        """returns a list with the postorder traversal of the trees"""
+        # self.draw()
+        result = []
+        self._postorder_list(self._root, result)
+        return result
+
+    def _postorder_list(self, node: BinaryNode, post_list: list) -> None:
+        """populates post_list with the postorder traversal of the subtree node"""
+        if node is not None:
+            self._postorder_list(node.left, post_list)
+            self._postorder_list(node.right, post_list)
+            post_list.append(node.elem)
+
+    def inorder(self) -> None:
+        """prints the inorder (left, root, right)  traversal of the trees"""
+        # self.draw()
+        print('Inorder traversal: ', end=' ')  # end=' ' avoid the newline
+        self._inorder(self._root)
+        print()
+
+    def _inorder(self, node: BinaryNode) -> None:
+        """prints the inorder (left, root, right) traversal of the subtree
+        than hangs from node"""
+        if node is not None:
+            self._inorder(node.left)
+            print(node.elem, end=' ')  # end=' ' avoid new line
+            self._inorder(node.right)
+
+    def inorder_list(self) -> list:
+        """returns a list with the inorder traversal of the trees"""
+        # self.draw()
+        result = []
+        self._inorder_list(self._root, result)
+        return result
+
+    def _inorder_list(self, node: BinaryNode, in_list: list) -> None:
+        """populates in_list with the inorder traversal of the subtree node"""
+        if node is not None:
+            self._postorder_list(node.left, in_list)
+            in_list.append(node.elem)
+            self._postorder_list(node.right, in_list)
+
+    def levelorder_list(self):
+        """returns a list with the level order traversal of the trees"""
+        levelorder = []
+        q = queue.Queue()
+        q.put(self._root)  # enqueue: we save the root
+
+        while q.empty() == False:
+            current = q.get()  # dequeue
+            levelorder.append(current.elem)
+            if current.left != None:
+                q.put(current.left)
+            if current.right != None:
+                q.put(current.right)
+
+        return levelorder
+
+    def draw(self) -> None:
+        """function to draw a trees. """
+        if self._root:
+            self._draw('', self._root, False)
+        else:
+            print('trees is empty')
+        print('\n\n')
+
+    def _draw(self, prefix: str, node: BinaryNode, is_left: bool) -> None:
+        if node is not None:
+            self._draw(prefix + "     ", node.right, False)
+            print(prefix + "|-- " + str(node.elem))
+            self._draw(prefix + "     ", node.left, True)
+
+
+if __name__ == '__main__':
     pass
```

### Comparing `graphdisplay-0.4.7/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.4.8/graphdisplay.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-Metadata-Version: 2.1
-Name: graphdisplay
-Version: 0.4.7
-Summary: Librería para representar grafos visualmente
-Home-page: https://github.com/seniorbeto
-Author: Alberto Penas Díaz (@seniorbeto)
-Author-email: albertopenasdiaz@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
-  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
-  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
-</p>
-
-## 💡Resumen
-
-graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
-
-## ⚡️¿Quieres contribuir?
-
-Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
-en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
-
-## 📐Método de uso
-
-Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
-tkinter y math (que muchas veces vienen instaladas por defecto en python). 
-
-Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
-asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
-Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
-**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
-de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
-o utilizar la implementación de grafos que viene por defecto con el paquete.
-Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
-gestiona el almacenado de grafos.
-
-Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
-
-+ Para representar el siguiente grafo:
-
-     <img src='https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png' width='25%'/>
-    
-    Se podría disponer del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, Graph
-    
-    # Implementaremos el grafo de la siguiente imagen:
-    # https://upload.wikimedia.org/wikipedia/commons/thumb/b/bc/CPT-Graphs-directed-weighted-ex1.svg/722px-CPT-Graphs-directed-weighted-ex1.svg.png
-    
-    labels = ['A', 'B', 'C', 'D', 'E']
-    g = Graph(labels)
-    
-    g.addEdge('A', 'C', 12)  # A->(12)C
-    g.addEdge('A', 'D', 60)  # A->(60)D
-    g.addEdge('B', 'A', 10)  # B->(10)A
-    g.addEdge('C', 'B', 20)  # C->(20)B
-    g.addEdge('C', 'D', 32)  # C->(32)D
-    g.addEdge('E', 'A', 7)   # E->(7)A
-    
-    # Para representar el grafo 
-    if __name__ == "__main__":
-        GraphGUI(g)
-    ```
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/9210f5d4-4903-45ea-9bb8-e625890adac3' width='30%'/>
-  
-+ Ejemplo con árboles binarios de búsqueda:
-
-    Para representar el siguiente árbol:
-
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1418ef2c-3215-4d88-93ce-3d1c67c4a58e' width='70%'/>
-    
-    Se dispondría del siguiente código:
-    ```python
-    from graphdisplay import GraphGUI, BinarySearchTree
-    
-    labels = [12, 4, 16, 2, 10, 14, 19, 1, 8, 13, 18, 20, 6, 24]
-    tree = BinarySearchTree()
-    for i in labels:
-        tree.insert(i)
-       
-    # Para representar el árbol
-    if __name__ == "__main__":
-        GraphGUI(tree)
-    ```
-    
-    <img src='https://github.com/seniorbeto/graphdisplay/assets/94072018/1e87b61d-d6fd-4635-bdf0-136509250de7' width='60%'/>
-
-## ⚡️Funcionalidades
-Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
-éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
-instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
-Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
-tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
-después poder cargarlo (file>load) en cualquier momento.
-
-Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
-al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
-Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
-issue #16
-
-
-## 🎯Ejemplos de uso
-
-
-```python
-from graphdisplay import GraphGUI, Graph
-
-my_gragph = Graph(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'Z', 'N', 'O', 'P', 'Q'])
-my_gragph.addEdge('A', 'B', 4)
-my_gragph.addEdge('B', 'C', 8)
-my_gragph.addEdge('C', 'A', 100)
-my_gragph.addEdge('D', 'E', 7)
-my_gragph.addEdge('E', 'F', 10)
-my_gragph.addEdge('F', 'G', 5)
-my_gragph.addEdge('G', 'Z', 6)
-my_gragph.addEdge('A', 'H', 2)
-my_gragph.addEdge('B', 'I', 3)
-my_gragph.addEdge('C', 'J', 4)
-my_gragph.addEdge('D', 'K', 5)
-my_gragph.addEdge('E', 'L', 6)
-my_gragph.addEdge('F', 'D', 3)
-my_gragph.addEdge('G', 'H', 9)
-my_gragph.addEdge('H', 'Z', 2)
-my_gragph.addEdge('I', 'J', 1)
-my_gragph.addEdge('J', 'A', 6)
-my_gragph.addEdge('K', 'L', 5)
-my_gragph.addEdge('L', 'M', 4)
-my_gragph.addEdge('M', 'H', 3)
-my_gragph.addEdge('N', 'O', 2)
-my_gragph.addEdge('O', 'P', 1)
-my_gragph.addEdge('P', 'Q', 7)
-my_gragph.addEdge('H', 'A', 20)
-my_gragph.addEdge('K', 'B', 7)
-my_gragph.addEdge('H', 'N', 9)
-my_gragph.addEdge('Q', 'D', 40)
-
-if __name__ == "__main__":
-    GraphGUI(g)
-```
-
-Y nos mostrará la ventana (reordenando los vértices):
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
-
-De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
-
-<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
+Metadata-Version: 2.1
+Name: graphdisplay
+Version: 0.4.8
+Summary: Librería para representar grafos visualmente
+Home-page: https://github.com/seniorbeto
+Author: Alberto Penas Díaz (@seniorbeto)
+Author-email: albertopenasdiaz@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <img width="200" src="https://github.com/seniorbeto/graphdisplay/assets/94072018/181477f3-b0e5-4efd-8e4f-2e7bad5c4d66" alt="logo">
+  <h1 align="center" style="margin: 0 auto 0 auto;">GraphDisplay</h1>
+  <h4 align="center" style="margin: 0 auto 0 auto;">An intuitive GUI for visualizing graphs</h4>
+</p>
+
+## 💡Resumen
+
+graphdisplay es un paquete de python elaborado e ideado por Alberto Penas Díaz, cuya finalidad es facilitar la visualización de grafos y árboles a los alumnos de Estructuras de Datos y Algoritmos. 
+
+## ⚡️¿Quieres contribuir?
+
+Este es un proyecto de código abierto hecho por y para estudiantes así que cualquier ayuda, comentario o sugerencia es bienvenido. La mejor manera de contribuir es añadir los bugs que os encontréis 
+en el apartado de Issues pero también estoy completamente abierto a responder cualquier duda o ayuda desde mi correo personal (disponible en mi perfil de github). ¡Muchas gracias de antemano!
+
+## 📐Método de uso
+
+Para instalar la librería, basta con escribir el siguiente comando en la terminal: `pip install graphdisplay`, con esta, se instalarán también otras dependencias, ya sean las librerías 
+tkinter y math (que muchas veces vienen instaladas por defecto en python). 
+
+Una vez instalado, se debe importar el paquete desde donde se esté trabajando con: `from graphdisplay import GraphGUI`. La librería también incluye la implementación oficial de grafos y árboles de la 
+asignatura, por lo que también son importables (`from graphdisplay import BinarySearchTree, Graph, GraphGUI, AVLTree`).
+Una vez instalada, se debe instanciar un grafo o árbol para finalmente introducirlo como argumento al generar un objeto de tipo GraphGUI, el cual mostrará en una ventana el grafo y ofrecerá la posibildad de mover los vértices con el ratón.
+**ES MUY IMPORTANTE** que éste parámetro sea implementado en base al código base de la asignatura. Si alguno
+de los atributos de las clases cambiase de nombre, es muy probable que el programa no funcionara correctamente. Para más información, consultar el [respositorio oficial de la asignatura](https://github.com/isegura/EDA)
+o utilizar la implementación de grafos que viene por defecto con el paquete.
+Además de una serie de funcionalidades accesibles en la barra superior, ya sean una pestaña de información adicional, otra pestaña de funcionalidades sobre el grafo y un menú desplegable que 
+gestiona el almacenado de grafos.
+
+Dicho esto, algunos ejemplos de uso podrían ser los siguientes:
+
++ Para representar el siguiente grafo:
+
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
+
+## ⚡️Funcionalidades
+Como ya se ha mencionado, una de las principales características de la aplicación consiste en la posibilidad de mover los vértices del grafo dentro de la ventana. Además,
+éstos conservarán su posición si se cierra la ventana y se vuelve a abrir. Así mismo, es posible abrir varias ventanas al mismo tiempo 
+instanciando varios objetos de tipo GraphGUI en el mismo programa. Es por esto que el sistema de autoguardado depende de en qué parte del programa se generen estos objetos GraphGUI.
+Por ejemplo, si se han generado dos grafos A y B y ha llamado primero al A y luego al B, si se vuelve a ejecutar el programa pero esta vez llamando primero al B, el sistema
+tratará de cargar el último estado del grafo A en el B. Para evitar esto, es recomendable generar una guardado permanente (pulsando el botón file>save y nombrando el guardado) para
+después poder cargarlo (file>load) en cualquier momento.
+
+Cabe destacar además, que las funcionalidades han sido testeadas únicamente en linux y en windows, variando las funcionalidades de la aplicación entre los sitemas. Por ejemplo,
+al generar un objeto GraphGUI en windows, si no se ha instanciado dentro de la cláusula `if __name__ == "__main__":` saltará un _Warning_, cosa que no pasará en Linux. Por otra parte,
+Windows permite generar sub-árboles presionando con el click derecho del ratón en un vértice (dicho árbol se generará en una nueva ventana), funcionalidad que no está disponible en linux debido al 
+issue #16
+
+
+## 🎯Ejemplos de uso
+
+
+```python
+from graphdisplay import GraphGUI, Graph
+
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
+
+if __name__ == "__main__":
+    GraphGUI(g)
+```
+
+Y nos mostrará la ventana (reordenando los vértices):
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/24120c29-839d-483c-a150-fefb678911f1" width="70%">
+
+De la misma manera, un ejemplo de display de un árbol binario de búsqueda: 
+
+<img src="https://github.com/seniorbeto/graphdisplay/assets/94072018/1fb39e40-52a0-4512-b52e-c613b96d1f79" width="200%">
```

### Comparing `graphdisplay-0.4.7/graphdisplay.egg-info/SOURCES.txt` & `graphdisplay-0.4.8/graphdisplay.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 graphdisplay/__init__.py
 graphdisplay/about_win_manager.py
 graphdisplay/general_config.py
 graphdisplay/graphdisplay.py
+graphdisplay/graphdisplay.pyi
 graphdisplay/json_manager.py
 graphdisplay/tools_win_manager.py
 graphdisplay.egg-info/PKG-INFO
 graphdisplay.egg-info/SOURCES.txt
 graphdisplay.egg-info/dependency_links.txt
 graphdisplay.egg-info/top_level.txt
 graphdisplay/graphs/__init__.py
```

### Comparing `graphdisplay-0.4.7/setup.py` & `graphdisplay-0.4.8/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-import pathlib
-import os
-from setuptools import find_packages, setup
-from graphdisplay.general_config import *
-
-HERE = pathlib.Path(__file__).parent
-
-VERSION = VERSION
-PACKAGE_NAME = 'graphdisplay'
-AUTHOR = 'Alberto Penas Díaz (@seniorbeto)'
-AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
-URL = 'https://github.com/seniorbeto'
-
-LICENSE = 'MIT' #Tipo de licencia
-DESCRIPTION = 'Librería para representar grafos visualmente'
-LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
-LONG_DESC_TYPE = "text/markdown"
-
-
-INSTALL_REQUIRES = [
-      'tk==0.1.1'
-      ]
-
-path = os.getcwd()
-try:
-    if os.path.exists(os.path.join(path, "permanent.json")):
-        os.remove(os.path.join(path, "permanent.json"))
-except FileNotFoundError:
-    pass
-
-store_path = os.path.join(path, "graphdisplay/store/")
-
-for file in os.listdir(store_path):
-    if file.endswith(".json"):
-        removing = os.path.join(store_path, file)
-        os.remove(removing)
-
-setup(
-    name=PACKAGE_NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type=LONG_DESC_TYPE,
-    author=AUTHOR,
-    author_email=AUTHOR_EMAIL,
-    url=URL,
-    #install_requires=INSTALL_REQUIRES,
-    license=LICENSE,
-    packages=find_packages(),
-    include_package_data=True,
-    classifiers=['Programming Language :: Python',
-                 'Programming Language :: Python :: 2.7',
-                 'Programming Language :: Python :: 3.3',
-                 'Programming Language :: Python :: 3.4',
-                 'Programming Language :: Python :: 3.5',
-                 'Programming Language :: Python :: 3.6',
-                 'Programming Language :: Python :: 3.7']
+import pathlib
+import os
+from setuptools import find_packages, setup
+from graphdisplay.general_config import *
+
+HERE = pathlib.Path(__file__).parent
+
+VERSION = VERSION
+PACKAGE_NAME = 'graphdisplay'
+AUTHOR = 'Alberto Penas Díaz (@seniorbeto)'
+AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com'
+URL = 'https://github.com/seniorbeto'
+
+LICENSE = 'MIT' #Tipo de licencia
+DESCRIPTION = 'Librería para representar grafos visualmente'
+LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
+LONG_DESC_TYPE = "text/markdown"
+
+
+INSTALL_REQUIRES = [
+      'tk==0.1.1'
+      ]
+
+path = os.getcwd()
+try:
+    if os.path.exists(os.path.join(path, "permanent.json")):
+        os.remove(os.path.join(path, "permanent.json"))
+except FileNotFoundError:
+    pass
+
+store_path = os.path.join(path, "graphdisplay/store/")
+
+for file in os.listdir(store_path):
+    if file.endswith(".json"):
+        removing = os.path.join(store_path, file)
+        os.remove(removing)
+
+setup(
+    name=PACKAGE_NAME,
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type=LONG_DESC_TYPE,
+    author=AUTHOR,
+    author_email=AUTHOR_EMAIL,
+    url=URL,
+    #install_requires=INSTALL_REQUIRES,
+    license=LICENSE,
+    packages=find_packages(),
+    package_data={'graphdisplay': ['graphdisplay.pyi']},
+    include_package_data=True,
+    classifiers=['Programming Language :: Python',
+                 'Programming Language :: Python :: 2.7',
+                 'Programming Language :: Python :: 3.3',
+                 'Programming Language :: Python :: 3.4',
+                 'Programming Language :: Python :: 3.5',
+                 'Programming Language :: Python :: 3.6',
+                 'Programming Language :: Python :: 3.7']
 )
```

