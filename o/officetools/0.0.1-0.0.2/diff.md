# Comparing `tmp/officetools-0.0.1.tar.gz` & `tmp/officetools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\officetools\dist\.tmp-t1pu04yb\officetools-0.0.1.tar", last modified: Fri Jun  9 20:17:05 2023, max compression
+gzip compressed data, was "C:\Users\u0138780\yForecasting_Github\officetools\dist\.tmp-4pg4jcvv\officetools-0.0.2.tar", last modified: Fri Jun  9 22:26:06 2023, max compression
```

## Comparing `officetools-0.0.1.tar` & `officetools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 20:17:05.971700 officetools-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-09 14:57:12.000000 officetools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      737 2023-06-09 20:17:05.970700 officetools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-06-09 14:57:12.000000 officetools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 20:17:05.915721 officetools-0.0.1/officetools/
--rw-rw-rw-   0        0        0        2 2023-06-09 14:55:05.000000 officetools-0.0.1/officetools/__init__.py
--rw-rw-rw-   0        0        0     3471 2023-06-09 17:37:28.000000 officetools-0.0.1/officetools/kpi.py
-drwxrwxrwx   0        0        0        0 2023-06-09 20:17:05.967703 officetools-0.0.1/officetools.egg-info/
--rw-rw-rw-   0        0        0      737 2023-06-09 20:17:05.000000 officetools-0.0.1/officetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-09 20:17:05.000000 officetools-0.0.1/officetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 20:17:05.000000 officetools-0.0.1/officetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-09 20:17:05.000000 officetools-0.0.1/officetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 20:17:05.000000 officetools-0.0.1/officetools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-09 20:17:05.971700 officetools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1279 2023-06-09 15:09:55.000000 officetools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:26:06.014052 officetools-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-09 14:57:12.000000 officetools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      737 2023-06-09 22:26:06.013061 officetools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-06-09 14:57:12.000000 officetools-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 22:26:05.962112 officetools-0.0.2/officetools/
+-rw-rw-rw-   0        0        0       46 2023-06-09 21:32:19.000000 officetools-0.0.2/officetools/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 21:28:31.000000 officetools-0.0.2/officetools/_version.py
+-rw-rw-rw-   0        0        0     3829 2023-06-09 22:14:17.000000 officetools-0.0.2/officetools/kpi.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:26:05.999038 officetools-0.0.2/officetools.egg-info/
+-rw-rw-rw-   0        0        0      737 2023-06-09 22:26:05.000000 officetools-0.0.2/officetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-06-09 22:26:05.000000 officetools-0.0.2/officetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:26:05.000000 officetools-0.0.2/officetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-09 22:26:05.000000 officetools-0.0.2/officetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-09 22:26:05.000000 officetools-0.0.2/officetools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 22:26:06.015052 officetools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1582 2023-06-09 21:40:28.000000 officetools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:26:06.008033 officetools-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1389 2023-06-09 22:21:36.000000 officetools-0.0.2/tests/test_copy_excel_cell.py
+-rw-rw-rw-   0        0        0     2001 2023-06-09 22:21:36.000000 officetools-0.0.2/tests/test_process_csv.py
```

### Comparing `officetools-0.0.1/LICENSE` & `officetools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `officetools-0.0.1/PKG-INFO` & `officetools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: officetools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Forecasting package for office automation
 Home-page: https://github.com/yForecasting/officetools
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `officetools-0.0.1/officetools/kpi.py` & `officetools-0.0.2/officetools/kpi.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         Notes:
             - This function uses the openpyxl library to read and write Excel files.
             - The source cell value is copied from the source file and pasted into the destination file.
             - The source and destination files must exist and be in the .xlsx format.
             - The source and destination sheets must exist in their respective files.
             - If the destination cell already contains a value, it will be overwritten.
         """
+    # D1
     # copy_excel_cell(
     #    source_file='source.xlsx',
     #    source_sheet='Sheet1',
     #    source_cell='A1',
     #    destination_file='destination.xlsx',
     #    destination_sheet='Sheet2',
     #    destination_cell='B2'
@@ -54,32 +55,42 @@
     # Save the changes to the destination workbook
     destination_workbook.save(destination_file)
 
     # Close the workbooks
     source_workbook.close()
     destination_workbook.close()
 
-
 def process_csv(csv_file):
     """
     Read the parameters for the copy_excel_cell function from a CSV file and execute it for each line.
 
     Parameters:
         csv_file (str): The path to the CSV file containing the function parameters.
 
     Returns:
         None
     """
+    # D3
     # process_csv('parameters.csv')
-    #  The CSV file should have the following format:
+    # The CSV file should have the following format:
+    # column headers
     # source_file1, source_sheet1, source_cell1, destination_file1, destination_sheet1, destination_cell1
     # source_file2, source_sheet2, source_cell2, destination_file2, destination_sheet2, destination_cell2
 
-    with open(csv_file, 'r') as file:
-        csv_reader = csv.reader(file)
+    with open(csv_file, 'r', newline='') as file:
+        # Read the first line of the CSV file
+        first_line = file.readline().strip()
+
+        # Determine the delimiter based on the first line
+        delimiter = ',' if ',' in first_line else ';'
+
+        # Reset the file pointer to the beginning
+        file.seek(0)
+
+        csv_reader = csv.reader(file, delimiter=delimiter)
         next(csv_reader)  # Skip the header row if present
 
         for line in csv_reader:
             # Extract the parameters from the CSV line
             source_file, source_sheet, source_cell, destination_file, destination_sheet, destination_cell = line
 
             # Call the copy_excel_cell function with the extracted parameters
```

### Comparing `officetools-0.0.1/officetools.egg-info/PKG-INFO` & `officetools-0.0.2/officetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: officetools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Forecasting package for office automation
 Home-page: https://github.com/yForecasting/officetools
 Author: Yves R. Sagaert
 Author-email: yves.r.sagaert@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `officetools-0.0.1/setup.py` & `officetools-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,31 @@
 import setuptools
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+import re
+VERSIONFILE="officetools/_version.py"
+verstrline = open(VERSIONFILE, "rt").read()
+VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
+mo = re.search(VSRE, verstrline, re.M)
+if mo:
+    verstr = mo.group(1)
+else:
+    raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
+
 setuptools.setup(
     author="Yves R. Sagaert",
     author_email="yves.r.sagaert@gmail.com",
     name='officetools',
     license="GNU GPLv3",
     description='Forecasting package for office automation',
-    version='v0.0.1',
+    version=verstr,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/yForecasting/officetools',
     packages=setuptools.find_packages(),
     include_package_data=True,
     python_requires=">=3.5",
     # Enable install requires when publishing on the normal PyPi
```

