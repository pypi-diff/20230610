# Comparing `tmp/yunxiao-0.1.8.tar.gz` & `tmp/yunxiao-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.8.tar", last modified: Thu May 18 01:49:34 2023, max compression
+gzip compressed data, was "yunxiao-0.1.9.tar", last modified: Sat Jun 10 02:56:51 2023, max compression
```

## Comparing `yunxiao-0.1.8.tar` & `yunxiao-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.312107 yunxiao-0.1.8/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    14304 2023-05-18 01:49:34.312107 yunxiao-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.1.8/README.md
--rw-rw-rw-   0        0        0      587 2023-05-18 01:49:19.000000 yunxiao-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-18 01:49:34.313108 yunxiao-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.305101 yunxiao-0.1.8/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.8/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    19319 2023-05-18 01:48:19.000000 yunxiao-0.1.8/yunxiao/app.py
--rw-rw-rw-   0        0        0     8914 2023-05-14 13:28:34.000000 yunxiao-0.1.8/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.8/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-05-18 01:49:34.311106 yunxiao-0.1.8/yunxiao.egg-info/
--rw-rw-rw-   0        0        0    14304 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 01:49:34.000000 yunxiao-0.1.8/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.312584 yunxiao-0.1.9/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    14308 2023-06-10 02:56:51.312584 yunxiao-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13817 2023-05-14 13:37:36.000000 yunxiao-0.1.9/README.md
+-rw-rw-rw-   0        0        0      882 2023-06-10 02:03:21.000000 yunxiao-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 02:56:51.312584 yunxiao-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.306036 yunxiao-0.1.9/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.9/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    21350 2023-06-10 02:31:52.000000 yunxiao-0.1.9/yunxiao/app.py
+-rw-rw-rw-   0        0        0    10138 2023-06-10 02:37:03.000000 yunxiao-0.1.9/yunxiao/web.py
+-rw-rw-rw-   0        0        0     4077 2023-06-10 01:55:31.000000 yunxiao-0.1.9/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-06-10 02:56:51.311578 yunxiao-0.1.9/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0    14308 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 02:56:51.000000 yunxiao-0.1.9/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.8/LICENSE` & `yunxiao-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.8/PKG-INFO` & `yunxiao-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.8
-Summary: An API tool for Cloud School Education Institution Management System.
+Version: 0.1.9
+Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `yunxiao-0.1.8/README.md` & `yunxiao-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.8/yunxiao/app.py` & `yunxiao-0.1.9/yunxiao/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
-from .yunxiao import AppOAuth, UsedTime
+import logging
+import os
+from .yunxiao import YunXiao, UsedTime
+import requests
 
 
-class App(AppOAuth):
+class App(YunXiao):
     def __init__(self, userphone: str, password: str, campus: list = None):
         """
         初始化，输入用户账号密码，以及要操作的校区。
         :param userphone: 账号
         :param password: 密码
         :param campus: 校区
         """
@@ -16,71 +19,102 @@
             self.campus = campus
 
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-report/report/"
         self.orderpath = "https://yunxiao.xiaogj.com/api/cs-edu/order"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-edu/"
         self.crmpath = "https://yunxiao.xiaogj.com/api/cs-crm/"
 
+    def request(self, **kwargs):
+        response = requests.request(
+            method=kwargs.get("method"),
+            url=kwargs.get("url"),
+            json=kwargs.get("json"),
+            params=kwargs.get("params"),
+            headers={"x3-authentication": os.environ.get("YUNXIAO_OAUTH_TOKEN")}
+        )
+
+        if response.status_code != 200:
+            logging.error("无法到连接云校服务器。")
+            return "无法到连接云校服务器。"
+
+        if response.json()["code"] == 401:
+            logging.error(response.json()["msg"])
+            self.renew_token()
+            response = requests.request(
+                method=kwargs.get("method"),
+                url=kwargs.get("url"),
+                json=kwargs.get("json"),
+                params=kwargs.get("params"),
+                headers={"x3-authentication": os.environ.get("YUNXIAO_OAUTH_TOKEN")}
+            )
+
+        return response.json()
+
     def find_now_data_report(self):
         """
         [数据/当前数据]
         总剩余学费，总欠缴费用，总欠缴物品费用，在读学员。
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findNowDataReport",
             json={"campusIds": self.campus, "_t_": UsedTime.stamp}
-        ).json()
+        )
 
     def find_course_money(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         课消数据。
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findCourseMoney",
             json={"campusIds": self.campus, "date": date, "dateType": datetype, "_t_": UsedTime.stamp}
-        ).json()
+        )
 
     def find_tuition(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         学费收入数据。
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findTuition",
             json={"campusIds": self.campus, "date": date, "dateType": datetype, "_t_": UsedTime.stamp}
-        ).json()
+        )
 
     def find_refund_money(self, date: str = UsedTime.yymm, datetype: int = 1):
         """
         学费退费数据
         :param date: 月份，格式示例： 2023-02
         :param datetype:
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findRefundMoney",
             json={"campusIds": self.campus, "date": date, "dateType": datetype, "_t_": UsedTime.stamp}
-        ).json()
+        )
 
     # [数据][每日简报]
     def find_data_report(self, date: str = UsedTime.today):
         """
         每日简报。
         :param date: 日期，格式示例 2023-02-01
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findDataReport",
             json={"campusIds": self.campus, "date": date, "_t_": UsedTime.stamp}
-        ).json()
+        )
 
     # [数据][报表][校区数据]
     def find_data_report_list(
             self,
             startdate: str = UsedTime.yymm01,
             enddate: str = UsedTime.today,
             orderbycampus: int = 1
@@ -88,72 +122,75 @@
         """
         某日到某日数据。
         :param startdate: 起始日期
         :param enddate: 截至日期
         :param orderbycampus:
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findDataReportList",
             json={
                 "campusIds": self.campus,
                 "startDate": startdate,
                 "endDate": enddate,
                 "orderByCampus": orderbycampus,
                 "_t_": UsedTime.stamp
             }
-        ).json()
+        )
 
     def find_student_course_fee(
             self,
             curriculumids: list = None,
             status: list = None,
             studentname: str = None
     ):
         """
         学生数据 - 费用报表。
         :param curriculumids: 课程ID列表
         :param status: 学生状态列表
         :param studentname: 按学生姓名检索
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findStudentCourseFee",
             json={
                 "campusIds": self.campus,
                 "curriculumIds": curriculumids,
                 "status": status,
                 "studentName": studentname,
                 "_t_": UsedTime.stamp
             }
-        ).json()
+        )
 
     def find_student_course_amount(
             self,
             curriculumids: list = None,
             status: list = None,
             studentname: str = None
     ):
         """
         学生数据 - 课时报表。
         :param curriculumids: 课程ID列表
         :param status: 学生状态列表
         :param studentname: 按学生姓名检索
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findStudentCourseAmount",
             json={
                 "campusIds": self.campus,
                 "curriculumIds": curriculumids,
                 "status": status,
                 "studentName": studentname,
                 "_t_": UsedTime.stamp
             }
-        ).json()
+        )
 
     def order(
             self,
             ordertype: int = 0,
             searchname: str = "",
             orderstatuslist: list = None,
             starttime: str = UsedTime.yymm01,
@@ -167,48 +204,51 @@
         :param searchname:
         :param orderstatuslist:
         :param starttime:
         :param endtime:
         :param pagesize:
         :return:
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "orderType": ordertype,
-            "searchName": searchname,
-            "campusIds": self.campus,
-            "teacherList": [],
-            "sourceTypeList": [],
-            "productTypeList": [],
-            "orderStatusList": orderstatuslist,
-            "oweFeeList": [],
-            "startTime": starttime,
-            "endTime": endtime,
-            "page": {
-                "pageNum": 1,
-                "pageSize": pagesize
+        return self.request(
+            method="post",
+            url=self.orderpath + "Info/pageAdbOrder",
+            json={
+                "_t_": UsedTime.stamp,
+                "orderType": ordertype,
+                "searchName": searchname,
+                "campusIds": self.campus,
+                "teacherList": [],
+                "sourceTypeList": [],
+                "productTypeList": [],
+                "orderStatusList": orderstatuslist,
+                "oweFeeList": [],
+                "startTime": starttime,
+                "endTime": endtime,
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": pagesize
+                }
             }
-        }
-        return self.session.post(url=self.orderpath + "Info/pageAdbOrder", json=data).json()
+        )
 
     def order_info(self, orderinfoid: int = 0):
         """
         [收银管理/订单管理/订单详情]
         查询订单详情。
         :param orderinfoid:
         :return:
         """
-        params = {
-            "_t_": UsedTime.stamp,
-            "orderInfoId": orderinfoid,
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.orderpath + "Info/get",
-            params=params
-        ).json()
+            params={
+                "_t_": UsedTime.stamp,
+                "orderInfoId": orderinfoid,
+            }
+        )
 
     # [工作台][订单管理][退费]
     def refund_order(
             self,
             searchname: str = "",
             starttime: str = UsedTime.yymm01,
             endtime: str = UsedTime.today,
@@ -219,133 +259,133 @@
         查询退费订单。
         :param searchname:
         :param starttime:
         :param endtime:
         :param pagesize:
         :return:
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "orderType": 2,
-            "searchName": searchname,
-            "campusIds": self.campus,
-            "productTypeList": [],
-            "startTime": starttime,
-            "endTime": endtime,
-            "page": {
-                "pageNum": 1,
-                "pageSize": pagesize
-            }
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.orderpath + "Refund/adbRefundOrderInfoPage",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "orderType": 2,
+                "searchName": searchname,
+                "campusIds": self.campus,
+                "productTypeList": [],
+                "startTime": starttime,
+                "endTime": endtime,
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": pagesize
+                }
+            }
+        )
 
     def course_absent(
             self,
             starttime: str = UsedTime.yymm01,
             endtime: str = UsedTime.today,
             pagesize: int = 1
     ):
         """
         [教务管理/缺勤管理]
         :param starttime: 起始时间
         :param endtime: 结束时间
         :param pagesize: 单页项目数量
         :return:
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "campusIds": self.campus,
-            "remedyStatusList": [0],
-            "courseRelations": [],
-            "type": 1,
-            "status": [1],
-            "startTime": starttime,
-            "endTime": endtime,
-            "page": {
-                "pageNum": 1,
-                "pageSize": pagesize
-            }
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "courseAbsent/list",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "campusIds": self.campus,
+                "remedyStatusList": [0],
+                "courseRelations": [],
+                "type": 1,
+                "status": [1],
+                "startTime": starttime,
+                "endTime": endtime,
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": pagesize
+                }
+            }
+        )
 
     def company_course(
             self,
             date: str = UsedTime.today,
             teacherids: list = None,
             pagesize: int = 1
     ):
         """
         [教务管理/课表点名/全部课表]
         :param date:
         :param teacherids:
         :param pagesize:
         :return:
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "date": date,
-            "campusIds": self.campus,
-            "teacherIds": teacherids,
-            "classStatusList": [0],
-            "page": {
-                "pageNum": 1,
-                "pageSize": pagesize
-            }
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "arrange/getCompanyCourse",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "date": date,
+                "campusIds": self.campus,
+                "teacherIds": teacherids,
+                "classStatusList": [0],
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": pagesize
+                }
+            }
+        )
 
     # [工作台][学员][学员卡包]
     def student_card(
             self,
             studentid=None
     ):
         """
         查看学员的课程卡包
         :param studentid: 学生ID
         :return: json数据
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "studentId": studentid,
-            "page": {
-                "pageNum": 1,
-                "pageSize": 20
-            }
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "cardInfo/findStudentCard",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "studentId": studentid,
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": 999
+                }
+            }
+        )
 
     # [工作台][学员][就读课程]
     def student_attend_course(
             self,
             studentid: str = None
     ):
-        data = {
-            "_t_": UsedTime.stamp,
-            "studentId": studentid,
-            "page": {
-                "pageNum": 1,
-                "pageSize": 20
-            }
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "courseStudent/findStudentAttendCourse",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "studentId": studentid,
+                "page": {
+                    "pageNum": 1,
+                    "pageSize": 999
+                }
+            }
+        )
 
     # [工作台][学员][就读课程][出入班记录]
     def operation_record_list(
             self,
             studentid: int = None,
             curriculum_id: int = None,
             campus_ids_index: int = None,
@@ -357,84 +397,95 @@
         :param campus_ids_index: 实例中选择的校区列表索引，必须从中列表中选择一个。
         :param studentid:
         :param curriculum_id:
         :return:
         """
         if campus_ids_index:
             campus_id = self.campus[campus_ids_index]
-        data = {
-            "_t_": UsedTime.stamp,
-            "campusId": campus_id,
-            "studentId": str(studentid),
-            "curriculumId": curriculum_id
-        }
-        return self.session.post(
+
+        return self.request(
+            method="post",
             url=self.edupath + "student/findOperationRecordList",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "campusId": campus_id,
+                "studentId": str(studentid),
+                "curriculumId": curriculum_id
+            }
+        )
 
     # [工作台][班级]
     def class_info_page(
             self,
             classstatus=0,
             curriculumids: list = None,
             teacherids: list = None
     ):
-        data = {
-            "_t_": UsedTime.stamp,
-            "orgTag": 1,
-            "campusIds": self.campus,
-            "classStatus": classstatus,
-            "curriculumIds": curriculumids,
-            "teacherIds": teacherids,
-            "page": {"pageNum": 1, "pageSize": 500}
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "classInfo/page",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "orgTag": 1,
+                "campusIds": self.campus,
+                "classStatus": classstatus,
+                "curriculumIds": curriculumids,
+                "teacherIds": teacherids,
+                "page": {"pageNum": 1, "pageSize": 500}
+            }
+        )
 
     def class_info(self, classid: int = None):
         """
         查询指定班级信息
         :param classid: 班级id
         :return:
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url=self.edupath + "classInfo/getClassInfoVo",
-            params={"_t_": UsedTime.stamp, "classId": classid}
-        ).json()
+            params={
+                "_t_": UsedTime.stamp,
+                "classId": classid
+            }
+        )
 
     def class_student(self, classid: int = None, inout: int = 1):
         """
         查询指定班级的学员
         :param classid:     班级id
         :param inout:       [1]当前在班学员 [2]历史学员
         :return:
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url=self.edupath + "classStudent/findClassStudent",
-            params={"_t_": UsedTime.stamp, "classId": classid, "inout": inout}
-        ).json()
+            params={
+                "_t_": UsedTime.stamp,
+                "classId": classid,
+                "inout": inout
+            }
+        )
 
     def class_arrange(self, classid: int = None):
         """
         查询指定班级排课。
         :param classid: 班级id
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "arrange/list",
             json={
                 "_t_": UsedTime.stamp,
                 "classId": classid,
                 "isDesc": False,
                 "status": None
             }
-        ).json()
+        )
 
     def arrange(
             self,
             starttime: str = None,
             endtime: str = None,
             page_num: int = 1,
             page_size: int = 99999
@@ -443,120 +494,129 @@
         排课管理。
         :param page_num:
         :param page_size:
         :param starttime: 查询起始时间
         :param endtime: 查询截止时间
         :return:
         """
-        data = {
-            "_t_": UsedTime.stamp,
-            "campusIds": self.campus,
-            "startDate": starttime,
-            "endDate": endtime,
-            "courseStatusList": [0, 1],
-            "displayCompletedClass": False,
-            "page": {"pageNum": page_num, "pageSize": page_size}
-        }
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "arrange/page",
-            json=data
-        ).json()
+            json={
+                "_t_": UsedTime.stamp,
+                "campusIds": self.campus,
+                "startDate": starttime,
+                "endDate": endtime,
+                "courseStatusList": [0, 1],
+                "displayCompletedClass": False,
+                "page": {"pageNum": page_num, "pageSize": page_size}
+            }
+        )
 
+    # 查询所有在开的课程
     def curriculum(
             self,
             searchname: str = None,
             haltsalelist: list = None
     ):
         """
         查询所有在开的课程
         :param searchname: 查找关键字。
         :param haltsalelist: 是否在售。0>在售 1>停售
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "curriculum/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "curriculumName": searchname,
                 "haltSaleList": haltsalelist,
                 "page": {
                     "pageNum": 1,
-                    "pageSize": 500
+                    "pageSize": 999
                 }
             }
-        ).json()
+        )
 
+    # 查询所有在开的课程
     def update_curriculum_price_item(
             self,
             searchname: str = None,
             haltsalelist: list = None
     ):
         """
         查询所有在开的课程
         :param searchname: 查找关键字。
         :param haltsalelist: 是否在售。0>在售 1>停售
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "curriculum/updateCurriculumPriceItem",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "curriculumName": searchname,
                 "haltSaleList": haltsalelist,
                 "page": {
                     "pageNum": 1,
                     "pageSize": 500
                 }
             }
-        ).json()
+        )
 
+    # 设为曾就读学生。
     def become_history(
             self,
             studentlist: list
     ):
         """
         设为曾就读学生。
         :param studentlist: 学生ID
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "student/becomeHistory",
             json={
                 "_t_": UsedTime.stamp, "studentIds": studentlist
             }
-        ).json()
+        )
 
+    # 设学生为停课状态。
     def student_suspend_course(
             self,
             student_id: str,
             suspend_course_date: str = UsedTime.today,
             remove_class: int = True
     ):
         """
         设为停课状态。
         :param student_id: 学生ID
         :param suspend_course_date: 停课时间。0000-00-00
         :param remove_class: 是否从班级中移除
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "student/studentSuspendCourse",
             json={
                 "_t_": UsedTime.stamp,
                 "recoveryCourseDate": "",
                 "extendDays": "",
                 "removeClass": remove_class,
                 "studentId": student_id,
                 "suspendCourseDate": suspend_course_date,
                 "type": 0
             }
-        ).json()
+        )
 
+    # [教务管理 / 学员] 列出学生
     def student_list(
             self,
             curriculumids: list = None,
             classids: list = None,
             name: str = "",
             status: list = None,
             class_student_status: int = 0
@@ -569,57 +629,62 @@
         :param name: 姓名查询关键字
         :param status: 学员状态 0>未收费 1>在读 6>曾就读 7>停课 99>无效学员
         :param class_student_status: 0>不筛选 1>未入班 2>已入班
         :return:
         """
         if status is None:
             status = [1, 7]
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.crmpath + "student/list",
             json={
                 "_t_": UsedTime.stamp,
                 "name": name,
                 "campusIds": self.campus,
                 "status": status,
                 "intentionStatus": 0,
                 "curriculumIds": curriculumids,
                 "classIds": classids,
                 "classStudentStatus": class_student_status,
                 "orgTag": 1,
                 "page": {"pageNum": 1, "pageSize": 1000000}
             }
-        ).json()
+        )
 
+    # [教务管理 / 学员 / 学员详情] 查询学员详细信息。
     def student_info(
             self,
             studentid: int = None
     ):
         """
         [教务管理/学员/学员详情]
         查询学员详细信息。
         :param studentid: 学生ID
         :return:
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url=self.crmpath + "student/getContainFace",
             params={"_t_": UsedTime.stamp, "id": studentid, "companyId": 658811}
-        ).json()
+        )
 
+    # 查询老师
     def get_teacher_list(
             self,
             querykey: str = None
     ):
         """
         查询老师
         :param querykey: 关键词检索
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.crmpath + "teacher/pageList",
             json={
                 "_t_": UsedTime.stamp,
                 "queryKey": querykey,
                 "campusIds": self.campus,
                 "statusList": [1],
                 "page": {"pageNum": 1, "pageSize": 1000}
             }
-        ).json()
+        )
```

### Comparing `yunxiao-0.1.8/yunxiao/web.py` & `yunxiao-0.1.9/yunxiao/web.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,66 @@
-from .yunxiao import WebOAuth, UsedTime
+import logging
+import os
 
+import requests
 
-class Web(WebOAuth):
+from .yunxiao import YunXiao, UsedTime
+
+
+class Web(YunXiao):
     def __init__(self, userphone: str, password: str, campus: list = None):
         super().__init__(userphone, password)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-pc-edu/"
 
+    def request(self, **kwargs):
+        response = requests.request(
+            method=kwargs.get("method"),
+            url=kwargs.get("url"),
+            json=kwargs.get("json"),
+            params=kwargs.get("params"),
+            headers={"Cookie": os.environ.get("YUNXIAO_OAUTH_COOKIE")}
+        )
+
+        if response.status_code != 200:
+            logging.error("无法到连接云校服务器。")
+            return "无法到连接云校服务器。"
+
+        if response.json()["code"] == 401:
+            logging.error(response.json()["msg"])
+            self.renew_token()
+            response = requests.request(
+                method=kwargs.get("method"),
+                url=kwargs.get("url"),
+                json=kwargs.get("json"),
+                params=kwargs.get("params"),
+                headers={"Cookie": os.environ.get("YUNXIAO_OAUTH_COOKIE")}
+            )
+
+        return response.json()
+
     def find_course_sign_charge(
             self,
             starttime: str = None,
             endtime: str = None,
             sort_field: str = "operationTime"
     ):
         """
         查询课消记录
         :param sort_field: 时间筛选模式。 <operationTime> - 操作时间
         :param starttime:
         :param endtime:
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findCourseSignCharge",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "courseStartTime": starttime,
                 "courseEndTime": endtime,
@@ -48,15 +80,16 @@
         :param starttime: 起始时间
         :param endtime: 结束时间
         :param orderstatus: 订单状态。
         :return:
         """
         if orderstatus is None:
             orderstatus = [1, 4, 6]
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findOrderItemAll/page",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": 1, "pageSize": 10000},
                 "campusIds": self.campus,
                 "startTime": starttime,
                 "endTime": endtime,
@@ -67,15 +100,16 @@
     def student_course_card(self, page_num: int = 1, page_size: int = 10000):
         """
         取得所有学员的课程卡片。
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "studentCourseCard/report",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": False,
                 "remainAmountMin": "1",
@@ -86,15 +120,16 @@
     def find_student_course_amount(self, page_num: int = 1, page_size: int = 10000):
         """
         取得所有学员的课时统计数据。
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findStudentCourseAmount",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": False,
                 "status": [1]
@@ -114,15 +149,16 @@
         :param student_name: 学员姓名。
         :param status: 学员状态。[0:"未收费"][1:"在读"][7:"停课"]
         :param display_history: 是否显示曾就读。<True:显示><False:不显示>
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findStudentCourseFee",
             json={
                 "_t_": UsedTime.stamp,
                 "page": {"pageNum": page_num, "pageSize": page_size},
                 "campusIds": self.campus,
                 "displayHistory": display_history,
                 "status": status,
@@ -143,15 +179,16 @@
         :param teacher_id: 查询的老师ID
         :param start_date: 起始日期，默认为本周一
         :param end_date: 结束日期，默认为本周日
         :param page_num: 页数。
         :param page_size: 每页记录数。
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.edupath + "arrange/page",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "startDate": start_date,
                 "endDate": end_date,
                 "teacherIds": [teacher_id],
@@ -180,15 +217,16 @@
         :param pay_start_date: 支付起始时间
         :param pay_end_date: 支付结束时间
         :param order_status: 订单状态 1>已付款 4>已作废
         :param page_num: 页数
         :param page_size: 每页项目数
         :return:
         """
-        return self.session.post(
+        return self.request(
+            method="post",
             url=self.reportpath + "findPaymentList",
             json={
                 "_t_": UsedTime.stamp,
                 "campusIds": self.campus,
                 "payType": "",
                 "payStartTime": pay_start_date,
                 "payEndTime": pay_end_date,
@@ -211,15 +249,16 @@
     ):
         """
         收据。
         :param order_id: 订单 ID
         :param payment_group_id: 支付 ID
         :return:
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/findReceipt",
             params={
                 "orderInfoId": order_id,
                 "paymentGroupId": payment_group_id,
                 "_t_": UsedTime.stamp
             }
         ).json()
@@ -231,15 +270,16 @@
     ):
         """
         收据。
         :param order_id: 订单 ID
         :param payment_group_id: 支付 ID
         :return:
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url="https://yunxiao.xiaogj.com/api/cs-pc-edu/public/receipt/snapInfoByPaymentGroupId",
             params={
                 "orderId": order_id,
                 "paymentGroupId": payment_group_id,
                 "_t_": UsedTime.stamp
             }
         ).json()
@@ -251,15 +291,16 @@
     ):
         """
         收据。
         :param order_id: 订单 ID
         :param payment_group_id: 支付 ID
         :return: Respose 数据
         """
-        return self.session.get(
+        return self.request(
+            method="get",
             url="https://yunxiao.xiaogj.com/web/teacher/#/receipt",
             params={
                 "orderId": order_id,
                 "paymentGroupId": payment_group_id
             }
         )
```

### Comparing `yunxiao-0.1.8/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.1.9/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.8
-Summary: An API tool for Cloud School Education Institution Management System.
+Version: 0.1.9
+Summary: An API SDK tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

