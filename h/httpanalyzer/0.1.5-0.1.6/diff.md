# Comparing `tmp/httpanalyzer-0.1.5.tar.gz` & `tmp/httpanalyzer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpanalyzer-0.1.5.tar", last modified: Wed May 17 06:54:38 2023, max compression
+gzip compressed data, was "httpanalyzer-0.1.6.tar", last modified: Sat Jun 10 16:59:41 2023, max compression
```

## Comparing `httpanalyzer-0.1.5.tar` & `httpanalyzer-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/
--rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0     3249 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2555 2023-03-16 17:24:20.000000 httpanalyzer-0.1.5/README.md
--rw-rw-rw-   0        0        0      779 2023-05-17 06:53:38.000000 httpanalyzer-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-17 06:54:38.151331 httpanalyzer-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.116483 httpanalyzer-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.134628 httpanalyzer-0.1.5/src/httpanalyzer/
--rw-rw-rw-   0        0        0     4338 2023-04-29 10:00:22.000000 httpanalyzer-0.1.5/src/httpanalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.146292 httpanalyzer-0.1.5/src/httpanalyzer/lists/
--rw-rw-rw-   0        0        0        0 2023-04-29 09:34:34.000000 httpanalyzer-0.1.5/src/httpanalyzer/lists/__init__.py
--rw-rw-rw-   0        0        0    10519 2023-04-29 09:25:06.000000 httpanalyzer-0.1.5/src/httpanalyzer/src.py
--rw-rw-rw-   0        0        0      444 2023-04-29 09:33:58.000000 httpanalyzer-0.1.5/src/httpanalyzer/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 06:54:38.145238 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/
--rw-rw-rw-   0        0        0     3249 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 06:54:38.000000 httpanalyzer-0.1.5/src/httpanalyzer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 16:59:41.771789 httpanalyzer-0.1.6/
+-rw-rw-rw-   0        0        0     1091 2023-01-16 19:33:15.000000 httpanalyzer-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     3249 2023-06-10 16:59:41.770788 httpanalyzer-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2023-03-16 17:24:20.000000 httpanalyzer-0.1.6/README.md
+-rw-rw-rw-   0        0        0      779 2023-06-10 16:58:49.000000 httpanalyzer-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 16:59:41.771789 httpanalyzer-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 16:59:41.758779 httpanalyzer-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 16:59:41.764790 httpanalyzer-0.1.6/src/httpanalyzer/
+-rw-rw-rw-   0        0        0     4338 2023-04-29 10:00:22.000000 httpanalyzer-0.1.6/src/httpanalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:59:41.769789 httpanalyzer-0.1.6/src/httpanalyzer/lists/
+-rw-rw-rw-   0        0        0        0 2023-04-29 09:34:34.000000 httpanalyzer-0.1.6/src/httpanalyzer/lists/__init__.py
+-rw-rw-rw-   0        0        0    11118 2023-06-10 16:56:47.000000 httpanalyzer-0.1.6/src/httpanalyzer/src.py
+-rw-rw-rw-   0        0        0      444 2023-04-29 09:33:58.000000 httpanalyzer-0.1.6/src/httpanalyzer/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-10 16:59:41.768788 httpanalyzer-0.1.6/src/httpanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     3249 2023-06-10 16:59:41.000000 httpanalyzer-0.1.6/src/httpanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-06-10 16:59:41.000000 httpanalyzer-0.1.6/src/httpanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 16:59:41.000000 httpanalyzer-0.1.6/src/httpanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-10 16:59:41.000000 httpanalyzer-0.1.6/src/httpanalyzer.egg-info/top_level.txt
```

### Comparing `httpanalyzer-0.1.5/LICENSE.txt` & `httpanalyzer-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.5/PKG-INFO` & `httpanalyzer-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.5 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.6 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
```

### Comparing `httpanalyzer-0.1.5/README.md` & `httpanalyzer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.5/pyproject.toml` & `httpanalyzer-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "httpanalyzer"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Martin Merkli", email="martin.merkli@protonmail.com" },
 ]
 description = "Library for analyzing http-requests"
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.6"
```

### Comparing `httpanalyzer-0.1.5/src/httpanalyzer/__init__.py` & `httpanalyzer-0.1.6/src/httpanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `httpanalyzer-0.1.5/src/httpanalyzer/src.py` & `httpanalyzer-0.1.6/src/httpanalyzer/src.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     'yandex',  # Yandex
 }
 BOTS_PATH = {
     '/robots.txt',
     '/sitemap.xml',
 }
 MALICIOUS_PATHS = {
-    '${\'\'.class.forname(\'javax',
     '${@die(md5',
+    '${\'\'.class.forname(\'javax',
     '${jndi:ldap://$',
     '&_method=__construct&method=*&filter[]=',
     '(*),concat(0x7e,md5(1)',
     '--exec=<divd',
     '.git/config',
     '.git/head',
     '.github/workflows/',
@@ -117,14 +117,15 @@
     '/.ssh/id',
     '/autodiscover/autodiscover.json?@',
     '/config/',
     '/console',
     '/solr/',
     '/xiao',
     '/~user/',
+    '10000000)alert(1337)settimeout(',
     '2ioep23yxgkpwamwajv0rhiznfa',
     '3c625c27b4da33d3d5c12e8d02104755',
     '9568f36-d428-11d2-a769-00aa001acf42',
     '<script>alert(document.domain)</script>',
     '<svg/onload=alert',
     '?gid=1&page=2&rlist[]=@`%27`',
     '?xdebug_session_start=phpstorm',
@@ -142,14 +143,15 @@
     'actuator',
     'adjuncts/3a890183',
     'admin',
     'ajax_url_encode.php?link_url=',
     'ajaxserversettingschk',
     'ansible.cfg',
     'api/tools/protocol/checkupdate',
+    'api/v2/cmdb/system',
     'app_dev.php/_profiler',
     'appstate&dumpconfig=',
     'appveyor.yml',
     'atmail/webmail/?format=',
     'audit/gui_detail_view.php',
     'bin/sqlnet.log',
     'binname.arm',
@@ -172,14 +174,15 @@
     'conn.php.bak',
     'controller?mode=8700&operation=1&datagrid=179',
     'core-cloud-config.yml',
     'core-r7rules',
     'cplugerror',
     'createpage-entervariables.action',
     'crlfinjection',
+    'css_parser.php',
     'cubemail/filemanagement.php?action=dl&f=',
     'dashboardlayoutonecol',
     'datagrid=179&json=',
     'debug.seam',
     'docker-cloud.yml',
     'docker-compose',
     'dockerfile',
@@ -194,21 +197,26 @@
     'fhem/filelog_logwrapper?dev=',
     'field=updatexml',
     'file:///etc/hosts',
     'foodbakery_radius',
     'forums/search/z-->"><',
     'ftpsync.settings',
     'gcloud/credentials.db',
+    'ghost/preview',
     'google-api-private-key.json',
     'gponform/diag_form',
     'hnap1',
+    'idp/profile/oidc/authorize'
+    'indexisto/assets/js/indexisto-inject.php',
+    'info/system?wt=json',
     'inicio.jsp',
     'inicio.pl',
     'interact.sh',
     'invokefunction&function=',
+    'invoker/jmxinvokerservlet',
     'irj/go/km/navigation',
     'java.io.inputstreamreader',
     'java.lang.processbuilder',
     'java.lang:type=memory',
     'javascript:alert',
     'jira-webapp-dist',
     'jmxinvokerservlet',
@@ -224,39 +232,43 @@
     'linusadmin-phpinfo',
     'loadframe?frame_name=x&src=x&single_signout=',
     'log_upload_wsgi.py',
     'magmi/web/ajax_pluginconf.php',
     'mailsms/s?func=a',
     'mapname=poc.conf',
     'mbeanserverdelegate',
+    'meta-inf/maven/com.atlassian.jira',
     'methodaccessor.denymethodexecution',
     'microsoft.exchange.ediscovery.exporttool.application',
     'microstrategy',
     'mifs/.;/services',
     'mirai.arm',
     'mozi.a+jaws',
     'mpxnode/www/appconfig',
     'msmtprc',
+    'nagiosxi/login.php',
     'nginx-status',
     'nmaplowercheck',
     'nomgif=tarik',
     'null,null,null,null',
+    'oa_html/bispgraph.jsp',
     'oa_html/jtfwrepo.xml',
     'oauth2login?error=',
     'ognlcontext@default_member_access',
     'onload=confirm',
     'onmouseover=',
     'opensso/sessionservice',
     'option=com_joomlaupdater&controller=',
     'org.apache.struts2.servletactioncontext',
     'org.apache.tomcat.instancemanager',
     'org.jenkinsci.plugins.workflow.cps.cpsflowdefinition',
     'owa/auth/logon.aspx',
     'path=x&site[x][text]',
     'paytm_action=curltest&url=',
+    'phpe9568f36-d428-11d2-a769-00aa001acf42',
     'phpmyadmin',
     'plugins/advanced-dewplayer',
     'plus/ajax_officebuilding.php?act=key&key=',
     'pools/default/buckets',
     'portal/portal.mwsl',
     'portal0000.htm',
     'portal_inc.lua',
@@ -283,14 +295,15 @@
     'sharebox&query=app=common',
     'showlogin.cc',
     'sms5/ajax.sms_emoticon',
     'spring-mvc-showcase/resources',
     'sqlitemanager',
     'src/util/php/eval-stdin',
     'sslvpn_websession',
+    'stalker_portal/server/tools/auth_simple.php',
     'streaming/clients_live.php',
     'string[]{\'sh\',\'-c\',\'id\'}',
     'sum:sys.cpu.nice',
     'syscommand',
     'syslog.rlog=',
     'system/accountmanage/account',
     'telerik.web.ui.webresource.axd',
@@ -302,18 +315,21 @@
     'username=root&db=mysql',
     'utl_inaddr.get_host_name',
     'vendor/phpunit',
     'ventrilo_srv.ini',
     'w1sizyisicjjb252zxj0iiwgii1zaxplidf4msatzgvwdgggocbncmf5oi9ldgmvcgfzc3dkiiwgim91dcjdxq',
     'web_vms/level15',
     'webfig',
+    'webmail/calendar/minimizer/index.php',
     'wgetrc',
     'widget_tabbedcontainer_tab_panel',
     'wlwmanifest',
     'wp-config',
     'wp-content',
     'wp-includes',
     'wp-login',
+    'wpsolr-search-engine/classes/extensions/managed-solr-servers',
+    'www/delivery/afr.php',
     'xmldata?item=cpqkey',
     'zimlet',
     '嘍嘊set-',
 }
```

### Comparing `httpanalyzer-0.1.5/src/httpanalyzer.egg-info/PKG-INFO` & `httpanalyzer-0.1.6/src/httpanalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpanalyzer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for analyzing http-requests
 Author-email: Martin Merkli <martin.merkli@protonmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/MartinMerkli/httpanalyzer
 Project-URL: repository, https://github.com/MartinMerkli/httpanalyzer
 Keywords: python,http
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.5 Summary: Library for
+Metadata-Version: 2.1 Name: httpanalyzer Version: 0.1.6 Summary: Library for
 analyzing http-requests Author-email: Martin Merkli
 merkli@protonmail.com> License: MIT License Project-URL: homepage, https://
 github.com/MartinMerkli/httpanalyzer Project-URL: repository, https://
 github.com/MartinMerkli/httpanalyzer Keywords: python,http Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: System Administrators Requires-
```

