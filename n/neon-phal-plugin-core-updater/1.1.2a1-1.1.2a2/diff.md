# Comparing `tmp/neon_phal_plugin_core_updater-1.1.2a1-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.1.2a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6671 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8286 b- defN 23-Jun-07 21:43 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2411 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-Jun-07 21:44 neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD
-7 files, 13278 bytes uncompressed, 5343 bytes compressed:  59.8%
+Zip file size: 6763 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8789 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-Jun-10 02:01 neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD
+7 files, 13781 bytes uncompressed, 5435 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_core_updater/__init__.py

```diff
@@ -59,41 +59,49 @@
         from neon_utils.packaging_utils import get_package_version_spec
         try:
             return get_package_version_spec(self.core_package)
         except ModuleNotFoundError as e:
             LOG.warning(e)
             return "0.0.0"
 
+    def _get_latest_github_release(self) -> str:
+        """
+        Get the latest GitHub release
+        """
+        url = f'https://api.github.com/repos/{self.github_ref}/releases/latest'
+        release = requests.get(url).json()
+        return release.get('tag_name')
+
     def _get_github_releases(self) -> List[str]:
         """
         Get GitHub release names in reverse-chronological order (newest first).
         """
         default_time = "2000-01-01T00:00:00Z"
         url = f'https://api.github.com/repos/{self.github_ref}/releases'
         releases: list = requests.get(url).json()
         releases.sort(key=lambda r: datetime.strptime(r.get('created_at',
                                                             default_time),
                                                       "%Y-%m-%dT%H:%M:%SZ"),
                       reverse=True)
-        return [r.get('name') for r in releases]
+        return [r.get('tag_name') for r in releases]
 
     def _get_pypi_releases(self):
         # TODO: Implement package release checks
         return []
 
     def check_core_updates(self, message: Message):
         """
         Check for a new core version and reply
         """
         LOG.debug(f"Checking for update. current={self._installed_version}")
         update_alpha = message.data.get("include_prerelease")
         new_version = None
         latest_version = None
         if self.pypi_ref:
-            releases = self._get_github_releases()
+            releases = self._get_pypi_releases()
         elif self.github_ref:
             releases = self._get_github_releases()
         else:
             LOG.error("No remote reference to check for updates")
             releases = []
 
         for release in releases:
@@ -105,15 +113,19 @@
                 # We Got to the installed version, stop parsing
                 break
             else:
                 latest_version = latest_version or release
                 new_version = new_version or release
 
         if new_version:
-            LOG.info(f"Found newer release: {new_version}")
+            LOG.info(f"Found newer version: {new_version}")
+        if not latest_version and self.github_ref:
+            LOG.info("No release found; get 'latest'")
+            latest_version = self._get_latest_github_release()
+        LOG.info(f"Got latest version: {latest_version}")
         if message:
             self.bus.emit(message.response({"new_version": new_version,
                                             "latest_version": latest_version,
                                             "installed_version": self._installed_version,
                                             "github_ref": self.github_ref,
                                             "pypi_ref": self.pypi_ref}))
```

## Comparing `neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.1.2a1
+Version: 1.1.2a2
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD` & `neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-neon_phal_plugin_core_updater/__init__.py,sha256=ZA9WEGuXFElnANSxuJEzVVbsfmSHOD4PDwhFwG7umaI,8286
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/METADATA,sha256=iqG-Ss5rCWp3_h5XkcSIOTKNKfMZHQfIFSx7C-vbHZQ,2411
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
-neon_phal_plugin_core_updater-1.1.2a1.dist-info/RECORD,,
+neon_phal_plugin_core_updater/__init__.py,sha256=Dw6m7hvR86FHUGKGceC2sBlPsZpov6EK2giGGOtWr4k,8789
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/METADATA,sha256=PJST2bOmuW9bmrm1diThgAo6LSbCkC5XN-dx7MxdmzY,2411
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
+neon_phal_plugin_core_updater-1.1.2a2.dist-info/RECORD,,
```

