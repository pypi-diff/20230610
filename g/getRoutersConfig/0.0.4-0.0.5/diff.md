# Comparing `tmp/getRoutersConfig-0.0.4.tar.gz` & `tmp/getRoutersConfig-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getRoutersConfig-0.0.4.tar", last modified: Wed May  3 09:44:45 2023, max compression
+gzip compressed data, was "getRoutersConfig-0.0.5.tar", last modified: Sat Jun 10 14:19:01 2023, max compression
```

## Comparing `getRoutersConfig-0.0.4.tar` & `getRoutersConfig-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.072579 getRoutersConfig-0.0.4/
--rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     4464 2023-05-03 09:44:45.068573 getRoutersConfig-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:44.969003 getRoutersConfig-0.0.4/app/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:44.995573 getRoutersConfig-0.0.4/app/getRoutersConfig/
--rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.056582 getRoutersConfig-0.0.4/app/getRoutersConfig/src/
--rw-rw-rw-   0        0        0     9798 2023-05-02 15:33:04.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/CiscoClass.py
--rw-rw-rw-   0        0        0     4106 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/HuaweiClass.py
--rw-rw-rw-   0        0        0     1096 2023-05-02 15:35:16.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/RouterClass.py
--rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-03 09:35:35.000000 getRoutersConfig-0.0.4/app/getRoutersConfig/src/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:44:45.037577 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/
--rw-rw-rw-   0        0        0     4464 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 09:44:44.000000 getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 09:44:45.073576 getRoutersConfig-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-02 15:36:10.000000 getRoutersConfig-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.137152 getRoutersConfig-0.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5286 2023-06-10 14:19:01.135157 getRoutersConfig-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.091156 getRoutersConfig-0.0.5/app/
+drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.104153 getRoutersConfig-0.0.5/app/getRoutersConfig/
+-rw-rw-rw-   0        0        0       48 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.132157 getRoutersConfig-0.0.5/app/getRoutersConfig/src/
+-rw-rw-rw-   0        0        0    11721 2023-06-10 12:41:37.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/CiscoClass.py
+-rw-rw-rw-   0        0        0     1281 2023-06-10 12:54:23.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/HuaweiClass.py
+-rw-rw-rw-   0        0        0     1216 2023-06-10 12:08:16.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/RouterClass.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 06:55:17.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/__init__.py
+-rw-rw-rw-   0        0        0     2449 2023-05-30 15:46:22.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/main.py
+-rw-rw-rw-   0        0        0      601 2023-06-10 12:42:51.000000 getRoutersConfig-0.0.5/app/getRoutersConfig/src/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-10 14:19:01.116157 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/
+-rw-rw-rw-   0        0        0     5286 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      501 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-10 14:19:00.000000 getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 14:19:01.137152 getRoutersConfig-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-03 10:07:23.000000 getRoutersConfig-0.0.5/setup.py
```

### Comparing `getRoutersConfig-0.0.4/LICENSE` & `getRoutersConfig-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `getRoutersConfig-0.0.4/PKG-INFO` & `getRoutersConfig-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.4
+Version: 0.0.5
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -18,58 +18,59 @@
 
 # What it does ?
 This return Cisco configuration and information like :
  - Sytem informations
  - Static routes
  - Interfaces
  - DHCP
+ - ACL
 
 # Informations
 bastion_ip and bastion_port are optional
 
 # Get system informations
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 system_information = router.getSystemInformation()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 {
-    "serie": "C870",
-    "version": "12.4(24)T4",
-    "hostname": "HomeC871",
+    "serie": "C800",
+    "model": "C891F-K9",
+    "version": "15.4(3)M6",
+    "hostname": "THE_ROUTER",
     "uptime": {
         "years": 0,
-        "weeks": 0,
-        "days": 2,
-        "hours": 2,
-        "minutes": 44
+        "weeks": 1,
+        "days": 1,
+        "hours": 11,
+        "minutes": 25
+    },
+    "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
+    "serial_number": "FCZ1234A5BC",
+    "config_register": "0x2102"
 }
 ```
 
-# Disconnect from router
-```python
-from getRoutersConfig import setInformations
-
-router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
-
-system_information = router.disconnect()
-```
-
 # Get static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 static_routes = router.getStaticRoutes()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 [
     {
         "subnet_address": "1.1.1.1",
@@ -92,14 +93,16 @@
 # Get interfaces
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 interfaces = router.getInterfaces()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 {
     "switched": [
@@ -129,14 +132,16 @@
 # Get DHCP
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 dhcp = router.getDhcp()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 [
     {
@@ -162,26 +167,65 @@
             ...
         ]
     },
     ...
 ]
 ```
 
+# Get ACL
+```python
+from getRoutersConfig import setInformations
+
+router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
+
+dhcp = router.getIpv4Acl()
+
+router.disconnect()
+```
+
+The Schema is :
+```json
+
+[
+    {
+        "type": "Extended",
+        "name": "acl-premium",
+        "rule": [
+            {
+                "sequence_number": 10,
+                "pass": "permit",
+                "protocol": "udp",
+                "source": "any",
+                "source_port": "all",
+                "destination": "host 192.168.10.3",
+                "destination_port": "snmp",
+                "macthes": 2417837
+            },
+            ...
+        ]
+    },
+    ...
+]
+```
+
 # Get full configuration
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 config = router.getFullConfiguration()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 {
     "system": {},
     "ipv4StaticRoutes": [],
     "interfaces": [],
-    "dhcp": []
+    "dhcp": [],
+    "acl": []
 }
 ```
```

### Comparing `getRoutersConfig-0.0.4/app/getRoutersConfig/src/CiscoClass.py` & `getRoutersConfig-0.0.5/app/getRoutersConfig/src/CiscoClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from ipaddress import IPv4Network
+from .tools import separate_section
 import re
 
 class Cisco:
     def __init__(self, net_connect):
         self.net_connect = net_connect
 
     def getIpv4StaticRoutes(self) -> list:
         output = self.net_connect.send_command(f"show running-config | i ip route")
 
         v4_routes = []
-        new_v4_routes = self.separate_section(r"(^.*ip route.*$)", output)
+        new_v4_routes = separate_section(r"(^.*ip route.*$)", output)
 
         for route in new_v4_routes:
             re_route = r'ip route( vrf (?P<vrf>\S+))? (?P<subnet_address>\d+.\d+.\d+.\d+) (?P<subnet_mask>\d+.\d+.\d+.\d+) (?P<gateway>\d+.\d+.\d+.\d+)( (?P<metric>\d+))?( tag (?P<tag>\d+))?( name (?P<name>(\S|\s)+))?' #(?!.*\btrack\b)
 
             match_route = re.search(re_route, route, flags=re.M)
 
             track = int(re.search(r'track\s+(\d+)', route).group(1)) if re.search(r'track\s+(\d+)', route) else ""
@@ -38,70 +39,51 @@
 
     def getSystemInformation(self) -> list:
         output = self.net_connect.send_command(f"show version")
 
         re_serie_version = r'Cisco IOS Software, (?P<serie>\S+) Software (\S+), Version (?P<version>\S+), RELEASE SOFTWARE \S+'
         re_hostname_uptime = r'(?P<hostname>\S+) uptime is( (?P<years>\d+) year(s)?,)?( (?P<weeks>\d+) week(s)?,)?( (?P<days>\d+) day(s)?,)?( (?P<hours>\d+) hour(s)?,)?( (?P<minutes>\d+) minute(s)?)?'
         re_system_image = r'System image file is "flash:(?P<system_image>\S+)"'
+        re_model = r'Cisco (?P<model>\S+) \(revision \S+\) with \S+ bytes of memory.'
         re_serial_number = r'Processor board ID (?P<serial_number>\S+)'
         re_config_register = r'Configuration register is (?P<config_register>\S+)'
 
         match_serie_version = re.search(re_serie_version, output, flags=re.M)
         match_hostname_uptime = re.search(re_hostname_uptime, output, flags=re.M)
         match_system_image = re.search(re_system_image, output, flags=re.M)
+        match_model = re.search(re_model, output, flags=re.M)
         match_serial_number = re.search(re_serial_number, output, flags=re.M)
         match_config_register = re.search(re_config_register, output, flags=re.M)
 
         return {
             "serie": match_serie_version.group('serie'),
+            "model": match_model.group('model'),
             "version": match_serie_version.group('version'),
             "hostname": match_hostname_uptime.group('hostname'),
             "uptime": {
                 "years": int(match_hostname_uptime.group('years')) if match_hostname_uptime.group('years') else 0,
                 "weeks": int(match_hostname_uptime.group('weeks')) if match_hostname_uptime.group('weeks') else 0,
                 "days": int(match_hostname_uptime.group('days')) if match_hostname_uptime.group('days') else 0,
                 "hours": int(match_hostname_uptime.group('hours')) if match_hostname_uptime.group('hours') else 0,
                 "minutes": int(match_hostname_uptime.group('minutes')),
             },
             "system_image": match_system_image.group('system_image'),
             "serial_number": match_serial_number.group('serial_number'),
             "config_register": match_config_register.group('config_register'),
         }
 
-    def separate_section(self, separator, content):
-        if content == "":
-            return []
-
-        lines = re.split(separator, content, flags=re.M)
-
-        if len(lines) == 1:
-            msg = "Unexpected output data:\n{}".format(lines)
-            raise ValueError(msg)
-
-        lines.pop(0)
-
-        if len(lines) % 2 != 0:
-            msg = "Unexpected output data:\n{}".format(lines)
-            raise ValueError(msg)
-
-        lines_iter = iter(lines)
-
-        try:
-            new_lines = [line + next(lines_iter, '') for line in lines_iter]
-        except TypeError:
-            raise ValueError()
-        return new_lines
+    
 
-    def getInterfaces(self):
+    def getInterfaces(self) -> list:
         output_v4 = self.net_connect.send_command('show ip interface')
         v4_interfaces = [{
             "switched": [],
             "routed": []
         }]
-        new_v4_interfaces = self.separate_section(r"(^.*line protocol is.*$)", output_v4)
+        new_v4_interfaces = separate_section(r"(^.*line protocol is.*$)", output_v4)
 
         for interface in new_v4_interfaces:
             re_intf_name_state = r"^(?P<intf_name>\S+).+is.(?P<intf_state>.+)., line protocol is .(?P<intf_protocol_state>.+)$"
             re_intf_ip = r"Internet address is\s+(?P<ip_address>\d+.\d+.\d+.\d+)\/(?P<prefix_length>\d+)"
 
             match_intf = re.search(re_intf_name_state, interface, flags=re.M)
 
@@ -129,40 +111,48 @@
                         "vlan": "1"
                     })
 
             for ip_info in match_ip:
                 # if ip_info:
                 re_vrf = r"ip vrf forwarding (?P<vrf>\S+)"
                 re_description = r"description (?P<description>.+)"
+                re_acl_in = r"ip access-group (?P<acl_in>.+) in"
+                re_acl_out = r"ip access-group (?P<acl_out>.+) out"
 
                 match_vrf = re.search(re_vrf, output_run, flags=re.M)
                 match_description = re.search(re_description, output_run, flags=re.M)
+                match_acl_in = re.search(re_acl_in, output_run, flags=re.M)
+                match_acl_out = re.search(re_acl_out, output_run, flags=re.M)
 
                 vrf = match_vrf.group('vrf') if match_vrf else ""
                 description = match_description.group('description') if match_description else ""
+                acl_in = match_acl_in.group('acl_in') if match_acl_in else ""
+                acl_out = match_acl_out.group('acl_out') if match_acl_out else ""
 
                 v4_interfaces[0]["routed"].append({
                     "name": intf_name,
                     "description": description,
                     "ip": ip_info[0],
                     "mask": {
                         "octets": str(IPv4Network((0, ip_info[1])).netmask),
                         "cidr": int(ip_info[1])
                     },
-                    "vrf": vrf
+                    "vrf": vrf,
+                    "acl_in": acl_in,
+                    "acl_out": acl_out
                 })
 
         return v4_interfaces
     
-    def getDhcp(self):
+    def getDhcp(self) -> list:
         output_v4 = self.net_connect.send_command('show run | s ip dhcp pool')
         res_dhcp = []
         options = []
 
-        new_dhcp = self.separate_section(r"(^ip dhcp pool.*$)", output_v4)
+        new_dhcp = separate_section(r"(^ip dhcp pool.*$)", output_v4)
 
         for dhcp in new_dhcp:
             re_dhcp_pool_name = r"^ip dhcp pool (?P<dhcp_pool_name>.+)$"
             re_network = r"(network (?P<network_address>\d+.\d+.\d+.\d+) (?P<network_mask>\d+.\d+.\d+.\d+))?"
             re_default_router = r"(default-router (?P<default_router>\d+.\d+.\d+.\d+))?"
             re_dns_server = r"(dns-server (?P<dns_server>.+))?"
             re_options = r"option (?P<code>\d+) (?P<string_type>\S+) (?P<string>\S+)"
@@ -191,8 +181,45 @@
                     }
                 },
                 "default_router": match_default_router.group('default_router') if match_default_router.group('default_router') else "",
                 "dns_server": [i for i in match_dns_server.group('dns_server').strip().split(' ')] if match_dns_server.group('dns_server') else "",
                 "option": options
             })
 
-        return res_dhcp
+        return res_dhcp
+    
+    def getIpv4Acl(self) -> list:
+        output_v4 = self.net_connect.send_command('show ip access-lists')
+        res_ipv4_acl = []
+
+        new_acl = separate_section(r"(^.*IP access list.*$)", output_v4)
+
+        for acl in new_acl:
+            acl_rule = []
+            re_acl_type_name = r"^(?P<acl_type>\S+) IP access list (?P<acl_name>.+)"
+            re_acl_rule = r"(?P<sequence_number>\d+) (?P<pass>\S+) (?P<protocol>\S+) (any|host \d+.\d+.\d+.\d+|\d+.\d+.\d+.\d+ \d+.\d+.\d+.\d+)( eq (\S+|\d+))? (any|host \d+.\d+.\d+.\d+|\d+.\d+.\d+.\d+ \d+.\d+.\d+.\d+)( eq (\S+|\d+))?( \((\d+) matches\))?"
+
+            match_acl_type_name = re.search(re_acl_type_name, acl, flags=re.M)
+            match_acl_rule = re.findall(re_acl_rule, acl, flags=re.M)
+
+            if match_acl_rule:
+                for acl in match_acl_rule:
+                    acl_rule.append({
+                        "sequence_number": int(acl[0]),
+                        "pass": acl[1],
+                        "protocol": acl[2],
+                        "source": acl[3],
+                        "source_port": acl[5] if acl[4] else "all",
+                        "destination": acl[6],
+                        "destination_port": acl[8] if acl[8] else "all",
+                        "macthes": int(acl[10]) if acl[10] else 0,
+                        # "option": acl[5] if acl[5] else ""
+                    })
+
+            if match_acl_type_name.group('acl_name') not in ["97", "98", "99", "ACL-IP-MANAGEMENT", "ACL-ControlPlane"]:
+                res_ipv4_acl.append({
+                    "type": match_acl_type_name.group('acl_type'),
+                    "name": match_acl_type_name.group('acl_name'),
+                    "rule": acl_rule
+                })
+
+        return res_ipv4_acl
```

### Comparing `getRoutersConfig-0.0.4/app/getRoutersConfig/src/RouterClass.py` & `getRoutersConfig-0.0.5/app/getRoutersConfig/src/RouterClass.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,25 @@
         self.net_connect.disconnect()
 
     def getFullConfiguration(self):
         return {
             "system": self.router.getSystemInformation(),
             "ipv4StaticRoutes": self.router.getIpv4StaticRoutes(),
             "interfaces": self.router.getInterfaces(),
-            "dhcp": self.router.getDhcp()
+            "dhcp": self.router.getDhcp(),
+            "acl": self.router.getIpv4Acl()
         }
 
     def getIpv4StaticRoutes(self):
         return self.router.getIpv4StaticRoutes()
     
     def getSystemInformation(self):
         return self.router.getSystemInformation()
     
     def getInterfaces(self):
         return self.router.getInterfaces()
     
     def getDhcp(self):
-        return self.router.getDhcp()
+        return self.router.getDhcp()
+    
+    def getIpv4Acl(self):
+        return self.router.getIpv4Acl()
```

### Comparing `getRoutersConfig-0.0.4/app/getRoutersConfig/src/main.py` & `getRoutersConfig-0.0.5/app/getRoutersConfig/src/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from netmiko import ConnectHandler, redispatch
 import time
 from .RouterClass import Router
 from pysnmp.hlapi import *
 
 def setInformations(host_ip: str='', host_port: int=22, host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: int=22) -> Router:
+    device_type: str = ""
+    
     if not bastion_ip:
-        device_type: str = getDeviceType(host_ip, host_snmp_community)
+        device_type = getDeviceType(host_ip, host_snmp_community)
 
     host = {
         'device_type': device_type if not bastion_ip else "terminal_server",
         'ip': host_ip if not bastion_ip else bastion_ip,
         'username': user,
         'password': password,
         'port': host_port if not bastion_ip else bastion_port,
@@ -23,34 +25,34 @@
     if bastion_ip:
 
         net_connect.write_channel(f"snmpwalk -v2c -c covareck {host_ip} SNMPv2-MIB::sysDescr\n")
         net_connect.write_channel(f"ssh {host_ip}\r\n")
 
         time.sleep(2)
         output = net_connect.read_channel()
-        print(output)
         if "huawei" in output.lower():
-            device_type: str = "huawei"
+            device_type = "huawei"
         elif "cisco" in output.lower():
-            device_type: str = "cisco_ios"
+            device_type = "cisco_ios"
 
+        # print(output.lower())
         time.sleep(2)
 
         if 'password' in output.lower():
             net_connect.write_channel(password)
 
         redispatch(net_connect, device_type=device_type)
 
     return Router(device_type, net_connect)
 
 def getDeviceType(ip, snmp_community):
     iterator = getCmd(
         SnmpEngine(),
         CommunityData(snmp_community, mpModel=0),
-        UdpTransportTarget((ip, 161)),
+        UdpTransportTarget((ip, 161), timeout=5, retries=10),
         ContextData(),
         ObjectType(ObjectIdentity('SNMPv2-MIB', 'sysDescr', 0))
     )
 
     errorIndication, errorStatus, errorIndex, varBinds = next(iterator)
 
     if errorIndication:
@@ -61,10 +63,10 @@
     else:
         for varBind in varBinds:
             output = ' = '.join([x.prettyPrint() for x in varBind])
             if "huawei" in output.lower():
                 return "huawei"
             elif "cisco" in output.lower():
                 return "cisco_ios"
-            raise ValueError("The router needs to be a Cisco_ios or Huawei")
+            raise ValueError("The router needs to be Cisco_ios or Huawei")
 
 # net_connect.disconnect()
```

### Comparing `getRoutersConfig-0.0.4/app/getRoutersConfig.egg-info/PKG-INFO` & `getRoutersConfig-0.0.5/app/getRoutersConfig.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getRoutersConfig
-Version: 0.0.4
+Version: 0.0.5
 Summary: get Cisco routers configuration as Json
 Home-page: https://github.com/DanielRicklin/getRoutersConfig
 Author: DanielRicklin
 Author-email: ricklin.daniel@outlook.fr
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -18,58 +18,59 @@
 
 # What it does ?
 This return Cisco configuration and information like :
  - Sytem informations
  - Static routes
  - Interfaces
  - DHCP
+ - ACL
 
 # Informations
 bastion_ip and bastion_port are optional
 
 # Get system informations
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 system_information = router.getSystemInformation()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 {
-    "serie": "C870",
-    "version": "12.4(24)T4",
-    "hostname": "HomeC871",
+    "serie": "C800",
+    "model": "C891F-K9",
+    "version": "15.4(3)M6",
+    "hostname": "THE_ROUTER",
     "uptime": {
         "years": 0,
-        "weeks": 0,
-        "days": 2,
-        "hours": 2,
-        "minutes": 44
+        "weeks": 1,
+        "days": 1,
+        "hours": 11,
+        "minutes": 25
+    },
+    "system_image": "c800-universalk9-mz.SPA.154-3.M6.bin",
+    "serial_number": "FCZ1234A5BC",
+    "config_register": "0x2102"
 }
 ```
 
-# Disconnect from router
-```python
-from getRoutersConfig import setInformations
-
-router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
-
-system_information = router.disconnect()
-```
-
 # Get static routes
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 static_routes = router.getStaticRoutes()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 [
     {
         "subnet_address": "1.1.1.1",
@@ -92,14 +93,16 @@
 # Get interfaces
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 interfaces = router.getInterfaces()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 {
     "switched": [
@@ -129,14 +132,16 @@
 # Get DHCP
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 dhcp = router.getDhcp()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 [
     {
@@ -162,26 +167,65 @@
             ...
         ]
     },
     ...
 ]
 ```
 
+# Get ACL
+```python
+from getRoutersConfig import setInformations
+
+router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
+
+dhcp = router.getIpv4Acl()
+
+router.disconnect()
+```
+
+The Schema is :
+```json
+
+[
+    {
+        "type": "Extended",
+        "name": "acl-premium",
+        "rule": [
+            {
+                "sequence_number": 10,
+                "pass": "permit",
+                "protocol": "udp",
+                "source": "any",
+                "source_port": "all",
+                "destination": "host 192.168.10.3",
+                "destination_port": "snmp",
+                "macthes": 2417837
+            },
+            ...
+        ]
+    },
+    ...
+]
+```
+
 # Get full configuration
 ```python
 from getRoutersConfig import setInformations
 
 router = setInformations(host_ip: str='', host_port: str='22', host_snmp_community: str='public', user: str='', password: str='', bastion_ip: str='', bastion_port: str='')
 
 config = router.getFullConfiguration()
+
+router.disconnect()
 ```
 
 The Schema is :
 ```json
 
 {
     "system": {},
     "ipv4StaticRoutes": [],
     "interfaces": [],
-    "dhcp": []
+    "dhcp": [],
+    "acl": []
 }
 ```
```

### Comparing `getRoutersConfig-0.0.4/setup.py` & `getRoutersConfig-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="getRoutersConfig",
-    version="0.0.4",
+    version="0.0.5",
     description="get Cisco routers configuration as Json",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DanielRicklin/getRoutersConfig",
     author="DanielRicklin",
```

