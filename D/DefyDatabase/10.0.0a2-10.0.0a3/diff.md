# Comparing `tmp/DefyDatabase-10.0.0a2.tar.gz` & `tmp/DefyDatabase-10.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a2.tar", last modified: Sat Jun 10 11:26:24 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a3.tar", last modified: Sat Jun 10 11:33:32 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a2.tar` & `DefyDatabase-10.0.0a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 11:26:24.006665 DefyDatabase-10.0.0a2/
-drwxrwxrwx   0        0        0        0 2023-06-10 11:26:23.999364 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      506 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-10 11:26:23.000000 DefyDatabase-10.0.0a2/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      506 2023-06-10 11:26:24.004661 DefyDatabase-10.0.0a2/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a2/README.md
--rw-rw-rw-   0        0        0     6986 2023-06-10 11:24:20.000000 DefyDatabase-10.0.0a2/defy.py
--rw-rw-rw-   0        0        0       42 2023-06-10 11:26:24.006665 DefyDatabase-10.0.0a2/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-06-10 11:25:17.000000 DefyDatabase-10.0.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 11:33:32.269659 DefyDatabase-10.0.0a3/
+drwxrwxrwx   0        0        0        0 2023-06-10 11:33:32.261357 DefyDatabase-10.0.0a3/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      551 2023-06-10 11:33:32.000000 DefyDatabase-10.0.0a3/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-10 11:33:32.000000 DefyDatabase-10.0.0a3/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 11:33:32.000000 DefyDatabase-10.0.0a3/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-10 11:33:32.000000 DefyDatabase-10.0.0a3/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      551 2023-06-10 11:33:32.267656 DefyDatabase-10.0.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a3/README.md
+-rw-rw-rw-   0        0        0     5671 2023-06-10 11:32:50.000000 DefyDatabase-10.0.0a3/defy.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 11:33:32.269659 DefyDatabase-10.0.0a3/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a3/setup.py
```

### Comparing `DefyDatabase-10.0.0a2/defy.py` & `DefyDatabase-10.0.0a3/defy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #Rules are meant to break by proudest ones.
 '''
 这是亮天计划的数据库官方API。
 '''
 import sqlite3,sys,os,datetime,io
 
 tor='DefyDatabase'
-version='10.0.0a2'
+version='10.0.0a3'
 
 commands=[
     'SELECT COUNT(*) FROM LIGHTSKY',
     'SELECT UID,BIND FROM BIND WHERE UID = "{}"',
     'SELECT UID, GRADE, JOB ,ABOUT FROM LIGHTSKY WHERE UID = "{}"',
     'SELECT UID, GRADE, JOB ,ABOUT from LIGHTSKY WHERE rowid={}',
     'SELECT COUNT(*) FROM BIND',
@@ -186,53 +186,7 @@
         self.__cur.close()
         self.__con.close()
 
 
 def open(file):
     return __DefyProject(file)
 
-def atest_defy():
-    with open('a.db') as a:
-        a.atest_many([['1',1,0,'0'],['2',50,0,'0'],['3',62,0,'0']])
-        print('应当："1"为1%，"2"为50%,"3"为62%')
-        print(a.queryuid('1'))
-        print(a.queryuid('2'))
-        print(a.queryuid('3'))
-        print()
-        a.atest_percent('1')
-        print('应当："1"为2%')
-        print(a.queryuid('1'))
-        print()
-        a.atest_percent('1',50)
-        print('应当："1"为52%')
-        print(a.queryuid('1'))
-        print()
-        a.atest_percent('1',-20)
-        print('应当："1"为32%')
-        print(a.queryuid('1'))
-        a.atest_percent('1',-50)
-        print('应当："1"为-18%')
-        print(a.queryuid('1'))
-
-def atest_speed(num=1000):
-    m=[]
-    tr=datetime.datetime.now()
-    for i in range(1,num+1):
-        m.append([str(i),i,i,str(i)])
-    with open('a.db') as a:
-        a.atest_many(m)
-    print(datetime.datetime.now()-tr)
-    del m
-    
-    a=open('a.db')
-    m=[]
-    tr=datetime.datetime.now()
-    for i in range(1,num+1):
-        a.atest_one(str(i),i,i,str(i))
-    print(datetime.datetime.now()-tr)
-    
-    tr=datetime.datetime.now()
-    for i in range(1,num+1):
-        a5=a.queryuid(str(i))
-    print(datetime.datetime.now()-tr)
-    a.close()
-    del a
```

