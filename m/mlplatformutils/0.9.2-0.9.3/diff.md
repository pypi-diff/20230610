# Comparing `tmp/mlplatformutils-0.9.2.tar.gz` & `tmp/mlplatformutils-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.2.tar", last modified: Fri Jun  9 22:20:49 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.3.tar", last modified: Sat Jun 10 01:12:48 2023, max compression
```

## Comparing `mlplatformutils-0.9.2.tar` & `mlplatformutils-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:20:49.639611 mlplatformutils-0.9.2/
--rw-rw-rw-   0        0        0     6101 2023-06-09 22:20:49.640612 mlplatformutils-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.2/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-09 22:20:49.644612 mlplatformutils-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-06-09 22:15:57.000000 mlplatformutils-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:20:49.311977 mlplatformutils-0.9.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 22:20:49.346989 mlplatformutils-0.9.2/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.2/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:20:49.636611 mlplatformutils-0.9.2/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    13534 2023-06-09 20:27:01.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    11009 2023-06-09 21:55:11.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-09 22:16:05.000000 mlplatformutils-0.9.2/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:20:49.411520 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6101 2023-06-09 22:20:48.000000 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-09 22:20:49.000000 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:20:48.000000 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-09 22:20:49.000000 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 22:20:49.000000 mlplatformutils-0.9.2/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/
+-rw-rw-rw-   0        0        0     6101 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-10 01:12:48.743474 mlplatformutils-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-06-10 01:12:37.000000 mlplatformutils-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.556629 mlplatformutils-0.9.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.580639 mlplatformutils-0.9.3/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.3/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-10 01:12:32.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.615703 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6101 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.2/PKG-INFO` & `mlplatformutils-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.2
+Version: 0.9.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.2/setup.py` & `mlplatformutils-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.2',
+    version='0.9.3',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/pandasutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,18 @@
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("delta"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
                                              "DataReadSource":dataprop})
     return pandas_df
 
@@ -77,20 +75,18 @@
     #pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs, use_legacy_dataset= True).to_pandas()
     pandas_df = pq.ParquetDataset(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
                                              "DataReadSource":dataprop})
 
     return pandas_df
@@ -151,20 +147,18 @@
     fs = pyarrow.fs.PyFileSystem(handler)
     pandas_df = pq.ParquetDataset(parquet_files_from_path_list,filesystem=fs).read().to_pandas()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
                                              "DataReadSource":dataprop})
     return pandas_df
 
@@ -207,20 +201,18 @@
     )
     """
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)
 
     if dataprop is None:
         dataprop = str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
-                                       "Type":"ADLS",\
-                                        "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
+                                       "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataWriteColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]",\
                                              "DataWriteTarget":dataprop})
 
     print("File Write Successful at "+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH+" !")
```

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.3/src/mlplatformutils/core/sparkutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,20 +32,18 @@
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
 
     df = spark.read.format(file_format).load(file_path)
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: file_path,\
-                                    "Type":"ADLS",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: file_path,\
-                                    "Type":"ADLS",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(file_path),\
                                              "FileFormat_"+sourcePostfix:str(file_format),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]",\
                                              "DataReadSource":dataprop})
 
     return df
@@ -86,20 +84,18 @@
         else:
             df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     targetPostfix,dataprop=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)  
     if dataprop is None:
         dataprop = str({"DataWriteTarget_"+targetPostfix: file_path,\
-                                    "Type":"ADLS",\
-                                    "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+targetPostfix: file_path,\
-                                    "Type":"ADLS",\
-                                    "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"ADLS"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+targetPostfix: str(file_path),\
                                              "FileFormat_"+targetPostfix:str(file_format),\
                                              "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]",\
                                              "DataWriteTarget":dataprop})
     
     return
@@ -117,20 +113,18 @@
                 option("kustoAadAuthorityID", kustoOptions["kustoAADAuthorityID"]). \
                 load()
     
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: "ADX-Cluster "+str(kustoOptions["kustoCluster"])+" ADX-Database"+str(kustoOptions["kustoDatabase"])+ " ADX-Table "+str(kustoOptions["kustoTable"]),\
-                                    "Type":"ADX",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]"})
+                                    "Type":"ADX"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: "ADX-Cluster "+str(kustoOptions["kustoCluster"])+" ADX-Database"+str(kustoOptions["kustoDatabase"])+ " ADX-Table "+str(kustoOptions["kustoTable"]),\
-                                    "Type":"ADX",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]"})
+                                    "Type":"ADX"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"KustoDataReadCluster_"+sourcePostfix: str(kustoOptions["kustoCluster"]),\
                                         "KustoDataReadDatabase_"+sourcePostfix: str(kustoOptions["kustoDatabase"]),\
                                         "KustoDataReadQuery_"+sourcePostfix: str(kustoOptions["kustoTable"]),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]",\
                                         "DataReadSource":dataprop})            
     return kustoDf
@@ -147,19 +141,17 @@
         .option("hostNameInCertificate", "*.database.windows.net") \
         .load()
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: "SQL SERVER INSTANCE "+str(SQL_SERVER_INSTANCE)+" SQL Query "+str(Query),\
-                                    "Type":"ADX",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"AzureSQL"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: "SQL SERVER INSTANCE "+str(SQL_SERVER_INSTANCE)+" SQL Query "+str(Query),\
-                                    "Type":"ADX",\
-                                    "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]"})
+                                    "Type":"AzureSQL"})
     dataprop = dataprop.replace("'",'"')
     LineageLogger.update_vertex(documentId, {"SqlDataReadServer_"+sourcePostfix: str(SQL_SERVER_INSTANCE),\
                                         "SqlDataReadQuery_"+sourcePostfix: str(Query),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(df.columns)+"]",\
                                         "DataReadSource":dataprop}) 
     return df
```

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.3/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.2
+Version: 0.9.3
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.2/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.3/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

