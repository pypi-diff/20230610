# Comparing `tmp/cardboard.py-0.0.8.tar.gz` & `tmp/cardboard.py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardboard.py-0.0.8.tar", last modified: Tue Jun  6 02:20:05 2023, max compression
+gzip compressed data, was "cardboard.py-0.0.9.tar", last modified: Wed Jun  7 01:15:19 2023, max compression
```

## Comparing `cardboard.py-0.0.8.tar` & `cardboard.py-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.651756 cardboard.py-0.0.8/
--rw-rw-rw-   0        0        0     5380 2023-06-06 02:20:05.649609 cardboard.py-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4417 2023-06-06 02:18:16.000000 cardboard.py-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.625615 cardboard.py-0.0.8/cardboard/
--rw-rw-rw-   0        0        0     1334 2023-06-06 01:19:09.000000 cardboard.py-0.0.8/cardboard/Exceptions.py
--rw-rw-rw-   0        0        0      191 2023-06-06 00:35:10.000000 cardboard.py-0.0.8/cardboard/__init__.py
--rw-rw-rw-   0        0        0    11468 2023-06-06 02:16:51.000000 cardboard.py-0.0.8/cardboard/cardboard.py
--rw-rw-rw-   0        0        0    12918 2023-06-06 01:57:32.000000 cardboard.py-0.0.8/cardboard/cardboard_async.py
--rw-rw-rw-   0        0        0     6023 2023-06-06 02:16:16.000000 cardboard.py-0.0.8/cardboard/flask_integration.py
-drwxrwxrwx   0        0        0        0 2023-06-06 02:20:05.645611 cardboard.py-0.0.8/cardboard.py.egg-info/
--rw-rw-rw-   0        0        0     5380 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-06 02:20:05.000000 cardboard.py-0.0.8/cardboard.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 02:20:05.652612 cardboard.py-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-06-06 00:42:12.000000 cardboard.py-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:15:19.366062 cardboard.py-0.0.9/
+-rw-rw-rw-   0        0        0     6202 2023-06-07 01:15:19.365063 cardboard.py-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5209 2023-06-07 01:15:02.000000 cardboard.py-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 01:15:19.353062 cardboard.py-0.0.9/cardboard/
+-rw-rw-rw-   0        0        0     1334 2023-06-06 01:19:09.000000 cardboard.py-0.0.9/cardboard/Exceptions.py
+-rw-rw-rw-   0        0        0      191 2023-06-06 00:35:10.000000 cardboard.py-0.0.9/cardboard/__init__.py
+-rw-rw-rw-   0        0        0    11468 2023-06-06 02:16:51.000000 cardboard.py-0.0.9/cardboard/cardboard.py
+-rw-rw-rw-   0        0        0    12918 2023-06-06 01:57:32.000000 cardboard.py-0.0.9/cardboard/cardboard_async.py
+-rw-rw-rw-   0        0        0    11229 2023-06-07 01:03:14.000000 cardboard.py-0.0.9/cardboard/flask_integration.py
+drwxrwxrwx   0        0        0        0 2023-06-07 01:15:19.363063 cardboard.py-0.0.9/cardboard.py.egg-info/
+-rw-rw-rw-   0        0        0     6202 2023-06-07 01:15:19.000000 cardboard.py-0.0.9/cardboard.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-07 01:15:19.000000 cardboard.py-0.0.9/cardboard.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 01:15:19.000000 cardboard.py-0.0.9/cardboard.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-07 01:15:19.000000 cardboard.py-0.0.9/cardboard.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-07 01:15:19.000000 cardboard.py-0.0.9/cardboard.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 01:15:19.366062 cardboard.py-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1160 2023-06-07 01:08:44.000000 cardboard.py-0.0.9/setup.py
```

### Comparing `cardboard.py-0.0.8/PKG-INFO` & `cardboard.py-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.8
+Version: 0.0.9
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,16 @@
 Initialize the Cardboard or CardboardAsync class. Make sure to pass `secret` and `client_id`.
 
 You can now use the client to make requests.
 
 ### Examples
 These examples will use Flask. Install it with `pip install Flask`
 
+Flask is included with `cardboard.py>=0.0.8`
+
 ```python
 # Python Example
 from flask import Flask, request, redirect, url_for, session, Response
 from cardboard import Cardboard
 
 app = Flask(__name__)
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
@@ -65,14 +67,29 @@
 def dashboard():
     token = session.get('cardboard_token')
     if not token:
         return redirect(cb.app_url)
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+def logout():
+    b = session.pop('cardboard_token', None)
+    if b:
+        try:
+            cb.revoke_token(b)
+        except:
+            pass
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ```python
 # Python Example using FlaskIntegration
 from flask import Flask, request, redirect, url_for, session, Response
@@ -82,38 +99,43 @@
 app.secret_key = 'hi' # set this to something secure, please.
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
 cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
 
 @app.route('/login')
 @cb.fi.autologin
 def login(token):
-    session['cardboard_token'] = token.token
     return redirect(url_for('dashboard'))
 
 @app.route('/dashboard')
-@cb.fi.logged_in('cardboard_token', check=True)
-def dashboard(token:str):
-    # v = cb.check_token(token)
-    # if not v:
-    #     return redirect(cb.app_url)
-    # uncomment above code if check=False
-    user = cb.get_user(token)
+@cb.fi.logged_in
+def dashboard(token):
+    user = cb.get_user(token.token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+@cb.fi.autologout
+def logout():
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
-For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
+For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b014-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
 A list of methods/attributes you can call with either Cardboard or CardboardAsync.
 - `.app_url` (str)
 - `.app_name` (str)
@@ -162,10 +184,18 @@
     - `.moderationStatus` (str|None)
     - `.aboutInfo` (class userAbout)
         - `.bio` (str|None)
         - `.tagline` (str|None)
         - `._raw` (dict)
     - `.userTransientStatus` (str|None)
     - `._raw` (dict)
+- `.check_token(token:str)` (bool)
+
+### FlaskIntegration
+- `@logged_in`
+- `@autologin`
+- `@autologout`
+- `@login_autoexchange` **DEPRECATED**
+- `@login_code` **DEPRECATED**
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `cardboard.py-0.0.8/README.md` & `cardboard.py-0.0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 Initialize the Cardboard or CardboardAsync class. Make sure to pass `secret` and `client_id`.
 
 You can now use the client to make requests.
 
 ### Examples
 These examples will use Flask. Install it with `pip install Flask`
 
+Flask is included with `cardboard.py>=0.0.8`
+
 ```python
 # Python Example
 from flask import Flask, request, redirect, url_for, session, Response
 from cardboard import Cardboard
 
 app = Flask(__name__)
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
@@ -45,14 +47,29 @@
 def dashboard():
     token = session.get('cardboard_token')
     if not token:
         return redirect(cb.app_url)
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+def logout():
+    b = session.pop('cardboard_token', None)
+    if b:
+        try:
+            cb.revoke_token(b)
+        except:
+            pass
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ```python
 # Python Example using FlaskIntegration
 from flask import Flask, request, redirect, url_for, session, Response
@@ -62,38 +79,43 @@
 app.secret_key = 'hi' # set this to something secure, please.
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
 cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
 
 @app.route('/login')
 @cb.fi.autologin
 def login(token):
-    session['cardboard_token'] = token.token
     return redirect(url_for('dashboard'))
 
 @app.route('/dashboard')
-@cb.fi.logged_in('cardboard_token', check=True)
-def dashboard(token:str):
-    # v = cb.check_token(token)
-    # if not v:
-    #     return redirect(cb.app_url)
-    # uncomment above code if check=False
-    user = cb.get_user(token)
+@cb.fi.logged_in
+def dashboard(token):
+    user = cb.get_user(token.token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+@cb.fi.autologout
+def logout():
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
-For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
+For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b014-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
 A list of methods/attributes you can call with either Cardboard or CardboardAsync.
 - `.app_url` (str)
 - `.app_name` (str)
@@ -142,10 +164,18 @@
     - `.moderationStatus` (str|None)
     - `.aboutInfo` (class userAbout)
         - `.bio` (str|None)
         - `.tagline` (str|None)
         - `._raw` (dict)
     - `.userTransientStatus` (str|None)
     - `._raw` (dict)
+- `.check_token(token:str)` (bool)
+
+### FlaskIntegration
+- `@logged_in`
+- `@autologin`
+- `@autologout`
+- `@login_autoexchange` **DEPRECATED**
+- `@login_code` **DEPRECATED**
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `cardboard.py-0.0.8/cardboard/Exceptions.py` & `cardboard.py-0.0.9/cardboard/Exceptions.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.8/cardboard/cardboard.py` & `cardboard.py-0.0.9/cardboard/cardboard.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.8/cardboard/cardboard_async.py` & `cardboard.py-0.0.9/cardboard/cardboard_async.py`

 * *Files identical despite different names*

### Comparing `cardboard.py-0.0.8/cardboard.py.egg-info/PKG-INFO` & `cardboard.py-0.0.9/cardboard.py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardboard.py
-Version: 0.0.8
+Version: 0.0.9
 Summary: API wrapper for https://cardboard.ink/api/v1/
 Home-page: https://github.com/cardboard-ink/cardboard.py/
 Author: YumYummity
 Author-email: 034nop@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,14 +35,16 @@
 Initialize the Cardboard or CardboardAsync class. Make sure to pass `secret` and `client_id`.
 
 You can now use the client to make requests.
 
 ### Examples
 These examples will use Flask. Install it with `pip install Flask`
 
+Flask is included with `cardboard.py>=0.0.8`
+
 ```python
 # Python Example
 from flask import Flask, request, redirect, url_for, session, Response
 from cardboard import Cardboard
 
 app = Flask(__name__)
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
@@ -65,14 +67,29 @@
 def dashboard():
     token = session.get('cardboard_token')
     if not token:
         return redirect(cb.app_url)
     user = cb.get_user(token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+def logout():
+    b = session.pop('cardboard_token', None)
+    if b:
+        try:
+            cb.revoke_token(b)
+        except:
+            pass
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ```python
 # Python Example using FlaskIntegration
 from flask import Flask, request, redirect, url_for, session, Response
@@ -82,38 +99,43 @@
 app.secret_key = 'hi' # set this to something secure, please.
 cb = Cardboard(client_id='', secret='') # get these at https://cardboard.ink
 cb.fi = FlaskIntegration(app=app, cardboard=cb) # make this class ONLY AFTER YOU SET A SECRET KEY for FLASK.
 
 @app.route('/login')
 @cb.fi.autologin
 def login(token):
-    session['cardboard_token'] = token.token
     return redirect(url_for('dashboard'))
 
 @app.route('/dashboard')
-@cb.fi.logged_in('cardboard_token', check=True)
-def dashboard(token:str):
-    # v = cb.check_token(token)
-    # if not v:
-    #     return redirect(cb.app_url)
-    # uncomment above code if check=False
-    user = cb.get_user(token)
+@cb.fi.logged_in
+def dashboard(token):
+    user = cb.get_user(token.token)
     return Response(f'{user.name} (user id {user.id})', mimetype='text/plain')
 
+@app.route('/')
+def home():
+    html = f'<html><head><title>Button Redirect</title></head><body><button onclick="window.location.href=\'{url_for("login")}\';">Login</button></body></html>'
+    return Response(html, mimetype='text/html')
+
+@app.route('/logout')
+@cb.fi.autologout
+def logout():
+    return redirect(url_for('home'))
+
 if __name__ == '__main__':
     app.run('0.0.0.0', port=5000)
 ```
 
 ### Async Example
 ```python
 # Python Async Example
 ```
 
 # Documentation
-For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b01-0fcaeaf062d3/docs/374610
+For detailed documentation on the Cardboard API, read https://www.guilded.gg/CardBoard/groups/3y446Rmz/channels/4539a4f9-fb51-4a23-b014-0fcaeaf062d3/docs/374610
 
 For detailed documentation on how to use the cardboard.py library, please wait while we write it lol.
 
 ### Methods
 A list of methods/attributes you can call with either Cardboard or CardboardAsync.
 - `.app_url` (str)
 - `.app_name` (str)
@@ -162,10 +184,18 @@
     - `.moderationStatus` (str|None)
     - `.aboutInfo` (class userAbout)
         - `.bio` (str|None)
         - `.tagline` (str|None)
         - `._raw` (dict)
     - `.userTransientStatus` (str|None)
     - `._raw` (dict)
+- `.check_token(token:str)` (bool)
+
+### FlaskIntegration
+- `@logged_in`
+- `@autologin`
+- `@autologout`
+- `@login_autoexchange` **DEPRECATED**
+- `@login_code` **DEPRECATED**
 
 # License
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `cardboard.py-0.0.8/setup.py` & `cardboard.py-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='cardboard.py',
-    version='0.0.8',
+    version='0.0.9',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://cardboard.ink/api/v1/',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cardboard-ink/cardboard.py/',
     packages=find_packages(),
```

