# Comparing `tmp/Spider_Toolkit-23.0.2.tar.gz` & `tmp/Spider_Toolkit-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spider_Toolkit-23.0.2.tar", last modified: Sat Jun 10 10:40:09 2023, max compression
+gzip compressed data, was "Spider_Toolkit-23.0.3.tar", last modified: Sat Jun 10 12:17:55 2023, max compression
```

## Comparing `Spider_Toolkit-23.0.2.tar` & `Spider_Toolkit-23.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.487496 Spider_Toolkit-23.0.2/
--rw-rw-rw-   0        0        0     1079 2023-06-09 06:25:44.000000 Spider_Toolkit-23.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      658 2023-06-10 10:40:09.487496 Spider_Toolkit-23.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.453487 Spider_Toolkit-23.0.2/Spider_Toolkit/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.481493 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/
--rw-rw-rw-   0        0        0     9259 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/Parameter_filtering_engine.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/engine/__init__.py
--rw-rw-rw-   0        0        0    12143 2023-06-10 10:19:44.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/spidertools.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.486495 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/
--rw-rw-rw-   0        0        0    11626 2023-06-10 10:31:24.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Download_byte.py
--rw-rw-rw-   0        0        0      314 2023-06-10 08:09:27.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Open_js.py
--rw-rw-rw-   0        0        0     4200 2023-06-10 09:36:32.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Save.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.2/Spider_Toolkit/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:40:09.479494 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/
--rw-rw-rw-   0        0        0      658 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-10 10:40:09.000000 Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-10 10:40:09.488497 Spider_Toolkit-23.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2114 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:17:55.686904 Spider_Toolkit-23.0.3/
+-rw-rw-rw-   0        0        0     1079 2023-06-09 06:25:44.000000 Spider_Toolkit-23.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      614 2023-06-10 12:17:55.686904 Spider_Toolkit-23.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-06-10 12:16:19.000000 Spider_Toolkit-23.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 12:17:55.669900 Spider_Toolkit-23.0.3/Spider_Toolkit/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:17:55.682902 Spider_Toolkit-23.0.3/Spider_Toolkit/engine/
+-rw-rw-rw-   0        0        0     9259 2023-06-10 10:39:49.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/engine/Parameter_filtering_engine.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/engine/__init__.py
+-rw-rw-rw-   0        0        0    12143 2023-06-10 10:19:44.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/spidertools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:17:55.685904 Spider_Toolkit-23.0.3/Spider_Toolkit/tools/
+-rw-rw-rw-   0        0        0    11626 2023-06-10 10:31:24.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/tools/Download_byte.py
+-rw-rw-rw-   0        0        0      314 2023-06-10 08:09:27.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/tools/Open_js.py
+-rw-rw-rw-   0        0        0     4200 2023-06-10 09:36:32.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/tools/Save.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.3/Spider_Toolkit/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 12:17:55.681903 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/
+-rw-rw-rw-   0        0        0      614 2023-06-10 12:17:55.000000 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-06-10 12:17:55.000000 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 12:17:55.000000 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-10 12:17:55.000000 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-10 12:17:55.000000 Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-10 12:17:55.687904 Spider_Toolkit-23.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2072 2023-06-10 12:17:47.000000 Spider_Toolkit-23.0.3/setup.py
```

### Comparing `Spider_Toolkit-23.0.2/LICENSE.txt` & `Spider_Toolkit-23.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.2/Spider_Toolkit/engine/Parameter_filtering_engine.py` & `Spider_Toolkit-23.0.3/Spider_Toolkit/engine/Parameter_filtering_engine.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.2/Spider_Toolkit/spidertools.py` & `Spider_Toolkit-23.0.3/Spider_Toolkit/spidertools.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Download_byte.py` & `Spider_Toolkit-23.0.3/Spider_Toolkit/tools/Download_byte.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.2/Spider_Toolkit/tools/Save.py` & `Spider_Toolkit-23.0.3/Spider_Toolkit/tools/Save.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.2/Spider_Toolkit.egg-info/PKG-INFO` & `Spider_Toolkit-23.0.3/Spider_Toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Spider-Toolkit
-Version: 23.0.2
+Version: 23.0.3
 Summary: 爬虫辅助模块
 Home-page: https://github.com/pypa/sampleproject
 Author: Uncle_Ming
 Author-email: 2462711716@qq.com
 Keywords: tools spider requests download
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
-爬虫辅助模块0.0.2版本更新了byte下载器function，保存器，js调用器
+爬虫辅助模块0.0.3版本修复了bug
```

### Comparing `Spider_Toolkit-23.0.2/setup.py` & `Spider_Toolkit-23.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     # 以下为必需参数
     name='Spider_Toolkit',  # 模块名
-    version='23.0.2',  # 当前版本
+    version='23.0.3',  # 当前版本
     description='爬虫辅助模块',  # 简短描述
     packages=find_packages(),  # 多文件模块写法 exclude=['contrib', 'docs', 'tests']
     # 以下均为可选参数
-    long_description="爬虫辅助模块0.0.2版本更新了byte下载器function，保存器，js调用器",  # 长描述
+    long_description="爬虫辅助模块0.0.3版本修复了bug",  # 长描述
     url='https://github.com/pypa/sampleproject',  # 主页链接
     author='Uncle_Ming',  # 作者名
     author_email='2462711716@qq.com',  # 作者邮箱
     classifiers=[
         'Development Status :: 1 - Planning',  # 当前开发进度等级（测试版，正式版等）
         'License :: OSI Approved :: MIT License',  # 模块的license
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='tools spider requests download',  # 模块的关键词，使用空格分割
-    install_requires=['requests','pandas','execjs','pymysql','redis','pymongo'],  # 依赖模块
+    install_requires=['requests','pandas','PyExecJS','pymysql','redis','pymongo'],  # 依赖模块
     # extras_require={  # 分组依赖模块，可使用pip install sampleproject[dev] 安装分组内的依赖
     #     'dev': ['check-manifest'],
     #     'test': ['coverage'],
     # },
     # package_data={  # 模块所需的额外文件
     #     'sample': ['package_data.dat'],
     # },
```

