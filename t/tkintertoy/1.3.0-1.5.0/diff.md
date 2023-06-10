# Comparing `tmp/tkintertoy-1.3.0.tar.gz` & `tmp/tkintertoy-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tkintertoy-1.3.0.tar", last modified: Mon May 11 22:10:49 2020, max compression
+gzip compressed data, was "tkintertoy-1.5.0.tar", last modified: Sat Jun 10 18:15:05 2023, max compression
```

## Comparing `tkintertoy-1.3.0.tar` & `tkintertoy-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2020-05-11 22:10:49.096454 tkintertoy-1.3.0/
--rw-rw-rw-   0        0        0     2877 2020-05-11 22:10:49.094461 tkintertoy-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2019-03-16 20:10:22.000000 tkintertoy-1.3.0/README.md
--rw-rw-rw-   0        0        0       42 2020-05-11 22:10:49.098448 tkintertoy-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      907 2020-05-11 21:36:49.000000 tkintertoy-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-05-11 22:10:49.049585 tkintertoy-1.3.0/tkintertoy/
--rw-rw-rw-   0        0        0       32 2019-02-19 20:11:05.000000 tkintertoy-1.3.0/tkintertoy/__init__.py
--rw-rw-rw-   0        0        0    72045 2020-05-04 02:31:00.000000 tkintertoy-1.3.0/tkintertoy/tt.py
--rw-rw-rw-   0        0        0    10089 2020-05-11 21:49:27.000000 tkintertoy-1.3.0/tkintertoy/ttgallery.py
-drwxrwxrwx   0        0        0        0 2020-05-11 22:10:49.087476 tkintertoy-1.3.0/tkintertoy.egg-info/
--rw-rw-rw-   0        0        0     2877 2020-05-11 22:10:47.000000 tkintertoy-1.3.0/tkintertoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2020-05-11 22:10:47.000000 tkintertoy-1.3.0/tkintertoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-05-11 22:10:47.000000 tkintertoy-1.3.0/tkintertoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2020-05-11 22:10:47.000000 tkintertoy-1.3.0/tkintertoy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/
+-rw-rw-rw-   0        0        0     1080 2020-01-12 00:42:26.000000 tkintertoy-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2522 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2023-05-08 23:33:42.000000 tkintertoy-1.5.0/README.md
+-rw-rw-rw-   0        0        0      857 2023-06-10 18:06:12.000000 tkintertoy-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.926439 tkintertoy-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/src/tkintertoy/
+-rw-rw-rw-   0        0        0  2190126 2019-07-15 23:19:56.000000 tkintertoy-1.5.0/src/tkintertoy/Shipman_tkinter8_5.pdf
+-rw-rw-rw-   0        0        0       32 2019-02-19 20:11:06.000000 tkintertoy-1.5.0/src/tkintertoy/__init__.py
+-rw-rw-rw-   0        0        0    73560 2023-06-04 18:20:58.000000 tkintertoy-1.5.0/src/tkintertoy/tt.py
+-rw-rw-rw-   0        0        0    13129 2023-06-04 02:15:07.000000 tkintertoy-1.5.0/src/tkintertoy/ttgallery.py
+drwxrwxrwx   0        0        0        0 2023-06-10 18:15:05.973339 tkintertoy-1.5.0/src/tkintertoy.egg-info/
+-rw-rw-rw-   0        0        0     2522 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-10 18:15:05.000000 tkintertoy-1.5.0/src/tkintertoy.egg-info/top_level.txt
```

### Comparing `tkintertoy-1.3.0/PKG-INFO` & `tkintertoy-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 Metadata-Version: 2.1
 Name: tkintertoy
-Version: 1.3.0
+Version: 1.5.0
 Summary: A simple GUI package based on Tkinter
-Home-page: https://github.com/mcalla314/tkintertoy
-Author: Mike Callahan
-Author-email: mcalla@twc.com
-License: UNKNOWN
+Author-email: Mike Callahan <mcalla@twc.com>
+Project-URL: Homepage, https://github.com/mcalla314/tkintertoy
 Project-URL: Documentation, https://tkintertoy.readthedocs.io
-Description: # Tkintertoy
-        
-        Tkintertoy was designed to be a easy to use GUI library based on Tkinter.
-        It was intended for "young" (as in experience) programmers to develop GUIs
-        with as little trouble as possible. However, more "advanced" programmers can
-        reach the more complex features of Tkinter easily. Here is a short example:
-        
-            from tkintertoy import Window
-            # create the window
-            gui = Window()
-            gui.setTitle('My First Tkintertoy GUI!')
-            # add the widgets
-            gui.addEntry('name', 'Type in your name')
-            gui.addLabel('welcome', 'Welcome message')
-            gui.addButton('commands')
-            # plot the widgets
-            gui.plot('name', row=0)
-            gui.plot('welcome', row=1)
-            gui.plot('commands', row=2, pady=10)
-            # start the event processing loop
-            while True:
-                gui.waitforUser()
-                if gui.content:
-                    gui.set('welcome', 'Welcome ' + gui.get('name'))
-                else:
-                    break
-            
-        This code will create a small window with an entry, label, and command button
-        widgets. The application will wait for the user to type in their first name.
-        After typing it in, and clicking on Ok, the application will display a welcome
-        label. The user exits the code by clicking on Cancel.
-        
-        ![Simple GUI](http://tkintertoy.readthedocs.io/en/latest/_images/first.png)
-        
-        As you can see in orgder to create a simple GUI, you create a window, add widgets,
-        plot the widgets in the desired location, and then call waitforUser.
-        
-        While Tkintertoy was designed to be an GUI library for simple interfaces it
-        has been used in more complex code as well. 
-        
-        Using Tkintertoy, it is hoped that Python instructors can quickly move students
-        from boring command-line applications to useful standard GUIs. A tutorial with
-        many useful examples in included with the documentation.
-            
-            
-        
-Keywords: GUI,Tkinter
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Keywords: GUI,novice
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: User Interfaces
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Tkintertoy
+
+Tkintertoy was designed to be a easy to use GUI library based on Tkinter.
+It was intended for novice programmers to develop GUIs with as little
+trouble as possible. However, more "advanced" programmers can reach the
+more complex features of Tkinter easily. Here is a short example:
+
+    from tkintertoy import Window
+    # create the window
+    gui = Window()
+    gui.setTitle('My First Tkintertoy GUI!')
+    # add the widgets
+    gui.addEntry('name', 'Type in your name')
+    gui.addLabel('welcome', 'Welcome message')
+    gui.addButton('commands')
+    # plot the widgets
+    gui.plot('name', row=0)
+    gui.plot('welcome', row=1)
+    gui.plot('commands', row=2, pady=10)
+    # start the event processing loop
+    while True:
+        gui.waitforUser()
+        if gui.content:
+            gui.set('welcome', 'Welcome ' + gui.get('name'))
+        else:
+            break
+    
+This code will create a small window with an entry, label, and command button
+widgets. The application will wait for the user to type in their first name.
+After typing it in, and clicking on Ok, the application will display a welcome
+label. The user exits the code by clicking on Cancel.
+
+![Simple GUI](http://tkintertoy.readthedocs.io/en/latest/_images/first.png)
+
+As you can see in order to create a simple GUI, you create a window, add widgets,
+plot the widgets in the desired location, and then call waitforUser.
+
+While Tkintertoy was designed to be an GUI library for simple interfaces it
+has been used in more complex code as well. 
+
+Using Tkintertoy, it is hoped that Python instructors can quickly move students
+from boring command-line applications to standard GUIs. A tutorial with many
+useful examples in included with the documentation. Also included with the source
+is John Shipman's Tkinter 8.5 Reference PDF.
+    
+
```

### Comparing `tkintertoy-1.3.0/README.md` & `tkintertoy-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tkintertoy
 
 Tkintertoy was designed to be a easy to use GUI library based on Tkinter.
-It was intended for "young" (as in experience) programmers to develop GUIs
-with as little trouble as possible. However, more "advanced" programmers can
-reach the more complex features of Tkinter easily. Here is a short example:
+It was intended for novice programmers to develop GUIs with as little
+trouble as possible. However, more "advanced" programmers can reach the
+more complex features of Tkinter easily. Here is a short example:
 
     from tkintertoy import Window
     # create the window
     gui = Window()
     gui.setTitle('My First Tkintertoy GUI!')
     # add the widgets
     gui.addEntry('name', 'Type in your name')
@@ -28,18 +28,19 @@
 This code will create a small window with an entry, label, and command button
 widgets. The application will wait for the user to type in their first name.
 After typing it in, and clicking on Ok, the application will display a welcome
 label. The user exits the code by clicking on Cancel.
 
 ![Simple GUI](http://tkintertoy.readthedocs.io/en/latest/_images/first.png)
 
-As you can see in orgder to create a simple GUI, you create a window, add widgets,
+As you can see in order to create a simple GUI, you create a window, add widgets,
 plot the widgets in the desired location, and then call waitforUser.
 
 While Tkintertoy was designed to be an GUI library for simple interfaces it
 has been used in more complex code as well. 
 
 Using Tkintertoy, it is hoped that Python instructors can quickly move students
-from boring command-line applications to useful standard GUIs. A tutorial with
-many useful examples in included with the documentation.
+from boring command-line applications to standard GUIs. A tutorial with many
+useful examples in included with the documentation. Also included with the source
+is John Shipman's Tkinter 8.5 Reference PDF.
```

### Comparing `tkintertoy-1.3.0/tkintertoy/tt.py` & `tkintertoy-1.5.0/src/tkintertoy/tt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,105 +1,126 @@
-# Name:         tkintertoy.py - Mike Callahan - Python 2.7 or at least 3.4
+# Name:         tkintertoy.py - Mike Callahan - Python 3.4 or later
 # Purpose:      Makes it easier to create tk/ttk guis
 #
 # Author:       Mike Callahan
 #
-# Created:      5/3/2020
-# Copyright:    (c) mike.callahan 2019, 2020
+# Created:      6/4/2023
+# Copyright:    (c) mike.callahan 2019 - 2023
 # License:      MIT
 #
 # History:
 # 1.00 - initial version
 # 1.01-1.04 - update comments for autodoc
 # 1.10 - make prompt second parameter for most methods, add popup
 #        open, saveas, choosedir
 # 1.20 - add changeWidget, changeState, fix cancel, improve documentation,
 #        remove time and sys imports
 # 1.30 - add return to most widgets, add usettk option to ttk widgets,
 #        fix __repr__
+# 1.31 - fix addButton, addCanvas
+# 1.40 - remove Python 2 support, add scrollbar option to addCanvas,
+#        add tk & ttk class variable, clean up code in many functions
+# 1.41 - fix vertical alignment to addCheck and addRadio, add reset,
+#        fix changeState, rename change* to set*
+# 1.42 - fix __init__, clean up comments
+# 1.50 - fix get for ledger & collector, fix get & set for spin
 ###################################################################
 
-try:
-    import Tkinter as tk                               # support Python 2
-    import ttk, warnings, tkFont as tkfont
-    from tkFileDialog import *
-    from tkMessageBox import *
-    from tkColorChooser import *
-except ImportError:
-    import tkinter as tk                               # support Python 3
-    import tkinter.ttk as ttk, warnings, tkinter.font as tkfont
-    from tkinter.filedialog import *
-    from tkinter.messagebox import *
-    from tkinter.colorchooser import *
+import tkinter as tk                               # support only Python 3
+import tkinter.ttk as ttk, warnings, tkinter.font as tkfont
+from tkinter.filedialog import *
+from tkinter.messagebox import *
+from tkinter.colorchooser import *
 
 
-class Window(object):
-    """ An easy GUI creator intended for early Python programmers, built upon
+class Window:
+    """ An easy GUI creator intended for novice Python programmers, built upon
     Tkinter.
 
     This will create a Tk window with a contents dictionary. The programmer
-    adds "ttwidgets" to the window using the add* methods where the programmer
-    assigns a string tag to a widget. Almost all ttk and most tk widgets are included
-    including some useful combined widgets. I call these ttwidgets because they are
-    not really complex enough to be called "megawidgets". Most tk/ttk widgets are
-    placed in a frame which can act as a label of the ttwidget to the user. The
-    programmer places the ttwidgets using the plot method which is a synonym for
-    the tkinter grid geometry manager. Contents of the widget are assigned and
-    retrieved by using the tags to the set and get methods. This greatly simplifies
-    working with GUIs. Also, all ttwidgets are bundled into the window object so
-    individual ttwidgets do not need to be passed to other routines, which simplifies
-    interfaces. However, more experienced Python programmers can access the tk/ttk
-    widget and frames directly and take advantage of the full power of Tk and ttk.
+    adds "ttWidgets" to the window using the add* methods where the programmer
+    assigns a string tag to a widget. Almost all ttk and most tk widgets are included,
+    with some useful combined widgets. Most tk/ttk widgets are placed in a frame which
+    can act as a prompt of the ttWidget to the user. The programmer places the ttWidgets
+    using the plot method which is a synonym for the tkinter grid geometry manager.
+    Contents of the widget are assigned and retrieved by using the tags to the set and
+    get methods. This greatly simplifies working with GUIs. Also, all ttWidgets are
+    bundled into the window object so individual ttWidgets do not need to be passed
+    to other routines, which simplifies interfaces. However, more experienced Python
+    programmers can access the tk/ttk widget and frames directly and take advantage
+    of the full power of Tk and ttk.
 
     In the below methods, not all the possible keyword arguments are listed, only
-    the most common ones were selected. The Tk documentation lists all for every
+    the most common ones were selected. The Tkinter documentation lists all for every
     widget. However, tk control variables should NOT be used since they might
     interfere on how the set and get methods work. Default values are shown in
     brackets [].
 
     In some themes, certain parameters (like background) will not work in ttk
     widgets. For this reason, all ttk widgets have an option to use the older
-    tk widget by setting the usetk argument to True. 
+    tk widget by setting the usetk argument to True.
+
+    Due to problems with textvariable in nested frames with ttk, the textvariable
+    option is not used in any of the below methods.
+
+    After creating a Window object, the master attribute will either be a Tk
+    Frame or a Toplevel window.
+
+    Here is a summary of the methods:
+        add* - add a new ttWidget to a window
+        get* - get the contents or an part of the ttWidget
+        set* - change the contents or an attribute of the widget
+        pop* - pop-up a dialog window
 
     Parameters:
-        master (tk.Toplevel): Toplevel window
+        master (tk.Toplevel or tk.Frame): The containing window
         extra (bool): True if this is an extra window apart from the main
 
     Keyword Arguments:
         borderwidth (int): Width of border (pixels)
         height (int): Height of frame (pixels)
         padding (int): Spaces between frame and widgets (pixels)
         relief (str): ['flat'],'raised','sunken','groove', or 'ridge'
         style (ttk.Style): Style used for ttk.Frame or ttk.LabelFrame
         width (int): Width of frame (pixels)
+
+    Included in the installation is a copy of John Shipman's "Tkinter 8.5 reference:
+    a GUI for Python" from New Mexico Tech, which is the best printed version known
+    to the author. Unfortunately, Dr. Shipman has passed away and it is getting harder
+    to find. When the code references Tkinter documentation it is referring to Dr.
+    Shipman's work.
     """
 
-    ver = 1.30                                                # version number
+    # class variables
+
+    VERSION = '1.50'                                              # version number
+        
     # basic class methods
 
     def __init__(self, master=None, extra=False, **tkparms):
         """ Set-up window and create content dictionary
 
         This creates the window and the content dictionary that all the methods
         use. This is always the first step. This method is called automatically
         for containers.
         """
 
         if not master:
             if not extra:
-                self.master = tk.Tk(**tkparms)         # first window
+                self.master = tk.Tk()                         # first window
+                self.master.configure(**tkparms)              # tk.Tk() doesn't accept **tkparm
             else:
-                self.master = tk.Toplevel(**tkparms)   # extra window
-            topwin = self.master.winfo_toplevel()      # get topwindow info
-            if 'destroy' in topwin.protocol(name='WM_DELETE_WINDOW'):  # set close window to cancel
-                topwin.protocol(name='WM_DELETE_WINDOW', func=self.cancel)
+                self.master = tk.Toplevel(**tkparms)          # extra window
+            self.topwin = self.master.winfo_toplevel()        # get topwindow info
+            if 'destroy' in self.topwin.protocol(name='WM_DELETE_WINDOW'):  # set close window to cancel
+                self.topwin.protocol(name='WM_DELETE_WINDOW', func=self.cancel)
         else:
             self.master = master
-        self.content = dict()                          # create the content dict
-        self.style = ttk.Style()                       # access Style database
+        self.content = dict()                                 # create the content dict
+        self.style = ttk.Style()                              # access Style database
 
     def __repr__(self):
         """ Display content dictionary structure, useful for debugging.
 
         Called using the builtin repr() function.
 
         Returns:
@@ -113,15 +134,15 @@
                 temp += "  '{}':\n    ".format(widget)
                 temp += "{{'frame':{},\n    ".format(repr(self.content[widget]['frame']))
                 temp += "'type':{},\n    ".format(self.content[widget]['type'])
                 temp += "'widget':{},\n    ".format(repr(self.content[widget]['widget']))
                 temp += "'value':{}}}\n".format(self.get(widget))
             except KeyError:
                 pass
-        return temp+'  }'
+        return temp+'  }\n'
 
     def __len__(self):
         """ Return number of widgets in window.
 
         Called using the builtin len() function.
 
         Returns:
@@ -152,20 +173,19 @@
         Parameters:
             prompt (str): The title of the window
         """
 
         self.master.title(prompt)
 
     def addLabel(self, tag, prompt='', effects='', usetk=False, **tkpamrs):
-        """ Create a ttlabel.
+        """ Create a ttLabel.
 
-        Labels are used to display simple messages to the user. Due to problems
-        with textvariable in nested frames with ttk, the textvariable is not used.
-        An effects parameter is included for the simplest font types but this
-        will override the font keyword argument. Get/set uses str.
+        Labels are used to display simple messages to the user. An effects parameter
+        is included for the simplest font types but this will override the font
+        keyword argument. Get/set uses str.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             effects (str): 'bold' and/or 'italic'
             usetk (bool): Use tk instead of ttk
 
@@ -179,15 +199,15 @@
             justify (str): Justification of text; ['left'], 'right', 'center'
             padding (list): Spacing (left, top, right, bottom) around widget (pixels)
             text (str): The text inside the widget
             width (int): Width of label (chars)
             wraplength (int): Character position to word wrap
 
         Returns:
-            ttk/tk.label 
+            ttk/tk.Label
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'label'}          # init content to tk var
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
@@ -203,42 +223,42 @@
             label['font'] = font                       # use it
         label.grid()                                   # widgets are gridded automatically
         self.content[tag]['frame'] = frame             # allow access to frame
         self.content[tag]['widget'] = label            # allow access to widget
         return label
 
     def addLine(self, tag, **tkparms):
-        """ Create a horizontal or vertical ttline across the entire frame.
+        """ Create a horizontal or vertical ttLine across the entire frame.
 
         Lines are useful for visually separating areas of widgets. They have no
-        frame. There is no tk version.
+        frame. There is no tk version. Be sure to use the sticky keyword when
+        plotting or it will be a single dot.
 
         Parameters:
             tag (str): Reference to widget
             
         Keyword Arguments:
             orient (str): ['horizontal'] or 'vertical'
             style (ttk.Style): Style to use for line
 
         Returns:
-            ttk.separator 
+            ttk.Separator
         """
 
         self.content[tag] = {'type': 'line'}
         line = ttk.Separator(self.master, **tkparms)  # create line
         self.content[tag]['widget'] = line
         return line
 
     def addMessage(self, tag, prompt, **tkparms):
-        """ Create a ttmessage which is like multiline label.
+        """ Create a ttMessage which is like multiline label.
 
         Messages are used to display multiline messages to the user. This is a
-        tk widget so the list of options is extensive. Due to problems with
-        textvariables in nested ttk windows, they are not used. This widget's
-        behavior is a little strange so you might prefer the Text or Label widgets.
+        tk widget so the list of options is extensive. This widget's behavior
+        is a little strange so you might prefer the Text or Label widgets.
         Get/set uses str.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
 
         Keyword Arguments:
@@ -251,48 +271,47 @@
             padx (int): Horizontal spaces to place around widget (pixels)
             pady (int): Vertical spaces to place around widget (pixels)
             relief (str): 'flat','raised','sunken','groove', or 'ridge'
             text (str): The text inside the widget
             width (int): Width of message (pixels)
 
         Returns:
-            tk.message
+            tk.Message
         """
 
         self.content[tag] = {'type': 'message'}         # init content to tk var
         if prompt:
             frame = tk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = tk.Frame(self.master)             # no title
         message = tk.Message(frame, **tkparms)         # create entry
         message.grid()
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = message
         return message
 
     def addEntry(self, tag, prompt='', usetk=False, **tkparms):
-        """ Create an ttentry.
+        """ Create an ttEntry.
 
-        Entries are the widget to get string input from the user. Due to problems
-        with textvariables in nested frames with ttk, they are not used. Get/set
+        Entries are the widget to get string input from the user. Get/set
         uses str.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             usetk (bool): Use tk instead of ttk
 
         Keyword Arguments:
             justify (str): Justification of text ('left' [def], 'right', 'center')
             show (str): Char to display instead of actual text
             style (ttk.Style): Style to use for widget
             width (int): Width of label [20] (chars)
 
         Returns:
-            ttk/tk.entry
+            ttk/tk.Entry
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'entry', 'value': tk.StringVar()} # init content to tk var
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt) # create titled frame
         else:
@@ -300,20 +319,20 @@
         entry = t.Entry(frame, **tkparms)            # create entry
         entry.grid()
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = entry
         return entry
 
     def addList(self, tag, prompt='', alist=[], **tkparms):
-        """ Create a ttlistbox.
+        """ Create a ttListbox.
 
-        Listboxes allow the user to select a series of options in a vertical list.
-        It is best for long titled options but does take up some screen space. This
-        implementation avoids the listvariable. Since this is a Tk widget, there
-        is no style keyword argument. Get/set uses list of str.
+        Lists allow the user to select a series of options in a vertical list.
+        It is best for long titled options but does take up some screen space.
+        Since this is a Tk widget, there is no style keyword argument. Get/set
+        uses list of str.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             alist (list): (str1, str2, ...)
 
         Keyword Arguments:
@@ -343,20 +362,19 @@
         for i in range(0, len(alist), 2):
             listbox.itemconfigure(i, background='#f0f0ff')  # color alt backgrounds
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = listbox
         return listbox
 
     def addCombo(self, tag, prompt='', values=None, **tkparms):
-        """ Create a ttcombobox.
+        """ Create a ttCombobox.
 
         Comboboxes combine features of Entry and Listbox into a single widget. The
         user can select one option out of the list or even type in their own. It is
-        better than listboxes for a large number of options. Due to problems with
-        textvariable in nested frames with ttk, they are not used. Get/set uses
+        better than lists for a large number of options. Get/set uses str or list of
         str. There is no tk version.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             values (list): (str1, str2, ...)
 
@@ -364,30 +382,30 @@
             height (int): Maximum number of rows in dropdown [10]
             justify (str): Justification of text (['left'], 'right', 'center')
             postcommand (callback): Function to call when user clicks on downarrow
             style (ttk.Style): Style to use for widget
             width (int): Width of label (chars) [20]
 
         Returns:
-            ttk.combobox 
+            ttk.Combobox
         """
 
         self.content[tag] = {'type': 'combo'}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
         combobox = ttk.Combobox(frame, values=values, **tkparms)  # create combobox
         combobox.grid()
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = combobox
         return combobox
 
     def addCheck(self, tag, prompt='', alist=[], orient='horizontal', usetk=False, **tkparms):
-        """ Create a ttcheckbutton box.
+        """ Create a ttCheckbutton box.
 
         Checkboxes are used to collect options from the user, similar to a listbox.
         Checkboxes might be better for short titled options because they don't take
         up as much screen space. The keyword arguments will apply to EVERY checkbutton.
         Get/set uses list of str.
 
         Parameters:
@@ -401,15 +419,15 @@
             command (callback): Function to execute when boxes are toggled
             compound (str): Display both image and text, see ttk docs
             image (tk.PhotoImage): GIF image to display
             style (ttk.Style): Style to use for checkboxes
             width (int): Width of max checkbox label (chars), negative sets minimum
 
         Returns:
-            [ttk/tk.checkbuttons]  
+            list of ttk/tk.Checkbuttons
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'check'}          # init content to dict
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
@@ -420,22 +438,22 @@
             temp = tk.BooleanVar()                     # create the booleanvar
             cvalues.append(temp)                       # set boolean into content
             checkbutton = t.Checkbutton(frame, variable=temp, text=item, **tkparms)  # create checkbutton
             cbuttons.append(checkbutton)               # add checkbutton to list
             if orient == 'horizontal':
                 checkbutton.grid(row=0, column=n)      # grid it horizontally
             else:
-                checkbutton.grid(row=n, column=0)      # grid it vertically
+                checkbutton.grid(row=n, column=0, sticky='w') # grid it vertically
         self.content[tag]['frame'] = frame
         self.content[tag]['value'] = cvalues
         self.content[tag]['widget'] = cbuttons
         return cbuttons
 
     def addRadio(self, tag, prompt='', alist=[], orient='horizontal', usetk=False, **tkparms):
-        """ Create a ttradiobutton box.
+        """ Create a ttRadiobutton box.
 
         Radiobuttons allow the user to select only one option. If they change options,
         the previous option is unselected. This was the way old car radios worked
         hence its name. They are better for short titled options. The keyword
         arguments will apply to EVERY radiobutton. Get/set uses str.
 
         Parameters:
@@ -449,15 +467,15 @@
             command (callback): Function to execute when boxes are toggled
             compound (str): Display both image and text, see ttk docs
             image (tk.PhotoImage): GIF image to display
             style (ttk.Style): Style to use for checkboxes
             width (int): Width of max label (chars), negative sets minimun
 
         Returns:
-            [ttk/tk.radiobuttons] 
+            list of ttk/tk.Radiobuttons
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'radio', 'value': tk.StringVar()}  # init var to tk var
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
@@ -465,53 +483,54 @@
         rbuttons = []                                  # list for radiobuttons
         for n, item in enumerate(alist):               # for every item in the given list
             radiobutton = t.Radiobutton(frame, text=item,
                 variable=self.content[tag]['value'], value=item, **tkparms)  # create the radiobutton
             if orient == 'horizontal':
                 radiobutton.grid(row=0, column=n)      # grid it horizontally
             else:
-                radiobutton.grid(row=n, column=0)      # grid it vertically
+                radiobutton.grid(row=n, column=0, sticky='w')      # grid it vertically
             rbuttons.append(radiobutton)               # add it to list
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = rbuttons         # list of radio buttons
         return rbuttons
 
     def addOption(self, tag, prompt='', alist=[]):
-        """ Create an ttoptionmenu.
+        """ Create an ttOptionmenu.
 
         Option menus allow the user to select one fixed option, similar to
         Radiobutton. However, option menu returns a tk.Menu and is more difficult
         to manipulate. There are no keyword arguments in tk.OptionMenu. Get/set
         uses str.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             alist (list): (str1, str2, ...)
 
         Returns:
-            tk.optionmenu 
+            tk.OptionMenu
         """
 
         self.content[tag] = {'type': 'option', 'value': tk.StringVar()}  # init var to tk var
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
         option = tk.OptionMenu(frame, self.content[tag]['value'], *alist)  # create optionmenu
         option.grid()
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = option
         return option
 
-    def addScale(self, tag, parms, prompt='', width=20, usetk=False, **tkparms):
-        """ Create a ttscale which is an integer scale with entry box.
+    def addScale(self, tag, parms, prompt='', width=4, usetk=False, **tkparms):
+        """ Create a ttScale which is an integer scale with entry box.
 
         Scale allows the user to enter an integer value using a sliding scale. The
         user can also type in a value directly in the entry box. Get/set uses int.
+        The tk widget has many more options
 
         Parameters:
             tag (str): Reference to widget
             parms (list): Limits of scale (from, to)
             prompt (str): Text of frame label
             width (int): Width of entry widget (chars)
             usetk (bool): Use tk instead of ttk
@@ -519,41 +538,41 @@
         Keyword Arguments:
             command (callback): Function to call when scale changes
             length (int): Length of scale (pixels) [100]
             orient (str): 'horizontal' or 'vertical'
             style (str): Style to use for ttk.Scale
 
         Returns:
-            list(ttk/tk.scale, ttk/tk.entry)  
+            list of ttk/tk.Scale and ttk/tk.Entry
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'scale', 'value': tk.IntVar()}
         xfrom, to = parms
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = t.Frame(self.master)             # no title
         scale = t.Scale(frame, from_=xfrom, to=to, variable=self.content[tag]['value'],
             command=lambda x: self.content[tag]['value'].set(int(float(x))), **tkparms)  # create scale
         # the lambda causes the values to always be integers
-        entry = t.Entry(frame, width=width, textvariable=self.content[tag]['value'])  # create entry
+        entry = t.Entry(frame, textvariable=self.content[tag]['value'], width=width)  # create entry
         scale.grid(row=0, column=0)
         entry.grid(row=0, column=1, padx=3)
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = [scale, entry]
         return [scale, entry]
 
-    def addSpin(self, tag, parms, between='', prompt='', usetk=False, **tkparms):
-        """ Create a ttspinbox.
+    def addSpin(self, tag, parms, between=' ', prompt='', usetk=False, **tkparms):
+        """ Create a ttSpinbox.
 
         Spinboxes allow the user to enter a series of integers. It is best used
         for items like dates, time, etc. The keyword arguments will apply to EVERY
         spinbox. Since this is a Tk widget, there is no style keyword argument.
-        Get/set uses list of int.
+        Get/set uses str.
 
         Parameters:
             tag (str): Reference to widget
             parms (list): Parmeters for each spinbox ((width, from, to),...)
             between (str): Label between each box
             prompt (str): Text of frame label
             usetk (bool): Use tk instead of ttk
@@ -561,23 +580,24 @@
         Keyword Arguments:
             command (callback): Function to call when arrows are clicked
             style (ttk.Style): Style to use for widget
             justify (str): Text justification; ['left'], 'right', 'center'
             wrap (bool): Arrow clicks wrap around
 
         Returns:
-            list(ttk/tk.spinboxes) 
+            list of ttk/tk.Spinboxes
         """
 
         t = tk if usetk else ttk   
-        self.content[tag] = {'type': 'spin', 'value': []}  # data is list
+        self.content[tag] = {'type': 'spin', 'value': []}  # data is list###
+        self.content[tag]['between'] = between             # save the between str
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
-            frame = t.Frame(self.master)             # no title
+            frame = t.Frame(self.master)               # no title
         col = 0                                        # set col
         spins = []
         for parm in parms:
             width, xfrom, to = parm                    # extract spinbox parms
             self.content[tag]['value'].append(tk.IntVar())  # add tkvar to list
             spin = t.Spinbox(frame, width=width, from_=xfrom, to=to,
                 textvariable=self.content[tag]['value'][col//2], **tkparms)  # create spinbox
@@ -587,51 +607,51 @@
             label.grid(row=0, column=col+1)            # grid the it
             col += 2
         label.destroy()                                # remove last between str
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = spins
         return spins                                   # list of spinboxes
 
-    def addProgress(self, tag, length, prompt='', orient='horizontal', **tkparms):
-        """ Create a ttprogressbar.
+    def addProgress(self, tag, prompt='', **tkparms):
+        """ Create a ttProgressbar.
 
         This indicates to the user how an action is progressing. The included method
         supports a determinate mode where the programmer tells the user exactly how
         far they have progressed. Ttk also supports a indeterminate mode where a rectangle
-        bounces back a forth. See the Tk documentation. Get/set uses int. There is no
+        bounces back a forth. See the Tkinter documentation. Get/set uses int. There is no
         tk version.
 
         Parameters:
             tag (str): Reference to widget
-            length (int): Length of widget (pixels)
             prompt (str): Text of frame label
-            orient (str): 'horizontal' or 'vertical'
-            
+                        
         Keyword Arguments:
             maximum (int): Maximum value [100]
             mode (str): ['determinate'] or 'indeterminate'
             style (str): Style to use for ttk.Progressbar
+            length (int): Length of widget (pixels)
+            orient (str): 'horizontal' or 'vertical'
 
         Returns:
-            ttk.progressbar 
+            ttk.Progressbar
         """
 
         self.content[tag] = {'type': 'progress', 'value': tk.IntVar()}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
-        progress = ttk.Progressbar(frame, length=length, orient=orient, variable=self.content[tag]['value'], **tkparms)
+        progress = ttk.Progressbar(frame, variable=self.content[tag]['value'], **tkparms)
         progress.grid()
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = progress
         return progress
 
     def addButton(self, tag, prompt='', cmd=[], space=3, orient='horizontal', usetk=False, **tkparms):
-        """ Create a ttbuttonbox, defaults to Ok - Cancel.
+        """ Create a ttButtonbox, defaults to Ok - Cancel.
 
         This widget is where one would place most of the command buttons for a GUI,
         usually at the bottom of the window. Clicking on a button will execute a
         method usually called a callback. Two basic ones are included; Ok and
         Cancel. The keyword arguments will apply to EVERY button.
 
         Parameters:
@@ -645,151 +665,156 @@
         Keyword Arguments:
             compound (str): Display both image and text, see ttk docs
             image (tk.PhotoImage): GIF/PNG image to display
             style (ttk.Style): Style to use for checkboxes
             width (int): Width of label (chars)
 
         Returns:
-            list(ttk/tk.buttons) 
+            list of ttk/tk.Buttons
         """
 
         t = tk if usetk else ttk 
         self.content[tag] = {'type': 'buttons'}
         if not cmd:                                    # use default buttons
             cmd = [['Ok', self.breakout], ['Cancel', self.cancel]]
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = t.Frame(self.master)             # no title
         buttons = []                                   # list for created buttons
         n = 0                                          # init counter
         for label, callback in cmd:
-            button = t.Button(frame, width=12, text=label,
+            button = t.Button(frame, text=label,
                 command=callback, **tkparms)             # create button
             if orient == 'horizontal':
                 button.grid(row=0, column=n, padx=space)  # grid it horizontally
                 n += 1
             else:
                 button.grid(row=n, column=0, pady=space)  # grid it vertically
                 n += 1
             buttons.append(button)
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = buttons           # list of buttons
         return buttons
 
-    def addText(self, tag, width, height, prompt='', **tkparms):
-        """ Create a tttext window.
+    def addText(self, tag, prompt='', **tkparms):
+        """ Create a ttText window.
 
         The tk.Text widget is an extremely powerful widget that can do many things,
         other than just displaying text. It is almost a mini editor. The default
         method allow the programmer to add and delete text. Be sure to read the
-        Tk documentation to discover all the features of this widget. Since this
+        Tkinter documentation to discover all the features of this widget. Since this
         is a Tk widget, there is no style keyword argument. Get/set uses str.
 
         Parameters:
             tag (str): Reference to widget
-            width (int): Width of window (chars)
-            height (int): Height of window (chars)
             prompt (str): Text of frame label
 
         Keyword Arguments:
             background (str): Background color
             font (tkfont.Font): Text font
             foreground (str): Text color
             wrap (str): Wordwrap method; ['char'], 'word', or 'none'
+            width (int): Width of window (chars)
+            height (int): Height of window (chars)
 
         Returns:
-            tk.text
+            tk.Text
         """
 
         self.content[tag] = {'type': 'text'}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
-        text = tk.Text(frame, width=width, height=height, **tkparms)  # create text widget
-        text.grid(row=0, sticky='wens')                # fill entire frame
+        text = tk.Text(frame, **tkparms)               # create text widget
+        text.grid(row=0, sticky='nsew')                # fill entire frame
         vbar = ttk.Scrollbar(frame)                    # create scrollbar
         text['yscrollcommand'] = vbar.set              # connect text to scrollbar
         vbar['command'] = text.yview                   # connect scrollbar to text
         if 'font' not in tkparms:
             text['font'] = ('Helvetica', '10')         # default font
-        vbar.grid(row=0, column=1, sticky='ns')        # grid scrollbar
+        vbar.grid(row=0, column=1, sticky='nse')        # grid scrollbar
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = text
         return text
 
-    def addCanvas(self, tag, width, height, prompt='', **tkparms):
-        """ Create a ttcanvas window.
+    def addCanvas(self, tag, prompt='', scrollbars=False, **tkparms):
+        """ Create a ttCanvas window.
 
         The tk.Canvas is another extremely powerful widget that displays graphics.
         Again, read the Tkinter documentation to discover all the features of this
         widget.
 
         Parameters:
             tag (str): Reference to widget
-            width (int): Width of window (pixels)
-            height (int): Height of window (pixels)
             prompt (str): Text of frame label
+            scrollbars (bool): True if scrollbars are added
 
         Keyword Arguments:
+            width (int): Width of window (pixels)
+            height (int): Height of window (pixels)
             background (str): Background color
             closeenough (float): Mouse threshold
             confine (bool): Canvas cannot be scrolled ourside scrolling region
             cursor (str): Mouse cursor
             scrollregion (list of int): w, n, e, s bondaries of scrolling region
 
         Returns:
-            tk.canvas 
+            tk.Canvas
         """
 
         self.content[tag] = {'type': 'canvas'}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
-        canvas = tk.Canvas(frame, width=width, height=height, **tkparms)  # create text widget
-        canvas.grid(row=0, sticky='wens')                # fill entire frame
-        vbar = ttk.Scrollbar(frame)                    # create scrollbar
-        canvas['yscrollcommand'] = vbar.set              # connect text to scrollbar
-        vbar['command'] = canvas.yview                   # connect scrollbar to text
-        vbar.grid(row=0, column=1, sticky='ns')        # grid scrollbar
-        hbar = ttk.Scrollbar(frame, orient='horizontal')  # create scrollbar
-        canvas['xscrollcommand'] = hbar.set              # connect text to scrollbar
-        hbar['command'] = canvas.xview                   # connect scrollbar to text
-        hbar.grid(row=1, column=0, sticky='we')        # grid scrollbar
+        canvas = tk.Canvas(frame, **tkparms)           # create canvas widget
+        canvas.grid(row=0, sticky='wens')              # fill entire frame
+        if scrollbars:
+            vbar = ttk.Scrollbar(frame)                    # create scrollbar
+            canvas['yscrollcommand'] = vbar.set            # connect text to scrollbar
+            vbar['command'] = canvas.yview                 # connect scrollbar to text
+            vbar.grid(row=0, column=1, sticky='ns')        # grid scrollbar
+            hbar = ttk.Scrollbar(frame, orient='horizontal') # create scrollbar
+            canvas['xscrollcommand'] = hbar.set            # connect text to scrollbar
+            hbar['command'] = canvas.xview                 # connect scrollbar to text
+            hbar.grid(row=1, column=0, sticky='we')        # grid scrollbar
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = canvas
         return canvas
-
+       
     # file/directory dialogs
 
     def addOpen(self, tag, prompt='', width=20, **tkparms):
-        """ Create a ttopen box which is a file entry and a browse button.
+        """ Create a ttOpenbox which is a file entry and a browse button.
 
         This has all the widgets needed to open a file. When the user clicks on
         the Browse button, a standard Open dialog box pops up. There are many
-        tkparms that are useful for limiting choices, see the Tk documentation.
+        tkparms that are useful for limiting choices, see the Tkinter documentation.
         Get/set uses str. Normally, this widget would be in a dialog. For a menu
-        command use popOpen.
+        command use popOpen. Width is a necessary option since **tkparms is for
+        the askopenfilename widget. If the programmer as an icon, they can replace
+        the 'Browse' text.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
-            width (int): Width of entry widget (chars)
-
+            width (int): Width of the entry widget
+            
+            
         Keyword Arguments:
             defaultextension (str): extention added to filename (must strat with .)
             filetypes (list): entrys in file listing ((label1, pattern1), (...))
             initialdir (str): Initial directory (space, ' ' remembers last directory)
             initialfile (str): Default filename
             title (str): Pop-up window's title
 
         Returns:
-            list(ttk/tk.entry, ttk/tk.button) 
+            list of ttk/tk.Entry and ttk/tk.Button
         """
 
         self.content[tag] = {'type': 'open', 'value': tk.StringVar()}  # init var to tk var
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
@@ -809,38 +834,38 @@
         """
 
         fn = askopenfilename(**tkparms)                # create the file dialog
         if fn:                                         # user selected file?
             self.set(tag, fn)                          # store it in content
 
     def addSaveAs(self, tag, prompt='', width=20, **tkparms):
-        """ Create an ttsaveas box which is a file entry with a browse button.
+        """ Create an ttSaveasbox which is a file entry with a browse button.
 
         This has all the widgets needed to save a file. When the user clicks on
         the Browse button, a standard SaveAs dialog box pops up. If the user
         selects an existing file, it will pop up a overwrite confirmation box.
-        There are many tkparms that are useful for limiting choices, see the Tk
+        There are many tkparms that are useful for limiting choices, see the Tkinter
         documentation. Get/set uses str. Normally, this widget would be in a
-        dialog. For a menu command, use popOpen.
+        dialog. For a menu command, use popSaveAs. Width is a necessary option
+        since **tkparms is for the asksaveasfilename widget.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
-            width (int): Width of entry widget
-
+            width (int): Width of the entry widget
 
         Keyword Arguments:
             defaultextension (str): extention added to filename (must strat with .)
             filetypes (list): entrys in file listing ((label1, pattern1), (...))
             initialdir (str): Initial directory (space, ' ' remembers last directory)
             initialfile (str): Default filename
             title (str): Pop-up window's title
 
         Returns:
-            list(ttk/tk.entry, ttk/tk.button) 
+            list of ttk/tk.Entry and ttk/tk.Button
         """
 
         self.content[tag] = {'type': 'saveas', 'value': tk.StringVar()}  # very similar to addOpen
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
@@ -858,33 +883,34 @@
         """
 
         fn = asksaveasfilename(**tkparms)                # similar to _openDialog
         if fn:
             self.set(tag, fn)
 
     def addChooseDir(self, tag, prompt='', width=20, **tkparms):
-        """ Create a ttchoosedir box which is a directory entry with a browse button.
+        """ Create a ttChoosedirbox which is a directory entry with a browse button.
 
         This has all the widgets needed to select a directory. When the user clicks
         on the Browse button, a standard Choose Directory dialog box pops up. There
-        are many tkparms that are useful for limiting choices, see the Tk
+        are many tkparms that are useful for limiting choices, see the Tkinter
         documentation. Get/set uses str. Normally, this would be use in a dialog.
-        For a menu command use popChooseDir.
+        For a menu command use popChooseDir. Width is a necessary option since **tkparms is for
+        the askopenfilename widget.
 
         Parameters:
             tag (str): Reference to widget
             prompt (str): Text of frame label
             width (int): Width of entry widget
 
         Keyword Arguments:
             initialdir (str): Initial directory (space, ' ' remembers last directory)
             title (str): Pop-up window's title
 
         Returns:
-            list(ttk/tk.entry, ttk/tk.button) 
+            list of ttk/tk.Entry and ttk/tk.Button
         """
 
         self.content[tag] = {'type': 'choosedir', 'value': tk.StringVar()}  # init var to tk var
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
@@ -903,89 +929,89 @@
 
         dirn = askdirectory(**tkparms)                 # similar to _openDialog
         if dirn:
             self.set(tag, dirn)
 
     # treeview based widgets
 
-    def addLedger(self, tag, height, columns, prompt='', **tkparms):
-        """ Create a ttledger which is based on a treeview that displays a simple
+    def addLedger(self, tag, columns, prompt='', **tkparms):
+        """ Create a ttLedger which is based on a treeview that displays a simple
         list with column headers.
 
         This widget allows a nice display of data in columns. It is a simplified
         version of the Collector widget. Due to a bug in ttk, sideways scrolling
         does not work correctly. If you need sideways scrolling use the Text widget.
         Get/set uses list of str. There is no tk version.
 
         Parameters:
             tag (str): Reference to widget
-            height (int): Height of widget
             columns (list): (Column headers, width (pixels))
             prompt (str): Text of frame label
 
         Keyword Arguments:
+            height (int): Height of widget
             padding (int): Spaces around values
             selectmode (str): ['browse'] or 'extended'
             style (ttk:Style): Style used for ttk.Treeview
 
         Returns:
-            ttk.treeview
+            ttk.Treeview
         """
 
         self.content[tag] = {'type': 'ledger'}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
         titles = [item[0] for item in columns]         # create the column titles
         tree = ttk.Treeview(frame, columns=titles, show='headings',
-            height=height, **tkparms)                  # create treeview
+            **tkparms)                  # create treeview
         yscroll = ttk.Scrollbar(frame, orient='vertical', command=tree.yview)
         tree['yscrollcommand'] = yscroll.set           # create scrollbar
         for title, width in columns:                   # init column headers
             tree.heading(title, text=title, anchor='w')  # set the title
             tree.column(title, width=width, stretch=False)  # set the width
         tree.grid(row=0, column=0, pady=3)             # grid the tree
         yscroll.grid(row=0, column=1, sticky='ns')     # grid scrollbar
         self.content[tag]['frame'] = frame
         self.content[tag]['widget'] = tree
         return tree
 
-    def addCollector(self, tag, height, columns, widgets, prompt='', **tkparms):
-        """ Create a ttcollector which is based on a treeview that collects contents
+    def addCollector(self, tag, columns, widgets, prompt='', **tkparms):
+        """ Create a ttCollectorbox which is based on a treeview that collects contents
         of other widgets.
 
         This collection of widgets allows the programmer to collect the contents
         of other widgets into a row. The user can add or delete rows as they
         wish using the included buttons. Get/set uses list of str. There is no tk
         version.
 
         Parameters:
             tag (str): Reference to widget
-            height (int): Height of widget
             columns (list): (Column headers, width (pixels))
             widgets (list): (Tags) for simple or (window, tag) for embedded widgets
             prompt (str): Text of frame label
 
         Keyword Arguments:
+            height (int): Height of widget
             padding (int): Spaces around values
             style (ttk.Style): Style used for ttk.Treeview
 
         Returns:
-            [ttk.treeview, ttk.button, ttk.button] 
+            list of ttk.Treeview and two ttk.Buttons
         """
 
         self.content[tag] = {'type': 'collector'}
         if prompt:
             frame = ttk.LabelFrame(self.master, text=prompt)  # create titled frame
         else:
             frame = ttk.Frame(self.master)             # no title
         titles = [item[0] for item in columns]         # create the column titles
         tree = ttk.Treeview(frame, columns=titles, show='headings',
-            selectmode='browse', height=height, **tkparms)  # create treeview
+            selectmode='browse', **tkparms)  # create treeview
         yscroll = ttk.Scrollbar(frame, orient='vertical', command=tree.yview)
         tree['yscrollcommand'] = yscroll.set           # create scrollbar
         for title, width in columns:                   # init column headers
             tree.heading(title, text=title, anchor='w')  # set the title
             tree.column(title, width=width, stretch=False)  # set the width
         tree.grid(row=0, column=0, pady=3)             # grid the tree
         yscroll.grid(row=0, column=1, sticky='ns')     # grid scrollbar
@@ -1031,55 +1057,55 @@
         select = tree.selection()                      # get the selection
         if select:
             tree.delete(select)                        # remove from treeview
 
     # widgets added for completeness
 
     def addSizegrip(self, tag, **tkparms):
-        """ Add a sizegrip widget to the window.
+        """ Add a ttSizegrip widget to the window.
 
         This places a sizegrip in the bottom right corner of the window. It is
         not needed since most platforms add this automatically. The programmer
         must use the configurerow and configurecolumn options when plotting
         widgets for this to work correctly. There is no frame. It was included
         for completeness. There is no tk version.
 
         Parameters:
             tag (str): Reference to widget
 
         Keyword Arguments:
             style (ttk.Style): Style used for ttk.Sizegrip, mainly background
 
         Returns:
-            ttk.sizegrip  
+            ttk.Sizegrip
         """
 
         self.content[tag] = {'type': 'sizegrip'}
         sizegrip = ttk.Sizegrip(self.master, **tkparms)
         sizegrip.grid(row=999, column=999, sticky='se')  # bottom right corner
         self.content[tag]['widget'] = sizegrip
         return sizegrip
 
     def addScrollbar(self, tag, widgetTag, orient='horizontal', usetk=False, **tkparms):
-        """ Add a scrollbar to a widget.
+        """ Add a ttScrollbar to a widget.
 
         This is usually this is done automatically. There is no frame. In order
         to plot the programmer must get the widget frame and use the correct sticky
         option. It was included for completeness.
 
         Parameters:
             tag (str): Reference to widget
             widgetTag (str): Tag of connected widget
             orient (str): ['horizontal'] or 'vertical'
 
         Keyword Arguments:
             style (ttk.Style): Style used for ttk.Scrollbar
 
         Returns:
-            ttk/tk.scrollbar
+            ttk/tk.Scrollbar
         """
 
         t = tk if usetk else ttk 
         self.content[tag] = {'type': 'scroll'}
         widget = self.getWidget(widgetTag)
         scroll = t.Scrollbar(self.master, orient=orient, **tkparms)
         if orient == 'horizontal':
@@ -1109,15 +1135,15 @@
             height (int): Height of frame (pixels)
             padding (int): Spaces between frame and widgets (pixels)
             relief (str): 'flat','raised','sunken','groove', or 'ridge'
             style (int): Style used for ttk.Frame or ttk.LabelFrame
             width (int): Width of frame (pixels)
 
         Returns:
-            tt.window
+            tt.Window
         """
 
         t = tk if usetk else ttk    
         self.content[tag] = {'type': 'frame'}
         if prompt:
             frame = t.LabelFrame(self.master, text=prompt, **tkparms)  # create titled frame
         else:
@@ -1144,15 +1170,15 @@
         Keyword Arguments:
             height (int): Height of frame (pixels)
             padding (int): Spaces between frame and widgets (pixels)
             style (int): Style used for ttk.Frame or ttk.LabelFrame
             width (int): Width of frame (pixels)
 
         Returns:
-            list(tt.windows)
+            list of tt.Windows
         """
 
         self.content[tag] = {'type': 'notebook'}        # data is list of lists
         pages = []                                     # pages will be other windows
         notebook = ttk.Notebook(self.master, **tkparms)  # create notebook
         for page in tabs:                              # each tab is a page
             window = self.addFrame(page)               # create frame
@@ -1160,98 +1186,85 @@
             pages.append(window)                       # remember created windows
         self.content[tag]['widget'] = notebook         # add widget
         return pages
 
     def addPanes(self, tag, titles, usetk=False, **tkparms):
         """ Create a multipaned window with user adjustable columns.
 
-        This is like a notebook but all the windows are visible. There is no
-        frame.
+        This is like a notebook but all the windows are visible and the
+        widths are adjustable. There is no frame.
 
         Parameters:
             tag (str): Reference to container
             titles (list): (titles) of all embedded windows
             usetk (bool): Use tk instead of ttk
 
         Keyword Arguments:
             height (int): Height of frame (pixels)
             orient (str): ['horizontal'] or 'vertical'
             padding (int): Spaces between frame and widgets (pixels)
             style (int): Style used for ttk.Frame or ttk.LabelFrame
             width (int): Width of frame (pixels)
 
         Returns:
-            [tt.windows]
+            list of tt.Windows
         """
 
         t = tk if usetk else ttk
         self.content[tag] = {'type': 'panes'}
         panes = []
         panedWindow = t.PanedWindow(self.master, **tkparms)
         for title in titles:
             window = self.addFrame(title, prompt=title, usetk=usetk)
             panedWindow.add(self.getFrame(title))
             panes.append(window)
         self.content[tag]['widget'] = panedWindow
         return panes
 
-    def addStyle(self, tag, **tkparms):
-        """ Add a ttk.Style to be used for other widgets.
-
-        This is the method for changing the appearance of ttk widgets. Styles are
-        strictly defined strings so look at the Tk documentation.
-
-        Parameter:
-            tag (str): Reference to style, must follow ttk naming
-
-        Keyword Arguments:
-            Varies with widget, see Tk documentation
-        """
-
-        self.style.configure(tag, **tkparms)
+    # menus
 
     def addMenuButton(self, tag, usetk=False, **tkparms):
-        """ Add a menu button
+        """ Add a ttMenubutton
 
-        A menubuuton always stays on the screen and is what the user clicks on. A menu
-        is attached to the menubutton. Menus are complex so read the Tk documentation
+        A menubutton always stays on the screen and is what the user clicks on. A menu
+        is attached to the menubutton. Menus are complex so read the Tkinter documentation
         carefully.
 
         Parameters:
             tag (str): Reference to menubutton
 
         Keyword Arguments:
-            Varies (dict): see Tk documentation
+            Varies (dict): see Tkinter documentation
 
         Returns:
-            ttk/tk.menubutton
+            ttk/tk.Menubutton
         """
 
         t = tk if usetk else ttk 
         self.content[tag] = {'type': 'menubutton'}
         menubutton = t.Menubutton(self.master, **tkparms)
         self.content[tag]['widget'] = menubutton
         return menubutton
 
     def addMenu(self, tag, parent, items=None, **tkparms):
-        """ Add a menu
+        """ Add a tt.Menu
 
-        Menus are complex so read the Tk documentation carefully.
+        Menus are complex so read the Tkinter documentation carefully.
 
         Parameters:
             tag (str): Reference to menu
             parent (ttk.Menubutton or tk.Frame): What menu is attached to
             items (list): ('cascade' or 'checkbutton' or 'command' or
-                'radiobutton' or 'separator', coptions) (see Tk Documentation)
+                'radiobutton' or 'separator', coptions) (see Tkinter Documentation)
  
         Keyword Arguments:
-            Varies (dict): see Tk documentation
+            Varies (dict): see Tkinter documentation
 
         Returns:
-            tk.menu 
+            tk.Menu
         """
 
         self.content[tag] = {'type': 'menu'}
         menu = tk.Menu(parent, **tkparms)
         if items:
             for wtype, coptions in items:
                 menu.add(wtype, **coptions)
@@ -1277,93 +1290,64 @@
             'ok' for show*, bool for ask*
         """
 
         # python magic, eval converts the string to a function and the...
         # parameter list calls the function
         return eval(mtype)(title, message, **tkparms)   # cool, yes?
 
-    def popOpen(self, **tkparms):
-        """ Popup a open dialog
+    def popDialog(self, dtype='askopenfilename', **tkparms):
+        """ Popup a standard dialog.
 
-        This pops up a standard open dialog.
-
-        Keyword Arguments:
-            defaultextension (str): extention added to filename (must strat with .)
-            filetypes (list): entrys in file listing ((label1, pattern1), (...))
-            initialdir (str): Initial directory (space, ' ' remembers last directory)
-            initialfile (str): Default filename
-            title (str): Pop-up window's title
-
-        Returns:
-            str
-        """
-
-        return askopenfilename(**tkparms)
-
-    def popSaveAs(self, **tkparms):
-        """ Popup a save as dialog
-
-        This pops up a standard save as dialog.
+        This pops up a standard tk dialog.
 
+        Parameters:
+           dtype (str): 'askopenfilename' or 'asksaveasfilename' or 'askdirectory'
+               or 'askcolor'message (str): Message in box
+           
         Keyword Arguments:
             defaultextension (str): extention added to filename (must strat with .)
             filetypes (list): entrys in file listing ((label1, pattern1), (...))
             initialdir (str): Initial directory (space, ' ' remembers last directory)
             initialfile (str): Default filename
             title (str): Pop-up window's title
+            color (str): Initial color (for askcolor)
 
         Returns:
-            str
+            str or (red, green, blue) for askcolor
         """
+        
+        return eval(dtype)(**tkparms)                     # cool again, yes?
+    
+    # support functions
 
-        return asksaveasfilename(**tkparms)
+    def addStyle(self, tag, **tkparms):
+        """ Add a ttk.Style to be used for other widgets.
 
-    def popChooseDir(self, **tkparms):
-        """ Popup a choose directory dialog
+        This is the method for changing the appearance of ttk widgets. Styles are
+        strictly defined strings so look at the Tkinter documentation.
 
-        This pops up a standard choose directory dialog. Normally, one would use
-        addChooseDir.
+        Parameter:
+            tag (str): Reference to style, must follow ttk naming
 
         Keyword Arguments:
-            initialdir (str): Initial directory (space, ' ' remembers last directory)
-            title (str): Pop-up window's title
-
-        Returns:
-            str
+            Varies with widget, see Tkinter documentation
         """
 
-        return askdirectory(**tkparms)
-
-    def popColorChooser(self, **tkparms):
-        """ Popup a color chooser dialog.
-
-        This pops up a standard color chooser dialog.
-
-        Keyword Arguments
-            color (str): Initial color
-            title (str): Title of pop-up window ['Color']
-
-        Returns:
-            (red, green blue)
-        """
-
-        return askcolor(**tkparms)
-
-    # support functions
+        self.style.configure(tag, **tkparms)
 
     def get(self, tag, allValues=False):
         """ Get the contents of the ttwidget. With more complex widgets the programmer
         can choose to get all the values rather than user selected values.
 
         Parameters:
             tag (str): Reference to widget, created in add*
             allValues (bool): if true return all the values
 
         Returns:
-            Contents of ttwidget
+            Contents of ttWidget
         """
 
         widgetType = self.getType(tag)                 # get type
         widget = self.getWidget(tag)                   # get widget(s)
         if widgetType in ('label', 'message'):
             value = widget['text']
         elif widgetType == 'entry':
@@ -1390,29 +1374,30 @@
                 for index in indices:
                     value.append(widget.get(index))    # get the row contenets
         elif widgetType == 'ledger':
             value = []
             if allValues:
                 for rid in widget.get_children():      # get all rows
                     row = widget.set(rid)              # get the items as a dict
-                    value.append(row)
+                    value.append(list(row.values()))
             else:
                 for rid in widget.selection():         # get the selected rows
                     row = widget.set(rid)
-                    value.append(row)
+                    value.append(list(row.values()))
         elif widgetType == 'collector':
             widget = widget[0]                         # get treeview
             value = []
             for rid in widget.get_children():          # get the top-level items
                 row = widget.set(rid)                  # get the dict
-                value.append(row)
+                value.append(list(row.values()))
         elif widgetType == 'spin':
-            value = []
+            values = []
             for item in self.content[tag]['value']:
-                value.append(item.get())               # get all tk variables
+                values.append(str(item.get()))         # get all tk.IntVars
+            value = self.content[tag]['between'].join(values) # create str    
         elif widgetType == 'text':
             value = widget.get('0.0', 'end')           # get all text
         elif widgetType == 'notebook':
             value = widget.index('current')            # get current page
         else:                                          # styles, menus, menubuttons
             value = widget                             # same as getWidget 
         return value
@@ -1461,71 +1446,98 @@
         elif widgetType == 'ledger':
             if allValues:
                 for wid in widget.get_children():      # get top-level items
                     widget.delete(wid)                 # delete them
             for item in value:
                 widget.insert('', 'end', values=item)  # add to tree
         elif widgetType == 'spin':
-            for item in self.content[tag]['value']:    # for spinboxes
+            sep = self.content[tag]['between']
+            if not sep:                                # sep cannot be ''
+                sep = ' '
+            values = value.split(sep)                  # split input str
+            for item in self.content[tag]['value']:    # fill tk.IntVars
                 if value == '':
                     item.set('')                       # clear it
                 else:
-                    item.set(value.pop(0))             # set it and get next
+                    item.set(int(values.pop(0)))       # set it and get next
         elif widgetType == 'notebook':
             widget.select(value)                       # display that page
         elif widgetType == 'text':                     # unlike other widget this inserts!
             if allValues:
                 widget.delete('1.0', 'end')            # clear everything
             widget.insert('end', value)                # add text
             widget.see('end')                          # scroll text so it is visible
         self.refresh()                                 # update display
 
+    def reset(self, tag):
+        """ Reset the selections in a widget 
+
+        This clears any selections in a widget. This was created mainly for
+        listboxes but is useful for all selection widgets.
+
+        Parameter:
+            tag (str): - Reference to widget
+
+        """
+        widgetType = self.getType(tag)
+        widget = self.getWidget(tag)
+        if widgetType in ('combo', 'radio', 'option', 'check'):
+            self.set(tag, '')
+        elif widgetType == 'list':
+            widget.selection_clear(0, 'end')
+        elif widgetType in ('ledger', 'collector'):
+            items = widget.get_children()
+            widget.selection_remove(items)
+        
     def plot(self, tag=None, **tkparms):
-        """ Plot the ttwidget.
+        """ Plot the ttWidget.
 
         Place a frame and widget in a cell of a window using the row and column.
-        Plot was selected as an easier name for beginners than grid. Other tkparms
-        are extremely useful here and should be understood. Look at the Tk
+        Plot was selected as an easier name for beginners than grid. Tkparms
+        are extremely useful here and should be understood. Look at the Tkinter
         documentation.
 
         Parameters:
             tag (str): Reference to widget
 
         Keyword Arguments:
             row (int): the row number counting from 0
             column (int): the column number
             rowspan (int): the number of rows to span
             columnspan (int): the number of columns to span
             sticky (str): the directions to fill the cell for the widget
-            rowconfigure (int): rate widget expands in vertical if resized
-            columnconfigure (int): rate widget expands in horizontal
             padx (int): horizontal space between widget cells (pixels)
             pady (int): vertical space between widget cells (pixels)
             ipadx (int): horizontal space within cell (pixels)
             ipady (int): vertical space within cell (pixels)
         """
 
         if not tag:
-            self.master.grid(**tkparms)
+            self.master.grid(**tkparms)  #
         elif self.content[tag]['type'] in ('line', 'notebook', 'panes', 'menubutton'):  # no frames
             self.content[tag]['widget'].grid(**tkparms)  # grid widget
         else:
             self.content[tag]['frame'].grid(**tkparms)  # grid frame
 
+    def grid(self, tag=None, **tkparms):
+        """ Some instructors prefer grid """
+
+        self.plot(tag, **tkparms)
+
     def getWidget(self, tag):
         """ Get the tk/ttk widget if present.
 
         Get the underlying tk or ttk widget so the programmer can use more advanced
         methods.
 
         Parameter:
             tag (str): - Reference to widget
 
         Returns:
-            The ttk/tk widget
+            ttk/tk.Widget
         """
 
         return self.content[tag].get('widget')
 
     def getFrame(self, tag):
         """ Get the ttk frame if present.
 
@@ -1537,60 +1549,61 @@
 
         Returns:
             ttk/tk.Frame or ttk/tk.LabelFrame
         """
 
         return self.content[tag].get('frame')
 
-    def changeWidget(self, tag, index=None, **tkparms):
-        """ Change a tk/ttk widget
+    def setWidget(self, tag, index=None, **tkparms):
+        """ Change a tk/ttk widget attribute
 
          Change the underlying tk or ttk widget appearance using
          tkparms. Index parameter allows you to change an individual
-         element in multipart widget. See Tk documentation.
+         element in multipart widget. See Tkinter documentation.
 
          Parameters:
              tag (str): Reference to widget
              index (int): Index to element in multipart widget
 
          Keyword Arguments:
-            justify (str): Justification of text ('left' [def], 'right', 'center')
-            show (str): Char to display instead of actual text
-            style (ttk.Style): Style to use for widget
-            text (str): Text inside widget
+             justify (str): Justification of text ('left' [def], 'right', 'center')
+             show (str): Char to display instead of actual text
+             style (ttk.Style): Style to use for widget
+             text (str): Text inside widget
          """
 
         widget = self.getWidget(tag)                   # get widget
         if index is not None:                          # if multiwidget...
             widget = widget[index]                     # get element
         widget.configure(**tkparms)                    # configure tkparms
 
-    def changeState(self, tag, index=None, *states):
+    def setState(self, tag, states, index=None):
         """ Set or clear ttk or tk widget states
 
          Change the underlying ttk or tk widget states. For ttk widgets
          the states are 'active', 'alternate', background', 'disabled',
          'focus', 'invalid', 'pressed', 'readonly', and 'selected'.
-         Preceding a state with '!' clears it. For tk widgets use 'disabled'
-         or 'normal'. Index parameter allows you to change an individual
-         element in multipart widget. See Tk documentation.
+         Preceding a state with '!' clears it. For tk widgets use 'disabled',
+         'normal', or 'readonly'. Index parameter allows you to change an
+         individual element in multipart widget. See Tkinter documentation.
 
          Parameters:
              tag (str): Reference to widget
+             states (list): States of widget, usually 'disabled' or
+                 '!disabled' for ttk
              index (int): Index to element in multipart widget
-             states (list): States of widget, usually ['disabled'] or ['!disabled']
          """
 
         widget = self.getWidget(tag)                   # get widget
         if index is not None:                          # if multiwidget...
             widget = widget[index]                     # get element
         try:    
-            widget.state(*states)                      # clear/set states
+            widget.state(states)                       # clear/set states
         except AttributeError:                         # tk widget   
-            widget.configure(state=states[0])          # 'disabled' or 'normal'
+            widget.configure(states[0])                # 'disabled','normal','readonly'
 
     def getType(self, tag):
         """ Get the type of widget.
 
         Get the type of widget as a string. All widgets have a type.
 
         Parameters:
@@ -1606,14 +1619,19 @@
         """ Alias for mainloop, better label for beginners.
 
         This starts the event loop so the user can interact with window.
         """
 
         self.master.mainloop()
 
+    def mainloop(self):
+        """ Some instructors prefer mainloop """
+
+        self.waitforUser()
+
     def close(self):
         """ Close the window.
 
         This stops the event loop and removes the window. However, the window
         structure can still be referenced, and the window can be redisplayed.
         """
```

### Comparing `tkintertoy-1.3.0/tkintertoy/ttgallery.py` & `tkintertoy-1.5.0/src/tkintertoy/ttgallery.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,154 @@
 #-------------------------------------------------------------------------------
 # Name:        ttgallery
 # Purpose:     Demostrate use of tkintertoy widgets
 #
 # Author:      mike.callahan
 #
-# Created:     1/3/2020
-# Copyright:   (c) mike.callahan 2019, 2020
+# Created:     5/28/2023
+# Copyright:   (c) mike.callahan 2019 - 2023
 # License:     MIT
 #-------------------------------------------------------------------------------
 
 from tkintertoy import Window
 
-class Gui(object):
+class Gui:
 
     def __init__(self):
         self.gui = Window()
+        self.gui2 = Window(extra=True)
         self.gui.setTitle('Tkintertoy Gallery')
+        self.gui2.setTitle('Tk Only Window')
         self.makeGui()
 
     def makeGui(self):
         # a simple menu
         mymenu = self.gui.addMenu('ttmainmenu', self.gui.master) # create a main menu
         fmenu = [['command', {'label':'Open...', 'command':self.popOpen}], # create a file menu
             ['command', {'label':'Save As...', 'command':self.popSaveAs}],
             ['command', {'label':'Choose Directory...', 'command':self.popChooseDir}],
             ['command', {'label':'Exit', 'command':self.gui.cancel}]]
         mmenu = [['command', {'label':'About', 'command':self.popAbout}], # create a misc menu
             ['command', {'label':'ChooseColor', 'command':self.popColor}]]
-        self.gui.addMenu('ttfmenu', mymenu, fmenu) # create sub menus
+        self.gui.addMenu('ttfmenu', mymenu, fmenu)               # create sub menus
         self.gui.addMenu('ttmmenu', mymenu, mmenu)
         mymenu.add('cascade', label='File', menu=self.gui.get('ttfmenu')) # add them to the main menu
         mymenu.add('cascade', label='Misc', menu=self.gui.get('ttmmenu'))
-        self.gui.master['menu'] = mymenu # connect the main menu to the window
+        self.gui.master['menu'] = mymenu                         # connect the main menu to the window
         # Notebook
-        tabs = ['Simple','Dialog','Multi','Other'] # label the tabs
-        self.pages = self.gui.addNotebook('ttnotebook', tabs) # create the notebook
+        tabs = ['Simple','Dialog','Multi','Other']               # label the tabs
+        self.pages = self.gui.addNotebook('ttnotebook', tabs)    # create the notebook
         # Text Box
-        self.gui.addText('ttext', 60, 10, 'Text Box') # create text area
+        self.gui.addText('ttext', 'Text Box', width=60, height=10) # create text area
         self.gui.plot('ttext', row=1)
         # Progress Bar
-        self.gui.addProgress('ttprogress', 100, 'Progress Bar') # create progrees bar
+        self.gui.addProgress('ttprogress', 'Progress Bar', length=200) # create progrees bar
         self.gui.plot('ttprogress', row=2)
         # Command Buttons
         cmd = [['Collect',self.collect],['Exit', self.gui.cancel]] # create two buttons
         self.gui.addButton('ttbutton', '', cmd)
         self.gui.plot('ttbutton', row=3)
         # Notebook Pages
         self.makeSimple()
         self.makeDialog()
         self.makeMulti()
         self.makeOther()
         self.gui.plot('ttnotebook', row=0, column=0)
+        self.secondWin()
 
     def makeSimple(self):
         self.simplePage = self.pages[0]
         # Label
-        self.simplePage.addLabel('ttlabel','','bold') # create a label
-        self.simplePage.set('ttlabel', 'This is a BOLD label') # fill in the value
+        self.simplePage.addLabel('ttlabel', '', 'bold',         # create a label with an    
+            text='This is a BOLD label')                        # initial text
         self.simplePage.plot('ttlabel', row=0)
         # Line
-        self.simplePage.addLine('ttline') # create a horizontal line
-        self.simplePage.plot('ttline', row=1)
+        self.simplePage.addLine('ttline')                       # create a horizontal line
+        self.simplePage.plot('ttline', row=1, sticky='we')      # stretch it horizontally
         # Message
-        self.simplePage.addMessage('ttmessage', 'Message') # create a message
-        self.simplePage.set('ttmessage', 'Useful for multi-line messages')
+        self.simplePage.addMessage('ttmessage', 'Message', justify='center') # create a message
+        self.simplePage.set('ttmessage', 'Useful for multi-line messages') # add the text
         self.simplePage.plot('ttmessage', row=2)
         # Entry
         self.simplePage.addStyle('g.TEntry', foreground='green') # create a green entry
         self.simplePage.addEntry('ttentry', 'Entry', style='g.TEntry')
-        self.simplePage.set('ttentry', 'Default Entry') # fill in the value
+        self.simplePage.set('ttentry', 'Green Text')            # add the text
         self.simplePage.plot('ttentry', row=3)
         # Option
         alist = ['Option1','Option2','Option3']
         self.simplePage.addOption('ttoption', 'Option List', alist) # create an option list
         self.simplePage.set('ttoption', 'Option1')
         self.simplePage.plot('ttoption', row=5)
         # Combobox and Style
         acombo = ['ComboOption1','ComboOption2','ComboOption3']
         self.simplePage.addCombo('ttcombo', 'Combo Box', acombo) # create combobox
         self.simplePage.plot('ttcombo', row=6)
         # Checkboxes
         achecks = ['CheckOption1','CheckOption2','CheckOption3']
         self.simplePage.addCheck('ttchecks', 'Check Box', achecks) # create 3 checkboxes
+        self.simplePage.set('ttchecks','checkOption1')          # preselect first checkbox
         self.simplePage.plot('ttchecks', row=7)
-        self.simplePage.changeState('ttchecks', 1, ['disabled']) # disable CheckOption2
+        self.simplePage.setState('ttchecks', ['disabled'], index=1) # disable CheckOption2
         # Radio Buttons
         aradio = ['RadioOption1','RadioOption2','RadioOption3']
         self.simplePage.addRadio('ttradio', 'RadioButton Box', aradio) # create 3 radiobuttons      self.simplePage.plot('ttradio', row=8)
+        self.simplePage.plot('ttradio', row=8)
         # Scale
-        self.simplePage.addScale('ttscale', [1,10], 'Scale', width=2) # create a scale
+        self.simplePage.addScale('ttscale', [1,10], 'Scale', width=2, length=200) # create a scale
         self.simplePage.plot('ttscale', row=9)
         # Spinners
         adate = [[2,1,12],[2,1,31],[4,2000,2099]]
         self.simplePage.addSpin('ttspin', adate, '/', 'Date Box') # create a date entry box
-        self.simplePage.set('ttspin', [11,17,2017])
+        self.simplePage.set('ttspin', '4/21/2023')               # set the initial date 
         self.simplePage.plot('ttspin', row=10)
 
     def makeDialog(self):
         self.dialogPage = self.pages[1]
         # Open
-        self.dialogPage.addOpen('ttopen', 'Open', width=40) # open dialog
+        self.dialogPage.addOpen('ttopen', 'Open', width=40)      # open dialog
         self.dialogPage.plot('ttopen', row=0)
         # SaveAs
         self.dialogPage.addSaveAs('ttsaveas', 'Save As', width=40) # save as dialog
         self.dialogPage.plot('ttsaveas', row=1)
         # ChooseDir
         self.dialogPage.addChooseDir('ttchoosedir', 'Choose Dir', width=40) # choose dir dialog
         self.dialogPage.plot('ttchoosedir', row=2)
 
     def popOpen(self):
         # open dialog
-        self.gui.set('ttext', self.gui.popOpen(title='Open a File')+'\n')
+        self.gui.set('ttext', self.gui.popDialog(title='Open a File')+'\n')
 
     def popSaveAs(self):
         # save as dialog
-        self.gui.set('ttext', self.gui.popSaveAs(title='Save a File')+'\n')
+        self.gui.set('ttext', self.gui.popDialog('asksaveasfilename',
+            title='Save a File')+'\n')
 
     def popChooseDir(self):
         # choose dir dialog
-        self.gui.set('ttext', self.gui.popChooseDir(title='Select a Directory')+'\n')
+        self.gui.set('ttext', self.gui.popDialog('askdirectory',
+            title='Select a Directory')+'\n')
 
     def popColor(self):
         # Color Chooser
-        self.gui.set('ttext', str(self.gui.popColorChooser(title='Select a Color'))+'\n')
+        self.gui.set('ttext', str(self.gui.popDialog('askcolor',
+            title='Select a Color'))+'\n')
 
     def popAbout(self):
         # Pop Up Message Box
         self.gui.popMessage('Tkintertoy Gallery')
 
     def makeMulti(self):
         self.multiPage = self.pages[2]
         # List
         alist = ['ListOption1','ListOption2','ListOption3']
         self.multiPage.addList('ttlist', 'List', alist, height=4) # create list
         self.multiPage.plot('ttlist', row=0)
         # Ledger
         cols = [['column1',100],['column2',80],['column3',80]]
-        self.multiPage.addLedger('ttledger', 4, cols, 'Ledger') # create ledger
+        self.multiPage.addLedger('ttledger', cols, 'Ledger', height=4) # create ledger
         self.multiPage.set('ttledger', [['header1','item1-1','item1-2']])
         self.multiPage.set('ttledger', [['header2','item2-1','item2-2']])
         self.multiPage.set('ttledger', [['header3','tiem3-1','item2-3']])
         self.multiPage.plot('ttledger', row=1)
         # Collector Frame
         self.subwin = self.multiPage.addFrame('ttframe', '', relief='groove')
         # -Combobox
@@ -148,73 +156,121 @@
         self.subwin.addCombo('ttcombo2', 'Combo Box 2', acombo)
         self.subwin.plot('ttcombo2', row=0)
         # -Radio Button
         aradio = ['Radio2-1','Radio2-2','Radio2-3']
         self.subwin.addRadio('ttradio2', 'RadioButton Box 2', aradio)
         self.subwin.plot('ttradio2', row=1)
         # -Collector
-        cols = [['Combo',100],['Radio', 100]]
-        self.subwin.addCollector('ttcollector', 4, cols, ['ttcombo2','ttradio2'], 'Collector')
+        cols = [['Combo',110],['Radio', 90]]
+        self.subwin.addCollector('ttcollector', cols, ['ttcombo2','ttradio2'],
+            'Collector', height=4)
         self.subwin.plot('ttcollector', row=2)
         self.multiPage.plot('ttframe', row=2)
 
     def makeOther(self):
         self.otherPage = self.pages[3]
         # Canvas
-        self.otherPage.addCanvas('ttcanvas', 300, 100, 'Canvas') # create canvas
-        self.otherPage.get('ttcanvas').create_oval(10 ,10 ,290 ,90 ,fill='green')
+        self.otherPage.addCanvas('ttcanvas', 'Canvas', width=300, height=100) # create canvas
+        self.otherPage.get('ttcanvas').create_oval(10, 10, 290, 90, fill='green')
         self.otherPage.plot('ttcanvas', row=0)
         # Multipane
         paneTitles = ['Pane 1','Pane 2','Pane 3']
         panes = self.otherPage.addPanes('ttpane', paneTitles, orient='horizontal')
         for i in range(3):
             # -Label
             tag = 'ttlabel' + str(i)
             panes[i].addLabel(tag)
             panes[i].set(tag, 'Inner label {}'.format(i+1))
             panes[i].plot(tag)
         self.otherPage.plot('ttpane', row=1)
 
     def collect(self):
         # show contents of all widgets
-        result = 'Contents of widgets\n  Simple Page:\n    '
+        result = '\nMain Window\n  Simple Page:\n    '
         result += self.simplePage.get('ttlabel') + '\n    '
         result += self.simplePage.get('ttmessage') + '\n    '
         result += self.simplePage.get('ttentry') + '\n    '
         result += self.simplePage.get('ttoption') + '\n    '
         result += self.simplePage.get('ttcombo') + '\n    '
         result += str(self.simplePage.get('ttchecks')) + '\n    '
         result += str(self.simplePage.get('ttradio')) + '\n    '
         result += str(self.simplePage.get('ttscale')) + '\n    '
         result += str(self.simplePage.get('ttspin')) + '\n    '
         self.gui.set('ttprogress', 33)
-        self.gui.set('ttext', result, allValues=True)
+        self.gui.set('ttext', result)
         self.gui.master.after(500) # wait .5 sec
         result = '  File Page:\n    '
         result += self.dialogPage.get('ttopen') + '\n    '
         result += self.dialogPage.get('ttsaveas') + '\n    '
         result += self.dialogPage.get('ttchoosedir') + '\n    '
         self.gui.set('ttprogress', 66)
         self.gui.set('ttext', result)
         self.gui.master.after(500) # wait .5 sec
         result = '  Multi Page:\n    '
         result += str(self.multiPage.get('ttlist')) + '\n    '
         result += str(self.multiPage.get('ttledger')) + '\n    '
         result += str(self.subwin.get('ttcollector', allValues=True)) + '\n    '
+        result += '\n\n' 
         # Progress Bar
         self.gui.set('ttprogress', 100)
         self.gui.set('ttext', result)
         self.gui.master.after(1000) # wait 1 sec
         self.gui.set('ttprogress', 0)
 
+    def secondWin(self):
+        # pop up a second independent window using tk widgets only
+        # Label
+        self.gui2.addLabel('ttlabel2',usetk=True, text='These are Tk widgets.',
+             effects='bold')
+        # Entry
+        self.gui2.addEntry('ttentry2','Type something here', usetk=True,
+             foreground='green')
+        # Checkboxes
+        achecks = ['CheckOption1','CheckOption2','CheckOption3']
+        self.gui2.addCheck('ttchecks2', 'Check Box', achecks, usetk=True) # create 3 checkboxes
+        self.gui2.set('ttchecks2','CheckOption3')          # preselect first checkbox
+        # Radio Buttons
+        aradio = ['RadioOption1','RadioOption2','RadioOption3']
+        self.gui2.addRadio('ttradio3', 'RadioButton Box', aradio, usetk=True) # create 3 radiobuttons
+        self.gui2.set('ttradio3', 'RadioOption3')
+        # Scale
+        self.gui2.addScale('ttscale2', [1,10], 'Scale', width=2, usetk=True,
+            orient='horizontal', length=200)                                         # create a scale
+        # Spinners
+        adate = [[2,1,12],[2,1,31],[4,2000,2099]]
+        self.gui2.addSpin('ttspin2', adate, '/', 'Date Box', usetk=True) # create a date entry box
+        self.gui2.set('ttspin2', '3/15/2001')               # set the initial date 
+        # Buttons
+        cmd = [['Collect',self.secondCollect],['Exit', self.gui2.close]] # create two buttons
+        self.gui2.addButton('ttbutton2', '', cmd, usetk=True)
+        # Plot widgets
+        self.gui2.plot('ttlabel2', row=0, padx=30)
+        self.gui2.plot('ttentry2', row=1)
+        self.gui2.plot('ttchecks2', row=2)
+        self.gui2.plot('ttradio3', row=3)
+        self.gui2.plot('ttscale2', row=4)
+        self.gui2.plot('ttspin2', row=5)
+        self.gui2.plot('ttbutton2', row=6, pady=10)
+
+    def secondCollect(self):
+        # collect the infomation from the second window and place in ttext
+        result = '\nSecond Window:\n'
+        result += self.gui2.get('ttlabel2')+'\n'
+        result += self.gui2.get('ttentry2')+'\n'
+        result += str(self.gui2.get('ttchecks2'))+'\n'
+        result += self.gui2.get('ttradio3')+'\n'
+        result += str(self.gui2.get('ttscale2'))+'\n'
+        result += str(self.gui2.get('ttspin2'))+'\n\n'
+        self.gui.set('ttext', result)
+
 def main():
     app = Gui()
     try:
         app.gui.waitforUser()
-    except:
+    except:                                                      # trap all Exceptions
         errorMessage = app.gui.catchExcept()
         app.gui.popMessage(errorMessage, 'showwarning', 'Error')
-        app.gui.destroy()
+        app.gui.cancel()
 
 main()
```

### Comparing `tkintertoy-1.3.0/tkintertoy.egg-info/PKG-INFO` & `tkintertoy-1.5.0/src/tkintertoy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 Metadata-Version: 2.1
 Name: tkintertoy
-Version: 1.3.0
+Version: 1.5.0
 Summary: A simple GUI package based on Tkinter
-Home-page: https://github.com/mcalla314/tkintertoy
-Author: Mike Callahan
-Author-email: mcalla@twc.com
-License: UNKNOWN
+Author-email: Mike Callahan <mcalla@twc.com>
+Project-URL: Homepage, https://github.com/mcalla314/tkintertoy
 Project-URL: Documentation, https://tkintertoy.readthedocs.io
-Description: # Tkintertoy
-        
-        Tkintertoy was designed to be a easy to use GUI library based on Tkinter.
-        It was intended for "young" (as in experience) programmers to develop GUIs
-        with as little trouble as possible. However, more "advanced" programmers can
-        reach the more complex features of Tkinter easily. Here is a short example:
-        
-            from tkintertoy import Window
-            # create the window
-            gui = Window()
-            gui.setTitle('My First Tkintertoy GUI!')
-            # add the widgets
-            gui.addEntry('name', 'Type in your name')
-            gui.addLabel('welcome', 'Welcome message')
-            gui.addButton('commands')
-            # plot the widgets
-            gui.plot('name', row=0)
-            gui.plot('welcome', row=1)
-            gui.plot('commands', row=2, pady=10)
-            # start the event processing loop
-            while True:
-                gui.waitforUser()
-                if gui.content:
-                    gui.set('welcome', 'Welcome ' + gui.get('name'))
-                else:
-                    break
-            
-        This code will create a small window with an entry, label, and command button
-        widgets. The application will wait for the user to type in their first name.
-        After typing it in, and clicking on Ok, the application will display a welcome
-        label. The user exits the code by clicking on Cancel.
-        
-        ![Simple GUI](http://tkintertoy.readthedocs.io/en/latest/_images/first.png)
-        
-        As you can see in orgder to create a simple GUI, you create a window, add widgets,
-        plot the widgets in the desired location, and then call waitforUser.
-        
-        While Tkintertoy was designed to be an GUI library for simple interfaces it
-        has been used in more complex code as well. 
-        
-        Using Tkintertoy, it is hoped that Python instructors can quickly move students
-        from boring command-line applications to useful standard GUIs. A tutorial with
-        many useful examples in included with the documentation.
-            
-            
-        
-Keywords: GUI,Tkinter
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
+Keywords: GUI,novice
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: User Interfaces
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Tkintertoy
+
+Tkintertoy was designed to be a easy to use GUI library based on Tkinter.
+It was intended for novice programmers to develop GUIs with as little
+trouble as possible. However, more "advanced" programmers can reach the
+more complex features of Tkinter easily. Here is a short example:
+
+    from tkintertoy import Window
+    # create the window
+    gui = Window()
+    gui.setTitle('My First Tkintertoy GUI!')
+    # add the widgets
+    gui.addEntry('name', 'Type in your name')
+    gui.addLabel('welcome', 'Welcome message')
+    gui.addButton('commands')
+    # plot the widgets
+    gui.plot('name', row=0)
+    gui.plot('welcome', row=1)
+    gui.plot('commands', row=2, pady=10)
+    # start the event processing loop
+    while True:
+        gui.waitforUser()
+        if gui.content:
+            gui.set('welcome', 'Welcome ' + gui.get('name'))
+        else:
+            break
+    
+This code will create a small window with an entry, label, and command button
+widgets. The application will wait for the user to type in their first name.
+After typing it in, and clicking on Ok, the application will display a welcome
+label. The user exits the code by clicking on Cancel.
+
+![Simple GUI](http://tkintertoy.readthedocs.io/en/latest/_images/first.png)
+
+As you can see in order to create a simple GUI, you create a window, add widgets,
+plot the widgets in the desired location, and then call waitforUser.
+
+While Tkintertoy was designed to be an GUI library for simple interfaces it
+has been used in more complex code as well. 
+
+Using Tkintertoy, it is hoped that Python instructors can quickly move students
+from boring command-line applications to standard GUIs. A tutorial with many
+useful examples in included with the documentation. Also included with the source
+is John Shipman's Tkinter 8.5 Reference PDF.
+    
+
```

