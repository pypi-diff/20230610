# Comparing `tmp/MMutils-0.0.3.tar.gz` & `tmp/MMutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MMutils-0.0.3.tar", last modified: Sat Jun 10 06:41:35 2023, max compression
+gzip compressed data, was "MMutils-0.0.4.tar", last modified: Sat Jun 10 16:35:13 2023, max compression
```

## Comparing `MMutils-0.0.3.tar` & `MMutils-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 06:41:35.233179 MMutils-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-06-10 03:00:52.000000 MMutils-0.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-10 06:41:35.194198 MMutils-0.0.3/MMutils.egg-info/
--rw-rw-rw-   0        0        0      472 2023-06-10 06:41:34.000000 MMutils-0.0.3/MMutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-06-10 06:41:35.000000 MMutils-0.0.3/MMutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 06:41:34.000000 MMutils-0.0.3/MMutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-10 06:41:34.000000 MMutils-0.0.3/MMutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-10 06:41:34.000000 MMutils-0.0.3/MMutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-06-10 06:41:35.231178 MMutils-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-06-10 06:16:28.000000 MMutils-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 06:41:35.228181 MMutils-0.0.3/mutils/
--rw-rw-rw-   0        0        0      366 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mcaptcha.py
--rw-rw-rw-   0        0        0     1930 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mdecorator.py
--rw-rw-rw-   0        0        0      543 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mfile.py
--rw-rw-rw-   0        0        0      966 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mlog.py
--rw-rw-rw-   0        0        0    29022 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mproxy.py
--rw-rw-rw-   0        0        0     4119 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mrequests.py
--rw-rw-rw-   0        0        0     4076 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/Mstr.py
--rw-rw-rw-   0        0        0        0 2023-06-10 06:40:58.000000 MMutils-0.0.3/mutils/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-10 06:41:35.233179 MMutils-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-06-10 06:41:31.000000 MMutils-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.763188 MMutils-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.712659 MMutils-0.0.4/MMutils.egg-info/
+-rw-rw-rw-   0        0        0      842 2023-06-10 16:35:13.000000 MMutils-0.0.4/MMutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      682 2023-06-10 16:35:13.000000 MMutils-0.0.4/MMutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:35:13.000000 MMutils-0.0.4/MMutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-10 16:35:13.000000 MMutils-0.0.4/MMutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-10 16:35:13.000000 MMutils-0.0.4/MMutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      842 2023-06-10 16:35:13.762168 MMutils-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-06-10 14:58:50.000000 MMutils-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.715654 MMutils-0.0.4/mmutils/
+-rw-rw-rw-   0        0        0        0 2023-06-10 06:40:58.000000 MMutils-0.0.4/mmutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.721650 MMutils-0.0.4/mmutils/decorator_utils/
+-rw-rw-rw-   0        0        0     2110 2023-06-10 12:37:13.000000 MMutils-0.0.4/mmutils/decorator_utils/Mdecorator.py
+-rw-rw-rw-   0        0        0        0 2023-06-10 06:54:10.000000 MMutils-0.0.4/mmutils/decorator_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.725669 MMutils-0.0.4/mmutils/file_utils/
+-rw-rw-rw-   0        0        0      842 2023-06-10 14:34:08.000000 MMutils-0.0.4/mmutils/file_utils/Mfile.py
+-rw-rw-rw-   0        0        0       21 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/file_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.732644 MMutils-0.0.4/mmutils/log_utils/
+-rw-rw-rw-   0        0        0     2972 2023-06-10 14:31:13.000000 MMutils-0.0.4/mmutils/log_utils/Mlog.py
+-rw-rw-rw-   0        0        0       18 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/log_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.737646 MMutils-0.0.4/mmutils/ocr_utils/
+-rw-rw-rw-   0        0        0      366 2023-06-10 14:34:19.000000 MMutils-0.0.4/mmutils/ocr_utils/Mcaptcha.py
+-rw-rw-rw-   0        0        0       22 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/ocr_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.742656 MMutils-0.0.4/mmutils/proxy_utils/
+-rw-rw-rw-   0        0        0    19201 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/proxy_utils/Mproxy.py
+-rw-rw-rw-   0        0        0     7312 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/proxy_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.747637 MMutils-0.0.4/mmutils/spider_utils/
+-rw-rw-rw-   0        0        0     3160 2023-06-10 14:53:46.000000 MMutils-0.0.4/mmutils/spider_utils/Mrequests.py
+-rw-rw-rw-   0        0        0      930 2023-06-10 14:51:33.000000 MMutils-0.0.4/mmutils/spider_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.753634 MMutils-0.0.4/mmutils/str_utils/
+-rw-rw-rw-   0        0        0     3443 2023-06-10 14:53:46.000000 MMutils-0.0.4/mmutils/str_utils/Mstr.py
+-rw-rw-rw-   0        0        0       20 2023-06-10 14:52:51.000000 MMutils-0.0.4/mmutils/str_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:35:13.759185 MMutils-0.0.4/mmutils/url_utils/
+-rw-rw-rw-   0        0        0      827 2023-06-10 12:37:13.000000 MMutils-0.0.4/mmutils/url_utils/Murl.py
+-rw-rw-rw-   0        0        0       18 2023-06-10 14:52:51.000000 MMutils-0.0.4/mmutils/url_utils/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-10 16:35:13.764166 MMutils-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-06-10 15:44:06.000000 MMutils-0.0.4/setup.py
```

### Comparing `MMutils-0.0.3/mutils/Mdecorator.py` & `MMutils-0.0.4/mmutils/decorator_utils/Mdecorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 # @Time : 10/30/2021 10:49 AM
 # @Author : MoMingLog
 # @File : Mdecorator.py
-# @Software: PyCharm
+
 import time
 from threading import Lock
 
+from mmutils.log_utils.Mlog import m_logger
+
 lock = Lock()
 
 
 def spend(func):
-    """
+    """ 用于计算函数运行时间的装饰器
 
     创建时间：2021.11.01 12:41
 
     :param func:
     :return:
     """
 
     def run(*args, **kwargs):
         start = time.time()
         f = func(*args, **kwargs)
         end = time.time()
         spend_time = end - start
-        print(f"{func.__name__}花费的时间为；{spend_time}")
+        m_logger.info(f"{func.__name__}花费的时间为；{spend_time}")
         return f
 
     return run
 
 
 def tips_txt(func):
     """
     创建时间：2021.10.31 20:30
+
     :param func:
     :return:
     """
 
     def run(content: str):
         lock.acquire()
-        print(f'正在写入数据{content}')
+        m_logger.debug(f'正在写入数据{content}')
         f = func(content)
-        print(f'数据写入完成'.center(50, '-'))
+        m_logger.debug(f'数据写入完成'.center(50, '-'))
         lock.release()
         return f
 
     return run
 
 
 def tips_csv(func):
@@ -88,7 +91,14 @@
         print(f'正在写入数据{args[0] if len(args) == 1 else ""}{kwargs if len(kwargs) != 0 else ""}')
         f = func(*args, **kwargs)
         print('数据写入完成'.center(50, '-'))
         lock.release()
         return f
 
     return run
+
+@spend
+def test():
+    time.sleep(1)
+
+if __name__ == '__main__':
+    test()
```

### Comparing `MMutils-0.0.3/mutils/Mfile.py` & `MMutils-0.0.4/mmutils/file_utils/Mfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import os
-
-"""
-更新日志：
-2021.10.28
-    1. 增加函数：folder
-
-"""
+import re
 
 
 def folder(path):
     """ 创建文件夹
 
     创建时间：2021.10.28
 
-    :param path:
+    :param path: 文件夹路径
     :return: 返回原的路径最后不包含 / 符号
     """
     # 判断文件夹是否存在
     if not os.path.exists(path):
         # 如果文件夹不存在，则创建文件夹
         os.makedirs(path)  # makedirs创建多级目录
     if path[-1] == '/':
         # 去掉最后面的 / 符号
         return path[0: -1]
     return path
+
+
+def replace_invalid_filename_char(filename, replaced_char='_'):
+    """ 去除非法文件名
+
+    创建时间：2021.10.28
+
+    :param filename: 原始的文件名
+    :param replaced_char: 替换非法字符的字符
+    :return:  返回过滤后的文件名
+    """
+    return re.sub('[<>/\\\\|:"*?]', replaced_char, filename)
```

### Comparing `MMutils-0.0.3/mutils/Mproxy.py` & `MMutils-0.0.4/mmutils/proxy_utils/Mproxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,215 +1,24 @@
 # @Time : 10/30/2021 2:22 PM
 # @Author : MoMingLog
 # @File : Mproxy.py
 # @Software: PyCharm
 
+
 import random
 import time
-import csv
-import re
+import concurrent.futures
+import threading
 from queue import Queue
 
 from lxml import etree
-from Mcaptcha import discern_ocr
-from Mrequests import request_, get_headers
-from Mlog import m_logger
-from threading import Thread
-
-"""
-更新日志：
-2021.10.30
-    1. 增加工具函数parse_by_xpath、check_usable
-
-
-"""
-
-
-def check_usable(item, save_item=None):
-    """ 检测代理是否可用
-
-    创建时间：2021.10.30 14:30
-
-    :param item:
-    :return:
-    """
-    if save_item is None:
-        raise ValueError('请传入对可用代理数据进行持久化存储的函数！')
-    else:
-        # 下方通过在百度搜索“ip”的结果来测试代理是否可用
-        url = 'https://www.baidu.com/s?wd=%E6%9C%AC%E6%9C%BAip'
-        headers = get_headers(ua_type='chrome')
-        headers.update({
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "Cookie": "BIDUPSID=417DCCD8A89DCD48C058253549BAFC98; PSTM=1652451950; BAIDUID=417DCCD8A89DCD488051FFBBCE3C78FA:SL=0:NR=10:FG=1; NOJS=1; BDUSS=WhVZmxmZnY4UUZZWm5GZm5ORVJFNWRiWXlsUFViQll0akdlNnNVMEFiOVFoMVJrSVFBQUFBJCQAAAAAAAAAAAEAAADyZor21MLTsNDHs71f0rnJqwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAFD6LGRQ-ixkL; BDUSS_BFESS=WhVZmxmZnY4UUZZWm5GZm5ORVJFNWRiWXlsUFViQll0akdlNnNVMEFiOVFoMVJrSVFBQUFBJCQAAAAAAAAAAAEAAADyZor21MLTsNDHs71f0rnJqwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAFD6LGRQ-ixkL; ISSW=1; ISSW=1; BD_UPN=12314753; BDORZ=B490B5EBF6F3CD402E515D22BCDA1598; H_PS_PSSID=38516_36544_38686_38860_38795_38755_38768_38486_38808_38822_38637_38764_26350_22159; BA_HECTOR=a4a42k8k2k0581a02h8l844n1i83sno1m; ZFY=5PXDGebmAhgKXNVJFPjDnyW0i39thwIeLGugKITJzwo:C; BAIDUID_BFESS=417DCCD8A89DCD488051FFBBCE3C78FA:SL=0:NR=10:FG=1; BD_HOME=1; BDRCVFR[feWj1Vr5u3D]=I67x6TjHwwYf0; delPer=0; BD_CK_SAM=1; PSINO=6; sug=3; sugstore=1; ORIGIN=2; bdime=0; H_PS_645EC=3addo3vWFEgz18E1b%2FteaT%2FJ62mNKIH0xav7W3YSF%2FmFkoXQMp72Ym6xWIrKPPwQeK9a",
-            "Host": "www.baidu.com"
-
-        })
-        proxies = {
-            'http': f'http://{item.get("ip")}:{item.get("port")}',
-            'https': f'http://{item.get("ip")}:{item.get("port")}'
-        }
-
-        try:
-            page_text = request_(url=url, proxies=proxies, headers=headers, timeout=10)
-            if page_text:
-                match_list = re.findall("本机IP", page_text)
-
-                if match_list:
-                    save_item(item)
-                else:
-                    m_logger.debug(page_text)
-        except Exception as te:
-            m_logger.exception(f"代理 {item.get('ip')}:{item.get('port')} 不可用！")
-
-
-def parse_by_xpath(*args, is_ip_domain=False, check_usable_func=check_usable, save_item=None):
-    """通过 xpath 来获取 ip 和 port
-
-    创建时间：2021.10.30 14.22
-
-    :param args: 实际最大参数为 5个：page_text、ip_xpath、port_xpath、ip_port_xpath、domain，程序会自动根据传进来的参数个数判断执行
-    :param is_ip_domain: 如果 domain不是 None 则需要通过这个参数来判断图片状态的是 ip（True） 还是 port（False），又或者两者都有（both）
-    :param check_usable_func: 检测代理是否可用的函数，默认为工具函数check_usable
-    :param save_item: 保存可用代理的函数
-    :return:
-    """
-    page_text = args[0]  # 网页源代码
-    ip_xpath = None  # ip对应的 xpath，默认为 None
-    port_xpath = None  # 对应的 xpath, 默认为 None
-    ip_port_xpath = None  # 当 抓取的数据是 “ip:port”形式的时候使用这个参数，默认值为 None
-    domain = None  # 如果存在图片形式的，则使用这个参数，默认值为None
-    ip_domain = None
-    port_domain = None
-    args_num = len(args)
-    if args_num == 3:
-        ip_xpath = args[1]
-        port_xpath = args[2]
-    elif args_num == 2:
-        ip_port_xpath = args[1]
-    elif args_num == 4:
-        ip_xpath = args[1]
-        port_xpath = args[2]
-        domain = args[3]
-        if is_ip_domain == 'both':
-            ip_domain = domain
-            port_domain = domain
-        elif is_ip_domain:
-            ip_domain = domain
-        elif not is_ip_domain:
-            port_domain = domain
-
-    element = etree.HTML(page_text)
-    if ip_port_xpath is None:
-        ip_ = element.xpath(ip_xpath)
-        port_ = element.xpath(port_xpath)
-        for ip, port in zip(ip_, port_):
-            item = {
-                # 使用三元运算，判断domain参数是否为空，如果不为空，则表示该网站使用了反爬，需要我们识别出ip或port
-                # 判断 ip_domain 是否为空，如果不为空，则识别图片
-                'ip': ip.strip() if ip_domain is None else discern_ocr(request_(url=domain + ip, ret_format='content')),
-                # 判断port_domain是否为空，如果不为空，则识别图片
-                'port': port.strip() if port_domain is None else discern_ocr(
-                    request_(url=domain + port, ret_format='content'))
-            }
-            Thread(target=check_usable_func, args=(item, save_item)).start()
-    else:
-        ip_port_ = element.xpath(ip_port_xpath)
-        for ip_port in ip_port_:
-            ip_port_list = ip_port.split(':')
-            item = {
-                # 使用三元运算，判断domain参数是否为空，如果不为空，则表示该网站使用了反爬，需要我们识别出ip或port
-                'ip': ip_port_list[0].strip() if ip_domain is None else discern_ocr(
-                    request_(domain + ip_port_list[0], ret_format='content')),
-                'port': ip_port_list[1].strip() if port_domain is None else discern_ocr(
-                    request_(domain + ip_port_list[1], ret_format='content'))
-            }
-            Thread(target=check_usable_func, args=(item, save_item)).start()
-
-
-def check_proxy(ip, port) -> bool:
-    url = 'http://www.baidu.com/s?ie=UTF-8&wd=本机ip'
-    headers = get_headers()
-    headers['Referer'] = 'https://www.baidu.com/'
-    headers[
-        'Cookie'] = 'BIDUPSID=D29624969C39994D9D17480DCF65EDB1; PSTM=1630857355; BAIDUID=D29624969C39994D183522665890A809:FG=1; BD_UPN=12314753; __yjs_duid=1_679dab97d101a0326f13b9a8a808bc0a1631104777407; H_WISE_SIDS=107314_110085_127969_131861_175668_175755_176399_177370_178384_178529_178634_179349_179458_179620_181106_181136_181251_181399_181588_181676_181712_182000_182530_183239_183330_183536_183611_183626_183869_183979_184042_184200_184267_184319_184326_184793_184809_184876_184894_185252_185275_185300_185519_185653_185746_185904_186026_186113_186313_186319_186412_186446_186455_186508_186595_186625_186643_186899_187067_187121_187185_187202_187214_187289_187325_187487_187563; MSA_WH=360_640; BDSFRCVID_BFESS=zJAOJexroG0vH6JHEJNeMdhrmmKKvV3TDYLtOwXPsp3LGJLVgWj3EG0PtoaGdu_-ox8EogKKQgOTHRCF_2uxOjjg8UtVJeC6EG0Ptf8g0M5; H_BDCLCKID_SF_BFESS=tRk8oI0aJDvDqTrP-trf5DCShUFsaJjWB2Q-XPoO3KJOqhuGy-A53Iu7jRnPQtbiW5cpoMbgylRM8P3y0bb2DUA1y4vpKhbBt2TxoUJ2abjne-53qtnWeMLebPRiQ4b9QgbN5hQ7tt5W8ncFbT7l5hKpbt-q0x-jLTnhVn0MBCK0hD0wD5thj6PVKgTa54cbb4o2WbCQMqcN8pcN2b5oQT8ByajZBUQZBDTu0nn-aR6vOPQKDpOUWfA3XpJvQnJjt2JxaqRC5M38hp5jDh3MhP_1bhode4ROfgTy0hvcLR3cShn-LUjrDRLbXU6BK5vPbNcZ0l8K3l02V-bIe-t2XjQh-p52f6LetJcP; BDUSS=tiNzBNaDZPbEszLUh2dUVVM2ZQSzhaMXhPNmpKMGltc3M5LWMtb2RuSGh5SkZoSVFBQUFBJCQAAAAAAAAAAAEAAADyZor21MLTsNDHs71f0rnJqwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAOE7amHhO2phb2; BDUSS_BFESS=tiNzBNaDZPbEszLUh2dUVVM2ZQSzhaMXhPNmpKMGltc3M5LWMtb2RuSGh5SkZoSVFBQUFBJCQAAAAAAAAAAAEAAADyZor21MLTsNDHs71f0rnJqwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAOE7amHhO2phb2; BDORZ=B490B5EBF6F3CD402E515D22BCDA1598; H_PS_PSSID=34947_34446_34067_31253_34967_34584_34517_34917_26350_34971_34868; channel=baidusearch; BAIDUID_BFESS=C3C7190A243B9F151317E636ACA16207:FG=1; BD_HOME=1; delPer=0; BD_CK_SAM=1; PSINO=5; H_PS_645EC=4665hF0GZnaGNwwZKaZxseXN9MXz99QpMkdK%2BtEvV2ySA7GJ0L7mPOA2nUo; BA_HECTOR=0l0l812h252l0h810r1gnprf90q; COOKIE_SESSION=597_0_5_2_11_2_1_0_5_2_0_0_45301_0_0_0_1635557263_0_1635577320%7C9%230_0_1635577320%7C1; baikeVisitId=a6cde87f-c5dd-4412-8f2f-c203b8eebe3f'
-    proxies = {
-        'http': 'http://' + ip + ':' + port,
-        'https': 'http://' + ip + ':' + port
-    }
-
-    try:
-        page_text = request_(url=url, proxies=proxies, headers=headers, timeout=6)
-        if page_text:
-            match_list = re.findall("本机IP", page_text)
-            if match_list:
-                m_logger.debug(f"代理：{ip}:{port}，请求成功")
-                return True
-            else:
-                m_logger.debug(f"代理：{ip}:{port}，请求失败")
-                return False
-        else:
-            m_logger.debug("请求失败")
-            return False
-    except Exception as te:
-        m_logger.error(f"代理：{ip}:{port}，请求失败, 异常")
-        return False
-
-
-import os
-
-
-def get_available_proxy(
-        num: int = 1,
-        file_data=None,
-        file_path: str = None,
-        is_recheck: bool = False,
-) -> list:
-    """获取可用代理
-
-    创建时间：2023.6.8
-
-    :param file_path: 代理文件路径
-    :param num: 需要获取的代理数量
-    :param is_recheck: 是否需要重新检测代理
-    :return:
-    """
-    if file_data is None:
-        if file_path is None:
-            file_path = os.path.join(os.path.dirname(__file__), 'proxies.csv')
-        with open(file_path, 'r', encoding='utf-8') as f:
-            reader = csv.reader(f)
-            next(reader)
-            proxies = list(reader)
-    else:
-        reader = csv.reader(file_data)
-        next(reader)
-        proxies = list(reader)
-
-    ret_data = []
-    for proxy in proxies:
-        if not proxy:
-            continue
-        ip = proxy[0]
-        port = proxy[1]
-        if is_recheck:
-            if check_proxy(ip, port):
-                ret_data.append(proxy)
-                if len(ret_data) == num:
-                    break
-        else:
-            ret_data.append(proxy)
-            if len(ret_data) == num:
-                break
-
-    return ret_data
-
-
-import concurrent.futures
-import threading
+from mmutils.ocr_utils.Mcaptcha import ocr_captcha
+from mmutils.proxy_utils import *
+from mmutils.spider_utils.Mrequests import request_, random_headers_with_ua
+from mmutils.log_utils.Mlog import m_logger
 
 
 class SpiderProxy:
     def __init__(self):
         self.proxies = []
         self._executor = concurrent.futures.ThreadPoolExecutor(max_workers=20)
 
@@ -296,15 +105,15 @@
         【 Tips】 这个网站有反爬措施，如果不加 Referer的话，貌似再多次访问后会封禁 ip，封禁时间未测试
 
         :param max_num: 爬取的最大页数，默认为 6
         :return:
         """
         for i in range(1, max_num + 1):
             url = f'https://www.zdaye.com/free/{i}/'
-            headers = get_headers()
+            headers = random_headers_with_ua()
             headers['Referer'] = 'https://www.zdaye.com/'
             # headers['Cookie'] = '__51vcke__1vh212XjimTsXGR8=6d56db57-69de-5f66-9239-7805d8214b1c; __51vuft__1vh212XjimTsXGR8=1635559887738; __root_domain_v=.zdaye.com; _qddaz=QD.999935559888059; ASPSESSIONIDCERASART=NFJJMNECNEKNMEIHCNKIGONA; ASPSESSIONIDCETBSDSR=MDCIPHHCMNNCHOCKKCDFHKMJ; __51uvsct__1vh212XjimTsXGR8=2; _qdda=3-1.3eaw95; _qddab=3-rw3ohm.kvdiuyjp; lastSE=baidu; acw_tc=2f624a7216355816418236717e35c17e3ff2562d2380cae09a05e73f25d7a3; __vtins__1vh212XjimTsXGR8={"sid": "e5c5030e-0037-59b4-97f8-2e7aa2d1df65", "vd": 7, "stt": 1943970, "dr": 393602, "expires": 1635583479751, "ct": 1635581679751}; Hm_lvt_80f407a85cf0bc32ab5f9cc91c15f88b=1635559888,1635559918,1635581272,1635581680; Hm_lpvt_80f407a85cf0bc32ab5f9cc91c15f88b=1635581680'
             page_text = request_(url=url, encoding='gb2312')
             ip_xpath = '//table[@id="ipc"]//tbody/tr/td[1]/text()'
             port_xpath = '//table[@id="ipc"]//tbody/tr/td[2]/text()'
             self.__parse_by_xpath(
                 page_text,
@@ -415,48 +224,48 @@
                 port_domain = domain
             elif is_ip_domain:
                 ip_domain = domain
             elif not is_ip_domain:
                 port_domain = domain
 
         def run(item):
-            # Thread(target=check_usable_func, args=(item, save_item)).start()
+            # Thread(target=check_usable_func, args=(item, __save_item)).start()
             if check_proxy(item['ip'], item['port']):
                 self.proxies.append(item)
 
         element = etree.HTML(page_text)
         if ip_port_xpath is None:
             ip_ = element.xpath(ip_xpath)
             port_ = element.xpath(port_xpath)
             for ip, port in zip(ip_, port_):
                 item = {
                     # 使用三元运算，判断domain参数是否为空，如果不为空，则表示该网站使用了反爬，需要我们识别出ip或port
                     # 判断 ip_domain 是否为空，如果不为空，则识别图片
-                    'ip': ip.strip() if ip_domain is None else discern_ocr(
+                    'ip': ip.strip() if ip_domain is None else ocr_captcha(
                         request_(url=domain + ip, ret_format='content')),
                     # 判断port_domain是否为空，如果不为空，则识别图片
-                    'port': port.strip() if port_domain is None else discern_ocr(
+                    'port': port.strip() if port_domain is None else ocr_captcha(
                         request_(url=domain + port, ret_format='content'))
                 }
-                Thread(target=run, args=(item,)).start()
+                threading.Thread(target=run, args=(item,)).start()
 
         else:
             ip_port_ = element.xpath(ip_port_xpath)
             for ip_port in ip_port_:
                 ip_port_list = ip_port.split(':')
                 item = {
                     # 使用三元运算，判断domain参数是否为空，如果不为空，则表示该网站使用了反爬，需要我们识别出ip或port
-                    'ip': ip_port_list[0].strip() if ip_domain is None else discern_ocr(
+                    'ip': ip_port_list[0].strip() if ip_domain is None else ocr_captcha(
                         request_(domain + ip_port_list[0], ret_format='content')),
-                    'port': ip_port_list[1].strip() if port_domain is None else discern_ocr(
+                    'port': ip_port_list[1].strip() if port_domain is None else ocr_captcha(
                         request_(domain + ip_port_list[1], ret_format='content'))
                 }
-                Thread(target=run, args=(item,)).start()
+                threading.Thread(target=run, args=(item,)).start()
 
-    def spider(self, func):
+    def _spider(self, func):
         # 将所有解析免费代理的功能函数封装到一个列表中
         proxy_func_list = [
             self.__proxy_89ip,
             self.__proxy_nima,
             self.__proxy_kaixin,
             self.__proxy_mipu,
             self.__proxy_zdaye,
@@ -471,15 +280,15 @@
         # 运行传进来的功能函数
         func()
 
         # 等待所有线程执行完毕
         concurrent.futures.wait(future_list)
 
 
-class GenerateProxy(SpiderProxy):
+class Proxy(SpiderProxy):
     CSV_FILE_NAME = 'proxies.csv'
     FILTER_CSV_FILE_NAME = 'proxies_filter.csv'
     FILE_PATH = os.path.join(os.path.dirname(__file__), CSV_FILE_NAME)
     FILTER_FILE_PATH = os.path.join(os.path.dirname(__file__), FILTER_CSV_FILE_NAME)
 
     def __init__(self):
         super().__init__()
@@ -507,15 +316,15 @@
     def __init(self):
         # 读取标题
         header_title = next(self.__dr, None)
         # 如果表头不存在，则写入表头
         if header_title != ['ip', 'port']:
             self.__dw_append.writeheader()
 
-    def save_item(self):
+    def __save_item(self):
         """
         保存代理
         :return:
         """
 
         def save():
             while True:
@@ -527,21 +336,25 @@
                     self.proxies = []
                     self.__lock.release()
 
                 time.sleep(1)
 
         threading.Thread(target=save, daemon=True).start()
 
-    def generate(self):
+    def spider_free_proxy(self, is_deduplication=False):
         """
         生成并持久化代理
+        :param is_deduplication: 是否去重, 默认不去重
         :return:
         """
         # 开始爬取代理
-        self.spider(self.save_item)
+        self._spider(self.__save_item)
+        # 判断是否去重
+        if is_deduplication:
+            self.deduplication()
 
     @classmethod
     def get_random_proxy_by_local(cls):
         """
         随机获取一个代理
         :return:
         """
@@ -558,37 +371,45 @@
         }
 
     def get_random_proxy_by_filter(self):
         """
         随机获取一个代理
         :return:
         """
-        proxies = random.choice(self.proxies)
+        if self.proxies == []:
+            self.__dr = csv.reader(self.__file_read_object)
+            next(self.__dr)
+            self.proxies = list(self.__dr)
+
+        proxy = random.choice(self.proxies)
+
         return {
-            "http": f"http://{proxies[0]}:{proxies[1]}",
-            "https": f"http://{proxies[0]}:{proxies[1]}"
+            "http://": f"{proxy[0]}:{proxy[1]}",
+            "https://": f"{proxy[0]}:{proxy[1]}"
         }
-        pass
-
-    def check_filter_proxy(self):
-        pass
 
-    def filter_proxy(self, path=None):
+    def filter_proxy(self, in_path=None, out_path=FILTER_FILE_PATH):
         """
         过滤代理
+        :param in_path:  输入csv文件的路径
+        :param out_path: 输出csv文件的路径
         :return:
         """
-        if path is None:
+        if in_path is None:
             proxies = list(self.__dr)
         else:
-            with open(path, 'r', encoding='utf-8-sig') as f:
+            with open(in_path, 'r', encoding='utf-8-sig') as f:
                 reader = csv.reader(f)
                 next(reader)
                 proxies = list(reader)
 
+        if proxies == []:
+            m_logger.warning("您的代理文件内容为空")
+            return
+
         # 用于存储可用代理
         temp_proxies = []
 
         # 定义过滤代理的功能函数
         def __filter(proxy):
             """
             过滤代理
@@ -607,32 +428,30 @@
         futures = [self._executor.submit(__filter, proxy) for proxy in proxies]
 
         # 等待所有线程执行完毕
         concurrent.futures.wait(futures)
 
         def save():
             self.proxies = temp_proxies
-            with open(self.FILTER_FILE_PATH, 'w', encoding='utf-8-sig', newline="") as f:
+            with open(out_path, 'w', encoding='utf-8-sig', newline="") as f:
                 writer = csv.DictWriter(f, fieldnames=['ip', 'port'])
                 writer.writeheader()
                 writer.writerows(temp_proxies)
 
-        # 写入表头
-
         # 将可用代理写入文件
         save()
 
         # if len(temp_proxies) < 20:
         #     self.generate()
 
     def filter_proxy_by_local(self, num: int = 1):
         """
         从本地文件中过滤代理
 
-        速度有限制
+        效率相对于filter_proxy()低
 
         :param num: 需要获取的代理数量
         :return:
         """
         with open(self.FILE_PATH, 'r', encoding='utf-8-sig') as f:
             reader = csv.reader(f)
             next(reader)
@@ -657,33 +476,30 @@
 
         future_list = [executor.submit(append_item, proxy) for proxy in proxies]
 
         for future in future_list:
             proxy = future.result()
             if proxy:
                 proxy_queue.put({
-                    "http": "http://" + proxy[0] + ":" + proxy[1],
-                    "https": "http://" + proxy[0] + ":" + proxy[1]
+                    "http://": f"{proxy[0]}:{proxy[1]}",
+                    "https://": f"{proxy[0]}:{proxy[1]}"
                 })
                 m_logger.info(f"可用代理为：{proxy}, 当前可用代理数量为：{proxy_queue.qsize()}，需要的代理数量为：{num}")
                 if proxy_queue.qsize() == num:
                     is_run = False
                     break
 
         # 将所有线程关闭
         executor.shutdown(wait=False, cancel_futures=True)
 
         if proxy_queue.qsize() < num:
             m_logger.info("可用代理不足")
             return proxy_queue
         return proxy_queue
 
-    def filter_proxy_by_parse(self):
-        pass
-
     # 去重
     def deduplication(self):
         """
         去重
         :return:
         """
         # 读取文件内容
@@ -695,13 +511,9 @@
         with open(self.FILE_PATH, 'w', newline="", encoding='utf-8-sig') as f:
             writer = csv.writer(f)
             writer.writerow(['ip', 'port'])
             writer.writerows(proxies)
 
 
 if __name__ == '__main__':
-    generate = GenerateProxy()
-    # generate.generate()
-    # usable_list = generate.filter_proxy_by_local(6)
-    # pprint.pprint(usable_list.qsize())
-    generate.filter_proxy(GenerateProxy.FILTER_FILE_PATH)
-    generate.deduplication()
+    proxy = Proxy()
+    proxy.filter_proxy()
```

### Comparing `MMutils-0.0.3/mutils/Mrequests.py` & `MMutils-0.0.4/mmutils/spider_utils/Mrequests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,9 @@
-# import json as jn
-
+from mmutils.spider_utils import *
 import requests
-from faker import Faker
-
-"""
-更新日志：
-2021.10.29
-    1. request_函数增加参数：verify=True、warning=True、allow_redirects=True
-
-2021.10.28
-    1. 增加函数：get_headers、requests_
-
-"""
-
-
-def get_headers(ua_type=None):
-    """ 获取随机UA的headers字典
-
-    创建时间：2021.10.28
-
-    更新时间：2022.03.05
-
-    更新日志
-    2022.03.05：
-        增加获取特定ua类型
-
-    :return: 返回headers
-    """
-    ua = None
-    if ua_type is None:
-        ua = Faker().user_agent()
-    elif ua_type == "chrome":
-        ua = Faker().chrome()
-
-    headers = {
-        'User-Agent': ua
-    }
-    return headers
-
-
-def get_ua(ua_type=None):
-    """
-    获取随机UA
-
-    创建时间：2022.03.07
-
-    :param ua_type: UA类型
-    :return:
-    """
-    ua = None
-    if ua_type is None:
-        ua = Faker().user_agent()
-    elif ua_type == "chrome":
-        ua = Faker().chrome()
-
-    return ua
 
 
 def request_(url, proxies=None, verify=True, warning=True, allow_redirects=True, headers=None, ua_type=None,
              params=None, data=None,
              json=None,
              timeout=15,
              encoding='utf-8',
@@ -90,15 +35,15 @@
     :param ret_format: 返回的数据类型：包括 text, json, content, headers, res，默认text
     :return:
     """
     if not warning:
         from requests.packages.urllib3.exceptions import InsecureRequestWarning
         requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
     if headers is None:
-        headers = get_headers(ua_type)
+        headers = random_headers_with_ua(ua_type)
     # 判断是否是post请求
     if data is not None:
         # 如果data不为空表示发送的是表单数据
         res = requests.post(url=url, proxies=proxies, verify=verify, allow_redirects=allow_redirects, headers=headers,
                             data=data)
     # 如果条件一不满足，则判断条件二是否满足，同样是post请求
     elif json is not None:
```

### Comparing `MMutils-0.0.3/mutils/Mstr.py` & `MMutils-0.0.4/mmutils/str_utils/Mstr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,9 @@
 import re
 
-"""
-更新日志：
-2021.11.18
-    1. 修复函数filter_str的一些小bug
-2021.10.29
-    1. 增加函数：filter_csv、filter_str、filter_
-    2. filter_str函数修改：to_str参数也支持 | 符号，与 rep_str 分割后的元素一一对应
-2021.10.28
-    1. 增加函数：split、filter_filename、get_filename
-
-"""
-
-
 def split_(ori_str, start_str, end_str):
     """ 截取字符串
 
     创建时间：2021.10.28
 
     :param ori_str: 需要截取的原始字符串
     :param start_str:  开始的字符串，通过这个来获取开始截取的索引
@@ -101,16 +88,8 @@
 
     :param filename: 原始的文件名
     :return:  返回过滤后的文件名
     """
     return re.sub('[<>/\\\\|:"*?]', "_", filename)
 
 
-def get_filename(url):
-    """ 从链接中截取文件名，包括后缀（扩展名）
 
-    创建时间：2021.10.28
-
-    :param url: 链接
-    :return: 返回截取的文件名，包括后缀（扩展名）
-    """
-    return filter_filename(re.search('.*/(.*)', url).group(1))
```

### Comparing `MMutils-0.0.3/setup.py` & `MMutils-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = '自用模块'
-LONG_DESCRIPTION = '自用模块'
 
 setup(
     name="MMutils",
     version=VERSION,
     author="MoMingLog",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
+    license='MIT',
     install_requires=[
         "Faker>=18.7.0",
         "ddddocr>=1.4.7",
         "requests>=2.30.0",
         "loguru>=0.7.0",
         "lxml>=4.9.2",
     ],
@@ -34,8 +34,9 @@
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
+
 )
```

