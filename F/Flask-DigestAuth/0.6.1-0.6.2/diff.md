# Comparing `tmp/Flask-DigestAuth-0.6.1.tar.gz` & `tmp/Flask-DigestAuth-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-DigestAuth-0.6.1.tar", last modified: Tue May  2 23:00:54 2023, max compression
+gzip compressed data, was "Flask-DigestAuth-0.6.2.tar", last modified: Sat Jun 10 08:27:41 2023, max compression
```

## Comparing `Flask-DigestAuth-0.6.1.tar` & `Flask-DigestAuth-0.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/
--rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.6.1/LICENSE
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/MANIFEST.in
--rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)     2787 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/README.rst
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/docs/
--rw-r--r--   0 imacat    (1000) users      (100)      638 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/Makefile
--rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/make.bat
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/docs/source/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/docs/source/_static/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/_static/.keep
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/docs/source/_templates/
--rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/_templates/.keep
--rw-r--r--   0 imacat    (1000) users      (100)     2254 2023-05-02 22:59:26.000000 Flask-DigestAuth-0.6.1/docs/source/changelog.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1071 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/conf.py
--rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/examples.rst
--rw-r--r--   0 imacat    (1000) users      (100)      678 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/flask_digest_auth.rst
--rw-r--r--   0 imacat    (1000) users      (100)      915 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/index.rst
--rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/intro.rst
--rw-r--r--   0 imacat    (1000) users      (100)       60 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.1/docs/source/modules.rst
--rw-r--r--   0 imacat    (1000) users      (100)     1845 2023-04-26 15:30:27.000000 Flask-DigestAuth-0.6.1/pyproject.toml
--rw-r--r--   0 imacat    (1000) users      (100)       38 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/setup.cfg
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.136977 Flask-DigestAuth-0.6.1/src/
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/
--rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/PKG-INFO
--rw-r--r--   0 imacat    (1000) users      (100)      708 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/SOURCES.txt
--rw-r--r--   0 imacat    (1000) users      (100)        1 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/dependency_links.txt
--rw-r--r--   0 imacat    (1000) users      (100)       37 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/requires.txt
--rw-r--r--   0 imacat    (1000) users      (100)       18 2023-05-02 23:00:54.000000 Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/top_level.txt
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/src/flask_digest_auth/
--rw-r--r--   0 imacat    (1000) users      (100)      939 2023-05-02 22:59:26.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/__init__.py
--rw-r--r--   0 imacat    (1000) users      (100)     4103 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/algo.py
--rw-r--r--   0 imacat    (1000) users      (100)    17796 2023-05-02 22:37:13.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/auth.py
--rw-r--r--   0 imacat    (1000) users      (100)     5569 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/src/flask_digest_auth/test.py
-drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-05-02 23:00:54.140977 Flask-DigestAuth-0.6.1/tests/
--rw-r--r--   0 imacat    (1000) users      (100)     1956 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.1/tests/test_algo.py
--rw-r--r--   0 imacat    (1000) users      (100)     7849 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/tests/test_auth.py
--rw-r--r--   0 imacat    (1000) users      (100)    10525 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.1/tests/test_flask_login.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/
+-rw-r--r--   0 imacat    (1000) users      (100)    11358 2018-06-01 15:46:07.000000 Flask-DigestAuth-0.6.2/LICENSE
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/MANIFEST.in
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)     2787 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/README.rst
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.609066 Flask-DigestAuth-0.6.2/docs/
+-rw-r--r--   0 imacat    (1000) users      (100)      638 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/Makefile
+-rw-r--r--   0 imacat    (1000) users      (100)      804 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/make.bat
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.609066 Flask-DigestAuth-0.6.2/docs/source/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.609066 Flask-DigestAuth-0.6.2/docs/source/_static/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/_static/.keep
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/docs/source/_templates/
+-rw-r--r--   0 imacat    (1000) users      (100)        0 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/_templates/.keep
+-rw-r--r--   0 imacat    (1000) users      (100)     2479 2023-06-10 07:49:41.000000 Flask-DigestAuth-0.6.2/docs/source/changelog.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1071 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/conf.py
+-rw-r--r--   0 imacat    (1000) users      (100)     6657 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/examples.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      678 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/flask_digest_auth.rst
+-rw-r--r--   0 imacat    (1000) users      (100)      915 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/index.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     4318 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/intro.rst
+-rw-r--r--   0 imacat    (1000) users      (100)       60 2023-04-26 15:27:42.000000 Flask-DigestAuth-0.6.2/docs/source/modules.rst
+-rw-r--r--   0 imacat    (1000) users      (100)     1845 2023-04-26 15:30:27.000000 Flask-DigestAuth-0.6.2/pyproject.toml
+-rw-r--r--   0 imacat    (1000) users      (100)       38 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/setup.cfg
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.609066 Flask-DigestAuth-0.6.2/src/
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/
+-rw-r--r--   0 imacat    (1000) users      (100)     3708 2023-06-10 08:27:41.000000 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/PKG-INFO
+-rw-r--r--   0 imacat    (1000) users      (100)      708 2023-06-10 08:27:41.000000 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 imacat    (1000) users      (100)        1 2023-06-10 08:27:41.000000 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       37 2023-06-10 08:27:41.000000 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/requires.txt
+-rw-r--r--   0 imacat    (1000) users      (100)       18 2023-06-10 08:27:41.000000 Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/top_level.txt
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/src/flask_digest_auth/
+-rw-r--r--   0 imacat    (1000) users      (100)      939 2023-06-10 06:23:15.000000 Flask-DigestAuth-0.6.2/src/flask_digest_auth/__init__.py
+-rw-r--r--   0 imacat    (1000) users      (100)     4103 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.2/src/flask_digest_auth/algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)    17799 2023-05-03 00:06:50.000000 Flask-DigestAuth-0.6.2/src/flask_digest_auth/auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)     5569 2023-05-02 22:57:59.000000 Flask-DigestAuth-0.6.2/src/flask_digest_auth/test.py
+drwxr-xr-x   0 imacat    (1000) users      (100)        0 2023-06-10 08:27:41.613066 Flask-DigestAuth-0.6.2/tests/
+-rw-r--r--   0 imacat    (1000) users      (100)     1956 2023-04-27 01:07:49.000000 Flask-DigestAuth-0.6.2/tests/test_algo.py
+-rw-r--r--   0 imacat    (1000) users      (100)     8118 2023-06-08 09:23:22.000000 Flask-DigestAuth-0.6.2/tests/test_auth.py
+-rw-r--r--   0 imacat    (1000) users      (100)    11012 2023-06-08 09:22:31.000000 Flask-DigestAuth-0.6.2/tests/test_flask_login.py
```

### Comparing `Flask-DigestAuth-0.6.1/LICENSE` & `Flask-DigestAuth-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/MANIFEST.in` & `Flask-DigestAuth-0.6.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/PKG-INFO` & `Flask-DigestAuth-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-DigestAuth
-Version: 0.6.1
+Version: 0.6.2
 Summary: The Flask HTTP Digest Authentication project.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://flask-digestauth.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/flask-digestauth
 Project-URL: Bug Tracker, https://github.com/imacat/flask-digestauth/issues
 Keywords: flask,digest-authentication
```

### Comparing `Flask-DigestAuth-0.6.1/README.rst` & `Flask-DigestAuth-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/Makefile` & `Flask-DigestAuth-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/make.bat` & `Flask-DigestAuth-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/source/changelog.rst` & `Flask-DigestAuth-0.6.2/docs/source/changelog.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 Change Log
 ==========
 
 
+Version 0.6.2
+-------------
+
+Released 2023/6/10
+
+* Changed logging from STDERR to the Flask logger.
+* Test case updates:
+  * Added missing documentation.
+  * Changed properties from public to private.
+  * Disabled logging.
+
+
 Version 0.6.1
 -------------
 
 Released 2023/5/3
 
 * Revised the code for the upcoming Werkzeug 2.4.
```

### Comparing `Flask-DigestAuth-0.6.1/docs/source/conf.py` & `Flask-DigestAuth-0.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/source/examples.rst` & `Flask-DigestAuth-0.6.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/source/flask_digest_auth.rst` & `Flask-DigestAuth-0.6.2/docs/source/flask_digest_auth.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/source/index.rst` & `Flask-DigestAuth-0.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/docs/source/intro.rst` & `Flask-DigestAuth-0.6.2/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/pyproject.toml` & `Flask-DigestAuth-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/PKG-INFO` & `Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-DigestAuth
-Version: 0.6.1
+Version: 0.6.2
 Summary: The Flask HTTP Digest Authentication project.
 Author-email: imacat <imacat@mail.imacat.idv.tw>
 Project-URL: Documentation, https://flask-digestauth.readthedocs.io
 Project-URL: Change Log, https://mia-accounting.readthedocs.io/en/latest/changelog.html
 Project-URL: Repository, https://github.com/imacat/flask-digestauth
 Project-URL: Bug Tracker, https://github.com/imacat/flask-digestauth/issues
 Keywords: flask,digest-authentication
```

### Comparing `Flask-DigestAuth-0.6.1/src/Flask_DigestAuth.egg-info/SOURCES.txt` & `Flask-DigestAuth-0.6.2/src/Flask_DigestAuth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/src/flask_digest_auth/__init__.py` & `Flask-DigestAuth-0.6.2/src/flask_digest_auth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 """The HTTP digest authentication.
 
 """
 from flask_digest_auth.algo import make_password_hash, calc_response
 from flask_digest_auth.auth import DigestAuth
 from flask_digest_auth.test import Client
 
-VERSION: str = "0.6.1"
+VERSION: str = "0.6.2"
 """The package version."""
```

### Comparing `Flask-DigestAuth-0.6.1/src/flask_digest_auth/algo.py` & `Flask-DigestAuth-0.6.2/src/flask_digest_auth/algo.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/src/flask_digest_auth/auth.py` & `Flask-DigestAuth-0.6.2/src/flask_digest_auth/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             state: AuthState = AuthState()
             try:
                 g.user = auth_user(state)
                 self.__on_login(g.user)
                 return view(*args, **kwargs)
             except UnauthorizedException as e:
                 if len(e.args) > 0:
-                    sys.stderr.write(e.args[0] + "\n")
+                    current_app.logger.warning(e.args[0])
                 response: Response = Response()
                 response.status = 401
                 response.headers["WWW-Authenticate"] \
                     = self.__make_response_header(state)
                 abort(response)
 
         return login_required_view
```

### Comparing `Flask-DigestAuth-0.6.1/src/flask_digest_auth/test.py` & `Flask-DigestAuth-0.6.2/src/flask_digest_auth/test.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/tests/test_algo.py` & `Flask-DigestAuth-0.6.2/tests/test_algo.py`

 * *Files identical despite different names*

### Comparing `Flask-DigestAuth-0.6.1/tests/test_auth.py` & `Flask-DigestAuth-0.6.2/tests/test_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,63 +14,71 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test case for the HTTP digest authentication.
 
 """
+import logging
 from secrets import token_urlsafe
 from typing import Any, Optional, Dict
 
 from flask import Response, Flask, g, redirect, request
 from flask_testing import TestCase
 from werkzeug.datastructures import WWWAuthenticate, Authorization
 
 from flask_digest_auth import DigestAuth, make_password_hash, Client
 
 _REALM: str = "testrealm@host.com"
+"""The realm."""
 _USERNAME: str = "Mufasa"
+"""The username."""
 _PASSWORD: str = "Circle Of Life"
+"""The password."""
 
 
 class User:
     """A dummy user"""
 
     def __init__(self, username: str, password: str):
         """Constructs a dummy user.
 
         :param username: The username.
         :param password: The clear-text password.
         """
         self.username: str = username
-        self.password_hash: str = make_password_hash(
-            _REALM, username, password)
+        """The username."""
+        self.password_hash: str = make_password_hash(_REALM, username, password)
+        """The password hash."""
         self.visits: int = 0
+        """The number of visits."""
 
 
 class AuthenticationTestCase(TestCase):
     """The test case for the HTTP digest authentication."""
 
     def create_app(self):
         """Creates the Flask application.
 
         :return: The Flask application.
         """
+        logging.getLogger("test_auth").addHandler(logging.NullHandler())
         app: Flask = Flask(__name__)
         app.config.from_mapping({
             "TESTING": True,
             "SECRET_KEY": token_urlsafe(32),
             "DIGEST_AUTH_REALM": _REALM,
         })
         app.test_client_class = Client
 
         auth: DigestAuth = DigestAuth()
         auth.init_app(app)
-        self.user: User = User(_USERNAME, _PASSWORD)
-        user_db: Dict[str, User] = {_USERNAME: self.user}
+        self.__user: User = User(_USERNAME, _PASSWORD)
+        """The user account."""
+        user_db: Dict[str, User] = {_USERNAME: self.__user}
 
         @auth.register_get_password
         def get_password_hash(username: str) -> Optional[str]:
             """Returns the password hash of a user.
 
             :param username: The username.
             :return: The password hash, or None if the user does not exist.
@@ -138,15 +146,15 @@
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data.decode("UTF-8"),
                          f"Hello, {_USERNAME}! #1")
         response: Response = self.client.get(self.app.url_for("admin-2"))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data.decode("UTF-8"),
                          f"Hello, {_USERNAME}! #2")
-        self.assertEqual(self.user.visits, 1)
+        self.assertEqual(self.__user.visits, 1)
 
     def test_stale_opaque(self) -> None:
         """Tests the stale and opaque value.
 
         :return: None.
         """
         admin_uri: str = self.app.url_for("admin-1")
@@ -215,8 +223,8 @@
 
         response = self.client.get(admin_uri,
                                    digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(admin_uri)
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(self.user.visits, 2)
+        self.assertEqual(self.__user.visits, 2)
```

### Comparing `Flask-DigestAuth-0.6.1/tests/test_flask_login.py` & `Flask-DigestAuth-0.6.2/tests/test_flask_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,43 +14,51 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """The test case for the Flask-Login integration.
 
 """
+import logging
 from secrets import token_urlsafe
 from typing import Optional, Dict
 
 from flask import Response, Flask, g, redirect, request
 from flask_testing import TestCase
 from werkzeug.datastructures import WWWAuthenticate, Authorization
 
 from flask_digest_auth import DigestAuth, make_password_hash, Client
 
 _REALM: str = "testrealm@host.com"
+"""The realm."""
 _USERNAME: str = "Mufasa"
+"""The username."""
 _PASSWORD: str = "Circle Of Life"
+"""The password."""
 
 
 class User:
     """A dummy user."""
 
     def __init__(self, username: str, password: str):
         """Constructs a dummy user.
 
         :param username: The username.
         :param password: The clear-text password.
         """
         self.username: str = username
-        self.password_hash: str = make_password_hash(
-            _REALM, username, password)
+        """The username."""
+        self.password_hash: str = make_password_hash(_REALM, username, password)
+        """The password hash."""
         self.visits: int = 0
+        """The number of visits."""
         self.is_active: bool = True
+        """True if the account is active, or False otherwise."""
         self.is_anonymous: bool = False
+        """True if the account is anonymous, or False otherwise."""
 
     def get_id(self) -> str:
         """Returns the username.
         This is required by Flask-Login.
 
         :return: The username.
         """
@@ -71,37 +79,40 @@
     """The test case with the Flask-Login integration."""
 
     def create_app(self) -> Flask:
         """Creates the Flask application.
 
         :return: The Flask application.
         """
+        logging.getLogger("test_flask_login").addHandler(logging.NullHandler())
         app: Flask = Flask(__name__)
         app.config.from_mapping({
             "TESTING": True,
             "SECRET_KEY": token_urlsafe(32),
             "DIGEST_AUTH_REALM": _REALM,
         })
         app.test_client_class = Client
 
-        self.has_flask_login: bool = True
+        self.__has_flask_login: bool = True
+        """Whether the Flask-Login package is installed."""
         try:
             import flask_login
         except ModuleNotFoundError:
-            self.has_flask_login = False
+            self.__has_flask_login = False
             return app
 
         login_manager: flask_login.LoginManager = flask_login.LoginManager()
         login_manager.init_app(app)
 
         auth: DigestAuth = DigestAuth()
         auth.init_app(app)
 
-        self.user: User = User(_USERNAME, _PASSWORD)
-        user_db: Dict[str, User] = {_USERNAME: self.user}
+        self.__user: User = User(_USERNAME, _PASSWORD)
+        """The user account."""
+        user_db: Dict[str, User] = {_USERNAME: self.__user}
 
         @auth.register_get_password
         def get_password_hash(username: str) -> Optional[str]:
             """Returns the password hash of a user.
 
             :param username: The username.
             :return: The password hash, or None if the user does not exist.
@@ -158,36 +169,36 @@
         return app
 
     def test_auth(self) -> None:
         """Tests the authentication.
 
         :return: None.
         """
-        if not self.has_flask_login:
+        if not self.__has_flask_login:
             self.skipTest("Skipped without Flask-Login.")
 
         response: Response = self.client.get(self.app.url_for("admin-1"))
         self.assertEqual(response.status_code, 401)
         response = self.client.get(
             self.app.url_for("admin-1"), digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data.decode("UTF-8"),
                          f"Hello, {_USERNAME}! #1")
         response: Response = self.client.get(self.app.url_for("admin-2"))
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.data.decode("UTF-8"),
                          f"Hello, {_USERNAME}! #2")
-        self.assertEqual(self.user.visits, 1)
+        self.assertEqual(self.__user.visits, 1)
 
     def test_stale_opaque(self) -> None:
         """Tests the stale and opaque value.
 
         :return: None.
         """
-        if not self.has_flask_login:
+        if not self.__has_flask_login:
             self.skipTest("Skipped without Flask-Login.")
 
         admin_uri: str = self.app.url_for("admin-1")
         response: Response
         www_authenticate: WWWAuthenticate
         auth_data: Authorization
 
@@ -227,15 +238,15 @@
         self.assertEqual(response.status_code, 200)
 
     def test_logout(self) -> None:
         """Tests the logging out.
 
         :return: None.
         """
-        if not self.has_flask_login:
+        if not self.__has_flask_login:
             self.skipTest("Skipped without Flask-Login.")
 
         admin_uri: str = self.app.url_for("admin-1")
         logout_uri: str = self.app.url_for("logout")
         response: Response
 
         response = self.client.get(admin_uri)
@@ -261,39 +272,39 @@
 
         response = self.client.get(admin_uri,
                                    digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 200)
 
         response = self.client.get(admin_uri)
         self.assertEqual(response.status_code, 200)
-        self.assertEqual(self.user.visits, 2)
+        self.assertEqual(self.__user.visits, 2)
 
     def test_disabled(self) -> None:
         """Tests the disabled user.
 
         :return: None.
         """
-        if not self.has_flask_login:
+        if not self.__has_flask_login:
             self.skipTest("Skipped without Flask-Login.")
 
         response: Response
 
-        self.user.is_active = False
+        self.__user.is_active = False
         response = self.client.get(self.app.url_for("admin-1"))
         self.assertEqual(response.status_code, 401)
         response = self.client.get(self.app.url_for("admin-1"),
                                    digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 401)
 
-        self.user.is_active = True
+        self.__user.is_active = True
         response = self.client.get(self.app.url_for("admin-1"),
                                    digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 200)
         response = self.client.get(self.app.url_for("admin-1"))
         self.assertEqual(response.status_code, 200)
 
-        self.user.is_active = False
+        self.__user.is_active = False
         response = self.client.get(self.app.url_for("admin-1"))
         self.assertEqual(response.status_code, 401)
         response = self.client.get(self.app.url_for("admin-1"),
                                    digest_auth=(_USERNAME, _PASSWORD))
         self.assertEqual(response.status_code, 401)
```

