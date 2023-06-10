# Comparing `tmp/proofs-0.0.2.tar.gz` & `tmp/proofs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proofs-0.0.2.tar", last modified: Wed Jun  7 01:30:27 2023, max compression
+gzip compressed data, was "proofs-0.0.3.tar", last modified: Sat Jun 10 19:57:18 2023, max compression
```

## Comparing `proofs-0.0.2.tar` & `proofs-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.976536 proofs-0.0.2/
--rw-r--r--   0 max        (501) staff       (20)    11337 2023-06-01 10:05:52.000000 proofs-0.0.2/LICENSE
--rw-r--r--   0 max        (501) staff       (20)      111 2023-06-01 10:05:52.000000 proofs-0.0.2/MANIFEST.in
--rw-r--r--   0 max        (501) staff       (20)     7552 2023-06-07 01:30:27.976380 proofs-0.0.2/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     5269 2023-06-07 01:25:51.000000 proofs-0.0.2/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.974910 proofs-0.0.2/proofs/
--rw-r--r--   0 max        (501) staff       (20)       22 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     1336 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/_modidx.py
--rw-r--r--   0 max        (501) staff       (20)      146 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/assistant.py
--rw-r--r--   0 max        (501) staff       (20)     7706 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/core.py
--rw-r--r--   0 max        (501) staff       (20)      155 2023-06-07 01:30:25.000000 proofs-0.0.2/proofs/polynomials.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-07 01:30:27.976112 proofs-0.0.2/proofs.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     7552 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      356 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       55 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/entry_points.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-06-06 03:31:59.000000 proofs-0.0.2/proofs.egg-info/not-zip-safe
--rw-r--r--   0 max        (501) staff       (20)     1863 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        7 2023-06-07 01:30:27.000000 proofs-0.0.2/proofs.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)     2768 2023-06-07 01:30:25.000000 proofs-0.0.2/settings.ini
--rw-r--r--   0 max        (501) staff       (20)       38 2023-06-07 01:30:27.976591 proofs-0.0.2/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)     2596 2023-06-01 10:05:52.000000 proofs-0.0.2/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-10 19:57:18.693976 proofs-0.0.3/
+-rw-r--r--   0 max        (501) staff       (20)    11337 2023-06-01 10:05:52.000000 proofs-0.0.3/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)      111 2023-06-01 10:05:52.000000 proofs-0.0.3/MANIFEST.in
+-rw-r--r--   0 max        (501) staff       (20)     7650 2023-06-10 19:57:18.693794 proofs-0.0.3/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     5359 2023-06-09 17:37:53.000000 proofs-0.0.3/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-10 19:57:18.691835 proofs-0.0.3/proofs/
+-rw-r--r--   0 max        (501) staff       (20)       22 2023-06-09 17:38:23.000000 proofs-0.0.3/proofs/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)     3192 2023-06-09 17:38:23.000000 proofs-0.0.3/proofs/_modidx.py
+-rw-r--r--   0 max        (501) staff       (20)      146 2023-06-09 17:38:23.000000 proofs-0.0.3/proofs/assistant.py
+-rw-r--r--   0 max        (501) staff       (20)     8318 2023-06-09 17:38:23.000000 proofs-0.0.3/proofs/core.py
+-rw-r--r--   0 max        (501) staff       (20)     3376 2023-06-09 17:38:23.000000 proofs-0.0.3/proofs/polynomials.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-06-10 19:57:18.693476 proofs-0.0.3/proofs.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     7650 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      356 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       55 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/entry_points.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-06-06 03:31:59.000000 proofs-0.0.3/proofs.egg-info/not-zip-safe
+-rw-r--r--   0 max        (501) staff       (20)     1863 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        7 2023-06-10 19:57:18.000000 proofs-0.0.3/proofs.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)     2768 2023-06-09 17:38:23.000000 proofs-0.0.3/settings.ini
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-06-10 19:57:18.694042 proofs-0.0.3/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)     2596 2023-06-01 10:05:52.000000 proofs-0.0.3/setup.py
```

### Comparing `proofs-0.0.2/LICENSE` & `proofs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proofs-0.0.2/PKG-INFO` & `proofs-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mathematical proof assistant for students and amateurs.
 Home-page: https://github.com/maxtheman/proofs
 Author: maxtheman
 Author-email: proofs@growth.wtf
 License: Apache Software License 2.0
 Description: # proofs
         
@@ -62,67 +62,68 @@
         2.  Look at examples
         3.  Decide on a proof strategy
         4.  Write the proof
         
         ``` python
         # Start by defining your domain
         arbitrary_x = variable("x")
-        expression = arbitrary_x + 1
+        expression = arbitrary_x + 2
         ```
         
         ``` python
         print(expression)
         ```
         
-            x + 1
+            x + 2
         
         ``` python
         # select a few examples from the reals
         make_examples('real', 3, expression)
         ```
         
-            [(-57, -56), (-100, -99), (-31, -30)]
+            [(-39, -37), (-13, -11), (7, 9)]
         
         Hopefully these examples convice us that the statement is false. This
         suggests that we can prove it by contradiction.
         
         ``` python
         # Then define your goal
         contradiction_goal = not_equals(expression, arbitrary_x)
         ```
         
         ``` python
         @contradiction_proof
         def proof_of_x_plus_one(x):
-            # Given x, Assume x + 1 = x is true for arbitrary_x
+            # Given x, Assume x + 1 = x is true for arbitrary x
             assumed_eq = equals(x + 1, x)
         
             # Calculate x + 1
             next = x + 1
         
             # Observing x + 1 != x, we have reached a contradiction
             return not_equals(next, assumed_eq.rhs)
         
         #Select an arbitrary x from the domain
         prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
         ```
         
-        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
+        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary x}}$$
         
         $$x + 1 = x$$
         
         $$\mathtt{\text{Calculate x + 1}}$$
         
         $$x + 1$$
         
         $$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
         
-        $$\text \quad x + 1 \neq x \quad Q.E.D.$$
+            Proof failed: Derived result Ne(x + 1, x) does not match goal Ne(x + 2, x)
+            Check your assumptions and proof function for errors.
         
-            True
+            False
         
         With this, we get:
         
         1.  Complete latex rendering of the math we are doing in python and our
             logic
         2.  validation that what we are returning from the proof matches the
             expected goal
```

### Comparing `proofs-0.0.2/README.md` & `proofs-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,67 +54,68 @@
 2.  Look at examples
 3.  Decide on a proof strategy
 4.  Write the proof
 
 ``` python
 # Start by defining your domain
 arbitrary_x = variable("x")
-expression = arbitrary_x + 1
+expression = arbitrary_x + 2
 ```
 
 ``` python
 print(expression)
 ```
 
-    x + 1
+    x + 2
 
 ``` python
 # select a few examples from the reals
 make_examples('real', 3, expression)
 ```
 
-    [(-57, -56), (-100, -99), (-31, -30)]
+    [(-39, -37), (-13, -11), (7, 9)]
 
 Hopefully these examples convice us that the statement is false. This
 suggests that we can prove it by contradiction.
 
 ``` python
 # Then define your goal
 contradiction_goal = not_equals(expression, arbitrary_x)
 ```
 
 ``` python
 @contradiction_proof
 def proof_of_x_plus_one(x):
-    # Given x, Assume x + 1 = x is true for arbitrary_x
+    # Given x, Assume x + 1 = x is true for arbitrary x
     assumed_eq = equals(x + 1, x)
 
     # Calculate x + 1
     next = x + 1
 
     # Observing x + 1 != x, we have reached a contradiction
     return not_equals(next, assumed_eq.rhs)
 
 #Select an arbitrary x from the domain
 prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
 ```
 
-$$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
+$$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary x}}$$
 
 $$x + 1 = x$$
 
 $$\mathtt{\text{Calculate x + 1}}$$
 
 $$x + 1$$
 
 $$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
 
-$$\text \quad x + 1 \neq x \quad Q.E.D.$$
+    Proof failed: Derived result Ne(x + 1, x) does not match goal Ne(x + 2, x)
+    Check your assumptions and proof function for errors.
 
-    True
+    False
 
 With this, we get:
 
 1.  Complete latex rendering of the math we are doing in python and our
     logic
 2.  validation that what we are returning from the proof matches the
     expected goal
```

### Comparing `proofs-0.0.2/proofs/core.py` & `proofs-0.0.3/proofs/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['Var', 'Const', 'Func', 'Goal', 'Expression', 'variable', 'constant', 'equation', 'equals', 'not_equals',
+__all__ = ['Var', 'Const', 'Func', 'Goal', 'Expression', 'variable', 'constant', 'equals', 'not_equals', 'equation',
            'make_examples', 'prove', 'print_proof', 'contradiction_proof', 'direct_proof']
 
 # %% ../nbs/00_core.ipynb 3
 from typing import Callable, List, Tuple, Union
 from sympy import Equality, Unequality
 from sympy.core.relational import Relational
 from sympy.core.basic import Basic
@@ -30,50 +30,60 @@
 # Helper functions to create a more user-friendly interface
 def variable(name: str) -> Var:
     return sp.Symbol(name)
 
 def constant(value: Union[int, float]) -> Const:
     return sp.Number(value)
 
-def equation(expr: str) -> sp.Expr:
-    return sp.sympify(expr, evaluate=False)
+# old - deprecated
+# def equation(expr: str) -> sp.Expr:
+#     return sp.sympify(expr, evaluate=False)
 
 def equals(lhs: sp.Expr, rhs: sp.Expr) -> Equality:
     return sp.Eq(lhs, rhs, evaluate=False)
 
 def not_equals(lhs: Expression, rhs: Expression) -> Unequality:
     return sp.Ne(lhs, rhs, evaluate=False)
 
-# %% ../nbs/00_core.ipynb 7
+def equation(name, variables, expression):
+    '''Creates a function with the given name, variables, and expression.'''
+    if not isinstance(variables, list):
+        variables = [variables]
+    return sp.Eq(sp.Function(name)(*variables), expression)
+
+# %% ../nbs/00_core.ipynb 8
 def make_examples(domain: str, #Domain of the example equation
                   N: int, #Number of examples
-                  equation: str #Equation to generate examples for
+                  equation: str, #Equation to generate examples for
+                  positive_only: bool = False, #Whether to only generate positive inputs
+                  increasing_only: bool = False #Whether the domain should be increasing
                   ) -> List[Tuple[sp.Expr, sp.Expr]]: #List of input-output pairs
     """For a given domain and equation, select N examples and generate a list of N input-output pairs.
-    Currently, the domain can be either 'real' or 'integer', and one variable is assumed."""
+    Currently, the domain can only be 'real', and one variable is assumed."""
     examples = []
     if domain == 'real':
         # select N random real numbers
         for _ in range(N):
             x = sp.Symbol('x')
             x_val = randint(-100, 100)
-            y_val = sp.sympify(equation).subs(x, x_val)
-            examples.append((x_val, y_val))
-    elif domain == 'integer':
-        # select N random integers
-        for _ in range(N):
-            x = sp.Symbol('x', integer=True)
-            x_val = randint(-100, 100)
+            if positive_only:
+                x_val = abs(x_val)
+            if increasing_only:
+                previous_example = examples[-1] if len(examples) > 0 else None
+                if previous_example is not None:
+                    while x_val <= previous_example[0]:
+                        # adding to ensure it's increasing. probably a better way to do this.
+                        x_val = randint(-100, 100) + previous_example[0]
             y_val = sp.sympify(equation).subs(x, x_val)
             examples.append((x_val, y_val))
     else:
         raise ValueError(f"Domain {domain} not supported.")
     return examples
 
-# %% ../nbs/00_core.ipynb 12
+# %% ../nbs/00_core.ipynb 16
 def prove(goal: Goal, #Goal to prove
           proof_func: Callable[..., Goal], #Proof function
           *args #Arguments to proof function
           ) -> bool: #True if proof succeeds, False otherwise
     """Prove a goal using a proof function and arguments.
     The proof function should take the goal as the last argument and return the derived result.
     The goal is proved if the derived result matches the goal."""
@@ -85,15 +95,15 @@
         else:
             raise Exception(f"Derived result {derived_result} does not match goal {goal}")
     except Exception as e:
         print(f"Proof failed: {str(e)}")
         print("Check your assumptions and proof function for errors.")
         return False
 
-# %% ../nbs/00_core.ipynb 16
+# %% ../nbs/00_core.ipynb 20
 def print_proof(proof: Callable[..., Goal], # the proof function
                  *args # the arguments to the proof function
                  ) -> None: # no return value
     """Print a proof step by step. Mostly used when defining a proof evaluation function.
     The proof function should take the goal as the last argument and return the derived result.
     The goal is proved if the derived result matches the goal.
     Comments do not support latex formatting, but the rest of the proof does."""
@@ -125,15 +135,15 @@
             if var_name in _printed:
                 continue
             else:
                 _printed.append(var_name)
             # if isinstance(var_value, (Var, Const, Func)):
             display(Latex(f"$${sp.latex(var_value)}$$"))
 
-# %% ../nbs/00_core.ipynb 19
+# %% ../nbs/00_core.ipynb 23
 def contradiction_proof(proof: Callable[..., Goal] # the proof function
                         ) -> Callable[..., Unequality]: # the wrapped contradiction proof function to evaluate
     """Wrap a proof function to prove a contradiction.
     The proof function should take the goal as the last argument and return the derived result.
     The goal is proved if the derived result matches the goal."""
     def wrapper(*args, **kwargs):
         hints = typing.get_type_hints(proof)
@@ -150,15 +160,15 @@
             # there might be something weird around result that would prevent it from being printed if it's in the proof. check that later
             result = proof(*args, **kwargs)
             if not isinstance(result, Unequality):
                 raise TypeError("Proof function must return Unequality")
             return result
     return wrapper
 
-# %% ../nbs/00_core.ipynb 21
+# %% ../nbs/00_core.ipynb 25
 def direct_proof(proof: Callable[..., Goal] # the proof function
                         ) -> Callable[..., Equality]: # the wrapped proof function to evaluate
     """Wrap a proof function to prove a direct proof.
     The proof function should take the goal as the last argument and return the derived result.
     The goal is proved if the derived result matches the goal."""
     def wrapper(*args, **kwargs):
         hints = typing.get_type_hints(proof)
```

### Comparing `proofs-0.0.2/proofs.egg-info/PKG-INFO` & `proofs-0.0.3/proofs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proofs
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mathematical proof assistant for students and amateurs.
 Home-page: https://github.com/maxtheman/proofs
 Author: maxtheman
 Author-email: proofs@growth.wtf
 License: Apache Software License 2.0
 Description: # proofs
         
@@ -62,67 +62,68 @@
         2.  Look at examples
         3.  Decide on a proof strategy
         4.  Write the proof
         
         ``` python
         # Start by defining your domain
         arbitrary_x = variable("x")
-        expression = arbitrary_x + 1
+        expression = arbitrary_x + 2
         ```
         
         ``` python
         print(expression)
         ```
         
-            x + 1
+            x + 2
         
         ``` python
         # select a few examples from the reals
         make_examples('real', 3, expression)
         ```
         
-            [(-57, -56), (-100, -99), (-31, -30)]
+            [(-39, -37), (-13, -11), (7, 9)]
         
         Hopefully these examples convice us that the statement is false. This
         suggests that we can prove it by contradiction.
         
         ``` python
         # Then define your goal
         contradiction_goal = not_equals(expression, arbitrary_x)
         ```
         
         ``` python
         @contradiction_proof
         def proof_of_x_plus_one(x):
-            # Given x, Assume x + 1 = x is true for arbitrary_x
+            # Given x, Assume x + 1 = x is true for arbitrary x
             assumed_eq = equals(x + 1, x)
         
             # Calculate x + 1
             next = x + 1
         
             # Observing x + 1 != x, we have reached a contradiction
             return not_equals(next, assumed_eq.rhs)
         
         #Select an arbitrary x from the domain
         prove(contradiction_goal, proof_of_x_plus_one, arbitrary_x)
         ```
         
-        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary\_x}}$$
+        $$\mathtt{\text{Given x, Assume x + 1 = x is true for arbitrary x}}$$
         
         $$x + 1 = x$$
         
         $$\mathtt{\text{Calculate x + 1}}$$
         
         $$x + 1$$
         
         $$\mathtt{\text{Observing x + 1 != x, we have reached a contradiction}}$$
         
-        $$\text \quad x + 1 \neq x \quad Q.E.D.$$
+            Proof failed: Derived result Ne(x + 1, x) does not match goal Ne(x + 2, x)
+            Check your assumptions and proof function for errors.
         
-            True
+            False
         
         With this, we get:
         
         1.  Complete latex rendering of the math we are doing in python and our
             logic
         2.  validation that what we are returning from the proof matches the
             expected goal
```

### Comparing `proofs-0.0.2/proofs.egg-info/requires.txt` & `proofs-0.0.3/proofs.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `proofs-0.0.2/settings.ini` & `proofs-0.0.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = proofs
 lib_name = proofs
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = proofs
 nbs_path = nbs
 recursive = True
```

### Comparing `proofs-0.0.2/setup.py` & `proofs-0.0.3/setup.py`

 * *Files identical despite different names*

