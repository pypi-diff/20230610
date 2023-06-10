# Comparing `tmp/ShadowPT-0.1.tar.gz` & `tmp/ShadowPT-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShadowPT-0.1.tar", last modified: Sat Jun 10 17:07:37 2023, max compression
+gzip compressed data, was "ShadowPT-0.2.tar", last modified: Sat Jun 10 19:01:47 2023, max compression
```

## Comparing `ShadowPT-0.1.tar` & `ShadowPT-0.2.tar`

### file list

```diff
@@ -1,30 +1,28 @@
--rw-r--r--   0        0        0     3078 2023-06-01 13:26:07.119486 ShadowPT-0.1/.gitignore
--rw-r--r--   0        0        0     1075 2023-06-01 13:27:53.727880 ShadowPT-0.1/LICENSE
--rw-r--r--   0        0        0       10 2023-06-01 13:26:07.119486 ShadowPT-0.1/README.md
--rw-r--r--   0        0        0     4297 2023-06-06 11:36:04.675957 ShadowPT-0.1/ShadowPT/__init__.py
--rw-r--r--   0        0        0      297 2023-06-02 16:40:03.337401 ShadowPT-0.1/ShadowPT/conf/config.json
--rw-r--r--   0        0        0     9319 2023-06-01 13:55:26.562096 ShadowPT-0.1/ShadowPT/dados/apelidos.txt
--rw-r--r--   0        0        0 26744514 2023-06-02 17:10:31.336431 ShadowPT-0.1/ShadowPT/dados/codigos_postais.csv
--rw-r--r--   0        0        0   187737 2023-06-02 19:21:40.916925 ShadowPT-0.1/ShadowPT/dados/moradas.txt
--rw-r--r--   0        0        0     2224 2023-06-06 11:31:08.223555 ShadowPT-0.1/ShadowPT/dados/moradas_model/config.cfg
--rw-r--r--   0        0        0      467 2023-06-06 11:31:08.223555 ShadowPT-0.1/ShadowPT/dados/moradas_model/meta.json
--rw-r--r--   0        0        0      221 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/ner/cfg
--rw-r--r--   0        0        0  3835000 2023-06-06 11:31:08.246889 ShadowPT-0.1/ShadowPT/dados/moradas_model/ner/model
--rw-r--r--   0        0        0      187 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/ner/moves
--rw-r--r--   0        0        0    38332 2023-06-06 11:31:08.220222 ShadowPT-0.1/ShadowPT/dados/moradas_model/tokenizer
--rw-r--r--   0        0        0        1 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/key2row
--rw-r--r--   0        0        0        1 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/lookups.bin
--rw-r--r--   0        0        0     7775 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/strings.json
--rw-r--r--   0        0        0      128 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/vectors
--rw-r--r--   0        0        0       22 2023-06-06 11:31:08.250223 ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/vectors.cfg
--rw-r--r--   0        0        0   118977 2017-01-04 08:03:16.000000 ShadowPT-0.1/ShadowPT/dados/nomes.pdf
--rw-r--r--   0        0        0    29143 2023-06-01 14:35:31.757445 ShadowPT-0.1/ShadowPT/dados/nomes.txt
--rw-r--r--   0        0        0     1197 2023-06-06 11:49:10.210332 ShadowPT-0.1/ShadowPT/exemplo.txt
--rw-r--r--   0        0        0     4593 2023-06-06 11:30:24.539238 ShadowPT-0.1/ShadowPT/moradas.py
--rw-r--r--   0        0        0       59 2023-06-04 22:26:13.312384 ShadowPT-0.1/ShadowPT/notas
--rw-r--r--   0        0        0      915 2023-06-06 11:49:19.713781 ShadowPT-0.1/ShadowPT/out.txt
--rw-r--r--   0        0        0      795 2023-06-04 22:23:16.066195 ShadowPT-0.1/ShadowPT/out3.txt
--rw-r--r--   0        0        0     1293 2023-06-06 11:33:59.713713 ShadowPT-0.1/ShadowPT/parse_args.py
--rw-r--r--   0        0        0     7466 2023-06-06 11:46:10.624759 ShadowPT-0.1/ShadowPT/utils.py
--rw-r--r--   0        0        0      537 2023-06-10 17:06:53.729870 ShadowPT-0.1/pyproject.toml
--rw-r--r--   0        0        0      446 1970-01-01 00:00:00.000000 ShadowPT-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-06-01 13:26:07.119486 ShadowPT-0.2/.gitignore
+-rw-r--r--   0        0        0     1075 2023-06-01 13:27:53.727880 ShadowPT-0.2/LICENSE
+-rw-r--r--   0        0        0     2521 2023-06-10 17:58:40.655118 ShadowPT-0.2/README.md
+-rw-r--r--   0        0        0     1665 2023-06-10 19:00:03.912153 ShadowPT-0.2/ShadowPT/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-02 16:40:03.337401 ShadowPT-0.2/ShadowPT/conf/config.json
+-rw-r--r--   0        0        0     9319 2023-06-01 13:55:26.562096 ShadowPT-0.2/ShadowPT/dados/apelidos.txt
+-rw-r--r--   0        0        0 26744514 2023-06-02 17:10:31.336431 ShadowPT-0.2/ShadowPT/dados/codigos_postais.csv
+-rw-r--r--   0        0        0   187737 2023-06-02 19:21:40.916925 ShadowPT-0.2/ShadowPT/dados/moradas.txt
+-rw-r--r--   0        0        0     2224 2023-06-06 11:31:08.223555 ShadowPT-0.2/ShadowPT/dados/moradas_model/config.cfg
+-rw-r--r--   0        0        0      467 2023-06-06 11:31:08.223555 ShadowPT-0.2/ShadowPT/dados/moradas_model/meta.json
+-rw-r--r--   0        0        0      221 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/ner/cfg
+-rw-r--r--   0        0        0  3835000 2023-06-06 11:31:08.246889 ShadowPT-0.2/ShadowPT/dados/moradas_model/ner/model
+-rw-r--r--   0        0        0      187 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/ner/moves
+-rw-r--r--   0        0        0    38332 2023-06-06 11:31:08.220222 ShadowPT-0.2/ShadowPT/dados/moradas_model/tokenizer
+-rw-r--r--   0        0        0        1 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/key2row
+-rw-r--r--   0        0        0        1 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/lookups.bin
+-rw-r--r--   0        0        0     7775 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/strings.json
+-rw-r--r--   0        0        0      128 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/vectors
+-rw-r--r--   0        0        0       22 2023-06-06 11:31:08.250223 ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/vectors.cfg
+-rw-r--r--   0        0        0   118977 2017-01-04 08:03:16.000000 ShadowPT-0.2/ShadowPT/dados/nomes.pdf
+-rw-r--r--   0        0        0    29143 2023-06-01 14:35:31.757445 ShadowPT-0.2/ShadowPT/dados/nomes.txt
+-rw-r--r--   0        0        0     1197 2023-06-06 11:49:10.210332 ShadowPT-0.2/ShadowPT/exemplo.txt
+-rw-r--r--   0        0        0     4669 2023-06-10 19:00:23.935675 ShadowPT-0.2/ShadowPT/moradas.py
+-rw-r--r--   0        0        0     2780 2023-06-10 19:00:31.545748 ShadowPT-0.2/ShadowPT/nomes.py
+-rw-r--r--   0        0        0      895 2023-06-10 18:58:06.787807 ShadowPT-0.2/ShadowPT/parse_args.py
+-rw-r--r--   0        0        0     7612 2023-06-10 19:01:00.376028 ShadowPT-0.2/ShadowPT/utils.py
+-rw-r--r--   0        0        0      537 2023-06-10 17:06:53.729870 ShadowPT-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 ShadowPT-0.2/PKG-INFO
```

### Comparing `ShadowPT-0.1/.gitignore` & `ShadowPT-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/LICENSE` & `ShadowPT-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/__init__.py` & `ShadowPT-0.2/ShadowPT/nomes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-#! /usr/bin/env python3
 """
-Modulo que anonimiza textos portugueses com nomes portugueses
+Módulo que trata os nomes e apelidos, sendo obtidos a partir de Web Scraping.
+Os nomes e apelidos são apenas os considerados válidos em Portugal.
 """
-__version__ = '0.1'
 
 import requests
 import bs4
-import json
-from utils import limpa, runcmd, trata_geral
-from parse_args import parse_args
+from .utils import limpa, runcmd
 import os
 
-conf = {}
-args = {}
-apelidos = {}
-nomes = {}
-
 path = os.path.dirname(os.path.abspath(__file__))
 
-def get_conf():
-    """
-    Função que atualiza o dicionario de configuração 
-    """
-    # current path
-    global path
-    with open(path + "/conf/config.json", "r") as f:
-        global conf 
-        conf = json.load(f)
-
-def guarda_apelidos():
+def guarda_apelidos(conf):
     """
     Função que guarda a lista de apelidos portugueses retirados da web
     Url usado definido no ficheiro de configuração
     """
     response = requests.get(conf["url_apelidos"])
     soup = bs4.BeautifulSoup(response.text, "html.parser")
 
@@ -47,15 +29,15 @@
                 columns = line.find_all("td")
                 if len(columns) == 6:
                     f.write(limpa(columns[1].text)+ "\n")
                     if len(columns[3].text.strip()) > 0:
                         for apelido in columns[3].text.split(","):
                             f.write(limpa(apelido) + "\n")
 
-def guarda_nomes():
+def guarda_nomes(conf):
     """
     Função que guarda a lista de nomes portugueses retirados da web
     Url usado definido no ficheiro de configuração
     """
 
     runcmd("wget -O dados/nomes.pdf " + conf["url_nomes"])
     runcmd("pdftotext dados/nomes.pdf dados/nomes.txt")
@@ -66,15 +48,15 @@
             line = limpa(line)
             if len(line) > 0:
                 nomes_limpos += line + "\n" 
 
     with open(path + "/" + conf["nomes"], "w") as f:
         f.write(nomes_limpos)
 
-def get_apelidos():
+def get_apelidos(conf):
     """
     Função que atualiza o dicionario de apelidos
     """
     global apelidos
     with open(path + "/" + conf["apelidos"], "r") as f:
         for line in f:
             line = line.strip()
@@ -82,80 +64,22 @@
                 nome = line[0].upper() + line[1:]
                 letra_inicial = nome[0] 
                 if letra_inicial in apelidos.keys():
                     apelidos[letra_inicial].append(line)
                 else:
                     apelidos[letra_inicial] = [line] 
 
-def get_nomes():
+def get_nomes(conf):
     """
     Função que atualiza o dicionario de nomes
     """
     global nomes
     with open(path + "/" + conf["nomes"], "r") as f:
         for line in f:
             line = line.strip()
             if len(line) > 0:
                 nome = line[0].upper() + line[1:]
                 letra_inicial = nome[0] 
                 if letra_inicial in nomes.keys():
                     nomes[letra_inicial].append(line)
                 else:
-                    nomes[letra_inicial] = [line]
-
-def separa_por_linhas(texto: str):
-    """
-    Função que separa o texto por linhas
-    """
-    return texto.split(". ")
-
-def init():
-    """
-    Função que inicializa o programa
-    """
-    global args
-    get_conf()
-    args = parse_args()
-    global path
-    if args["input"] == "stdin":
-        print("Exemplo de input a partir do texto em "+ path + "/exemplo.txt")
-        args['input'] = path + "/exemplo.txt"
-        #args["input"] = input("Ficheiro de input: ")
-
-#    if args["nomes"]:
-#        guarda_nomes()
-#    
-#    if args["apelidos"]:
-#        guarda_apelidos()
-    
-    get_nomes()
-    get_apelidos()
-
-def main():
-    init()
-    
-    global args
-    global apelidos
-    global nomes
-
-    texto = ""
-    with open(args["input"], "r") as f:
-        texto = f.read()
-    
-    linhas = separa_por_linhas(texto)
-    out = ""
-    nlp = None
-    print("A anonimizar...")
-    for linha in linhas:
-        res,nlp = trata_geral(linha,{"nomes": nomes, "apelidos" : apelidos},nlp=nlp,extra=args['nlp'])
-        out += res + ". "
-
-    if args["output"] == "stdout":
-        print(out)
-    else:
-        with open(args["output"], "w") as f:
-            f.write(out)
-
-    with open("out.txt", "w") as f:
-            f.write(out)
-
-main()
+                    nomes[letra_inicial] = [line]
```

### Comparing `ShadowPT-0.1/ShadowPT/dados/apelidos.txt` & `ShadowPT-0.2/ShadowPT/dados/apelidos.txt`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/codigos_postais.csv` & `ShadowPT-0.2/ShadowPT/dados/codigos_postais.csv`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/moradas.txt` & `ShadowPT-0.2/ShadowPT/dados/moradas.txt`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/moradas_model/config.cfg` & `ShadowPT-0.2/ShadowPT/dados/moradas_model/config.cfg`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/moradas_model/ner/model` & `ShadowPT-0.2/ShadowPT/dados/moradas_model/ner/model`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/moradas_model/tokenizer` & `ShadowPT-0.2/ShadowPT/dados/moradas_model/tokenizer`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/moradas_model/vocab/strings.json` & `ShadowPT-0.2/ShadowPT/dados/moradas_model/vocab/strings.json`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/nomes.pdf` & `ShadowPT-0.2/ShadowPT/dados/nomes.pdf`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/dados/nomes.txt` & `ShadowPT-0.2/ShadowPT/dados/nomes.txt`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/exemplo.txt` & `ShadowPT-0.2/ShadowPT/exemplo.txt`

 * *Files identical despite different names*

### Comparing `ShadowPT-0.1/ShadowPT/moradas.py` & `ShadowPT-0.2/ShadowPT/moradas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+"""
+Módulo que serviu para treinar um modelo cujo intuito é identifcar moradas, datas e nomes
+"""
+
 import csv
 import re
 import os
 import spacy
 
-from faker import Faker
-
 input = [
     # input com morada, nome próprio e localidade
 ("O meu nome é João e moro na Rua da Alegria, 123, 4567-890 Lisboa", {"entities" : [(13, 17, "NOME"), (28, 64, "MOR")]}),
 ("A minha morada é Rua do Meio  3850-093 Albergaria-a-velha, nasci em 1990 e chamo-me Karim Benzema",   {"entities" : [(17, 57, "MOR"), (68,72,"DATA"),(84, 97, "NOME")]}),
 ("Desde o dia 27 de Agosto que moro na Praceta Professor Júlio Catarino  Ílhavo Ílhavo 3830-216", {"entities" : [(12, 23, "DATA"),(37, 93, "MOR")]}),
 ("Sou o Gonçalo da Cunha Freitas, nasci na Avenida General Humberto Delgado 7780-123 Castro Verde",{ "entities" : [(6, 30, "NOME"),(41, 95, "MOR")]}),
 ("O novo local será no Caminho do Espinheiro Milhazes, tendo sido o Henrique Machado o organizador do evento", {"entities" : [(21, 51, "MOR"),(67, 82, "NOME")]}),
```

### Comparing `ShadowPT-0.1/ShadowPT/parse_args.py` & `ShadowPT-0.2/ShadowPT/parse_args.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+"""
+Módulo de tratamento de argumentos com argparse
+"""
 import argparse
 
 
 def parse_args():
     """
     Processa e gera o dicionário de argumentos
     """
     parser = argparse.ArgumentParser(
-                    prog='Anonimator',
-                    description='Ferramenta anonimizadora de texto',
-                    epilog='Trabalho realizado no contexto da UC de SPLN do Mestrado Integrado em Engenharia Informática da Universidade do Minho (UMinho).')
+                    prog='ShadowPT',
+                    description='Ferramenta de anonimização de texto',
+                    epilog='Módulo desenvolvido no contexto da UC de SPLN do Mestrado Integrado em Engenharia Informática da Universidade do Minho (UMinho).')
     
     dic = {}
 
     parser.add_argument('-i', '--input', help='Ficheiro de input', default='stdin')
     parser.add_argument('-o', '--output', help='Ficheiro de output', default='stdout')
-    #parser.add_argument('-n', '--nomes', help='Diretoria do ficheiro de nomes próprios, apenas utilizar esta flag se pretender atualizar o programa com um novo ficheiro de nomes', default=None)
-    #parser.add_argument("-a", "--apelidos", help="Diretoria do ficheiro de apelidos, apenas utilizar esta flag se pretender atualizar o programa com um novo ficheiro de apelidos", default=None)
     parser.add_argument('--nlp', help='Flag para funcionalidade experimental', action='store_true')
     
     args = parser.parse_args()
     dic['input'] = args.input
     dic['output'] = args.output
-    #dic['nomes'] = args.nomes
-    #dic['apelidos'] = args.apelidos
     dic['nlp'] = args.nlp
 
     return dic
```

### Comparing `ShadowPT-0.1/ShadowPT/utils.py` & `ShadowPT-0.2/ShadowPT/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Módulo onde se encontram todas as funções de anonimização.
+"""
 import subprocess
 import re
 import spacy
 import spacy.cli
 import os
 
 path = os.path.dirname(os.path.abspath(__file__)) 
@@ -29,15 +32,15 @@
     std_out, std_err = process.communicate()
     if verbose:
         print(std_out.strip(), std_err)
     pass
 
 def trata_usernames_url(linha):
     """
-    Função que trata os usernames imbutidos em urls, facebook e linkedin 
+    Função que trata os usernames imbutidos em urls
     """
     # https://www.facebook.com/goncalo.freitas.12/
     
     regex_1 = r'((https|http)\:\/\/)?(www\.)?facebook\.com\/[a-zA-Z0-9\.\-\_]+\/?'
         
     # https://www.linkedin.com/in/pedro-ferreira-56031a267/
     regex_2 = r'((https|http)\:\/\/)?(www\.)?linkedin\.com\/in\/[a-zA-Z0-9\.\-\_]+\/?'
@@ -85,15 +88,15 @@
     regex = r'(((http|https|ftp|ftps)\:\/\/)?[a-zA-Z0-9\-\.]+\.[a-zA-Z]{2,3}(\/\S*)?)'
     regex += r'|((www\.)?[a-zA-Z0-9\-\.]+\.[a-z]{2,3}(\/\S*)?)'
 
     return re.sub(regex, 'www...', linha)
 
 def trata_nomes(linha: str,dic_nomes,dic_apelidos):
     """
-    Função que trata os nomes e apelidos
+    Função que trata os nomes e apelidos, utilizando para isso os nomes e apelidos de Portugal, obtimos no módulo nomes.py
     """
     
     for word in linha.split(" "):
         if len(word) > 0:
             inicial = word[0]
             if (inicial in dic_nomes.keys() and word in dic_nomes[inicial]) or \
                (inicial in dic_apelidos.keys() and word in dic_apelidos[inicial]):
@@ -181,15 +184,15 @@
     regex = r'(\d{4})\s*\-\s*(\d{3})'
     return re.sub(regex, 'cod-postal...', linha)
 
 def trata_entre_aspas(linha):
     """
     Função que trata o texto entre aspas
     """
-    regex = r'\"(.+?)\"'
+    regex = r'(\"(.+?)\")|(\'(.+?)\')'
     return re.sub(regex, '"..."', linha)
 
 
 def trata_moradas(linha):
     """
     Função que trata as moradas
     """ 
@@ -248,15 +251,15 @@
     linha = trata_urls(linha)    
     linha = trata_moradas(linha)
     linha = trata_nomes(linha,args["nomes"],args["apelidos"])
     linha = trata_documentos(linha)
     linha = trata_codigos_postais(linha)
     linha = trata_datas(linha)
 
-    words, nlp = trata_spacy(linha,nlp)
+    words, nlp = trata_spacy(init,nlp)
     for word in words:
         linha = linha.replace(word, "ORG...")
 
     if extra:
         linha = trata_experimental(linha)
 
     return linha,nlp
```

### Comparing `ShadowPT-0.1/pyproject.toml` & `ShadowPT-0.2/pyproject.toml`

 * *Files identical despite different names*

