# Comparing `tmp/nsb_toolbox-0.5.2.tar.gz` & `tmp/nsb_toolbox-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsb_toolbox-0.5.2.tar", max compression
+gzip compressed data, was "nsb_toolbox-0.5.3.tar", max compression
```

## Comparing `nsb_toolbox-0.5.2.tar` & `nsb_toolbox-0.5.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-01-27 02:57:03.554152 nsb_toolbox-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0    15412 2023-01-27 02:57:03.554152 nsb_toolbox-0.5.2/README.md
--rw-r--r--   0        0        0        2 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/__init__.py
--rw-r--r--   0        0        0     4295 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/_base_questions.py
--rw-r--r--   0        0        0    10499 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/assign.py
--rw-r--r--   0        0        0     3629 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/classes.py
--rw-r--r--   0        0        0     2933 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/cli.py
--rw-r--r--   0        0        0     8468 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/docx_utils.py
--rw-r--r--   0        0        0      972 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/importers.py
--rw-r--r--   0        0        0    18685 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/tables.py
--rw-r--r--   0        0        0     9971 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/nsb_toolbox/yamlparsers.py
--rw-r--r--   0        0        0      912 2023-01-27 02:57:03.558152 nsb_toolbox-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 nsb_toolbox-0.5.2/setup.py
--rw-r--r--   0        0        0    16012 1970-01-01 00:00:00.000000 nsb_toolbox-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0    15412 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/README.md
+-rw-r--r--   0        0        0        2 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/_base_questions.py
+-rw-r--r--   0        0        0    10499 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/assign.py
+-rw-r--r--   0        0        0     3629 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/classes.py
+-rw-r--r--   0        0        0     2929 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/cli.py
+-rw-r--r--   0        0        0     8468 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/docx_utils.py
+-rw-r--r--   0        0        0      972 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/importers.py
+-rw-r--r--   0        0        0    19604 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/tables.py
+-rw-r--r--   0        0        0     9971 2023-06-10 03:49:48.972602 nsb_toolbox-0.5.3/nsb_toolbox/yamlparsers.py
+-rw-r--r--   0        0        0      912 2023-06-10 03:49:48.976602 nsb_toolbox-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    15964 1970-01-01 00:00:00.000000 nsb_toolbox-0.5.3/PKG-INFO
```

### Comparing `nsb_toolbox-0.5.2/LICENSE.txt` & `nsb_toolbox-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/README.md` & `nsb_toolbox-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/_base_questions.py` & `nsb_toolbox-0.5.3/nsb_toolbox/_base_questions.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,20 +93,30 @@
             ]
         )
 
     @cached_property
     def qtypes(self) -> np.ndarray:
         return np.array(
             [
-                QuestionType(self._cells[i].paragraphs[0].runs[0].text).value
+                QuestionType(qtype).value
+                if (qtype := self._cells[i].paragraphs[0].runs[0].text)
+                else ""
                 for i in column_indexer(2, len(self._cells), self._col_count)
             ],
             dtype="<U20",
         )
 
+    @property
+    def qtype_stats(self) -> Dict[str, int]:
+        return {
+            val: count
+            for val, count in zip(*np.unique(self.qtypes, return_counts=True))
+            if val
+        }
+
     @cached_property
     def subcategories(self) -> np.ndarray:
         return np.array(
             [
                 self._cells[i].text
                 for i in column_indexer(12, len(self._cells), self._col_count)
             ],
```

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/assign.py` & `nsb_toolbox-0.5.3/nsb_toolbox/assign.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/classes.py` & `nsb_toolbox-0.5.3/nsb_toolbox/classes.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/cli.py` & `nsb_toolbox-0.5.3/nsb_toolbox/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from .yamlparsers import ParsedQuestionSpec
 
 
 def make(args):
     path = Path(args.path).with_suffix(".docx")
     if args.subj is not None:
         args.subj = Subject.from_string(args.subj).value
-    questions = RawQuestions.make(
+    RawQuestions.make(
         nrows=args.rows, name=args.name, subj=args.subj, set=args.set
-    )
-    questions.save(path)
+    ).format(verbose=False).save(path)
 
 
 def format(args):
 
     questions = RawQuestions.from_docx_path(args.path)
     questions.format(force_capitalize=args.capitalize)
     questions.save(args.path)
```

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/docx_utils.py` & `nsb_toolbox-0.5.3/nsb_toolbox/docx_utils.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/importers.py` & `nsb_toolbox-0.5.3/nsb_toolbox/importers.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/tables.py` & `nsb_toolbox-0.5.3/nsb_toolbox/tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,17 +137,14 @@
             Set. If not none, fills the set column of the table.
 
         Returns
         -------
         Self
         """
         document = Document()
-        font = document.styles["Normal"].font
-        font.name = "Times New Roman"
-        font.size = Pt(12)
 
         table = document.add_table(rows=1 + nrows, cols=13)
 
         table.style = "Table Grid"
         table.autofit = False
         table.allow_autofit = False
 
@@ -163,16 +160,14 @@
 
         for col_name, col_idx in COL_MAPPING.items():
 
             for cell_idx in col_iter(col_idx):
 
                 cell = _cells[cell_idx]
                 cell.width = Inches(COL_WIDTHS[col_idx])
-                if COL_COLORS[col_name]:
-                    shade_cell(cell, COL_COLORS[col_name])
 
                 if cell_idx < _col_count:
                     cell.paragraphs[0].add_run(col_name)
 
                 elif col_name == "Subj" and subj is not None:
                     cell.paragraphs[0].text = subj
 
@@ -185,15 +180,15 @@
 
         # ques header is italicized
         ques_run = table.cell(0, COL_MAPPING["Ques"]).paragraphs[0].runs[0]
         ques_run.italic = True
 
         return cls(document)
 
-    def format(self, force_capitalize: Optional[bool] = False):
+    def format(self, force_capitalize: Optional[bool] = False, verbose: bool = True):
         """Formats a Word document containing a Science Bowl question table.
 
         Specifically, this function makes sure the columns fit the following
         criteria:
 
         TUB: Contains only TOSS-UP or BONUS
         Subj: Contains only one of the valid subject areas
@@ -205,21 +200,34 @@
 
         Parameters
         ----------
         force_capitalize : bool, default True
             If True, all answer lines will be capitalized
         """
 
-        cols_to_format = ("TUB", "Subj", "Ques", "LOD", "Set", "Author", "Subcat")
+        cols_to_format = (
+            "TUB",
+            "Subj",
+            "Ques",
+            "LOD",
+            "Set",
+            "Rd",
+            "Q Letter",
+            "Author",
+            "Subcat",
+        )
 
         FORMATTERS = {
             "TUB": TuBCellFormatter(),
             "Subj": SubjectCellFormatter(),
             "Ques": QuestionCellFormatter(force_capitalize=force_capitalize),
             "LOD": DifficultyFormatter(),
+            "Set": SetFormatter(),
+            "Rd": RdFormatter(),
+            "Q Letter": QLetterFormatter(),
         }
 
         _cells = self.document.tables[0]._cells
         _col_count = self.document.tables[0]._column_count
 
         font = self.document.styles["Normal"].font
         font.name = "Times New Roman"
@@ -233,28 +241,36 @@
         )
 
         for col_name in cols_to_format:
             formatter = FORMATTERS.get(col_name, CellFormatter())
             formatter.preprocess_format_column(
                 _cells[i] for i in col_iter(COL_MAPPING[col_name])
             )
-        if row_filter._num_records == 0:
-            print("Found no errors 😄")
-        self.print_stats()
+        if verbose:
+            if row_filter._num_records == 0:
+                print("Found no errors 😄")
+            self.print_stats()
+
+        return self
 
     def print_stats(self):
         print("\nStatistics")
         print(f"{'-':->34}")
         print(f"{'Set':<9}{'LOD':^}{'TUB':>10}{'Have':>11}")
         print(f"{'-':->34}")
 
         for key in sorted(self.stats.keys()):
             have = self.stats.get(key, 0)
             print(f"{key}{have:>10}")
 
+        print(f"{'-':->34}")
+        for key in sorted(self.qtype_stats.keys()):
+            have = self.qtype_stats.get(key, 0)
+            print(f"{key :<15}{have :>18}")
+
     @cached_property
     def tubs(self) -> np.ndarray:
         """Overridden because TUB might be malformed."""
         return np.array(
             [
                 TossUpBonus(self._cells[i].text).value
                 if self._cells[i].text in ("TOSS-UP", "BONUS", "VISUAL BONUS")
@@ -284,14 +300,16 @@
     def format(self, cell: _Cell) -> _Cell:
         """All CellFormatters have a format function."""
         return cell
 
     def preprocess_format(self, cell: _Cell) -> _Cell:
         """Convenience function to preprocess and format a cell."""
         cell = preprocess_cell(cell)
+        if hasattr(self, "color"):
+            shade_cell(cell, self.color)
         if cell.text.strip() != "":
             return self.format(cell)
 
     def preprocess_format_column(self, cells: Iterable[_Cell]) -> _Cell:
         """Convenience function to preprocess and format an entire column."""
         for idx, cell in enumerate(cells):
             row_filter.curr_row = idx + 1
@@ -473,26 +491,48 @@
             highlight_cell_text(cell, WD_COLOR_INDEX.RED)
             logger.error("Invalid subject.")
 
         return cell
 
 
 class DifficultyFormatter(CellFormatter):
+    """Formats the difficulty cell and shades it with the appropriate color."""
+
+    color = COL_COLORS["LOD"]
+
     def format(self, cell: _Cell) -> _Cell:
 
         if cell.text:
             try:
                 int(cell.text)
             except ValueError:
                 highlight_cell_text(cell, WD_COLOR_INDEX.RED)
                 logger.error("LOD should be blank or an integer.")
 
         return cell
 
 
+class SetFormatter(CellFormatter):
+    """Formats the set cell and shades it with the appropriate color."""
+
+    color = COL_COLORS["Set"]
+
+
+class RdFormatter(CellFormatter):
+    """Formats the round cell and shades it with the appropriate color."""
+
+    color = COL_COLORS["Rd"]
+
+
+class QLetterFormatter(CellFormatter):
+    """Formats the question letter cell and shades it with the appropriate color."""
+
+    color = COL_COLORS["Q Letter"]
+
+
 def _format_question_type_run(q_type_run: Run, run_match: re.Match) -> QuestionType:
     """Returns the type (Multiple Choice or Short Answer) of the question.
 
     Also handles italicizing the run containing the question type."""
     _q_type = QuestionType.from_string(run_match.group(1))
     # if the run contains more than the question type, split
     # the run into two
```

### Comparing `nsb_toolbox-0.5.2/nsb_toolbox/yamlparsers.py` & `nsb_toolbox-0.5.3/nsb_toolbox/yamlparsers.py`

 * *Files identical despite different names*

### Comparing `nsb_toolbox-0.5.2/pyproject.toml` & `nsb_toolbox-0.5.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsb-toolbox"
-version = "0.5.2"
+version = "0.5.3"
 repository = "https://github.com/rishi-kulkarni/nsbtoolbox"
 description = "Utilities for editing Science Bowl questions"
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 license = "LICENSE.txt"
 readme = "README.md"
 packages = [{include = "nsb_toolbox"}]
 classifiers = [
```

### Comparing `nsb_toolbox-0.5.2/setup.py` & `nsb_toolbox-0.5.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,377 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nsb-toolbox
+Version: 0.5.3
+Summary: Utilities for editing Science Bowl questions
+Home-page: https://github.com/rishi-kulkarni/nsbtoolbox
+License: LICENSE.txt
+Author: Rishi Kulkarni
+Author-email: rishi@kulkarni.science
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: python-docx (>=0.8.11,<0.9.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
+Project-URL: Repository, https://github.com/rishi-kulkarni/nsbtoolbox
+Description-Content-Type: text/markdown
 
-packages = \
-['nsb_toolbox']
+# NSB Toolbox
 
-package_data = \
-{'': ['*']}
+## A command-line utility for formatting Science Bowl questions
 
-install_requires = \
-['python-docx>=0.8.11,<0.9.0',
- 'pyyaml>=6.0,<7.0',
- 'scipy>=1.8.0,<2.0.0',
- 'typing-extensions>=4.2.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['nsb = nsb_toolbox.cli:main']}
-
-setup_kwargs = {
-    'name': 'nsb-toolbox',
-    'version': '0.5.2',
-    'description': 'Utilities for editing Science Bowl questions',
-    'long_description': '# NSB Toolbox\n\n## A command-line utility for formatting Science Bowl questions\n\nVersion 0.5.2 - Updated for 2024 NSB\n\nThe NSB Toolbox contains a set of tools to make it easier to write and edit Science Bowl questions. It ensures that questions are compliant with the official Science Bowl format, allowing writers to focus on just writing the questions. It also highlights common formatting errors for editors, allowing them to focus on checking content without worrying that they\'re missing formatting issues here and there.\n\n## Table of Contents\n\n1. [Installation](#installation)\n2. [Documentation](#documentation)\n    1. [nsb format](#nsb-format)\n        1. [Auto-Formatting](#auto-format)\n        2. [Linting](#linting)\n    2. [nsb assign](#nsb-assign)\n        1. [Sample Configuration](#assign-config)\n    3. [nsb make](#nsb-make)\n3. [Known Issues](#known-issues)\n\n<a name="installation"></a>\n## Installation\nCurrently, the NSB Toolbox can be installed via pip from this github. To do so, you will need:\n\n* Python 3.8 or greater installed on your computer.\n* Enter and run ```pip install nsb-toolbox``` in your command line.\n* Verify the installation worked by running ```nsb -h``` in your command line. If the help information for the toolbox appears, the installation was successful.\n\n<a name="documentation"></a>\n## Documentation\nYou can access the NSB Toolbox via the ```nsb``` commandlet. Running ```nsb -h``` displays the following help menu.\n\n```powershell\n(base) PS C:\\Users\\rishik> nsb -h\nusage: nsb [-h] {format,make} ...\n\nUtilities for managing Science Bowl .docx files.\n\noptional arguments:\n  -h, --help     show this help message and exit\n\nsubcommands:\n  {format,make}\n    format       format a Science Bowl file\n    make         make a Science Bowl table\n```\n<a name="nsb-format"></a>\n## nsb format\n```nsb format``` provides two functions in one - first, it is a formatter than ensures Science Bowl questions are properly spaced (four spaces between question type and start of stem, blank line between stem and answer, etc). Second, it is a linter that highlights questions that it cannot fix. It is important to note that ```nsb format``` cannot catch every problem with the question! For example, ```nsb format``` will never be able to check question content for correctness. All ```nsb format``` can do is eliminate or highlight typical formatting errors.\n\n### Usage\n\n```nsb format``` takes a single mandatory argument, the path to the target .docx file. For example:\n\n```nsb format path/to/nsb/questions.docx```\n\nIt also takes a single optional argument, `--capitalize`. If given, `nsb format` will force every answer line to be capitalized. For example:\n\n```nsb format path/to/nsb/questions.docx --capitalize```\n\n<a name="auto-format"></a>\n### Auto-Formatting\n\n```nsb format``` outright fixes a number of formatting errors. It strives to produce questions that have the following characteristics:\n\n* The question class (TOSS-UP, BONUS) is uppercase.\n* Subject (Biology, Chemistry, etc.) are title case.\n* Question type (Multiple Choice, Short Answer) are italicized and title case.\n* There are four spaces between the question type and the start of the stem.\n* For multiple choice questions, the stem and choices are each separated by a single paragraph break.\n* There are two paragraph breaks before the answer line.\n* The answer line is uppercase, assuming the `--capitalize` argument is used.\n\nNotably, `nsb format` operates by moving, copying, and inserting XML elements. This ensures that **user-provided formatting won\'t be overwritten** (for example, superscripts and subscripts for mathematical formulae). \n\nFor example, all of the following improperly formatted questions:\n\n![Before Formatting](/docs/images/before_format.png) \n\n```nsb format``` will automatically convert these questions to be compliant with the Science Bowl format:\n\n![After Formatting](/docs/images/after_format.png)\n\nShorthand notation can also be used to reduce the amount of time writers spend writing boilerplate.\n\n![Before Shorthand](/docs/images/before_shorthand.png)\n\nTU and B will be converted to TOSS-UP and BONUS, respectively. The shorthand for the subject categories is the first letter of the subject, aside for Earth and Space (ES) and Energy (EN). MC and SA will be converted to Multiple Choice and Short Answer, as well.\n\n![After Shorthand](/docs/images/after_shorthand.png)\n\nFinally, ```nsb format``` will automatically correct minor errors in question structure. For example, the following question has multiple X) choices:\n\n![Before Multiple Choice Correction](/docs/images/before_mc_correct.png)\n\nThe mislabeled choices will be automatically corrected. Note that an answer line that has been explicitly given will not be auto-capitalized:\n\n![After Multiple Choice Correction](/docs/images/after_mc_correct.png)\n\n<a name="linting"></a>\n### Linting\n\nIf ```nsb format``` fails to parse a cell, it will raise linting errors by highlighting the question and printing the error in the command line. There are two levels of errors: parsing errors, which will highlight a cell red, and question structure errors, which will highlight the problematic structure yellow. `nsb format` searches for the following errors:\n\n* The question has a class, subject, type, stem, and answer. Multiple Choice questions should also have four choices.\n* Question type is correctly labeled - Multiple Choice questions should have choices, Short Answer questions should not.\n* For multiple choice questions, the wording of the answer line should match the wording of the choice.\n\nFor example:\n\n![Linter Errors](/docs/images/linter_errors.png)\n\nThe first question is missing two choices, so it can\'t be fully parsed, raising a red error. The second question is merely mislabeled - it says it\'s a Multiple Choice question, but is recognized as a Short Answer question. This raises a yellow error, highlighting the question type. Messages corresponding to these errors are printed in the terminal, as well:\n\n```\n(base) rishi@RISHI-DESKTOP:~$ nsb format after_format.docx\nQuestion 6: Couldn\'t parse question, was looking for QuestionFormatterState.CHOICES\nQuestion 7: Question type is MC, but has no choices.\n```\n\n```nsb format``` is not capable of deleting lines that contain text. This is intentional - while there are errors that ```nsb format```  highlights that it could probably fix automatically, the maintainer believes it is more prudent to leave whitespace formatting to ```nsb format``` and making any other changes by hand.\n\n<a name="nsb-assign"></a>\n## nsb assign\n`nsb assign` uses a set of configuration options to automatically assign a set of edited questions to rounds. \n\n### Usage\n\n```nsb assign``` takes two mandatory arguments, the path to the edited set of Science Bowl questions and the path to the configuration file. For example:\n\n```nsb assign path/to/nsb/questions.docx -c path/to/config.yaml```\n\nIt also takes an optional `--dry-run` argument, which will report statistics on the assignment procedure, but will not write the successful assignment to disk. This is primarily useful for determining what additional questions of a given difficulty or type are required. For example:\n\n```zsh\n❯ nsb assign Kulkarni_HS_Chemistry_Regionals.docx -c assign.yaml --dry-run\nSet      LOD       TUB       Need      Have\nHSR       1       BONUS         8        40\nHSR       1     TOSS-UP         8        46\nHSR       2       BONUS         0        21\nHSR       2     TOSS-UP        10        31\nHSR       3       BONUS         0        22\nHSR       3     TOSS-UP         0        30\nHSR-A     1       BONUS        25        10\nHSR-A     1     TOSS-UP        25         5\nHSR-A     2       BONUS        23         3\nHSR-A     2     TOSS-UP        30         5\nHSR-A     3       BONUS        13        13\nHSR-A     3     TOSS-UP         6         9\nHSR-B     1       BONUS        25         7\nHSR-B     1     TOSS-UP        25         6\nHSR-B     2       BONUS        23         6\nHSR-B     2     TOSS-UP        30         4\nHSR-B     3       BONUS        13        13\nHSR-B     3     TOSS-UP         6         9\nNot writing assignments as this is a dry run.\n```\n\n<a name="assign-config"></a>\n### Sample Configuration File\n\nBelow is a sample configuration file for a High School Regional set. The sections are explained in more detail further below.\n\n```yaml\nConfiguration:\n  Shuffle Subcategory: True \n  Shuffle Pairs: False \n  Shuffle LOD: False\n  Random Seed: ~\n  Subcategory Mismatch Penalty: 1\n  Preferred Writers: []\n\nRound Definitions:\n  Tiebreakers:\n    TU:\n      LOD: [2]\n\n  RoundRobin:\n    TU:\n      LOD: [1, 1, 1, 1]\n      Subcategory: [Organic, ~, ~, ~]\n\n    B:\n      LOD: [1, 1, 1, 1]\n      Subcategory: [Organic, ~, ~, ~]\n\n  DoubleElim1-4:\n    TU:\n      LOD: [2, 2, 2, 2]\n\n    B:\n      LOD: [2, 2, 2, 2]\n\n  DoubleElim5-6:\n    TU:\n      LOD: [2, 2, 2, 2]\n\n    B:\n      LOD: [2, 2, 3, 3]\n\n  DoubleElim7-9:\n    TU:\n      LOD: [2, 2, 3, 3]\n    B:\n      LOD: [2, 3, 3, 3]\n\nSets:\n  - Set: [HSR]\n    Prefix: RR\n    Rounds: [1, 2]\n    Template: RoundRobin\n\n  - Set: [HSR]\n    Prefix: TB\n    Rounds: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]\n    Template: Tiebreakers\n\n  - Set: [HSR-A, HSR-B]\n    Prefix: RR\n    Rounds: [3, 4, 6, 7, 8]\n    Template: RoundRobin\n\n  - Set: [HSR-A, HSR-B]\n    Prefix: RR\n    Rounds: [5]\n    Template:\n      from: RoundRobin\n      add:\n        TU:\n          LOD: [1]\n        B:\n          LOD: [1]\n\n  - Set: [HSR-A, HSR-B]\n    Prefix: DE\n    Rounds: [1, 2, 3, 4]\n    Template: DoubleElim1-4\n\n  - Set: [HSR-A, HSR-B]\n    Prefix: DE\n    Rounds: [5, 6]\n    Template: DoubleElim5-6\n\n  - Set: [HSR-A, HSR-B]\n    Prefix: DE\n    Rounds: [7, 8, 9]\n    Template: DoubleElim7-9\n\n```\n\n### Configuration Options\n\n`Shuffle Subcategory`: Setting this option to `True` randomizes the order that any subcategory specification appears in a round. For example, if you have requested `["Organic", ~, ~, ~]`, setting this option to `True` makes the `"Organic"` subcategory uniformly distributed rather than the first question of each round. Note that setting this option to `True` breaks any matching between `TU` and `B` subcategories.\n\n`Shuffle Pairs`: Setting this option to `True` adds a randomization step after each pair of questions has been constructed. This is useful when you have intentionally matched `TU` and `B` subcategories, for example, but want to randomize the order that the subcategories appear in each round. Note that even when this is enabled, the final pair of each round will be `Short Answer` questions.\n\n`Shuffle LOD`: Setting this option to `True` randomizes the order that question difficulties appear in each round, similar to the above options.\n\n`Random Seed`: Setting this option to an integer fixes the generated assignment, all else being equal. If left unspecified or set to None, the assignment will have a slight random element to it.\n\n`Subcategory Mismatch Penalty`: Setting this option to an integer specifies how much cost is incurred by creating a subcategory mismatch. Common options include: \n\n`1`, which says that matching a question with the right difficulty but wrong subcategory is equally costly as using a question whose difficulty is off by `1`, but the subcategory is correct. \n\n`2`, which says that matching a question with the right difficulty but wrong subcategory is always less preferable than using a question with the right subcategory but off-by-one difficulty, but also always more preferable than using a question with the right subcategory but off-by-two difficulty.\n\n`Preferred Writers`: If specified, any writers NOT in this list are given a small penalty, encouraging the optimization algorithm to use the preferred writers. This penalty is very small and should never result in a question of the wrong subcategory or difficulty from a preferred writer being used over a question of the right subcategory and difficulty from an unpreferred writer.\n\n### Round Definitions\n\n```yaml\nRound Definitions:\n  Tiebreakers:\n    TU:\n      LOD: [2]\n\n  RoundRobin:\n    TU:\n      LOD: [1, 1, 1, 1]\n      Subcategory: [Organic, ~, ~, ~]\n    B:\n      LOD: [1, 1, 1, 1]\n      Subcategory: [Organic, ~, ~, ~]\n```\n\n`Round Definitions` serve as templates to build round specifications. Each round definition needs to specify the question types it uses (`TU` and/or `B` for TOSS-UP and BONUS) and the Level of Difficulty of each question. Optionally, the subcategories can be specified. Entering a `~` indicates that there is no subcategory preference for that slot.\n\nTo explain the above specification in plain English, we want all Tiebreaker rounds to consist of a single\nTOSS-UP question with a difficulty of 2, and all Round Robin rounds to consist of 4 TOSS-UPs and 4 BONUSes that each have a difficulty of 1. Finally, a quarter of TOSS-UPs and BONUSes should use the "Organic" subcategory.\n\n### Sets\n\n```yaml\nSets:\n  - Set: [HSR-A, HSR-B]\n    Prefix: RR\n    Rounds: [1, 2]\n    Template: RoundRobin\n```\n\nThe `Sets` section actually specifies what rounds will be built. A set is defined with the `Set`, `Prefix`, `Rounds`, and `Template` keys. The `Set`, `Prefix`, and `Rounds` keys are round meta-data, while the `Template` key will build the round using the matching entry in the `Round Specifications` section. \n\nThese keys are used combinatorially - the above set will generate 4 rounds: HSR-A RR1, HSR-A RR2, HSR-B RR1, and HSR-B RR2. \n\nOptionally, `Sets` can use the `from:`, `add:` syntax:\n\n```yaml\n  - Set: [HSR-A, HSR-B]\n    Prefix: RR\n    Rounds: [5]\n    Template:\n      from: RoundRobin\n      add:\n        TU:\n          LOD: [1]\n        B:\n          LOD: [1]\n```\nThis syntax specifies that the `RoundRobin` template should be used, but there should be an extra TOSS-UP and BONUS that each have a difficulty of 1.\n\n<a name="nsb-make"></a>\n## nsb make\n```nsb make``` produces a blank Science Bowl question table with a designated number of lines. This is a convenience function for writers. ```nsb make -h``` shows the following help menu:\n\n```powershell\n(base) PS C:\\Users\\rishik> nsb make -h\nusage: nsb make [-h] [-n NAME] [-st {HSR,HSN,MSR,MSN}] [-su {B,C,P,M,ES,EN}] path rows\n\npositional arguments:\n  path                  path to the Science Bowl docx file\n  rows                  number of rows in output table\n\noptions:\n  -h, --help            show this help message and exit\n  -n NAME, --name NAME  Last, First name of author\n  -st {HSR,HSN,MSR,MSN}, --set {HSR,HSN,MSR,MSN}\n                        Set\n  -su {B,C,P,M,ES,EN}, --subj {B,C,P,M,ES,EN}\n                        Subject\n```\n\nFor example, to create a table for 120 high school regional Physics questions for author: "Kulkarni, Rishi" the following command would work:\n\n```powershell \nnsb make -n "Kulkarni, Rishi" -st HSR -su P Kulkarni_HS_Physics_Regionals 120\n```\n\n<a name="known-issues"></a>\n## Known Issues\n\n* If ```nsb format``` is used on a document with tracked changes, it will assume the changes were accepted. \n\nPlease report any other issues you find on [Github](https://github.com/rishi-kulkarni/nsb-toolbox).\n',
-    'author': 'Rishi Kulkarni',
-    'author_email': 'rishi@kulkarni.science',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/rishi-kulkarni/nsbtoolbox',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
+Version 0.5.2 - Updated for 2024 NSB
 
+The NSB Toolbox contains a set of tools to make it easier to write and edit Science Bowl questions. It ensures that questions are compliant with the official Science Bowl format, allowing writers to focus on just writing the questions. It also highlights common formatting errors for editors, allowing them to focus on checking content without worrying that they're missing formatting issues here and there.
+
+## Table of Contents
+
+1. [Installation](#installation)
+2. [Documentation](#documentation)
+    1. [nsb format](#nsb-format)
+        1. [Auto-Formatting](#auto-format)
+        2. [Linting](#linting)
+    2. [nsb assign](#nsb-assign)
+        1. [Sample Configuration](#assign-config)
+    3. [nsb make](#nsb-make)
+3. [Known Issues](#known-issues)
+
+<a name="installation"></a>
+## Installation
+Currently, the NSB Toolbox can be installed via pip from this github. To do so, you will need:
+
+* Python 3.8 or greater installed on your computer.
+* Enter and run ```pip install nsb-toolbox``` in your command line.
+* Verify the installation worked by running ```nsb -h``` in your command line. If the help information for the toolbox appears, the installation was successful.
+
+<a name="documentation"></a>
+## Documentation
+You can access the NSB Toolbox via the ```nsb``` commandlet. Running ```nsb -h``` displays the following help menu.
+
+```powershell
+(base) PS C:\Users\rishik> nsb -h
+usage: nsb [-h] {format,make} ...
+
+Utilities for managing Science Bowl .docx files.
+
+optional arguments:
+  -h, --help     show this help message and exit
+
+subcommands:
+  {format,make}
+    format       format a Science Bowl file
+    make         make a Science Bowl table
+```
+<a name="nsb-format"></a>
+## nsb format
+```nsb format``` provides two functions in one - first, it is a formatter than ensures Science Bowl questions are properly spaced (four spaces between question type and start of stem, blank line between stem and answer, etc). Second, it is a linter that highlights questions that it cannot fix. It is important to note that ```nsb format``` cannot catch every problem with the question! For example, ```nsb format``` will never be able to check question content for correctness. All ```nsb format``` can do is eliminate or highlight typical formatting errors.
+
+### Usage
+
+```nsb format``` takes a single mandatory argument, the path to the target .docx file. For example:
+
+```nsb format path/to/nsb/questions.docx```
+
+It also takes a single optional argument, `--capitalize`. If given, `nsb format` will force every answer line to be capitalized. For example:
+
+```nsb format path/to/nsb/questions.docx --capitalize```
+
+<a name="auto-format"></a>
+### Auto-Formatting
+
+```nsb format``` outright fixes a number of formatting errors. It strives to produce questions that have the following characteristics:
+
+* The question class (TOSS-UP, BONUS) is uppercase.
+* Subject (Biology, Chemistry, etc.) are title case.
+* Question type (Multiple Choice, Short Answer) are italicized and title case.
+* There are four spaces between the question type and the start of the stem.
+* For multiple choice questions, the stem and choices are each separated by a single paragraph break.
+* There are two paragraph breaks before the answer line.
+* The answer line is uppercase, assuming the `--capitalize` argument is used.
+
+Notably, `nsb format` operates by moving, copying, and inserting XML elements. This ensures that **user-provided formatting won't be overwritten** (for example, superscripts and subscripts for mathematical formulae). 
+
+For example, all of the following improperly formatted questions:
+
+![Before Formatting](/docs/images/before_format.png) 
+
+```nsb format``` will automatically convert these questions to be compliant with the Science Bowl format:
+
+![After Formatting](/docs/images/after_format.png)
+
+Shorthand notation can also be used to reduce the amount of time writers spend writing boilerplate.
+
+![Before Shorthand](/docs/images/before_shorthand.png)
+
+TU and B will be converted to TOSS-UP and BONUS, respectively. The shorthand for the subject categories is the first letter of the subject, aside for Earth and Space (ES) and Energy (EN). MC and SA will be converted to Multiple Choice and Short Answer, as well.
+
+![After Shorthand](/docs/images/after_shorthand.png)
+
+Finally, ```nsb format``` will automatically correct minor errors in question structure. For example, the following question has multiple X) choices:
+
+![Before Multiple Choice Correction](/docs/images/before_mc_correct.png)
+
+The mislabeled choices will be automatically corrected. Note that an answer line that has been explicitly given will not be auto-capitalized:
+
+![After Multiple Choice Correction](/docs/images/after_mc_correct.png)
+
+<a name="linting"></a>
+### Linting
+
+If ```nsb format``` fails to parse a cell, it will raise linting errors by highlighting the question and printing the error in the command line. There are two levels of errors: parsing errors, which will highlight a cell red, and question structure errors, which will highlight the problematic structure yellow. `nsb format` searches for the following errors:
+
+* The question has a class, subject, type, stem, and answer. Multiple Choice questions should also have four choices.
+* Question type is correctly labeled - Multiple Choice questions should have choices, Short Answer questions should not.
+* For multiple choice questions, the wording of the answer line should match the wording of the choice.
+
+For example:
+
+![Linter Errors](/docs/images/linter_errors.png)
+
+The first question is missing two choices, so it can't be fully parsed, raising a red error. The second question is merely mislabeled - it says it's a Multiple Choice question, but is recognized as a Short Answer question. This raises a yellow error, highlighting the question type. Messages corresponding to these errors are printed in the terminal, as well:
+
+```
+(base) rishi@RISHI-DESKTOP:~$ nsb format after_format.docx
+Question 6: Couldn't parse question, was looking for QuestionFormatterState.CHOICES
+Question 7: Question type is MC, but has no choices.
+```
+
+```nsb format``` is not capable of deleting lines that contain text. This is intentional - while there are errors that ```nsb format```  highlights that it could probably fix automatically, the maintainer believes it is more prudent to leave whitespace formatting to ```nsb format``` and making any other changes by hand.
+
+<a name="nsb-assign"></a>
+## nsb assign
+`nsb assign` uses a set of configuration options to automatically assign a set of edited questions to rounds. 
+
+### Usage
+
+```nsb assign``` takes two mandatory arguments, the path to the edited set of Science Bowl questions and the path to the configuration file. For example:
+
+```nsb assign path/to/nsb/questions.docx -c path/to/config.yaml```
+
+It also takes an optional `--dry-run` argument, which will report statistics on the assignment procedure, but will not write the successful assignment to disk. This is primarily useful for determining what additional questions of a given difficulty or type are required. For example:
+
+```zsh
+❯ nsb assign Kulkarni_HS_Chemistry_Regionals.docx -c assign.yaml --dry-run
+Set      LOD       TUB       Need      Have
+HSR       1       BONUS         8        40
+HSR       1     TOSS-UP         8        46
+HSR       2       BONUS         0        21
+HSR       2     TOSS-UP        10        31
+HSR       3       BONUS         0        22
+HSR       3     TOSS-UP         0        30
+HSR-A     1       BONUS        25        10
+HSR-A     1     TOSS-UP        25         5
+HSR-A     2       BONUS        23         3
+HSR-A     2     TOSS-UP        30         5
+HSR-A     3       BONUS        13        13
+HSR-A     3     TOSS-UP         6         9
+HSR-B     1       BONUS        25         7
+HSR-B     1     TOSS-UP        25         6
+HSR-B     2       BONUS        23         6
+HSR-B     2     TOSS-UP        30         4
+HSR-B     3       BONUS        13        13
+HSR-B     3     TOSS-UP         6         9
+Not writing assignments as this is a dry run.
+```
+
+<a name="assign-config"></a>
+### Sample Configuration File
+
+Below is a sample configuration file for a High School Regional set. The sections are explained in more detail further below.
+
+```yaml
+Configuration:
+  Shuffle Subcategory: True 
+  Shuffle Pairs: False 
+  Shuffle LOD: False
+  Random Seed: ~
+  Subcategory Mismatch Penalty: 1
+  Preferred Writers: []
+
+Round Definitions:
+  Tiebreakers:
+    TU:
+      LOD: [2]
+
+  RoundRobin:
+    TU:
+      LOD: [1, 1, 1, 1]
+      Subcategory: [Organic, ~, ~, ~]
+
+    B:
+      LOD: [1, 1, 1, 1]
+      Subcategory: [Organic, ~, ~, ~]
+
+  DoubleElim1-4:
+    TU:
+      LOD: [2, 2, 2, 2]
+
+    B:
+      LOD: [2, 2, 2, 2]
+
+  DoubleElim5-6:
+    TU:
+      LOD: [2, 2, 2, 2]
+
+    B:
+      LOD: [2, 2, 3, 3]
+
+  DoubleElim7-9:
+    TU:
+      LOD: [2, 2, 3, 3]
+    B:
+      LOD: [2, 3, 3, 3]
+
+Sets:
+  - Set: [HSR]
+    Prefix: RR
+    Rounds: [1, 2]
+    Template: RoundRobin
+
+  - Set: [HSR]
+    Prefix: TB
+    Rounds: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+    Template: Tiebreakers
+
+  - Set: [HSR-A, HSR-B]
+    Prefix: RR
+    Rounds: [3, 4, 6, 7, 8]
+    Template: RoundRobin
+
+  - Set: [HSR-A, HSR-B]
+    Prefix: RR
+    Rounds: [5]
+    Template:
+      from: RoundRobin
+      add:
+        TU:
+          LOD: [1]
+        B:
+          LOD: [1]
+
+  - Set: [HSR-A, HSR-B]
+    Prefix: DE
+    Rounds: [1, 2, 3, 4]
+    Template: DoubleElim1-4
+
+  - Set: [HSR-A, HSR-B]
+    Prefix: DE
+    Rounds: [5, 6]
+    Template: DoubleElim5-6
+
+  - Set: [HSR-A, HSR-B]
+    Prefix: DE
+    Rounds: [7, 8, 9]
+    Template: DoubleElim7-9
+
+```
+
+### Configuration Options
+
+`Shuffle Subcategory`: Setting this option to `True` randomizes the order that any subcategory specification appears in a round. For example, if you have requested `["Organic", ~, ~, ~]`, setting this option to `True` makes the `"Organic"` subcategory uniformly distributed rather than the first question of each round. Note that setting this option to `True` breaks any matching between `TU` and `B` subcategories.
+
+`Shuffle Pairs`: Setting this option to `True` adds a randomization step after each pair of questions has been constructed. This is useful when you have intentionally matched `TU` and `B` subcategories, for example, but want to randomize the order that the subcategories appear in each round. Note that even when this is enabled, the final pair of each round will be `Short Answer` questions.
+
+`Shuffle LOD`: Setting this option to `True` randomizes the order that question difficulties appear in each round, similar to the above options.
+
+`Random Seed`: Setting this option to an integer fixes the generated assignment, all else being equal. If left unspecified or set to None, the assignment will have a slight random element to it.
+
+`Subcategory Mismatch Penalty`: Setting this option to an integer specifies how much cost is incurred by creating a subcategory mismatch. Common options include: 
+
+`1`, which says that matching a question with the right difficulty but wrong subcategory is equally costly as using a question whose difficulty is off by `1`, but the subcategory is correct. 
+
+`2`, which says that matching a question with the right difficulty but wrong subcategory is always less preferable than using a question with the right subcategory but off-by-one difficulty, but also always more preferable than using a question with the right subcategory but off-by-two difficulty.
+
+`Preferred Writers`: If specified, any writers NOT in this list are given a small penalty, encouraging the optimization algorithm to use the preferred writers. This penalty is very small and should never result in a question of the wrong subcategory or difficulty from a preferred writer being used over a question of the right subcategory and difficulty from an unpreferred writer.
+
+### Round Definitions
+
+```yaml
+Round Definitions:
+  Tiebreakers:
+    TU:
+      LOD: [2]
+
+  RoundRobin:
+    TU:
+      LOD: [1, 1, 1, 1]
+      Subcategory: [Organic, ~, ~, ~]
+    B:
+      LOD: [1, 1, 1, 1]
+      Subcategory: [Organic, ~, ~, ~]
+```
+
+`Round Definitions` serve as templates to build round specifications. Each round definition needs to specify the question types it uses (`TU` and/or `B` for TOSS-UP and BONUS) and the Level of Difficulty of each question. Optionally, the subcategories can be specified. Entering a `~` indicates that there is no subcategory preference for that slot.
+
+To explain the above specification in plain English, we want all Tiebreaker rounds to consist of a single
+TOSS-UP question with a difficulty of 2, and all Round Robin rounds to consist of 4 TOSS-UPs and 4 BONUSes that each have a difficulty of 1. Finally, a quarter of TOSS-UPs and BONUSes should use the "Organic" subcategory.
+
+### Sets
+
+```yaml
+Sets:
+  - Set: [HSR-A, HSR-B]
+    Prefix: RR
+    Rounds: [1, 2]
+    Template: RoundRobin
+```
+
+The `Sets` section actually specifies what rounds will be built. A set is defined with the `Set`, `Prefix`, `Rounds`, and `Template` keys. The `Set`, `Prefix`, and `Rounds` keys are round meta-data, while the `Template` key will build the round using the matching entry in the `Round Specifications` section. 
+
+These keys are used combinatorially - the above set will generate 4 rounds: HSR-A RR1, HSR-A RR2, HSR-B RR1, and HSR-B RR2. 
+
+Optionally, `Sets` can use the `from:`, `add:` syntax:
+
+```yaml
+  - Set: [HSR-A, HSR-B]
+    Prefix: RR
+    Rounds: [5]
+    Template:
+      from: RoundRobin
+      add:
+        TU:
+          LOD: [1]
+        B:
+          LOD: [1]
+```
+This syntax specifies that the `RoundRobin` template should be used, but there should be an extra TOSS-UP and BONUS that each have a difficulty of 1.
+
+<a name="nsb-make"></a>
+## nsb make
+```nsb make``` produces a blank Science Bowl question table with a designated number of lines. This is a convenience function for writers. ```nsb make -h``` shows the following help menu:
+
+```powershell
+(base) PS C:\Users\rishik> nsb make -h
+usage: nsb make [-h] [-n NAME] [-st {HSR,HSN,MSR,MSN}] [-su {B,C,P,M,ES,EN}] path rows
+
+positional arguments:
+  path                  path to the Science Bowl docx file
+  rows                  number of rows in output table
+
+options:
+  -h, --help            show this help message and exit
+  -n NAME, --name NAME  Last, First name of author
+  -st {HSR,HSN,MSR,MSN}, --set {HSR,HSN,MSR,MSN}
+                        Set
+  -su {B,C,P,M,ES,EN}, --subj {B,C,P,M,ES,EN}
+                        Subject
+```
+
+For example, to create a table for 120 high school regional Physics questions for author: "Kulkarni, Rishi" the following command would work:
+
+```powershell 
+nsb make -n "Kulkarni, Rishi" -st HSR -su P Kulkarni_HS_Physics_Regionals 120
+```
+
+<a name="known-issues"></a>
+## Known Issues
+
+* If ```nsb format``` is used on a document with tracked changes, it will assume the changes were accepted. 
+
+Please report any other issues you find on [Github](https://github.com/rishi-kulkarni/nsb-toolbox).
 
-setup(**setup_kwargs)
```

