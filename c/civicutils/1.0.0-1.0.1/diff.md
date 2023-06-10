# Comparing `tmp/civicutils-1.0.0.tar.gz` & `tmp/civicutils-1.0.1.tar.gz`

## Comparing `civicutils-1.0.0.tar` & `civicutils-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.0/info_on_matching_framework.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/__init__.py
--rw-r--r--   0        0        0    40428 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/filtering.py
--rw-r--r--   0        0        0   111690 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/match.py
--rw-r--r--   0        0        0    16920 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/query.py
--rw-r--r--   0        0        0    33551 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/read_and_write.py
--rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/utils.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/data/data.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/data/example_cnv.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/data/example_expr.txt
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 civicutils-1.0.0/civicutils/data/example_snv.txt
--rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.0/images/civicutils-workflow.png
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.0/tcga_analysis/data/civic_available_diseases_31052023.txt
--rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.0/tcga_analysis/scripts/Query_CIViCutils.py
--rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.0/tcga_analysis/scripts/civicutils_manuscript_figures.R
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.0/tcga_analysis/scripts/get_available_diseases_in_civic.py
--rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.0/tcga_analysis/scripts/process_civic_predictions.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    45370 2020-02-02 00:00:00.000000 civicutils-1.0.0/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 civicutils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    86899 2020-02-02 00:00:00.000000 civicutils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 civicutils-1.0.1/info_on_matching_framework.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/__init__.py
+-rw-r--r--   0        0        0    40439 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/filtering.py
+-rw-r--r--   0        0        0   111701 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/match.py
+-rw-r--r--   0        0        0    16931 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/query.py
+-rw-r--r--   0        0        0    33562 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/read_and_write.py
+-rw-r--r--   0        0        0    20645 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/utils.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/data.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_cnv.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_expr.txt
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 civicutils-1.0.1/civicutils/data/example_snv.txt
+-rw-r--r--   0        0        0    82463 2020-02-02 00:00:00.000000 civicutils-1.0.1/dist_backup/civicutils-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   439302 2020-02-02 00:00:00.000000 civicutils-1.0.1/dist_backup/civicutils-1.0.0.tar.gz
+-rw-r--r--   0        0        0   396868 2020-02-02 00:00:00.000000 civicutils-1.0.1/images/civicutils-workflow.png
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/.DS_Store
+-rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/data/civic_available_diseases_31052023.txt
+-rw-r--r--   0        0        0    36985 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/Query_CIViCutils.py
+-rw-r--r--   0        0        0    78674 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/civicutils_manuscript_figures.R
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/get_available_diseases_in_civic.py
+-rw-r--r--   0        0        0   128034 2020-02-02 00:00:00.000000 civicutils-1.0.1/tcga_analysis/scripts/process_civic_predictions.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 civicutils-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0    45370 2020-02-02 00:00:00.000000 civicutils-1.0.1/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 civicutils-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    86899 2020-02-02 00:00:00.000000 civicutils-1.0.1/PKG-INFO
```

### Comparing `civicutils-1.0.0/info_on_matching_framework.md` & `civicutils-1.0.1/info_on_matching_framework.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/civicutils/filtering.py` & `civicutils-1.0.1/civicutils/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 import re
 
-from utils import check_string_filter_arguments, check_cutoff_filter_arguments, check_is_bool, check_keys, check_keys_not, check_is_none
+from civicutils.utils import check_string_filter_arguments, check_cutoff_filter_arguments, check_is_bool, check_keys, check_keys_not, check_is_none
 
 
 def filter_in(field, field_name, in_list, list_name, match_type="exact"):
     """
     Check if a given field is contained in a list of strings to be selected for during filtering.
     :param field:       String to check in the provided list. If 'NULL', then match will not be attempted (i.e. if list is non-empty, then 'match=False' will be returned by the function).
     :param field_name:  Name of the field being checked (for error handling).
```

### Comparing `civicutils-1.0.0/civicutils/match.py` & `civicutils-1.0.1/civicutils/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 import re
 
-from utils import check_arguments, check_argument, translate_aa, check_is_dict, check_is_list, check_is_str, check_keys, check_keys_not, check_tier_selection, parse_input, check_empty_input, check_dict_entry, check_is_chgvs, check_is_phgvs, check_identifier_type, check_data_type, check_is_bool, uppercase_list, check_is_none, check_logfc
+from civicutils.utils import check_arguments, check_argument, translate_aa, check_is_dict, check_is_list, check_is_str, check_keys, check_keys_not, check_tier_selection, parse_input, check_empty_input, check_dict_entry, check_is_chgvs, check_is_phgvs, check_identifier_type, check_data_type, check_is_bool, uppercase_list, check_is_none, check_logfc
 
 
 def civic_name_to_hgvs(var_name):
     """
     Given a single CIViC variant name, extract potential HGVS annotations by parsing and modifying the name while using prior knowledge about CIViC naming conventions.
     Function only applicable to SNV data.
     :param var_name:	Name of CIViC variant record.
```

### Comparing `civicutils-1.0.0/civicutils/query.py` & `civicutils-1.0.1/civicutils/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 import re
 
-from utils import check_identifier_type, check_empty_field, check_argument, check_is_list
+from civicutils.utils import check_identifier_type, check_empty_field, check_argument, check_is_list
 
 
 def query_civic(genes, identifier_type="entrez_symbol"):
     """
     Given a list of gene identifiers, query CIViC using 'civic.get_all_genes()' (from Python package CIViCpy) and return a nested dictionary summarizing the evidences from the database. Only a selection of the complete record is processed and returned.
     :param genes:    		List containing gene identifiers to query.
     :param identifier_type:     ['entrez_symbol', 'entrez_id', 'civic_id']
@@ -231,15 +231,15 @@
                             # Only non-Predictive evidences and Predictive ones without drugs will have this dummy level
                             # Introduced for consistency purposes within the varMap structure
                             drugs = ["NULL"]
 
                         # Sanity checks that only "PREDICTIVE" evidences have drugs associated
                         # Submitted evidence items can fulfill having "PREDICTIVE" evidence type and no drugs ("NULL")
                         if (evidence_type != "PREDICTIVE") and (drugs != ["NULL"]):
-                            raise ValueError("Only evidences of type "PREDICTIVE" can have drugs associated!")
+                            raise ValueError("Only evidences of type 'PREDICTIVE' can have drugs associated!")
                             
                 # Iterate through drugs to add evidences associated to them
                 #   For non-Predictive evidences or Predictive with empty drugs, drugs=["NULL"]
                 #   For Predictive and interaction=None, len(drugs) = 1
                 #   For Predictive and interaction="Substitutes", len(drugs)>1
                 #   For Predictive and interaction!="Substitutes", len(drugs)=1 (combiantion of several using "+")
                 for drug in drugs:
```

### Comparing `civicutils-1.0.0/civicutils/read_and_write.py` & `civicutils-1.0.1/civicutils/read_and_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,15 +480,15 @@
     # NOTE: uppercase is critical for matching!
     sorted_evidence_types = ["PREDICTIVE", "DIAGNOSTIC", "PROGNOSTIC", "PREDISPOSING"]
     evidence_type = "PREDICTIVE"
     special_cases = ["NON_SNV_MATCH_ONLY", "NON_CNV_MATCH_ONLY", "NON_EXPR_MATCH_ONLY"]
     sorted_cts = ["ct", "gt", "nct"]
     varmap_entries_variant = ["name", "hgvs", "types"]
     
-    from utils import check_match_before_writing, check_keys, check_keys_not, check_data_type, check_dict_entry
+    from civicutils.utils import check_match_before_writing, check_keys, check_keys_not, check_data_type, check_dict_entry
     check_match_before_writing(match_map, var_map, raw_map, has_support, has_ct, write_ct, write_support, write_complete)
     check_data_type(data_type)
     outfile = open(outfile, "w")
     
     # Retrieve the output header given the argument selection
     (out_header, clean_header, write_impact, write_exon) = write_header_line(data_type, header, write_support)
     outfile.write(out_header + "\n")
```

### Comparing `civicutils-1.0.0/civicutils/utils.py` & `civicutils-1.0.1/civicutils/utils.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/civicutils/data/data.yml` & `civicutils-1.0.1/civicutils/data/data.yml`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/images/civicutils-workflow.png` & `civicutils-1.0.1/images/civicutils-workflow.png`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/tcga_analysis/data/civic_available_diseases_31052023.txt` & `civicutils-1.0.1/tcga_analysis/data/civic_available_diseases_31052023.txt`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/tcga_analysis/scripts/Query_CIViCutils.py` & `civicutils-1.0.1/tcga_analysis/scripts/Query_CIViCutils.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/tcga_analysis/scripts/civicutils_manuscript_figures.R` & `civicutils-1.0.1/tcga_analysis/scripts/civicutils_manuscript_figures.R`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/tcga_analysis/scripts/get_available_diseases_in_civic.py` & `civicutils-1.0.1/tcga_analysis/scripts/get_available_diseases_in_civic.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/tcga_analysis/scripts/process_civic_predictions.py` & `civicutils-1.0.1/tcga_analysis/scripts/process_civic_predictions.py`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/LICENSE.md` & `civicutils-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/README.md` & `civicutils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `civicutils-1.0.0/pyproject.toml` & `civicutils-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "civicutils"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python package for querying, matching and downstream processing of CIViC information."
 requires-python = ">=3.7"
 dependencies = ["civicpy>=3.0.0"]
 readme = "README.md"
 license = {file = "LICENSE.md"}
 authors = [
   { name="María Lourdes Rosano-Gonzalez", email="lourdes.rosanogonzalez@gmail.com" },
```

### Comparing `civicutils-1.0.0/PKG-INFO` & `civicutils-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civicutils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for querying, matching and downstream processing of CIViC information.
 Project-URL: Homepage, https://github.com/ETH-NEXUS/civicutils
 Project-URL: Bug Tracker, https://github.com/ETH-NEXUS/civicutils/issues
 Author-email: María Lourdes Rosano-Gonzalez <lourdes.rosanogonzalez@gmail.com>, "Vipin T. Sreedharan" <vipin.sreedharan@nexus.ethz.ch>, Antoine Hanns <hanns@nexus.ethz.ch>, "Daniel J. Stekhoven" <stekhoven@nexus.ethz.ch>, Franziska Singer <singer@nexus.ethz.ch>
 Maintainer-email: Antoine Hanns <hanns@nexus.ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

