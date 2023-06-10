# Comparing `tmp/berhoelODF-0.2.3.tar.gz` & `tmp/berhoelodf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berhoelODF-0.2.3.tar", last modified: Thu Dec 31 15:31:48 2020, max compression
+gzip compressed data, was "berhoelodf-0.2.5.tar", max compression
```

## Comparing `berhoelODF-0.2.3.tar` & `berhoelodf-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     1064 2020-05-10 11:17:17.945919 berhoelODF-0.2.3/LICENSE
--rw-r--r--   0        0        0      921 2020-06-07 18:05:02.378842 berhoelODF-0.2.3/README.rst
--rw-r--r--   0        0        0      570 2020-05-10 11:20:06.017168 berhoelODF-0.2.3/berhoel/__init__.py
--rw-r--r--   0        0        0     2522 2020-06-07 16:29:20.559323 berhoelODF-0.2.3/berhoel/odf/__init__.py
--rw-r--r--   0        0        0       22 2020-12-31 14:16:55.806359 berhoelODF-0.2.3/berhoel/odf/_version.py
--rw-r--r--   0        0        0     6554 2020-06-07 16:41:50.483738 berhoelODF-0.2.3/berhoel/odf/ods.py
--rw-r--r--   0        0        0      916 2020-05-26 20:36:47.545459 berhoelODF-0.2.3/berhoel/odf/test/conftest.py
--rw-r--r--   0        0        0     1099 2020-05-26 20:35:33.681842 berhoelODF-0.2.3/berhoel/odf/test/test_odf_base.py
--rw-r--r--   0        0        0     3747 2020-05-26 19:52:07.227563 berhoelODF-0.2.3/berhoel/odf/test/test_ods.py
--rw-r--r--   0        0        0     1458 2020-12-31 15:30:42.652578 berhoelODF-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1669 2020-12-31 15:31:48.481720 berhoelODF-0.2.3/setup.py
--rw-r--r--   0        0        0     1645 2020-12-31 15:31:48.481953 berhoelODF-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-01-02 12:54:32.193852 berhoelodf-0.2.5/LICENSE
+-rw-r--r--   0        0        0      921 2021-01-02 12:54:32.193852 berhoelodf-0.2.5/README.rst
+-rw-r--r--   0        0        0      580 2023-06-10 19:58:57.760935 berhoelodf-0.2.5/berhoel/__init__.py
+-rw-r--r--   0        0        0     2718 2022-08-11 18:44:03.849002 berhoelodf-0.2.5/berhoel/odf/__init__.py
+-rw-r--r--   0        0        0     6832 2023-03-25 12:17:46.419354 berhoelodf-0.2.5/berhoel/odf/ods.py
+-rw-r--r--   0        0        0      928 2022-08-09 13:42:57.993979 berhoelodf-0.2.5/berhoel/odf/tests/conftest.py
+-rw-r--r--   0        0        0     1142 2022-08-09 13:43:09.517969 berhoelodf-0.2.5/berhoel/odf/tests/test_odf_base.py
+-rw-r--r--   0        0        0     3784 2022-08-09 13:43:19.533960 berhoelodf-0.2.5/berhoel/odf/tests/test_ods.py
+-rw-r--r--   0        0        0     2155 2023-06-10 19:59:45.544928 berhoelodf-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 berhoelodf-0.2.5/PKG-INFO
```

### Comparing `berhoelODF-0.2.3/LICENSE` & `berhoelodf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `berhoelODF-0.2.3/README.rst` & `berhoelodf-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `berhoelODF-0.2.3/berhoel/odf/__init__.py` & `berhoelodf-0.2.5/berhoel/odf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,97 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Give access to ods files.
 """
 
-# Standard libraries.
+# Standard library imports.
 from typing import List, Union
 from pathlib import Path
 from zipfile import ZipFile
 
-# Third party libraries.
+# Third party library imports.
 from lxml import etree
 
-__date__ = "2020/06/07 18:29:20 hoel"
+__date__ = "2022/08/11 20:44:03 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2020 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
 try:
+    # Local library imports.
     from ._version import __version__
 except ImportError:
     __version__ = "0.0.0+unknown0"
 
 
 class OdfXml:
-    """Base XML handling class for ODF processing.
-"""
+    """Base XML handling class for ODF processing."""
+
     def __init__(self, elem: etree._Element):
         """
-Args:
-    element (etree._Element): XML Element
+        Args:
+            element (etree._Element): XML Element
         """
         self.root = elem
         self.nsmap = (
             self.root.nsmap if hasattr(elem, "nsmap") else self.root.getroot().nsmap
         )
 
     def find(self, tag: str) -> etree._Element:
         """Find ``tag`` in this element.
 
-Args:
-    tag (str): XML tag to serarch for.
+        Args:
+            tag (str): XML tag to serarch for.
 
-Returns:
-   etree._Element: Element acc. to ``tag``.
-"""
+        Returns:
+           etree._Element: Element acc. to ``tag``."""
         return self.root.find(tag, namespaces=self.nsmap)
 
     def findall(self, tag: str) -> List[etree._Element]:
         """Find all of ``tag``.
 
-Args:
-   tag (str): XML tag to find.
+        Args:
+           tag (str): XML tag to find.
 
-Returns:
-   List[etree._Element]: Element acc. to ``tag``.
-"""
+        Returns:
+           List[etree._Element]: Element acc. to ``tag``."""
         return self.root.findall(tag, namespaces=self.nsmap)
 
     def _attrib_map(self, attrib: str) -> str:
         """Helper for ``get``: provide namespace.
 
-Args:
-   attrib (str): attribute name in the form of <namespace name>:<attr name>.
+        Args:
+           attrib (str): attribute name in the form of <namespace name>:<attr name>.
 
-Returns:
-   str: attribute name with extended namespace.
-"""
+        Returns:
+           str: attribute name with extended namespace."""
         ns, tag = attrib.split(":")
         return f"{{{self.nsmap[ns]}}}{tag}"
 
     def get(self, attrib: str) -> str:
         """Get atribute of this element, honors namespace.
 
-Args:
-   attrib(str): Attrribute name.
+        Args:
+           attrib(str): Attrribute name.
 
-Returns:
-   str: Attribute value.
-"""
+        Returns:
+           str: Attribute value."""
         return self.root.get(self._attrib_map(attrib))
 
 
 class Odf(OdfXml):
-    """Base class for OpenDocument Format files.
-"""
+    """Base class for OpenDocument Format files."""
 
     def __init__(self, path: Union[str, Path]):
         """Open ODF file from ``path``.
 
-Args:
-   path ([str,Path]): Location of OpenOffice file.
+        Args:
+           path ([str,Path]): Location of OpenOffice file.
         """
         with ZipFile(path) as odf_zip:
             with odf_zip.open("content.xml") as content:
                 doc = etree.parse(content)
         super().__init__(doc)
```

### Comparing `berhoelODF-0.2.3/berhoel/odf/ods.py` & `berhoelodf-0.2.5/berhoel/odf/ods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Processing ods (OpenDocument spreadsheets).
 """
 
-# Standard libraries.
+# Standard library imports.
 import re
 import typing
 import datetime
 import functools
 
+# Local library imports.
 from . import Odf, OdfXml
 
-__date__ = "2020/06/07 18:41:50 hoel"
+__date__ = "2023/03/25 13:17:46 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2020 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
 
 # Identify hyperlink in formula.
@@ -36,123 +37,114 @@
 class P(OdfXml):
     """Representing a paragraph in a cell."""
 
     @property
     def text(self) -> typing.Optional[str]:
         """Get text from paragraph.
 
-Returns:
-   str: Whole paragraph text if available.
-"""
+        Returns:
+           str: Whole paragraph text if available."""
         res = " ".join([i for i in self.root.itertext()])
         return res if res.strip() else None
 
 
 class Cell(OdfXml):
     """Representing a cell in a table row."""
 
     @property
     def text(self) -> typing.Optional[str]:
         """Return text associated with cell.
 
-Returns:
-   str: Cell text if avaliable.
-"""
+        Returns:
+           str: Cell text if avaliable."""
         if self.root is None:
             return None
         res = self.find("text:p")
         return None if res is None else P(res).text
 
     @property
     def date(self) -> typing.Optional[datetime.date]:
         """Return date value of cell if available.
 
-Returns:
-   datetime.date: Date value of cell if available.
-"""
+        Returns:
+           datetime.date: Date value of cell if available."""
         val = self.get("office:date-value")
         return (
             None if val is None else datetime.datetime.strptime(val, "%Y-%m-%d").date()
         )
 
     @property
     def value(self) -> typing.Optional[str]:
         """Return value of cell.
 
-Returns:
-   str: Value of cell if available.
-"""
+        Returns:
+           str: Value of cell if available."""
         return self.get("office:value")
 
     @property
     def float(self) -> typing.Optional[float]:
         """Return float value of cell.
 
-Returns:
-   float: ``float`` falue of cell if available.
-"""
+        Returns:
+           float: ``float`` falue of cell if available."""
         return None if self.value is None else float(self.value)
 
     @property
     def int(self) -> typing.Optional[int]:
         """Return integer value of cell.
 
-Returns:
-   int: ``int`` value if cell if available.
-"""
+        Returns:
+           int: ``int`` value if cell if available."""
         return None if self.value is None else int(self.value)
 
     @property
     def url(self) -> typing.Optional[str]:
         """Return URL associated with cell from hyperlink function.
 
-Returns:
-   str: url from ``HYPERLINK`` formula or cell hyperlink.
-"""
+        Returns:
+           str: url from ``HYPERLINK`` formula or cell hyperlink."""
         s_val: str = self.get("table:formula")
         val = None if s_val is None else IMDB_HYPERLINK.match(s_val)
         return None if val is None else val.group("url")
 
     @property
     def link(self) -> typing.Optional[typing.Dict[str, str]]:
         """Provide Link information.
 
-This link information is information of values referenced from diffrent tables in
-formula.
+        This link information is information of values referenced from diffrent tables in
+        formula.
 
-Returns:
-   dict: Result of ``re.match.groupdict``. Provided keys are ``sheet``, ``row``, and ``line.``
-"""
+        Returns:
+           dict: Result of ``re.match.groupdict``. Provided keys are ``sheet``, ``row``, and ``line.``
+        """
         dvd_link: str = self.get("table:formula")
         if dvd_link is not None:
             match = LINKED_CELL.match(dvd_link)
             if match is not None:
                 return match.groupdict()
         return None
 
 
 class Row(OdfXml):
-    """Representing table row.
-"""
+    """Representing table row."""
 
     def __init__(self, *args, **kw):
         super().__init__(*args, **kw)
         self.content_cell: str = self._attrib_map("table:table-cell")
         self.covered_cell: str = self._attrib_map("table:covered-table-cell")
         self.columns_repeated: str = self._attrib_map("table:number-columns-repeated")
 
     @functools.cached_property
     def cells(self) -> typing.List[typing.Optional[Cell]]:
         """Provide list of cells in row.
 
-Empty cells are replaced by ``None``, as are cells covered by merged cells.
+        Empty cells are replaced by ``None``, as are cells covered by merged cells.
 
-Returns:
-   List[Cell]: The cells making up the current row.
-"""
+        Returns:
+           List[Cell]: The cells making up the current row."""
         res: typing.List[typing.Optional[Cell]] = []
         for cell in self.root:
             if cell.tag == self.content_cell:
                 elem = Cell(cell)
                 res.extend(
                     [elem]
                     * (
@@ -173,74 +165,66 @@
                 )
             else:
                 raise NotImplementedError(f"Unknown tag {cell.tag}")
         return res
 
 
 class Table(OdfXml):
-    """Representation of spreadsheet table.
-"""
+    """Representation of spreadsheet table."""
 
     @functools.cached_property
     def name(self) -> str:
         """Return name attriute of table.
 
-Returns:
-   str: table name.
-"""
+        Returns:
+           str: table name."""
         return self.get("table:name")
 
     @functools.cached_property
     def rows(self) -> typing.List[Row]:
         """Return rows in table.
 
-Returns:
-   List[Row]: list of ``Row`` intances.
-"""
+        Returns:
+           List[Row]: list of ``Row`` intances."""
         return [Row(e) for e in self.findall("table:table-row")]
 
     @functools.cached_property
     def style_name(self) -> str:
         """Return table style-name.
 
-I Know of ``ta1`` for ordinary tables, and ``ta2`` for hidden tables.
+        I Know of ``ta1`` for ordinary tables, and ``ta2`` for hidden tables.
 
-Returns:
-   str: style name of table.
-"""
+        Returns:
+           str: style name of table."""
         return self.get("table:style-name")
 
     @property
     def hidden(self) -> bool:
         """Return whether table is hidden.
 
-Returns:
-   bool: ``True`` if table is hidden.
-"""
+        Returns:
+           bool: ``True`` if table is hidden."""
         return self.style_name == "ta2"
 
 
 class Ods(Odf):
-    """Processing ODS files.
-"""
+    """Processing ODS files."""
 
     def __init__(self, *args, **kw):
-        """Open ODF spreadsheet file.
-"""
+        """Open ODF spreadsheet file."""
         super().__init__(*args, **kw)
 
         self.root = self.find("office:body/office:spreadsheet")
 
     @functools.cached_property
     def tables(self) -> typing.List[Table]:
         """Return all tables in spreadsheet.
 
-Returns:
-   List[Table]: Tables in OpenOffice spreadsheet.
-"""
+        Returns:
+           List[Table]: Tables in OpenOffice spreadsheet."""
         return [Table(e) for e in self.findall("table:table")]
 
 
 # Local Variables:
 # mode: python
 # compile-command: "poetry run tox"
 # time-stamp-pattern: "30/__date__ = \"%:y/%02m/%02d %02H:%02M:%02S %u\""
```

### Comparing `berhoelODF-0.2.3/berhoel/odf/test/conftest.py` & `berhoelodf-0.2.5/berhoel/odf/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Common settiongs for testing `berhoel.odf`.
 """
-# Standard libraries.
+# Standard library imports.
 from pathlib import Path
 
-# Third party libraries.
+# Third party library imports.
 import pytest
 
-__date__ = "2020/05/26 22:36:47 hoel"
+__date__ = "2022/08/09 15:42:57 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2020 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
```

### Comparing `berhoelODF-0.2.3/berhoel/odf/test/test_odf_base.py` & `berhoelodf-0.2.5/berhoel/odf/tests/test_odf_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Testing base functionalities of berhoel.odf library.
 """
 
-# Standard libraries.
+# Standard library imports.
 from pathlib import Path
 
-# Third party libraries.
+# Third party library imports.
 import toml
 import pytest
 
+# First party library imports.
 from berhoel.odf import Odf, __version__
 
-__date__ = "2020/05/26 22:35:33 hoel"
+__date__ = "2022/08/09 15:43:09 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2020 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
```

### Comparing `berhoelODF-0.2.3/berhoel/odf/test/test_ods.py` & `berhoelodf-0.2.5/berhoel/odf/tests/test_ods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """Testing accessing ods files.
 """
 
-# Third party libraries.
+# Third party library imports.
 import pytest
 
+# First party library imports.
 from berhoel.odf.ods import LINKED_CELL, IMDB_HYPERLINK, Ods
 
-__date__ = "2020/05/26 21:49:34 hoel"
+__date__ = "2022/08/09 15:43:19 hoel"
 __author__ = "Berthold Höllmann"
 __copyright__ = "Copyright © 2020 by Berthold Höllmann"
 __credits__ = ["Berthold Höllmann"]
 __maintainer__ = "Berthold Höllmann"
 __email__ = "berhoel@gmail.com"
```

### Comparing `berhoelODF-0.2.3/pyproject.toml` & `berhoelodf-0.2.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,80 @@
 [tool.poetry]
 name = "berhoelODF"
-version = "0.2.3"
+version = "0.2.5"
 
 description = "Lightweight and limited access to odf files using lxml."
 
-packages = [
-    { include = "berhoel" },
-]
-exclude=["**/.#*.py", "**/#*.py#"]
+packages = [{ include = "berhoel" }]
+exclude = ["**/.#*.py", "**/#*.py#"]
 
 authors = ["Berthold Höllmann <berthold-gitlab@xn--hllmanns-n4a.de>"]
 license = "MIT"
 
 repository = "https://gitlab.com/berhoel/python/berhoelodf.git"
 homepage = "https://python.xn--hllmanns-n4a.de/berhoelODF/"
 documentation = "https://www.xn--hllmanns-n4a.de/python/berhoelODF/"
 readme = "README.rst"
 
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Topic :: Utilities",
-]
+classifiers = ["Development Status :: 4 - Beta", "Topic :: Utilities"]
 
 [tool.poetry.dependencies]
-python = ">3.8"
+python = "^3.8,<4.0"
 lxml = "*"
 
 [tool.poetry.dev-dependencies]
+black = "*"
+flake8 = "*"
+pdbpp = "*"
 tox = "*"
-toml = "*"
+pylint = "*"
+pylint-plugin-utils = "*"
 pytest = "*"
+pytest-benchmark = "*"
+pytest-black = "*"
 pytest-cov = "*"
+pytest-flake8 = "*"
+pytest-isort = "*"
+pytest-mock = "*"
 pytest-runner = "*"
-pytest-cache = "*"
 pytest-sugar = "*"
-pytest-isort = "*"
-isort = "*"
+xdoctest = "*"
 rope = "*"
-flake8 = "*"
-pylint = "*"
-pylint-common = "*"
-pylint-plugin-utils = "*"
-black = "*"
-Sphinx = "*"
-sphinx-rtd-theme = "*"
-sphinx-argparse = "*"
-sphinx_bootstrap_theme = "*"
-pdbpp = "*"
-numpydoc = "*"
+bhoelHelper = "*"
+berhoel-sphinx-settings = { git = "https://gitlab.com/berhoel/python/berhoel-sphinx-settings.git", rev = "main" }
+
+[tool.berhoel.helper.set_version]
+version_files = ["berhoel/odf/_version.py"]
 
 [tool.isort]
-profile = "black"
 multi_line_output = 3
+dedup_headings = true
 include_trailing_comma = true
 indent = '    '
+float_to_top = true
+namespace_packages = ['berhoel']
+force_grid_wrap = 0
+balanced_wrapping = true
+use_parentheses = true
 length_sort = true
 line_length = 88
-balanced_wrapping = true
 combine_as_imports = true
-import_heading_stdlib = 'Standard libraries.'
-import_heading_thirdparty = 'Third party libraries.'
-known_first_party = ['berhoel']
+sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
+import_heading_stdlib = 'Standard library imports.'
+import_heading_thirdparty = 'Third party library imports.'
+import_heading_firstparty = 'First party library imports.'
+import_heading_localfolder = 'Local library imports.'
+default_section = "THIRDPARTY"
+known_first_party = ["berhoel"]
+known_third_party = ["pytest"]
+
+[tool.pytest.ini_options]
+minversion = "7.0"
+addopts = "--doctest-modules --ff --pdb -s --cov=berhoel --cov-report=term --cov-report=html --cov-branch --isort --black"
+testpaths = ["berhoel"]
 
 [flake8]
 max-line-length = 88
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `berhoelODF-0.2.3/PKG-INFO` & `berhoelodf-0.2.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: berhoelodf
-Version: 0.2.3
+Version: 0.2.5
 Summary: Lightweight and limited access to odf files using lxml.
 Home-page: https://python.xn--hllmanns-n4a.de/berhoelODF/
 License: MIT
 Author: Berthold Höllmann
 Author-email: berthold-gitlab@xn--hllmanns-n4a.de
-Requires-Python: >3.8
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: lxml
 Project-URL: Documentation, https://www.xn--hllmanns-n4a.de/python/berhoelODF/
 Project-URL: Repository, https://gitlab.com/berhoel/python/berhoelodf.git
 Description-Content-Type: text/x-rst
 
 ``berhoelODF``
```

