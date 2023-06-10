# Comparing `tmp/trissotech-0.0.5.tar.gz` & `tmp/trissotech-0.0.6.tar.gz`

## Comparing `trissotech-0.0.5.tar` & `trissotech-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/Libreria_Trisso.iml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/modules.xml
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 trissotech-0.0.5/src/Trissotech/API.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.5/src/Trissotech/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.5/LICENSE
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 trissotech-0.0.5/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 trissotech-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 trissotech-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/Libreria_Trisso.iml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 trissotech-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 trissotech-0.0.6/src/Trissotech/API.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trissotech-0.0.6/src/Trissotech/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 trissotech-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 trissotech-0.0.6/README.md
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 trissotech-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 trissotech-0.0.6/PKG-INFO
```

### Comparing `trissotech-0.0.5/.idea/inspectionProfiles/Project_Default.xml` & `trissotech-0.0.6/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.5/src/Trissotech/API.py` & `trissotech-0.0.6/src/Trissotech/API.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import base64
 import time
 import io
 from PIL import Image
 from datetime import datetime
 import os
-
+import cv2
 
 def yolo_fire_prediction(url, image_path, download_path, save_img=True, verbose=True):
     """
     Predicción de incendios - YOLO - SoF/TT:
     ########################################
 
     Realiza una predicción de detección de incendios utilizando el modelo YOLO alojado en el servidor.
@@ -120,7 +120,127 @@
                 except:
                     pass
 
             else:
                 print('Error en la solicitud del resultado:', result_response.text)
     else:
         print('Error en la solicitud:', response.text)
+
+
+
+def yolo_fire_prediction_no_img(url, image_path, model, threshold, image_size, verbose=True):
+    """
+    Predicción de incendios - YOLO - SoF/TT:
+    ########################################
+
+    Realiza una predicción de detección de incendios utilizando el modelo YOLO alojado en el servidor.
+
+    -----
+
+    :Example:
+
+    Por ejemplo:
+    ############
+
+    Código::
+
+        import time
+        # URL de la API
+        url_endpoint = 'http://ip:puerto'
+
+        # Ruta de la imagen que deseas enviar
+        image_path_fire = '../data/test_facu/quema_controlada132.jpg'
+
+        predic, posi = yolo_fire_prediction_no_img(url=url_endpoint,
+                                            image_path=image_path_fire,
+                                            model = 'v3',
+                                            threshold = 0.1,
+                                            image_size = (416,416),
+                                            verbose=True)
+    Esto devuelve por consola::
+
+        >> Cargando quema_controlada132.jpg
+        >> El servidor recibió la imagen correctamente. Procesando... Id de tarea: 8008e8b8-bcfd-4dd3-b648-5a012e909bf2
+        >> Obteniendo imagen procesada, espere
+        >> Imagen procesada con éxito. 00:04:34
+        >> Detecciones realizadas: Detección: Fuego
+        >> [['humo', 2, 109, 45, 47, '0.71'], ['humo', 15, 81, 202, 84, '0.6'], ['humo', 216, 135, 21, 29, '0.48'], ['humo', 23, 132, 26, 27, '0.46']]
+
+    Parametros y returns:
+    #####################
+
+    -----
+
+    :param url: URL del servicio de detección de incendios (str).
+    :param image_path: Ruta de la imagen que se desea enviar para la predicción (str).
+    :param model: Modelo a utilizar para la inferencia (str).
+    :param threshold: sensibilidad a utilizar para la inferencia (float).
+    :param image_size: Indica el tamaño de la imagen de entrada al modelo (tuple).
+    :param verbose: Indica si se deben imprimir mensajes de información durante la ejecución. Valor predeterminado: True (bool).
+
+    :return: Texto con las predicciones realizadas (str).
+    :return: Texto con las posiciones de las detecciones (str).
+
+    """
+
+
+    nombre_imagen = image_path.split('/')[-1]
+    if verbose:
+        print(f'Cargando {nombre_imagen}')
+
+
+    # Leer la imagen
+    img = cv2.imread(image_path)
+
+    # Redimensionar la imagen a 416x416 píxeles
+    resized_img = cv2.resize(img, image_size)
+
+    # Crear un diccionario que contenga la imagen redimensionada y el string
+    data = {'image': cv2.imencode('.jpg', resized_img)[1].tobytes(), 'sensibilidad': f'{threshold}'}
+
+    # Realizar la solicitud POST con la imagen
+    response = requests.post(f'{url}/detect_{model}', files=data)
+
+    # Verificar el estado de la respuesta
+    if response.status_code == 200:
+        # Obtener los datos de la respuesta JSON
+        response_data = response.json()
+        if verbose:
+            print(f"El servidor recibió la imagen correctamente. Procesando... Id de tarea: {response_data['job_id']}")
+
+        # Obtener el ID del trabajo encolado
+        job_id = response_data['job_id']
+
+        # Ruta para obtener el resultado del trabajo
+        result_url = f'{url}/result/{job_id}'
+
+        if verbose:
+            print('Obteniendo imagen procesada, espere')
+        while True:
+            time.sleep(0.5)
+
+            # Realizar la solicitud GET para obtener el resultado
+            result_response = requests.get(result_url)
+
+            # Verificar el estado de la respuesta
+            if result_response.status_code == 200:
+
+                # Obtener los datos del resultado JSON
+                result_data = result_response.json()
+
+                try:
+                    predicción = result_data['text']
+                    pos = result_data['posiciones']
+
+                    if verbose:
+                        print(f'Imagen procesada con éxito. {datetime.now().strftime("%H:%M:%S")}')
+                        print(f'Detecciones realizadas: {predicción}')
+                        print(f'{pos}')
+                    return predicción, pos
+
+                except:
+                    pass
+
+            else:
+                print('Error en la solicitud del resultado:', result_response.text)
+    else:
+        print('Error en la solicitud:', response.text)
```

### Comparing `trissotech-0.0.5/LICENSE` & `trissotech-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trissotech-0.0.5/README.md` & `trissotech-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 pip install Trissotech
 ```
 
 ---
 
 ## Trissotech.API:
 - yolo_fire_prediction: Función para detectar incendios en imágenes utilizando un modelo YOLO.
+- yolo_fire_prediction_no_img: Función para detectar incendios en imágenes utilizando un modelo YOLO.
 
 ---
 
 ### - yolo_fire_prediction()
 Para ejecutar este proyecto, se deben seguir los siguientes pasos:
```

### Comparing `trissotech-0.0.5/pyproject.toml` & `trissotech-0.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Trissotech"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Facu", email="facundonieto@mi.unc.edu.ar" },
 ]
 description = "Trissotech library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
   "pillow",
+  "opencv-python",
 ]
 
 [project.urls]
 "Homepage" = "https://www.trissotech.com/"
 "Bug Tracker" = "https://www.facundonieto.com/contact"
```

### Comparing `trissotech-0.0.5/PKG-INFO` & `trissotech-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Trissotech
-Version: 0.0.5
+Version: 0.0.6
 Summary: Trissotech library
 Project-URL: Homepage, https://www.trissotech.com/
 Project-URL: Bug Tracker, https://www.facundonieto.com/contact
 Author-email: Facu <facundonieto@mi.unc.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: opencv-python
 Requires-Dist: pillow
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <img src="https://trissotech.s3.sa-east-1.amazonaws.com/TT-icon.png" alt="TT" style="width: 200px; height: auto;">
 </p>
@@ -26,14 +27,15 @@
 pip install Trissotech
 ```
 
 ---
 
 ## Trissotech.API:
 - yolo_fire_prediction: Función para detectar incendios en imágenes utilizando un modelo YOLO.
+- yolo_fire_prediction_no_img: Función para detectar incendios en imágenes utilizando un modelo YOLO.
 
 ---
 
 ### - yolo_fire_prediction()
 Para ejecutar este proyecto, se deben seguir los siguientes pasos:
```

