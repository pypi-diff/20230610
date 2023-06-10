# Comparing `tmp/tool_server_generator-0.4.2.tar.gz` & `tmp/tool_server_generator-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tool_server_generator-0.4.2.tar", last modified: Sat Jun 10 15:28:49 2023, max compression
+gzip compressed data, was "tool_server_generator-0.4.3.tar", last modified: Sat Jun 10 21:09:51 2023, max compression
```

## Comparing `tool_server_generator-0.4.2.tar` & `tool_server_generator-0.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.4.2/LICENSE
--rwxr-xr-x   0        0        0      653 2023-06-08 22:39:34.183032 tool_server_generator-0.4.2/config_server.txt
--rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.4.2/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-05 17:15:32.717658 tool_server_generator-0.4.2/readme.md
--rwxr-xr-x   0        0        0     3775 2023-06-10 15:14:01.192644 tool_server_generator-0.4.2/tool_server_generator/__init__.py
--rwxr-xr-x   0        0        0      990 2023-06-09 13:32:47.222267 tool_server_generator-0.4.2/tool_server_generator/examples/config_server.json
--rwxr-xr-x   0        0        0      653 2023-06-08 22:39:31.488290 tool_server_generator-0.4.2/tool_server_generator/examples/config_server.txt
--rwxr-xr-x   0        0        0      984 2023-06-09 13:33:25.461589 tool_server_generator-0.4.2/tool_server_generator/examples/config_server2.txt
--rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.4.2/tool_server_generator/model/app.js
--rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.4.2/tool_server_generator/model/bin/www
--rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.4.2/tool_server_generator/model/package-lock.json
--rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.4.2/tool_server_generator/model/package.json
--rwxr-xr-x   0        0        0      318 2023-06-09 13:30:36.974342 tool_server_generator-0.4.2/tool_server_generator/model/public/images/favicon.ico
--rwxr-xr-x   0        0        0      940 2023-06-09 17:03:39.505128 tool_server_generator-0.4.2/tool_server_generator/model/public/javascripts/jquery.js
--rwxr-xr-x   0        0        0     1297 2023-06-10 15:25:19.412547 tool_server_generator-0.4.2/tool_server_generator/model/public/javascripts/requests.js
--rwxr-xr-x   0        0        0      421 2023-06-09 17:15:12.284029 tool_server_generator-0.4.2/tool_server_generator/model/public/stylesheets/color.css
--rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.4.2/tool_server_generator/model/public/stylesheets/w3.css
--rwxr-xr-x   0        0        0     2755 2023-06-09 17:13:40.296604 tool_server_generator-0.4.2/tool_server_generator/model/routes/index.js
--rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.4.2/tool_server_generator/model/views/error.pug
--rwxr-xr-x   0        0        0     1046 2023-06-09 17:09:04.085388 tool_server_generator-0.4.2/tool_server_generator/model/views/layout.pug
--rwxr-xr-x   0        0        0     1950 2023-06-09 17:16:28.853886 tool_server_generator-0.4.2/tool_server_generator/model/views/requests.pug
--rwxr-xr-x   0        0        0     1899 2023-06-09 17:04:43.374738 tool_server_generator-0.4.2/tool_server_generator/model/workers/process_command.js
--rwxr-xr-x   0        0        0     6296 2023-06-09 17:04:43.379737 tool_server_generator-0.4.2/tool_server_generator/model/workers/request_listener.js
--rwxr-xr-x   0        0        0    18264 2023-06-10 13:47:20.778475 tool_server_generator-0.4.2/tool_server_generator/utils/config_parser.py
--rwxr-xr-x   0        0        0     9443 2023-06-09 18:03:18.725394 tool_server_generator-0.4.2/tool_server_generator/utils/config_server.py
--rwxr-xr-x   0        0        0      824 2023-06-08 22:05:58.703064 tool_server_generator-0.4.2/tool_server_generator/utils/utils.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 tool_server_generator-0.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-03-30 17:06:52.175851 tool_server_generator-0.4.3/LICENSE
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:34.183032 tool_server_generator-0.4.3/config_server.txt
+-rwxr-xr-x   0        0        0      526 2023-06-08 17:49:02.430745 tool_server_generator-0.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0     6169 2023-06-10 21:08:13.696305 tool_server_generator-0.4.3/readme.md
+-rwxr-xr-x   0        0        0     3982 2023-06-10 21:08:35.450249 tool_server_generator-0.4.3/tool_server_generator/__init__.py
+-rwxr-xr-x   0        0        0      990 2023-06-09 13:32:47.222267 tool_server_generator-0.4.3/tool_server_generator/examples/config_server.json
+-rwxr-xr-x   0        0        0      653 2023-06-08 22:39:31.488290 tool_server_generator-0.4.3/tool_server_generator/examples/config_server.txt
+-rwxr-xr-x   0        0        0      984 2023-06-09 13:33:25.461589 tool_server_generator-0.4.3/tool_server_generator/examples/config_server2.txt
+-rwxr-xr-x   0        0        0      927 2023-06-06 15:38:53.995935 tool_server_generator-0.4.3/tool_server_generator/model/app.js
+-rwxr-xr-x   0        0        0     1524 2023-06-06 13:59:55.077587 tool_server_generator-0.4.3/tool_server_generator/model/bin/www
+-rwxr-xr-x   0        0        0    46221 2023-06-05 17:39:59.097911 tool_server_generator-0.4.3/tool_server_generator/model/package-lock.json
+-rwxr-xr-x   0        0        0      266 2023-06-05 21:25:25.521566 tool_server_generator-0.4.3/tool_server_generator/model/package.json
+-rwxr-xr-x   0        0        0      318 2023-06-09 13:30:36.974342 tool_server_generator-0.4.3/tool_server_generator/model/public/images/favicon.ico
+-rwxr-xr-x   0        0        0      940 2023-06-09 17:03:39.505128 tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/jquery.js
+-rwxr-xr-x   0        0        0     1297 2023-06-10 15:25:19.412547 tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/requests.js
+-rwxr-xr-x   0        0        0      421 2023-06-09 17:15:12.284029 tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/color.css
+-rwxr-xr-x   0        0        0    23424 2023-06-05 14:50:39.170516 tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/w3.css
+-rwxr-xr-x   0        0        0     2755 2023-06-09 17:13:40.296604 tool_server_generator-0.4.3/tool_server_generator/model/routes/index.js
+-rwxr-xr-x   0        0        0       84 2023-06-05 14:49:43.482781 tool_server_generator-0.4.3/tool_server_generator/model/views/error.pug
+-rwxr-xr-x   0        0        0     1046 2023-06-09 17:09:04.085388 tool_server_generator-0.4.3/tool_server_generator/model/views/layout.pug
+-rwxr-xr-x   0        0        0     1950 2023-06-09 17:16:28.853886 tool_server_generator-0.4.3/tool_server_generator/model/views/requests.pug
+-rwxr-xr-x   0        0        0     1899 2023-06-09 17:04:43.374738 tool_server_generator-0.4.3/tool_server_generator/model/workers/process_command.js
+-rwxr-xr-x   0        0        0     6296 2023-06-09 17:04:43.379737 tool_server_generator-0.4.3/tool_server_generator/model/workers/request_listener.js
+-rwxr-xr-x   0        0        0    18255 2023-06-10 21:07:37.157664 tool_server_generator-0.4.3/tool_server_generator/utils/config_parser.py
+-rwxr-xr-x   0        0        0     9443 2023-06-10 21:07:10.092230 tool_server_generator-0.4.3/tool_server_generator/utils/config_server.py
+-rwxr-xr-x   0        0        0      824 2023-06-08 22:05:58.703064 tool_server_generator-0.4.3/tool_server_generator/utils/utils.py
+-rw-r--r--   0        0        0     6509 1970-01-01 00:00:00.000000 tool_server_generator-0.4.3/PKG-INFO
```

### Comparing `tool_server_generator-0.4.2/LICENSE` & `tool_server_generator-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/config_server.txt` & `tool_server_generator-0.4.3/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/pyproject.toml` & `tool_server_generator-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/__init__.py` & `tool_server_generator-0.4.3/tool_server_generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 import json
 from pyngrok import ngrok
 from .utils.utils import *
 from .utils.config_parser import *
 from .utils.config_server import *
 
-__version__ = '0.4.2'
+__version__ = '0.4.3'
 project_dir = os.path.dirname(os.path.realpath(__file__))
 model_server = f'{project_dir}/model'
 tunnel = None
 
 def start_ngrok(config):
     '''Tenta expor a porta do servidor utilizando o ngrok'''
     global tunnel
@@ -25,30 +25,34 @@
         tunnel = ngrok.connect(config['porta'],'http')
         print('Public URL: ',tunnel.public_url)
     except Exception as e:
         print(e)
         print('Error: Could not expose port using ngrok.')
         tunnel = None
 
-
-def start_server(server_dir,config):
-    '''Inicia o servidor'''
-    global tunnel
+def install_server_dependencies(server_dir,config):
+    '''Instala as dependencias do servidor'''
     server_path = f'{os.getcwd()}/{server_dir}'
     dependencies = ['express','http-errors','adm-zip']
 
     # multer apenas se ferramentas levarem ficheiros como input
     if has_file_input(config['ferramentas']):
         dependencies += ['multer']
         
     dependencies = ' '.join(dependencies)
+    print(f'Installing server dependencies: [{dependencies}]')
+    p = subprocess.call(f'npm i {dependencies} -s', cwd=server_path,shell=True)
+    print('Dependencies installed')
+
+
+def start_server(server_dir):
+    '''Inicia o servidor'''
+    global tunnel
+    server_path = f'{os.getcwd()}/{server_dir}'
     try:
-        print(f'Installing server dependencies: [{dependencies}]')
-        p = subprocess.call(f'npm i {dependencies} -s', cwd=server_path,shell=True)
-        print('Dependencies installed')
         print('Starting server')
         p = subprocess.call(f'npm start', cwd=server_path,shell=True)
     except Exception as e:
         print('Server closed')
         # desconectar ngrok
         if tunnel:
             print('Closing ngrok')
@@ -100,18 +104,20 @@
                 shutil.copy(favicon,destino_favicon)
             except FileNotFoundError:
                 print("Favicon not found!")
                 exit(-1)
             except Exception as e:
                 print(f"Error copying the favicon: {e}")
                 exit(-1)
-                
+        # instalar dependencias do servidor
+        install_server_dependencies(destino,config)
+
         #iniciar servidor
         if args.start_server:
             # expor porta de ngrok
             if args.ngrok:
                 start_ngrok(config)
 
-            start_server(destino,config)
+            start_server(destino)
     else:
         print('Error on the configuration file.')
         exit(-1)
```

### Comparing `tool_server_generator-0.4.2/tool_server_generator/examples/config_server.json` & `tool_server_generator-0.4.3/tool_server_generator/examples/config_server.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/examples/config_server.txt` & `tool_server_generator-0.4.3/tool_server_generator/examples/config_server.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/examples/config_server2.txt` & `tool_server_generator-0.4.3/tool_server_generator/examples/config_server2.txt`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/app.js` & `tool_server_generator-0.4.3/tool_server_generator/model/app.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/bin/www` & `tool_server_generator-0.4.3/tool_server_generator/model/bin/www`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/package-lock.json` & `tool_server_generator-0.4.3/tool_server_generator/model/package-lock.json`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/public/javascripts/jquery.js` & `tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/jquery.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/public/javascripts/requests.js` & `tool_server_generator-0.4.3/tool_server_generator/model/public/javascripts/requests.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/public/stylesheets/w3.css` & `tool_server_generator-0.4.3/tool_server_generator/model/public/stylesheets/w3.css`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/routes/index.js` & `tool_server_generator-0.4.3/tool_server_generator/model/routes/index.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/views/layout.pug` & `tool_server_generator-0.4.3/tool_server_generator/model/views/layout.pug`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/views/requests.pug` & `tool_server_generator-0.4.3/tool_server_generator/model/views/requests.pug`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/workers/process_command.js` & `tool_server_generator-0.4.3/tool_server_generator/model/workers/process_command.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/model/workers/request_listener.js` & `tool_server_generator-0.4.3/tool_server_generator/model/workers/request_listener.js`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/utils/config_parser.py` & `tool_server_generator-0.4.3/tool_server_generator/utils/config_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ROTA: /[\w\-\/]+/
 STR: /"[^"]"/
 TEXTO: /"[^"]*"/
 NOME: /[\w\-]+/
 PALAVRA: /[\w\.\-_]+/
 INPUT: /INPUT\d+/
 FLAG: /-{1,2}\w+/
-TYPE: /(STR)|(NUM)|(FILE)|(FOLDER)/
+TYPE: /(STR)|(NUM)|(FILE)/
 PIPE: /\|/
 REDIRECIONAMENTO: /<|>/
 AND: /&/
 COLOR: /(PrimaryBgColor)|(SecondaryBgColor)|(PrimaryTextColor)|(SecondaryTextColor)|(LabelColor)|(BorderColor)/
 HEXCODE: /#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})/
 
 %import common.WS
```

### Comparing `tool_server_generator-0.4.2/tool_server_generator/utils/config_server.py` & `tool_server_generator-0.4.3/tool_server_generator/utils/config_server.py`

 * *Files identical despite different names*

### Comparing `tool_server_generator-0.4.2/tool_server_generator/utils/utils.py` & `tool_server_generator-0.4.3/tool_server_generator/utils/utils.py`

 * *Files identical despite different names*

