# Comparing `tmp/yunxiao-0.2.0.tar.gz` & `tmp/yunxiao-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.2.0.tar", last modified: Sat Jun 10 06:17:16 2023, max compression
+gzip compressed data, was "yunxiao-0.2.1.tar", last modified: Sat Jun 10 13:47:08 2023, max compression
```

## Comparing `yunxiao-0.2.0.tar` & `yunxiao-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.407701 yunxiao-0.2.0/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    14308 2023-06-10 06:17:16.407701 yunxiao-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.0/README.md
--rw-rw-rw-   0        0        0      905 2023-06-10 06:16:55.000000 yunxiao-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 06:17:16.407701 yunxiao-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.385879 yunxiao-0.2.0/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.0/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    21418 2023-06-10 04:23:34.000000 yunxiao-0.2.0/yunxiao/app.py
--rw-rw-rw-   0        0        0    10205 2023-06-10 06:16:21.000000 yunxiao-0.2.0/yunxiao/web.py
--rw-rw-rw-   0        0        0     5237 2023-06-10 06:16:21.000000 yunxiao-0.2.0/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-06-10 06:17:16.406688 yunxiao-0.2.0/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    14308 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-10 06:17:16.000000 yunxiao-0.2.0/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.407558 yunxiao-0.2.1/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    14308 2023-06-10 13:47:08.392860 yunxiao-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.2.1/README.md
+-rw-rw-rw-   0        0        0      943 2023-06-10 13:46:34.000000 yunxiao-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:47:08.407558 yunxiao-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.386794 yunxiao-0.2.1/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.2.1/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21418 2023-06-10 04:23:34.000000 yunxiao-0.2.1/yunxiao/app.py
+-rw-rw-rw-   0        0        0    10142 2023-06-10 13:46:06.000000 yunxiao-0.2.1/yunxiao/web.py
+-rw-rw-rw-   0        0        0     5237 2023-06-10 06:16:21.000000 yunxiao-0.2.1/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:47:08.391850 yunxiao-0.2.1/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    14308 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 13:47:08.000000 yunxiao-0.2.1/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.2.0/LICENSE` & `yunxiao-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.0/PKG-INFO` & `yunxiao-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.0
+Version: 0.2.1
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.2.0/README.md` & `yunxiao-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.0/pyproject.toml` & `yunxiao-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.2.0"
+version = "0.2.1"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
@@ -22,9 +22,10 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.2.1" = "web 端请求 BUG 修复"
 "0.2.0" = "BUG修复"
 "0.1.9" = "更改鉴权方式，保存鉴权到系统环境变量。当因鉴权失效导致请求失败时，自动更新鉴权并重新发起请求。意图减少更新鉴权的次数。"
```

### Comparing `yunxiao-0.2.0/yunxiao/app.py` & `yunxiao-0.2.1/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.0/yunxiao/web.py` & `yunxiao-0.2.1/yunxiao/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "courseStartTime": starttime,
                 "courseEndTime": endtime,
                 "sort": 1,
                 "sortField": sort_field
             }
-        ).json()
+        )
 
     def find_order_item_all(
             self,
             starttime: str = UsedTime.yymm01,
             endtime: str = UsedTime.today,
             orderstatus: list = None
     ):
@@ -93,15 +93,15 @@
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "startTime": starttime,
                 "endTime": endtime,
                 "orderStatusAllList": orderstatus
             }
-        ).json()
+        )
 
     def student_course_card(self, page_num: int = 1, page_size: int = 10000):
         """
         取得所有学员的课程卡片。
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
@@ -113,15 +113,15 @@
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": False,
                 "remainAmountMin": "1",
                 "remainAmountMax": ""
             }
-        ).json()
+        )
 
     def find_student_course_amount(self, page_num: int = 1, page_size: int = 10000):
         """
         取得所有学员的课时统计数据。
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
@@ -132,15 +132,15 @@
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": False,
                 "status": [1]
             }
-        ).json()
+        )
 
     def find_student_course_fee(
             self,
             display_history: int = False,
             status: list = None,
             student_name: str = None,
             page_num: int = 1,
@@ -162,15 +162,15 @@
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": display_history,
                 "status": status,
                 "studentName": student_name
             }
-        ).json()
+        )
 
     def teacher_arrange(
             self,
             teacher_id: int,
             start_date: str = UsedTime.weekstrat,
             end_date: str = UsedTime.weekend,
             page_num: int = 1,
@@ -198,15 +198,15 @@
                 "classRoomIds": [],
                 "studentIds": [],
                 "reserve": 0,
                 "displayCompletedClass": False,
                 "courseStatusList": [],
                 "page": {"pageNum": page_num, "pageSize": page_size}
             }
-        ).json()
+        )
 
     def find_payment_list(
             self,
             pay_start_date: str = UsedTime.weekstrat,
             pay_end_date: str = UsedTime.weekend,
             order_status: int = "",
             group_no: str = "",
@@ -238,15 +238,15 @@
                 "orderEndTime": "",
                 "btransactionId": "",
                 "aymentAccountCustomIds": [],
                 "confirmStatusList": [],
                 "revenueType": "",
                 "page": {"pageNum": page_num, "pageSize": page_size}
             }
-        ).json()
+        )
 
     def find_receipt(
             self,
             order_id: int,
             payment_group_id: int
     ):
         """
@@ -259,15 +259,15 @@
             method="get",
             url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/findReceipt",
             params={
                 "orderInfoId": order_id,
                 "paymentGroupId": payment_group_id,
                 "_t_": UsedTime.stamp
             }
-        ).json()
+        )
 
     def snap_info_by_payment_group_id(
             self,
             order_id: int,
             payment_group_id: int
     ):
         """
@@ -280,15 +280,15 @@
             method="get",
             url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/snapInfoByPaymentGroupId",
             params={
                 "orderId": order_id,
                 "paymentGroupId": payment_group_id,
                 "_t_": UsedTime.stamp
             }
-        ).json()
+        )
 
     def receipt(
             self,
             order_id: int,
             payment_group_id: int
     ):
         """
```

### Comparing `yunxiao-0.2.0/yunxiao/yunxiao.py` & `yunxiao-0.2.1/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.2.0/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.2.1/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.2.0
+Version: 0.2.1
 Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

