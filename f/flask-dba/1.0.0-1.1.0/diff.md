# Comparing `tmp/flask-dba-1.0.0.tar.gz` & `tmp/flask-dba-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-dba-1.0.0.tar", last modified: Sun May 28 17:32:59 2023, max compression
+gzip compressed data, was "flask-dba-1.1.0.tar", last modified: Sat Jun 10 21:55:01 2023, max compression
```

## Comparing `flask-dba-1.0.0.tar` & `flask-dba-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-28 17:32:59.601552 flask-dba-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2023-05-28 17:30:35.000000 flask-dba-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.597552 flask-dba-1.0.0/flask_dba/
--rw-r--r--   0 root         (0) root         (0)     3342 2023-05-28 17:22:23.000000 flask-dba-1.0.0/flask_dba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/agendamento/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-27 01:16:23.000000 flask-dba-1.0.0/flask_dba/models/agendamento/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-27 01:14:29.000000 flask-dba-1.0.0/flask_dba/models/agendamento/agendamento.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-27 01:13:36.000000 flask-dba-1.0.0/flask_dba/models/agendamento/coleta.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-27 01:11:15.000000 flask-dba-1.0.0/flask_dba/models/agendamento/credencial.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-27 01:15:31.000000 flask-dba-1.0.0/flask_dba/models/agendamento/execucao.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-05-27 01:15:27.000000 flask-dba-1.0.0/flask_dba/models/agendamento/execucao_item.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/base/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-28 15:08:28.000000 flask-dba-1.0.0/flask_dba/models/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-27 01:27:36.000000 flask-dba-1.0.0/flask_dba/models/base/endereco.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/empresa/
--rw-r--r--   0 root         (0) root         (0)      277 2023-05-27 02:32:04.000000 flask-dba-1.0.0/flask_dba/models/empresa/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-05-27 02:30:50.000000 flask-dba-1.0.0/flask_dba/models/empresa/colaborador.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-05-27 02:31:10.000000 flask-dba-1.0.0/flask_dba/models/empresa/empresa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/endereco/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-27 02:13:23.000000 flask-dba-1.0.0/flask_dba/models/endereco/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/permission/
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-27 01:53:07.000000 flask-dba-1.0.0/flask_dba/models/permission/__init__.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-05-28 17:10:14.000000 flask-dba-1.0.0/flask_dba/models/permission/grupo.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-05-27 00:51:52.000000 flask-dba-1.0.0/flask_dba/models/permission/grupo_usuario.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-05-28 17:14:31.000000 flask-dba-1.0.0/flask_dba/models/permission/permissao.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-05-28 17:22:12.000000 flask-dba-1.0.0/flask_dba/models/permission/permissao_grupo.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-05-27 00:55:25.000000 flask-dba-1.0.0/flask_dba/models/permission/permissao_usuario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.601552 flask-dba-1.0.0/flask_dba/models/usuario/
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-27 01:56:50.000000 flask-dba-1.0.0/flask_dba/models/usuario/__init__.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-27 01:58:29.000000 flask-dba-1.0.0/flask_dba/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-28 17:32:59.597552 flask-dba-1.0.0/flask_dba.egg-info/
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-28 17:32:59.000000 flask-dba-1.0.0/flask_dba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-28 17:32:59.000000 flask-dba-1.0.0/flask_dba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-28 17:32:59.000000 flask-dba-1.0.0/flask_dba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-28 17:32:59.000000 flask-dba-1.0.0/flask_dba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-28 17:32:59.000000 flask-dba-1.0.0/flask_dba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-28 17:32:59.601552 flask-dba-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      959 2023-05-28 17:31:17.000000 flask-dba-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-10 21:55:01.204823 flask-dba-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 21:54:43.000000 flask-dba-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.200823 flask-dba-1.1.0/flask_dba/
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.200823 flask-dba-1.1.0/flask_dba/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/exceptions/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.200823 flask-dba-1.1.0/flask_dba/models/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/agendamento/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-27 01:16:23.000000 flask-dba-1.1.0/flask_dba/models/agendamento/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/agendamento/agendamento.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/agendamento/coleta.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-27 01:11:15.000000 flask-dba-1.1.0/flask_dba/models/agendamento/credencial.py
+-rw-r--r--   0 root         (0) root         (0)      897 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/agendamento/execucao.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/agendamento/execucao_item.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/base/
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2023-05-27 01:27:36.000000 flask-dba-1.1.0/flask_dba/models/base/endereco.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/empresa/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-05-27 02:32:04.000000 flask-dba-1.1.0/flask_dba/models/empresa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-05-27 02:30:50.000000 flask-dba-1.1.0/flask_dba/models/empresa/colaborador.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-05-27 02:31:10.000000 flask-dba-1.1.0/flask_dba/models/empresa/empresa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/endereco/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-27 02:13:23.000000 flask-dba-1.1.0/flask_dba/models/endereco/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/permission/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-27 01:53:07.000000 flask-dba-1.1.0/flask_dba/models/permission/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/permission/grupo.py
+-rw-r--r--   0 root         (0) root         (0)      538 2023-05-27 00:51:52.000000 flask-dba-1.1.0/flask_dba/models/permission/grupo_usuario.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/permission/permissao.py
+-rw-r--r--   0 root         (0) root         (0)     1754 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/permission/permissao_grupo.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/permission/permissao_usuario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.204823 flask-dba-1.1.0/flask_dba/models/usuario/
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-06-10 21:54:43.000000 flask-dba-1.1.0/flask_dba/models/usuario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-27 01:58:29.000000 flask-dba-1.1.0/flask_dba/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 21:55:01.200823 flask-dba-1.1.0/flask_dba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-10 21:55:01.000000 flask-dba-1.1.0/flask_dba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-10 21:55:01.000000 flask-dba-1.1.0/flask_dba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 21:55:01.000000 flask-dba-1.1.0/flask_dba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-10 21:55:01.000000 flask-dba-1.1.0/flask_dba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-10 21:55:01.000000 flask-dba-1.1.0/flask_dba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-10 21:55:01.204823 flask-dba-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      959 2023-06-10 21:54:43.000000 flask-dba-1.1.0/setup.py
```

### Comparing `flask-dba-1.0.0/PKG-INFO` & `flask-dba-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dba
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/flask_dba
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
@@ -24,10 +24,16 @@
 app = Flask(__name__)
 app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///test.db'
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 dba = FlaskDBA(app, db)
 dba.init_usuario()
 dba.init_permissions(
-    with_usuario=True
+    usuario=True
 )
 ```
+> Iniciando a permissoes junto as rotas do servidor
+permisssoes usa a env FLASK_DBA_NAME para definir o app na permissao por padrão é "principal".
+
+```bash
+flask init_rules
+```
```

### Comparing `flask-dba-1.0.0/flask_dba/models/agendamento/agendamento.py` & `flask-dba-1.1.0/flask_dba/models/endereco/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,41 @@
-"""Modelo de agendamento para o scheduler."""
-from sqlalchemy import Column, Integer, ForeignKey, String
+from sqlalchemy import Column, String, ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.ext.declarative import declared_attr
 from ..base import ModelBase
+from ..base.endereco import EnderecoModelBase
 
 
-class Agendamento(ModelBase):
-    """Agendamento para o scheduler."""
-    __tablename__ = 'Agendamento'
-
-    dia = Column(Integer, nullable=False)
-    hora = Column(Integer, nullable=False)
-    minuto = Column(Integer, nullable=False)
+class Endereco(EnderecoModelBase, ModelBase):
+    """Modelo de endereço."""
+    __tablename__ = 'Endereco'
+    estado_uuid = Column(
+        String(36),
+        ForeignKey('Estado.uuid'),
+        nullable=False
+    )
+    estado = declared_attr(
+        lambda cls: relationship(
+            'Estado', backref='Endereco',
+        ))
 
-    credencial_uuid = Column(
+
+class UsuarioEndereco(ModelBase):
+    """Modelo de endereço de usuário."""
+    __tablename__ = 'UsuarioEndereco'
+
+    endereco_uuid = Column(
         String(36),
-        ForeignKey("Credencial.uuid"),
+        ForeignKey('Endereco.uuid'),
         nullable=False
     )
-    credencial = declared_attr(
+    endereco = declared_attr(
         lambda cls: relationship(
-            'Credencial', backref='Agendamento',
+            'Endereco', backref='UsuarioEndereco',
         ))
+
+
+class Estado(ModelBase):
+    """Modelo de estado."""
+    __tablename__ = 'Estado'
+    nome = Column(String(100), nullable=False)
+    sigla = Column(String(2), nullable=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flask-dba-1.0.0/flask_dba/models/base/__init__.py` & `flask-dba-1.1.0/flask_dba/models/base/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,34 @@
 from sqlalchemy import Column, String, DateTime, Boolean
 from datetime import datetime
 from ..utils import uuid_default
 
 
 class ModelMetodosBase():
     """Model base para todos os modelos."""
+    _instancia = {
+        'app': None,
+        'db': None,
+        'dba': None,
+    }
 
-    def add(self, db):
+    def add(self):
         """Adiciona o obj ao banco de dados."""
-        db.session.add(self)
-        self.flush(db)
+        self._instancia['db'].session.add(self)
+        return self.flush()
 
-    def save(self, db):
+    def save(self):
         """Faz Commit no banco de dados."""
-        db.session.commit()
+        self._instancia['db'].session.commit()
+        return self
 
-    def flush(self, db):
+    def flush(self):
         """Atualiza as informações do banco de dados."""
-        db.session.flush()
+        self._instancia['db'].session.flush()
+        return self
 
 
 class ModelBase(ModelMetodosBase):
     """Model base para todos os modelos."""
     uuid = Column(
         String(36),
         primary_key=True,
```

### Comparing `flask-dba-1.0.0/flask_dba/models/empresa/colaborador.py` & `flask-dba-1.1.0/flask_dba/models/empresa/colaborador.py`

 * *Files identical despite different names*

### Comparing `flask-dba-1.0.0/flask_dba/models/empresa/empresa.py` & `flask-dba-1.1.0/flask_dba/models/empresa/empresa.py`

 * *Files identical despite different names*

### Comparing `flask-dba-1.0.0/flask_dba/models/permission/grupo.py` & `flask-dba-1.1.0/flask_dba/models/permission/grupo.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,19 +16,19 @@
         grupo = cls.query.filter(
             cls.custom == 0,
             cls.excludo == 0,
             cls.nome == nome,
         ).first()
         if not grupo:
             grupo = cls(nome=nome, custom=False)
-            grupo.add(db)
+            grupo.add()
         return grupo
 
     @staticmethod
     def gerar_grupos(cls, permissao, db):
         raws = permissao.permissoes_sem_grupo_correspondente(
             db
         )
         for raw in raws:
             grupo = cls(nome=raw[0], custom=False)
-            grupo.add(db)
+            grupo.add()
         db.session.commit()
```

### Comparing `flask-dba-1.0.0/flask_dba/models/permission/grupo_usuario.py` & `flask-dba-1.1.0/flask_dba/models/permission/grupo_usuario.py`

 * *Files identical despite different names*

### Comparing `flask-dba-1.0.0/flask_dba/models/permission/permissao_grupo.py` & `flask-dba-1.1.0/flask_dba/models/permission/permissao_grupo.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     def gerar_relacoes(cls, db):
         """Gera as relações entre permissão e grupo."""
         for match in cls.permissoes_com_grupo_sem_match(db):
             permissao_grupo = cls(
                 permissao_uuid=match[0],
                 grupo_uuid=match[1],
             )
-            permissao_grupo.add(db)
+            permissao_grupo.add()
         db.session.commit()
```

### Comparing `flask-dba-1.0.0/flask_dba/models/utils.py` & `flask-dba-1.1.0/flask_dba/models/utils.py`

 * *Files identical despite different names*

### Comparing `flask-dba-1.0.0/flask_dba.egg-info/PKG-INFO` & `flask-dba-1.1.0/flask_dba.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-dba
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/flask_dba
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
@@ -24,10 +24,16 @@
 app = Flask(__name__)
 app.config['SQLALCHEMY_DATABASE_URI'] = 'sqlite:///test.db'
 app.config['SQLALCHEMY_TRACK_MODIFICATIONS'] = False
 db = SQLAlchemy(app)
 dba = FlaskDBA(app, db)
 dba.init_usuario()
 dba.init_permissions(
-    with_usuario=True
+    usuario=True
 )
 ```
+> Iniciando a permissoes junto as rotas do servidor
+permisssoes usa a env FLASK_DBA_NAME para definir o app na permissao por padrão é "principal".
+
+```bash
+flask init_rules
+```
```

### Comparing `flask-dba-1.0.0/flask_dba.egg-info/SOURCES.txt` & `flask-dba-1.1.0/flask_dba.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 setup.py
 flask_dba/__init__.py
 flask_dba.egg-info/PKG-INFO
 flask_dba.egg-info/SOURCES.txt
 flask_dba.egg-info/dependency_links.txt
 flask_dba.egg-info/requires.txt
 flask_dba.egg-info/top_level.txt
+flask_dba/exceptions/__init__.py
+flask_dba/exceptions/utils.py
 flask_dba/models/utils.py
 flask_dba/models/agendamento/__init__.py
 flask_dba/models/agendamento/agendamento.py
 flask_dba/models/agendamento/coleta.py
 flask_dba/models/agendamento/credencial.py
 flask_dba/models/agendamento/execucao.py
 flask_dba/models/agendamento/execucao_item.py
```

### Comparing `flask-dba-1.0.0/setup.py` & `flask-dba-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='flask-dba',
-    version='1.0.0',
+    version='1.1.0',
     url='https://github.com/feiticeiro-tec/flask_dba',
     license='BSD3',
     author='Silvio Henrique Cruz Da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silviohenriquecruzdasilva@gmail.com',
     keywords='Pacote',
```

