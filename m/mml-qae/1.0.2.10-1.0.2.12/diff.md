# Comparing `tmp/mml_qae-1.0.2.10.tar.gz` & `tmp/mml_qae-1.0.2.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.2.10.tar", last modified: Fri May 26 14:54:20 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.2.12.tar", last modified: Sat Jun 10 09:45:49 2023, max compression
```

## Comparing `mml_qae-1.0.2.10.tar` & `mml_qae-1.0.2.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/
--rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.2.10/LICENSE
--rw-rw-rw-   0        0        0     4337 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/PKG-INFO
--rw-rw-rw-   0        0        0     3574 2023-05-26 14:54:14.000000 mml_qae-1.0.2.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/mml_qae/
--rw-rw-rw-   0        0        0     1960 2023-05-26 14:52:53.000000 mml_qae-1.0.2.10/mml_qae/Chinese_dealing.py
--rw-rw-rw-   0        0        0     1916 2023-05-15 13:52:21.000000 mml_qae-1.0.2.10/mml_qae/MoreErrors.py
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.2.10/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     2905 2023-05-15 13:22:26.000000 mml_qae-1.0.2.10/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1407 2023-05-15 13:23:01.000000 mml_qae-1.0.2.10/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     4337 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 14:54:19.000000 mml_qae-1.0.2.10/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2023-05-26 14:53:53.000000 mml_qae-1.0.2.10/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 14:54:20.000000 mml_qae-1.0.2.10/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-26 14:53:51.000000 mml_qae-1.0.2.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.2.12/LICENSE
+-rw-rw-rw-   0        0        0     4396 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/PKG-INFO
+-rw-rw-rw-   0        0        0     3633 2023-06-10 09:35:00.000000 mml_qae-1.0.2.12/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae/
+-rw-rw-rw-   0        0        0     1960 2023-05-26 14:52:53.000000 mml_qae-1.0.2.12/mml_qae/Chinese_dealing.py
+-rw-rw-rw-   0        0        0     1916 2023-05-15 13:52:21.000000 mml_qae-1.0.2.12/mml_qae/MoreErrors.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.2.12/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     3025 2023-06-10 09:42:23.000000 mml_qae-1.0.2.12/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1416 2023-05-26 15:00:20.000000 mml_qae-1.0.2.12/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     4396 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2023-06-10 09:45:38.000000 mml_qae-1.0.2.12/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 09:45:49.000000 mml_qae-1.0.2.12/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-10 09:45:34.000000 mml_qae-1.0.2.12/setup.py
```

### Comparing `mml_qae-1.0.2.10/PKG-INFO` & `mml_qae-1.0.2.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mml_qae
-Version: 1.0.2.10
+Version: 1.0.2.12
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
 + 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
++ 1.0.2.11 2023.6.10 修复了上次更新的遗留问题.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
@@ -51,15 +52,15 @@
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.10  加入中文处理模型(初步).
+> > > + 1.0.2.1  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.2.10/README.md` & `mml_qae-1.0.2.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
 + 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
++ 1.0.2.11 2023.6.10 修复了上次更新的遗留问题.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
@@ -35,15 +36,15 @@
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.10  加入中文处理模型(初步).
+> > > + 1.0.2.1  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.2.10/mml_qae/Chinese_dealing.py` & `mml_qae-1.0.2.12/mml_qae/Chinese_dealing.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.2.10/mml_qae/MoreErrors.py` & `mml_qae-1.0.2.12/mml_qae/MoreErrors.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.2.10/mml_qae/lists_of_number.py` & `mml_qae-1.0.2.12/mml_qae/lists_of_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,37 +13,40 @@
             i=float(i)
         except:
             raise me.DataError2   
     for j in range(0,len(l)-1):
         a=l[j];b=l[j+1]
         if b>a:
             maxium=b
-    return maxium        
+    return int(maxium)        
 
 def cut(path:str,to_name:str,useless_name:str ):
     """给定csv文件路径path(以*.csv结尾)、csv文件中的目标组所在列名、csv文件中的无用列(如序号等)\n返回划分好的四个集合和初步预测模型"""
     try:data1=pd.read_csv(path,header=0)#读入csv数据
     except:raise me.CSVError
     try: 
         data=data1.drop([useless_name],axis=1)#去除无用的id列
         x_data=data.drop([to_name],axis=1)#从data中摘取特征组
         y_data=np.ravel(data[[to_name]])#从data中摘取目标组
     except:raise me.DataError3    
     x_trainset , x_testset , y_trainset , y_testset = tts(x_data,y_data,random_state=1)
     #建立训练集(训练特征组 和 训练目标组)和测试集(测试特征组 和 训练目标组)
-    n=range(1,30)
+    n=range(2,30)
     KNNs=[knc(n_neighbors=i) for i in n]
     scores=[KNNs[i].fit(x_trainset,y_trainset).score(x_testset,y_testset) for i in range(len(KNNs))]
     best=max_of_list(scores)
     model=knc(algorithm="kd_tree",n_neighbors=best)#建立基础模型,用kd_tree算法做超级参数
     return model,x_trainset,y_trainset,x_testset,y_testset
 
 def check(path:str,to_name:str,useless_name:str ):
     """给定csv文件路径path(以*.csv结尾)、csv文件中的目标组所在列名、csv文件中的无用列(如序号等),返回模型预测准确度"""
-    model,x_trainset,y_trainset,x_testset,y_testset=cut(path=path,to_name=to_name,useless_name=useless_name)
+    try:
+        model,x_trainset,y_trainset,x_testset,y_testset=cut(path=path,to_name=to_name,useless_name=useless_name)
+    except:
+        model,x_trainset,y_trainset,x_testset,y_testset=cut(path=path,to_name=to_name)
     model.fit(x_trainset,y_trainset) 
     y_predict=model.predict(x_testset) 
     score=acc(y_testset,y_predict)
     return score
 
 def predict(path:str,to_name:str,useless_name:str,need_predict_list:list):
     """给定csv文件路径path(以*.csv结尾)、csv文件中的目标组所在列名、csv文件中的无用列(如序号等)、需要预测的数据列(以pandas阅读csv文件结果的list格式给入)\n返回预测后的数据目标,过程中如果有错误则返回127错误."""
```

### Comparing `mml_qae-1.0.2.10/mml_qae/one_list_of_number.py` & `mml_qae-1.0.2.12/mml_qae/one_list_of_number.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """给定两个列表(顺序:特征组,目标组)\n无返回值,但直接打开模型预测的可视化界面""" 
     results=make_results(X,Y)
     Y_predict=results.predict()
     plt.scatter(X,Y,color="blue",label="real")
     plt.plot(X,Y_predict,color="orange",label="predicted")
     plt.legend(loc='upper left')
     plt.show()
-def predict(X:list,Y:list,x:float ):
+def predict(X:list,Y:list,x:float,i=False):
     """给定两个列表(顺序:特征组,目标组)和需要预测的数字\n返回需要预测的数字的预测结果(如果返回0则说明该值存在问题(如inf或nan)"""
-    results=make_results(X,Y)
+    results=make_results(X,Y,i)
     try:
         p=results.predict([1,x,np.power(x,2),np.power(x,3),np.power(x,4),np.sin(x),np.tan(x),np.cos(x)])
         return p
     except:
         raise me.DataError5
```

### Comparing `mml_qae-1.0.2.10/mml_qae.egg-info/PKG-INFO` & `mml_qae-1.0.2.12/mml_qae.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mml-qae
-Version: 1.0.2.10
+Version: 1.0.2.12
 Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
 Home-page: https://www.python.org
 Author: ETRO_secondleader
 Author-email: ETRO_secondleader <ETRO_gfyx@163.com>
 Project-URL: Homepage, https://github.com/pypa/mml_qae
 Project-URL: Author's Git, https://github.com/ZYpS-leader?tab=repositories
 Classifier: Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 + 1.0.0 2023.5.14 初代版本.框架构建.
 + 1.0.1 ----------- 略微扩充了方法.
 + 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
 + 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
 + 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
 + 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
 + 1.0.2.10 2023.5.26 中文语言处理(简易版).在测试中本版本出现了一些问题待修复.请见谅.
++ 1.0.2.11 2023.6.10 修复了上次更新的遗留问题.
 ---
 ## 开发者发言
 + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
 + Packages needed
 > + statsmodels
 > + sklearn
 > + jieba
@@ -51,15 +52,15 @@
 > > + 1.0.1
 >      修复1.0.0中的明显问题。
 > > > + 1.0.1.1  加入项目描述.
 > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
 > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
 > >  + 1.0.2
 >      加入封装好的自然语言处理快捷方法。
-> > > + 1.0.2.10  加入中文处理模型(初步).
+> > > + 1.0.2.1  加入中文处理模型(初步).
 > > > + 1.0.2.2  加入英语处理模型.
 > >  + 1.0.3     修复1.0版本的bug和问题。
 > +  1.1 完善版本
 > >  + 1.1.1 加入数据库处理方法。
 > > > + 1.1.1.1 MySQL
 > > > + 1.1.1.2 NoSQL
 > > > + 1.1.1.3 更多数据库
```

### Comparing `mml_qae-1.0.2.10/pyproject.toml` & `mml_qae-1.0.2.12/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mml_qae"
-version = "1.0.2.10"
+version = "1.0.2.12"
 authors = [
   { name="ETRO_secondleader", email="ETRO_gfyx@163.com" },
 ]
 description = "The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning."
 readme = "README.md"
 requires-python = "==3.7.2"
 classifiers = [
```

### Comparing `mml_qae-1.0.2.10/setup.py` & `mml_qae-1.0.2.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='mml_qae',
-      version='1.0.2.10',
+      version='1.0.2.12',
       description='The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='ETRO_secondleader',
       author_email='ETRO_gfyx@163.com',
       url='https://www.python.org', 
       packages=setuptools.find_packages(),
```

