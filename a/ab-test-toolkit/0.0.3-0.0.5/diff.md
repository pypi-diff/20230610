# Comparing `tmp/ab-test-toolkit-0.0.3.tar.gz` & `tmp/ab-test-toolkit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-toolkit-0.0.3.tar", last modified: Mon Jun  5 08:38:57 2023, max compression
+gzip compressed data, was "ab-test-toolkit-0.0.5.tar", last modified: Sat Jun 10 16:04:19 2023, max compression
```

## Comparing `ab-test-toolkit-0.0.3.tar` & `ab-test-toolkit-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-05 08:38:57.054157 ab-test-toolkit-0.0.3/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.3/LICENSE
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.3/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7208 2023-06-05 08:38:57.054066 ab-test-toolkit-0.0.3/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4853 2023-06-05 08:26:06.000000 ab-test-toolkit-0.0.3/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-05 08:38:57.053118 ab-test-toolkit-0.0.3/ab_test_toolkit/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4746 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1136 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/analyze.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4502 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5974 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     8334 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2033 2023-06-05 08:24:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-05 08:38:57.053897 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7208 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-05 08:38:57.000000 ab-test-toolkit-0.0.3/ab_test_toolkit.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-05 08:38:46.000000 ab-test-toolkit-0.0.3/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-05 08:38:57.054189 ab-test-toolkit-0.0.3/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.3/setup.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     1064 2023-06-03 07:13:56.000000 ab-test-toolkit-0.0.5/LICENSE
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      111 2023-04-27 10:12:58.000000 ab-test-toolkit-0.0.5/MANIFEST.in
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)    20044 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)    17217 2023-06-10 15:56:55.000000 ab-test-toolkit-0.0.5/README.md
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/ab_test_toolkit/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       22 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/__init__.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     4245 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/_modidx.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     4453 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/generator.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     7366 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/plotting.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     8370 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/power.py
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2033 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/wrappers.py
+drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)    20044 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      490 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       73 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-03 07:19:15.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       98 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       16 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)      951 2023-06-10 16:04:07.000000 ab-test-toolkit-0.0.5/settings.ini
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)       38 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/setup.cfg
+-rw-rw-r--   0 kolja     (1000) kolja     (1000)     2711 2023-06-03 07:16:06.000000 ab-test-toolkit-0.0.5/setup.py
```

### Comparing `ab-test-toolkit-0.0.3/LICENSE` & `ab-test-toolkit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.3/ab_test_toolkit/_modidx.py` & `ab-test-toolkit-0.0.5/ab_test_toolkit/_modidx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/ab-test-toolkit',
                 'doc_host': 'https://k111git.github.io',
                 'git_url': 'https://github.com/k111git/ab-test-toolkit',
                 'lib_path': 'ab_test_toolkit'},
-  'syms': { 'ab_test_toolkit.analyze': { 'ab_test_toolkit.analyze.p_value_binary': ( 'analyze.html#p_value_binary',
-                                                                                     'ab_test_toolkit/analyze.py'),
-                                         'ab_test_toolkit.analyze.p_value_binary_from_counts': ( 'analyze.html#p_value_binary_from_counts',
-                                                                                                 'ab_test_toolkit/analyze.py')},
-            'ab_test_toolkit.generator': { 'ab_test_toolkit.generator.contingency_from_counts': ( 'data_generation.html#contingency_from_counts',
+  'syms': { 'ab_test_toolkit.generator': { 'ab_test_toolkit.generator.contingency_from_counts': ( 'data_generation.html#contingency_from_counts',
                                                                                                   'ab_test_toolkit/generator.py'),
                                            'ab_test_toolkit.generator.data_to_contingency': ( 'data_generation.html#data_to_contingency',
                                                                                               'ab_test_toolkit/generator.py'),
                                            'ab_test_toolkit.generator.generate_binary_data': ( 'data_generation.html#generate_binary_data',
                                                                                                'ab_test_toolkit/generator.py'),
                                            'ab_test_toolkit.generator.generate_contingency': ( 'data_generation.html#generate_contingency',
                                                                                                'ab_test_toolkit/generator.py'),
```

### Comparing `ab-test-toolkit-0.0.3/ab_test_toolkit/generator.py` & `ab-test-toolkit-0.0.5/ab_test_toolkit/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,48 +61,44 @@
         users=("target", "size"), converted=("target", "sum")
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
     return df_result
 
 # %% ../nbs/00_data_generation.ipynb 11
-def generate_contingency(
-    N=1000, split=0.50, cr0=0.010, cr1=0.011, exact=False
-):
+def generate_contingency(N=1000, split=0.50, cr0=0.010, cr1=0.011,exact=False):
     """
     Generate contingency table using binominal distribution
     For exact=False, we draw the numbers from the binominal distribution.
     For exact=True, we calculate the numbers from multiplying number users * conversion rate
     """
     assert N > 5, "N need to be more than 5"
     assert split >= 0.01, "Split needs to be >= 1%"
     assert split <= 0.99, "Split needs to be <= 99%"
-    if exact == False:
+    if exact==False:
         while True:
             n1 = binom.rvs(N, split, loc=0, size=1)[0]
             if n1 < N and n1 > 0:
                 break
         n0 = N - n1
         c0 = binom.rvs(n0, cr0, loc=0, size=1)[0]
         c1 = binom.rvs(n1, cr1, loc=0, size=1)[0]
-    elif exact == True:
-        n0 = int(np.round(N * split))
-        n1 = N - n1
-        c0 = int(np.round(n0 * cr0))
-        c1 = int(np.round(n1 * cr1))
+    elif exact==True:
+        n0=int(np.round(N*split))
+        n1=N-n1
+        c0=int(np.round(n0*cr0))
+        c1=int(np.round(n1*cr1))
     else:
-        raise Exception(
-            "Invalid input for exact parameter in generate_contingency function."
-        )
+        raise Exception("Invalid input for exact parameter in generate_contingency function.")
     df_result = pd.DataFrame(
         {"group": [0, 1], "users": [n0, n1], "converted": [c0, c1]}
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
-    return df_result.set_index("group")
+    return df_result.set_index('group')
 
 # %% ../nbs/00_data_generation.ipynb 12
 def contingency_from_counts(n0, c0, n1, c1):
     """
     Generate contingency table from following input:
     n0: users in control group
     c0: number of converted users in control group
```

### Comparing `ab-test-toolkit-0.0.3/ab_test_toolkit/plotting.py` & `ab-test-toolkit-0.0.5/ab_test_toolkit/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import plotly.figure_factory as ff
 
 from scipy.stats import beta
 
 from .power import sample_size_binary, sample_size_continuous
 
 # %% ../nbs/03_plotting.ipynb 7
-def plot_distribution(df,show_rug=True):
+def plot_distribution(df, show_rug=True):
     """
     Plots the distribution for both groups of generate_continuous_data
     """
     fig = ff.create_distplot(
         [
             df[df["group"] == 0]["target"].values,
             df[df["group"] == 1]["target"].values,
@@ -36,20 +36,32 @@
         xaxis_title="Target",
         yaxis_title="PDF",
         legend=dict(yanchor="top", y=0.99, xanchor="right", x=0.95),
     )
     return fig
 
 # %% ../nbs/03_plotting.ipynb 8
-def plot_power(simulation, added_lines=[]):
+def plot_power(simulation, added_lines=[], is_effect=True):
     """
     Takes simulation dict and plots the power over sample sizes
     Added lines: plot horizontal lines for additional sample size estimations, takes a list of dicts with sample_size=sample_size,label=label
+    is_effect: True: there is an effect in reality, hence we are interested in power. False: we are interested in false positives.
     """
     approaches = simulation["approaches"]
+    if is_effect == True:
+        ytitle = "Power"
+        yrange=[0,1]
+    elif is_effect == False:
+        ytitle = "False positives"
+        yrange=[0,0.1]
+    else:
+        raise Exception(
+            "Non boolean for is effect encountered in power plot function."
+        )
+        
     fig = go.Figure()
     for approach in approaches:
         fig.add_trace(
             go.Scatter(
                 x=simulation["sizes"] / 2.0,
                 y=simulation[f"power_{approach}"],
                 mode="lines+markers",
@@ -73,22 +85,38 @@
                 x=2 * [added_line["sample_size"]],
                 y=[0, 1],
                 mode="lines",
                 line_dash="dash",
                 name=added_line["label"],
             )
         )
+    if is_effect == False:
+        fig.add_trace(
+            go.Scatter(
+                x=[0, simulation["sizes"].max() / 2.0],
+                y=[0.05, 0.05],
+                mode="lines",
+                line_dash="dash",
+                line_color="gray",
+                line_width=1,
+            )
+        )
+
 
     fig.update_layout(
         template="simple_white",
         xaxis_title="Sample size per variation",
-        yaxis_title="PDF",
-        yaxis_range=[0, 1],
+        yaxis_title=ytitle,
+        yaxis_range=yrange,
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
+    fig.update_xaxes(showspikes=True, spikemode="across", spikethickness=1)
+    fig.update_yaxes(showspikes=True, spikemode="across", spikethickness=1)
+    fig.update_layout(spikedistance=1000, hoverdistance=100)
+
     # fig.update_layout(showlegend=True)
     return fig
 
 # %% ../nbs/03_plotting.ipynb 10
 def plot_betas(df_contingency, xmin=0.0, xmax=0.2, names=["A", "B"]):
     """
     Plots two beta distributions, one for control and for variant.
@@ -162,14 +190,17 @@
         title="Statistical power vs sample size (binary)",
         template="simple_white",
         xaxis_title="Sample size per variant",
         yaxis_title="Power",
         hovermode="y unified",
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
+    fig.update_xaxes(showspikes=True, spikemode="across", spikethickness=1)
+    fig.update_yaxes(showspikes=True, spikemode="across", spikethickness=1)
+    fig.update_layout(spikedistance=1000, hoverdistance=100)
     return fig
 
 # %% ../nbs/03_plotting.ipynb 13
 def plot_continuous_power(
     mu1=5.0, mu2=5.05, sigma=1, alpha=0.05, one_sided=True, vline_power=0.8
 ):
     powers = np.arange(0.1, 0.91, 0.025)
@@ -212,8 +243,11 @@
         title="Statistical power vs sample size (continuous)",
         template="simple_white",
         xaxis_title="Sample size per variant",
         yaxis_title="Power",
         hovermode="y unified",
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
+    fig.update_xaxes(showspikes=True, spikemode="across",spikethickness=1)
+    fig.update_yaxes(showspikes=True, spikemode="across",spikethickness=1)
+    fig.update_layout(spikedistance=1000, hoverdistance=100)
     return fig
```

### Comparing `ab-test-toolkit-0.0.3/ab_test_toolkit/power.py` & `ab-test-toolkit-0.0.5/ab_test_toolkit/power.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     """
     if one_sided == True:
         alternative = "greater"
         alternative_z = "larger"
         print("One sided.")
     else:
         alternative = "two-sided"
+        alternative_z = "two-sided"
         print("Two sided tests, except for bayesian which is one sided.")
     approaches = ["fisher", "z", "bayes"]
     pvs = dict()
     pvs_fisher = dict()
     pvs_z = dict()
     # run simulations for each sample size
     for idx, size in enumerate(sizes):
@@ -85,15 +86,15 @@
             test = BinaryDataTest()
             for group in [0, 1]:
                 nUser = df_contingency.loc[group].users
                 nConverted = df_contingency.loc[group].converted
                 test.add_variant_data_agg(
                     str(group), totals=nUser, positives=nConverted
                 )
-            results = test.evaluate(sim_count=5000)
+            results = test.evaluate(sim_count=2000)
             pvs[idx].append(results[1]["prob_being_best"])
             _, p_fischer = fisher_exact(
                 np.array(df_contingency[["not_converted", "converted"]]),
                 alternative=alternative,
             )
             pvs_fisher[idx].append(p_fischer)
             _, p_z = proportions_ztest(
```

### Comparing `ab-test-toolkit-0.0.3/ab_test_toolkit/wrappers.py` & `ab-test-toolkit-0.0.5/ab_test_toolkit/wrappers.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.3/settings.ini` & `ab-test-toolkit-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-toolkit
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_toolkit
```

### Comparing `ab-test-toolkit-0.0.3/setup.py` & `ab-test-toolkit-0.0.5/setup.py`

 * *Files identical despite different names*

