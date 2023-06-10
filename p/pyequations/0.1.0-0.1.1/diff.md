# Comparing `tmp/pyequations-0.1.0.tar.gz` & `tmp/pyequations-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyequations-0.1.0.tar", max compression
+gzip compressed data, was "pyequations-0.1.1.tar", max compression
```

## Comparing `pyequations-0.1.0.tar` & `pyequations-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1092 2023-05-29 01:59:52.040409 pyequations-0.1.0/LICENSE
--rwxr-xr-x   0        0        0      426 2023-06-07 23:17:21.370640 pyequations-0.1.0/pyequations/__init__.py
--rwxr-xr-x   0        0        0     6498 2023-06-10 17:55:56.942066 pyequations-0.1.0/pyequations/context_stack.py
--rwxr-xr-x   0        0        0      494 2023-05-30 23:47:56.863751 pyequations-0.1.0/pyequations/decorators.py
--rwxr-xr-x   0        0        0     9584 2023-06-10 18:00:05.797632 pyequations-0.1.0/pyequations/generate_units_subs.py
--rwxr-xr-x   0        0        0    24694 2023-06-10 20:00:33.856906 pyequations-0.1.0/pyequations/inheritables.py
--rwxr-xr-x   0        0        0     9585 2023-06-10 17:53:55.847770 pyequations-0.1.0/pyequations/utils.py
--rwxr-xr-x   0        0        0      456 2023-05-29 01:59:52.045941 pyequations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 pyequations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 01:58:26.642083 pyequations-0.1.1/LICENSE
+-rw-r--r--   0        0        0      426 2023-06-10 20:52:03.052114 pyequations-0.1.1/pyequations/__init__.py
+-rw-r--r--   0        0        0     6303 2023-06-10 18:08:24.869111 pyequations-0.1.1/pyequations/context_stack.py
+-rw-r--r--   0        0        0      471 2023-05-31 00:06:36.282730 pyequations-0.1.1/pyequations/decorators.py
+-rw-r--r--   0        0        0     9349 2023-06-10 18:08:24.869275 pyequations-0.1.1/pyequations/generate_units_subs.py
+-rw-r--r--   0        0        0    24128 2023-06-10 20:37:48.132386 pyequations-0.1.1/pyequations/inheritables.py
+-rw-r--r--   0        0        0     9294 2023-06-10 18:08:24.869792 pyequations-0.1.1/pyequations/utils.py
+-rw-r--r--   0        0        0      439 2023-06-10 20:51:37.449609 pyequations-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 pyequations-0.1.1/PKG-INFO
```

### Comparing `pyequations-0.1.0/pyequations/context_stack.py` & `pyequations-0.1.1/pyequations/context_stack.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from sympy import Symbol
-
-
-def verify_names(var_names: list[str]) -> None:
-    """
-    Checks that the variable names are valid
-    :param var_names: The variable names
-    :return: None. Throws an error if the variable names are invalid
-    """
-
-    # Check that the variable names are unique
-    if len(var_names) != len(set(var_names)):
-        raise ValueError("var_names must be unique")
-
-    for name in var_names:
-        # Check that the variable names are strings
-        if not isinstance(name, str):
-            raise TypeError("var_names must be a list of strings")
-
-        # Check that the variables names can all be identified as attributes
-        if not name.isidentifier():
-            raise ValueError("var_names must be valid identifiers")
-
-
-class ContextStack:
-    """
-    A class to manage the context stack for branching systems
-    Must be initialized with a list of variables to track
-    """
-
-    def __init__(self, var_names: list[str] = None):
-
-        # Validate the variable names
-        if var_names is not None:
-            verify_names(var_names)
-
-        self._contexts = [{name: Symbol(name) for name in var_names} if var_names else {}]
-        """
-        A list of dictionaries containing the variables in each context
-        """
-        self._context_idx: int = 0
-        """
-        The index of the current context
-        """
-        self._locked: bool = False
-        """
-        A flag to indicate if the context stack is locked
-        """
-
-    def add_variables(self, var_names: list[str]) -> None:
-        """
-        Adds variables to the current context
-        Can only be done before the context stack is locked
-        Locking happens when any operation is done on the stack to compute or branch
-        :param var_names: the names of the variables to add
-        :return: None
-        """
-
-        # Check that the context stack is not locked
-        if self._locked:
-            raise RuntimeError("Context stack is locked. Variables can only be added before the system branches.")
-
-        verify_names(var_names)
-
-        # Add the variables to the current context
-        self._contexts[self._context_idx].update({name: Symbol(name) for name in var_names})
-
-    @property
-    def context_idx(self):
-        return self._context_idx
-
-    @property
-    def contexts(self):
-        return self._contexts
-
-    @property
-    def locked(self):
-        return self._locked
-
-    @context_idx.setter
-    def context_idx(self, value):
-        if 0 <= value < len(self._contexts):
-            self._context_idx = value
-        else:
-            raise IndexError("Invalid context_idx")
-
-    def __getattr__(self, key):
-        if 0 <= self._context_idx < len(self._contexts):
-            return self._contexts[self._context_idx].get(key)
-        else:
-            raise IndexError("Invalid context_idx")
-
-    def set_value(self, name: str, value, context: int = None) -> None:
-        """
-        Sets the value of a variable in the given context
-        :param name: the name of the variable
-        :param value: the value to set the variable to
-        :param context: the index of the context to set the value in. If None, the current context is used
-        :return: None
-        """
-
-        # If name is not a string, raise an error
-        if not isinstance(name, str):
-            raise TypeError('Name must be a string')
-
-        if context is not None:
-            self._context_idx = context
-
-        if 0 <= self._context_idx < len(self._contexts):
-            self._contexts[self._context_idx][name] = value
-        else:
-            raise IndexError('Invalid context_idx')
-
-    def get_value(self, name, context: int = None):
-        """
-        Gets the value of a variable in the current context
-        :param context: the index of the context to get the value from
-        :param name: the name of the variable
-        :return: the value of the variable
-        """
-
-        if context is None:
-            context = self._context_idx
-
-        if 0 <= context < len(self._contexts):
-            return self._contexts[context].get(name)
-        else:
-            raise IndexError("Invalid context_idx")
-
-    def set_value_all_contexts(self, name: str, value) -> None:
-        """
-        Sets the value of a variable in all contexts
-        :param name:
-        :param value:
-        :return:
-        """
-
-        # If name is not a string, raise an error
-        if not isinstance(name, str):
-            raise TypeError('Name must be a string')
-
-        for context in self._contexts:
-            context[name] = value
-
-    def add_context(self, reference: int = None) -> None:
-        """
-        Adds a new context to the stack, copying all values from the current context
-        If no reference is given, the new context is a copy of the current context
-        """
-
-        # Lock the context stack to prevent adding variables
-        self._locked = True
-
-        if reference is None:
-            reference = self._context_idx
-
-        if 0 <= reference < len(self._contexts):
-            self._contexts.append(self._contexts[reference].copy())
-        else:
-            raise IndexError("Invalid context_idx")
-
-    def remove_context(self, index: int) -> None:
-        """
-        Removes a context from the stack
-        """
-
-        # Lock the context stack to prevent adding variables
-        self._locked = True
-
-        if 0 <= index < len(self._contexts):
-            self._contexts.pop(index)
-            # Need to ensure that the current context index is not greater than the index of the context to remove
-            self._context_idx = min(self._context_idx, len(self._contexts) - 1)
-        else:
-            raise IndexError("Invalid context_idx")
-
-    @property
-    def num_contexts(self) -> int:
-        return len(self._contexts)
-
-    @property
-    def variables(self) -> list[str]:
-        return list(self._contexts[self._context_idx].keys())
-
-    def rotate_context(self) -> None:
-        """
-        Rotates the context stack by one
-        """
-        self._context_idx = (self._context_idx + 1) % len(self._contexts)
-
-    def has_variable(self, variable) -> bool:
-        """
-        Returns True if the current context has a variable
-        """
-        return variable in self._contexts[self._context_idx]
+from sympy import Symbol
+
+
+def verify_names(var_names: list[str]) -> None:
+    """
+    Checks that the variable names are valid
+    :param var_names: The variable names
+    :return: None. Throws an error if the variable names are invalid
+    """
+
+    # Check that the variable names are unique
+    if len(var_names) != len(set(var_names)):
+        raise ValueError("var_names must be unique")
+
+    for name in var_names:
+        # Check that the variable names are strings
+        if not isinstance(name, str):
+            raise TypeError("var_names must be a list of strings")
+
+        # Check that the variables names can all be identified as attributes
+        if not name.isidentifier():
+            raise ValueError("var_names must be valid identifiers")
+
+
+class ContextStack:
+    """
+    A class to manage the context stack for branching systems
+    Must be initialized with a list of variables to track
+    """
+
+    def __init__(self, var_names: list[str] = None):
+
+        # Validate the variable names
+        if var_names is not None:
+            verify_names(var_names)
+
+        self._contexts = [{name: Symbol(name) for name in var_names} if var_names else {}]
+        """
+        A list of dictionaries containing the variables in each context
+        """
+        self._context_idx: int = 0
+        """
+        The index of the current context
+        """
+        self._locked: bool = False
+        """
+        A flag to indicate if the context stack is locked
+        """
+
+    def add_variables(self, var_names: list[str]) -> None:
+        """
+        Adds variables to the current context
+        Can only be done before the context stack is locked
+        Locking happens when any operation is done on the stack to compute or branch
+        :param var_names: the names of the variables to add
+        :return: None
+        """
+
+        # Check that the context stack is not locked
+        if self._locked:
+            raise RuntimeError("Context stack is locked. Variables can only be added before the system branches.")
+
+        verify_names(var_names)
+
+        # Add the variables to the current context
+        self._contexts[self._context_idx].update({name: Symbol(name) for name in var_names})
+
+    @property
+    def context_idx(self):
+        return self._context_idx
+
+    @property
+    def contexts(self):
+        return self._contexts
+
+    @property
+    def locked(self):
+        return self._locked
+
+    @context_idx.setter
+    def context_idx(self, value):
+        if 0 <= value < len(self._contexts):
+            self._context_idx = value
+        else:
+            raise IndexError("Invalid context_idx")
+
+    def __getattr__(self, key):
+        if 0 <= self._context_idx < len(self._contexts):
+            return self._contexts[self._context_idx].get(key)
+        else:
+            raise IndexError("Invalid context_idx")
+
+    def set_value(self, name: str, value, context: int = None) -> None:
+        """
+        Sets the value of a variable in the given context
+        :param name: the name of the variable
+        :param value: the value to set the variable to
+        :param context: the index of the context to set the value in. If None, the current context is used
+        :return: None
+        """
+
+        # If name is not a string, raise an error
+        if not isinstance(name, str):
+            raise TypeError('Name must be a string')
+
+        if context is not None:
+            self._context_idx = context
+
+        if 0 <= self._context_idx < len(self._contexts):
+            self._contexts[self._context_idx][name] = value
+        else:
+            raise IndexError('Invalid context_idx')
+
+    def get_value(self, name, context: int = None):
+        """
+        Gets the value of a variable in the current context
+        :param context: the index of the context to get the value from
+        :param name: the name of the variable
+        :return: the value of the variable
+        """
+
+        if context is None:
+            context = self._context_idx
+
+        if 0 <= context < len(self._contexts):
+            return self._contexts[context].get(name)
+        else:
+            raise IndexError("Invalid context_idx")
+
+    def set_value_all_contexts(self, name: str, value) -> None:
+        """
+        Sets the value of a variable in all contexts
+        :param name:
+        :param value:
+        :return:
+        """
+
+        # If name is not a string, raise an error
+        if not isinstance(name, str):
+            raise TypeError('Name must be a string')
+
+        for context in self._contexts:
+            context[name] = value
+
+    def add_context(self, reference: int = None) -> None:
+        """
+        Adds a new context to the stack, copying all values from the current context
+        If no reference is given, the new context is a copy of the current context
+        """
+
+        # Lock the context stack to prevent adding variables
+        self._locked = True
+
+        if reference is None:
+            reference = self._context_idx
+
+        if 0 <= reference < len(self._contexts):
+            self._contexts.append(self._contexts[reference].copy())
+        else:
+            raise IndexError("Invalid context_idx")
+
+    def remove_context(self, index: int) -> None:
+        """
+        Removes a context from the stack
+        """
+
+        # Lock the context stack to prevent adding variables
+        self._locked = True
+
+        if 0 <= index < len(self._contexts):
+            self._contexts.pop(index)
+            # Need to ensure that the current context index is not greater than the index of the context to remove
+            self._context_idx = min(self._context_idx, len(self._contexts) - 1)
+        else:
+            raise IndexError("Invalid context_idx")
+
+    @property
+    def num_contexts(self) -> int:
+        return len(self._contexts)
+
+    @property
+    def variables(self) -> list[str]:
+        return list(self._contexts[self._context_idx].keys())
+
+    def rotate_context(self) -> None:
+        """
+        Rotates the context stack by one
+        """
+        self._context_idx = (self._context_idx + 1) % len(self._contexts)
+
+    def has_variable(self, variable) -> bool:
+        """
+        Returns True if the current context has a variable
+        """
+        return variable in self._contexts[self._context_idx]
```

### Comparing `pyequations-0.1.0/pyequations/inheritables.py` & `pyequations-0.1.1/pyequations/inheritables.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,566 +1,566 @@
-from itertools import combinations
-from sympy import solve, Eq, simplify, Mul, Add, Pow, Symbol, Number, N, Expr
-from warnings import warn
-from pyequations.context_stack import ContextStack
-from pyequations.utils import get_symbols, composes_equation, BoolWrapper, IntWrapper, MinFloatTracker
-from copy import deepcopy
-
-
-class PyEquations:
-
-    def _super_setattr(self, name, value):
-        """
-        Set the attribute for the class using the default __setattr__ method
-        :param name: the attribute name
-        :param value: the attribute value
-        :return: None
-        """
-        super(PyEquations, self).__setattr__(name, value)
-
-    def __init__(self, var_descriptions: dict[str, str] | list[str]):
-
-        # Set attributes using super to avoid recursion
-        #  would spawn from the overriden __getattr__ method
-
-        # Sympy expressions to solve for
-        self._super_setattr('eqs', [])
-        # User defined functions
-        self._super_setattr('funcs', [])
-
-        # Branches marked for pruning
-        self._super_setattr('contexts_to_prune', {})
-        # Advance branch flag -- used when a branch is pruned, and we need to advance to the next branch
-        self._super_setattr('advance_branch', BoolWrapper(False))
-        # Number of deletions for a current solve
-        # Important for determining if there are any valid solutions
-        self._super_setattr('deletions', IntWrapper(0))
-
-        # If the object has been solved
-        self._super_setattr('solved', BoolWrapper(False))
-
-        # If a bad solution was found
-        self._super_setattr('bad_solution', BoolWrapper(False))
-
-        # The minimum numerical quantity handled in the system
-        # Used to use as a reference if a value is compared to zero
-        # Ex. if the minimum number dealt ith is 5e-20, then technically 5e-15 is within the margin of error
-        self._super_setattr('min_float', MinFloatTracker())
-
-        if var_descriptions:
-            if isinstance(var_descriptions, dict):
-                self._super_setattr('context_stack', ContextStack(list(var_descriptions.keys())))
-                self._super_setattr('var_descriptions', var_descriptions)
-            elif isinstance(var_descriptions, list):
-                self._super_setattr('context_stack', ContextStack(var_descriptions))
-                self._super_setattr('var_descriptions', {name: '' for name in var_descriptions})
-        else:
-            raise ValueError('Must have at least one variable description')
-
-        # Get all methods defined in the class
-        methods = [getattr(self, name) for name in dir(self) if callable(getattr(self, name))]
-
-        # Add all methods that are decorated with @calc to the calculation_functions list
-        for method in methods:
-            if hasattr(method, '__equation__'):
-                self.eqs.append(method)
-            elif hasattr(method, '__user_func__'):
-                self.funcs.append(method)
-
-    @property
-    def num_branches(self) -> int:
-        """
-        Get the number of branches
-        :return: The number of branches
-        """
-
-        return self.context_stack.num_contexts
-
-    @property
-    def vars(self) -> list[dict[str, Symbol | Number]]:
-        """
-        Get the variables for all branches
-        :return: A list of dictionaries containing the variables for each branch
-        """
-
-        return self.context_stack.contexts
-
-    @property
-    def vars_decimal(self) -> list[dict[str, float]]:
-        """
-        Get the variables for all branches
-        Understandably could have this and the above be a function, but since these are used so often, it is
-        better to have them as a property
-        :return: A list of dictionaries containing the variables for each branch
-        """
-
-        non_decimal = self.vars
-        return [{key: N(value) for key, value in branch.items()} for branch in non_decimal]
-
-    @property
-    def locked(self) -> bool:
-        """
-        Get if the object is locked
-        :return: True if the object is locked, False otherwise
-        """
-
-        return self.context_stack.locked
-
-    def __getattr__(self, name):
-        """
-        Get the attribute for the current branch
-        This function is called when the attribute is not found, and therefore we should check the context stack
-        :param name: the attribute name
-        :return: the attribute value
-        """
-
-        # If the attribute is not in the context stack, raise an error
-        if name not in self.context_stack.variables:
-            raise AttributeError(f'Variable {name} does not exist')
-        else:
-            # Return the value of the attribute
-            return self.context_stack.get_value(name)
-
-    def __setattr__(self, name, value):
-        """
-        Set the attribute for all branches, if the attribute does not exist and the value is an int, float, or complex
-        :param name: the attribute name
-        :param value: the attribute value
-        :return: None
-        """
-
-        # If we have already solved the equations, raise a warning and do not set the attribute
-        if self.solved:
-            warn('Equations have already been solved. Cannot add new variables')
-            return
-
-        # If the value is an int, float, or complex, set the value for all branches
-        # (Also include the sympy types)
-        if isinstance(value, int | float | complex | Mul | Add | Pow | Symbol | Number):
-            # Check if the variables is in the context stack
-            if name in self.context_stack.variables:
-                # If it is, set the value for all branches
-                self.context_stack.set_value_all_contexts(name, value)
-            # Otherwise, raise an exception as the variable cannot be added
-            else:
-                raise AttributeError(f'Variable {name} cannot be added after initialization')
-
-        # Otherwise, use the default __setattr__ method for this branch
-        else:
-            self._super_setattr(name, value)
-
-    def add_variables(self, var_descriptions: dict[str, str] | list[str]) -> None:
-        """
-        Add variables to the context stack
-        Cannot be done after the context stack has branched
-        In this case, an exception will be raised
-        :param var_descriptions: The variable descriptions to add
-        :return: None
-        """
-
-        # If the variable descriptions are a dictionary, add them to the context stack
-        if isinstance(var_descriptions, dict):
-            self.context_stack.add_variables(list(var_descriptions.keys()))
-            self.var_descriptions.update(var_descriptions)
-        # Otherwise, if the variable descriptions are a list, add them to the context stack
-        elif isinstance(var_descriptions, list):
-            self.context_stack.add_variables(var_descriptions)
-            self.var_descriptions.update({name: '' for name in var_descriptions})
-
-    def _eval_funcs(self) -> None:
-        """
-        Evaluate all the user defined functions for the current branch
-        :return: None
-        """
-
-        # Loop through all the user-defined functions and evaluate them
-        for f in self.funcs:
-            try:
-                f()
-            except TypeError:
-                continue
-
-    def context_switch(self, target_branch: int) -> None:
-        """
-        Switch the current branch to the specified branch
-        :param target_branch: The branch number to switch to
-        :return: None
-        """
-
-        # If the branch number is out of range, throw an exception
-        if target_branch >= self.context_stack.num_contexts:
-            raise IndexError(f'Branch {target_branch} does not exist')
-
-        # Otherwise, set the current branch to the specified branch by moving it to the front of the list
-        self.context_stack.context_idx = target_branch
-
-    def rotate_context(self) -> None:
-        """
-        Rotate the current branch to the next branch
-        :return: None
-        """
-
-        self.context_stack.rotate_context()
-
-    def _verify_and_extract_solution(self, solution, target_variables) -> dict | None:
-        """
-        Check if the solution is a numeric solution
-        If multiple solutions, branch the solution set by adding contexts
-        :param solution: The solution to check
-        :param target_variables: The corresponding variables to check, match the order of the solution
-        :return: A dict containing the solution for the branch or None if the solution is not valid
-        """
-
-        if not bool(solution):
-            return None
-
-        # If solution is a list, it is not an individual solution
-        if isinstance(solution, list):
-            # If the solution has multiple elements, there are multiple solutions
-            # and a new solution branch should be created
-            if len(solution) > 1:
-                # [(solution 1), (solution 2), ...]
-                valid_sols = []
-
-                for sol in solution:
-                    add_flag = True
-                    # If the sol itself is composed of multiple variables, loop through them
-                    if isinstance(sol, tuple):
-                        # [(x, y, z), (x, y, z), ...]
-                        for variable in sol:
-                            # If the variable contains free symbols, it is not a numeric solution
-                            if bool(variable.free_symbols):
-                                add_flag = False
-                                break
-
-                    # Otherwise, for one variable, if the variable contains free symbols, it is not a numeric solution
-                    elif bool(sol.free_symbols):
-                        # [x, x, ...]
-                        add_flag = False
-                        break
-
-                    if add_flag:
-                        valid_sols.append(sol)
-
-                if len(valid_sols) == 0:
-                    return None
-
-                # With the valid solutions, create a new solution branch for each solution after the first
-                for sol in valid_sols[1:]:
-
-                    old_context_idx = self.context_stack.context_idx
-
-                    # Create a new branch (context)
-                    self.context_stack.add_context()
-
-                    # Switch to the new branch
-                    self.context_switch(self.context_stack.num_contexts - 1)
-
-                    # Set the values for the new branch
-                    for var, val in zip(target_variables, sol):
-                        self.context_stack.set_value(str(var), val)
-
-                    # Switch back to the old branch
-                    self.context_switch(old_context_idx)
-
-                # Return the first solution
-                # Create a dictionary to map the target variables to the solution
-                return dict(zip(target_variables, valid_sols[0]))
-
-            # If it is a list with one element, it is not a complete solution
-            else:
-                return None
-
-        elif isinstance(solution, dict):
-            # Trivial case, single solution for all variables
-            # Loop through the variables in the solution
-            for value in solution.values():
-                # If the value contains free symbols, it is not a numeric solution
-                if bool(value.free_symbols):
-                    return None
-
-            # In this case, we will already have a dictionary
-            return solution
-
-        else:
-            # Unknown type, not a valid solution. Throw an exception
-            raise RuntimeError(f'Unknown solution type {solution}')
-
-    def _mark_for_pruning(self, equations: list) -> None:
-        """
-        Mark the current context for pruning by adding a hash to the list of hashes to prune
-        Also carry the offending equation with the hash, so it can be printed if an exception is thrown
-        :return: None
-        """
-
-        # Generate a hash for the current context
-        current_context = self.context_stack.contexts[self.context_stack.context_idx]
-        # Specifically, we want to hash the values of the context, not the keys
-        context_hash = hash(tuple(sorted(current_context.items())))
-        # Add the context hash to the list of contexts to prune
-        # Also have the value be the equation that caused the contradiction, so it can be printed
-        # if an exception is thrown
-        self.contexts_to_prune[context_hash] = equations
-        # Mark that we can now advance to the next context
-        self.advance_branch.set(True)
-
-    def _observe_floats(self, equations: list) -> None:
-        """
-        Observe the specified floats and add them to the list of floats to observe
-        :param equations: The equations to observe
-        :return: None
-        """
-
-        for equation in equations:
-            # Extract the floats from the equation and add observe them
-            for num in Expr(equation).atoms(Number):
-                self.min_float.add(abs(num))
-
-    def _retrieve_equations(self) -> set:
-        """
-        Retrieve all the equations from the calculation functions
-        :return: A set of equations
-        """
-
-        equations = set()
-
-        for function in self.eqs:
-
-            # Call the function from the context of the branch
-            result = function()
-            if len(result) == 2:
-                # Simplify the results here to make all other operations faster
-                result = [simplify(e) for e in result]
-                # Check if the result is an equation that could produce a valid solution
-                # Also, handle the case where there is a contradiction (return -1)
-                can_compose = composes_equation(*result, self.min_float.value)
-                match can_compose:
-                    # Valid equation
-                    case 1:
-                        # Can only observe once we have samples of the magnitude of numbers that compose the solution
-                        self._observe_floats(result)
-                        resulting_eq = Eq(*result)
-                        equations.add(resulting_eq)
-                    # Invalid equation
-                    case 0:
-                        continue
-                    # Contradiction
-                    case -1:
-                        # Mark the current context for pruning
-                        # Note how a list type is passed, this is because this same function can be called elsewhere
-                        # with a list of equations that are all contradictory (but not necessarily on their own)
-                        self._mark_for_pruning([result])
-            else:
-                raise ValueError(f'Function does not return two elements {function}')
-
-        return equations
-
-    def _run_solver_this_branch(self) -> None:
-        """
-        Solve the equations by substituting solutions in place of unknown variables
-        Recursively attempts all combinations of equations
-        :return: None
-        """
-
-        # Evaluate all the user defined functions
-        self._eval_funcs()
-
-        # Gather all the equations from the calculation functions that have an unknown variable
-        # Remove any equations that are True as they are redundant
-        equations = self._retrieve_equations()
-
-        # If the advance_branch flag is set, return
-        # This means that a contradiction was found and the branch should be pruned
-        if self.advance_branch:
-            return
-
-        # Attempt to solve every subgroup of the equations
-        for r in range(1, len(equations) + 1):
-            for subgroup in combinations(equations, r):
-
-                target_variables = get_symbols(subgroup)
-
-                # Attempt to solve the subgroup of equations
-                solution = solve(subgroup, *target_variables)
-
-                # If solution == [], there is no solution for this subgroup
-                if not solution:
-                    # This branch shouldn't necessarily be pruned, but we need to throw special flag
-                    # Specifically, if the vars before solving and the vars after solving are the same, then
-                    # we should throw the flag. This is because some solutions may have branches that lead to this point
-                    # and we don't want to prune those branches because that set of equations could spawn a valid
-                    # solution. So, we need to check if the variables are the same before and after solving.
-                    # This would indicate that the equations are not solvable, and we should throw an exception.
-                    self.bad_solution.set(True)
-
-                # Verify the solution is valid; handle solution branching
-                sol = self._verify_and_extract_solution(solution, target_variables)
-
-                # If a solution was found, set the variables to the solution in this branch
-                if sol is not None:
-                    for key, value in sol.items():
-                        # Found a solution, set the variable to the solution
-                        self.context_stack.set_value(str(key), value)
-
-                    # If there are still unknown variables, attempt to solve again with the new information
-                    self._run_solver_this_branch()
-
-                    # Return to prevent further solving (want to utilize the most information possible)
-                    return
-
-        # Re-evaluate all the user defined functions in case of new information
-        self._eval_funcs()
-
-    def _prune_branches(self) -> None:
-        """
-        Prune the branches that are marked for pruning
-        :return: None
-        """
-
-        # If there are as many branches as there are contexts, raise an exception because there are no solutions
-        # Also need to offset the number of branches by the number of deletions
-        if self.num_branches - self.deletions.value == len(self.contexts_to_prune):
-
-            # Make quick-and-dirty pretty_equation function for use in just this exception throwing
-            # (Cannot have the second string be an f-string because that would mean nested f-strings)
-            def pretty_equation(equations):
-                s = ''
-                for eqn in equations:
-                    s += f'{eqn[0]} = {eqn[1]}, '
-                return s[:-2]
-
-            raise RuntimeError('Given equations have no consistent solutions. '
-                               'Please check your equations and try again. '
-                               'Contradiction(s) found: '
-                               f'{[pretty_equation(equations) for equations in self.contexts_to_prune.values()]}')
-
-        # Otherwise, prune the branches by finding the branches that match the hash
-        # Also, ensure that the context idx is not greater than the number of contexts
-        for context_hash, equation in self.contexts_to_prune.items():
-            for branch_idx, branch in enumerate(self.context_stack.contexts):
-                # If the branch matches the hash, prune it
-                if hash(tuple(sorted(branch.items()))) == context_hash:
-                    # Remove the context
-                    self.context_stack.remove_context(branch_idx)
-                    # Break out of the inner loop as we have found the branch to prune
-                    break
-
-        # Ensure that the actual idx pointer is not greater than the number of contexts
-        self.context_stack.context_idx = min(self.context_stack.context_idx, self.context_stack.num_contexts - 1)
-
-        # Reset the prune branches dictionary
-        self.contexts_to_prune.clear()
-
-    def solve(self) -> None:
-        """
-        Trigger the solver on all existing branches
-        Solver could branch into additional branches, of which the solver will also be triggered on
-        :return: None
-        """
-
-        # If the object has been solved before, throw a warning
-        if self.solved:
-            warn('This object has already been solved. '
-                 'Please create a new object to solve again.'
-                 'Solving multiple times could cause undetermined behavior in the branching behavior'
-                 'if variables are changed after the first solve.')
-
-        # Clear contexts_to_prune dictionary
-        self.contexts_to_prune.clear()
-
-        # Reset the bad_solution flag
-        self.bad_solution.set(False)
-
-        # Store the current context idx
-        old_context_idx = self.context_stack.context_idx
-
-        # Store the current solution as a copy of self.vars
-        old_solution = deepcopy(self.vars)
-
-        # Iterate through all the branches and solve them
-        # Iterate by rotating the context stack until we are back at where we started
-        # This accounts for new branches being added during the solving process
-
-        # Local function to run the solver on the current branch
-        def run_single():
-            # Run the solver on the current branch
-            self._run_solver_this_branch()
-            # Rotate off the first context
-            self.context_stack.rotate_context()
-            # Reset the advance_branch flag
-            self.advance_branch.set(False)
-            # Reset the number of deleted branches
-            self.deletions.set(0)
-
-        run_single()
-
-        # Wishing do-while loops were a thing in python...
-
-        # Continue rotating until we are back at the first context
-        while self.context_stack.context_idx != old_context_idx:
-            run_single()
-
-        # After solving, prune any branches that are marked for pruning
-        # Also check if there are no solutions and throw an exception accordingly
-        self._prune_branches()
-
-        # If the solution is bad and the branches did not change, throw an exception
-        if self.bad_solution and old_solution == self.vars:
-            raise RuntimeError('Given equations have no consistent solutions. '
-                               'Please check your equations and try again.')
-
-        # Mark the object as solved
-        self.solved.set(True)
-
-    def var_description(self, name: str) -> str:
-        """
-        Get the description of a variable
-        :param name: The name of the variable
-        :return: The description of the variable
-        """
-
-        # Raise an exception if the variable does not exist
-        if name not in self.var_descriptions:
-            raise KeyError(f'Variable {name} does not exist')
-
-        # Return the description of the variable
-        return self.var_descriptions[name]
-
-    def get_var_vals(self, name: str) -> list:
-        """
-        Get the value of a variable for each branch
-        :param name: The name of the variable
-        :return: A list of the values of the variable for each branch
-        """
-
-        # Raise an exception if the variable does not exist
-        if name not in self.context_stack.variables:
-            raise KeyError(f'Variable {name} does not exist')
-
-        # Return a list of the value of the variable for each branch
-        return list({self.context_stack.get_value(name, idx) for idx in range(self.context_stack.num_contexts)})
-
-    def get_var_vals_decimal(self, name: str) -> list:
-        """
-        Get the decimal value of a variable for each branch
-        :param name: The name of the variable
-        :return: A list of the values of the variable for each branch
-        """
-
-        # Raise an exception if the variable does not exist
-        if name not in self.context_stack.variables:
-            raise KeyError(f'Variable {name} does not exist')
-
-        # Return a list of the value of the variable for each branch
-        return list({N(self.context_stack.get_value(name, idx)) for idx in range(self.context_stack.num_contexts)})
-
-    def del_branch(self) -> None:
-        """
-        Delete the current branch of the current context
-        :return: None
-        """
-
-        # Delete the old context
-        # This handles updating the context idx
-        self.context_stack.remove_context(self.context_stack.context_idx)
-        # Note that we have deleted a branch
-        self.deletions.increment()
+from itertools import combinations
+from sympy import solve, Eq, simplify, Mul, Add, Pow, Symbol, Number, N, Expr
+from warnings import warn
+from pyequations.context_stack import ContextStack
+from pyequations.utils import get_symbols, composes_equation, BoolWrapper, IntWrapper, MinFloatTracker
+from copy import deepcopy
+
+
+class PyEquations:
+
+    def _super_setattr(self, name, value):
+        """
+        Set the attribute for the class using the default __setattr__ method
+        :param name: the attribute name
+        :param value: the attribute value
+        :return: None
+        """
+        super(PyEquations, self).__setattr__(name, value)
+
+    def __init__(self, var_descriptions: dict[str, str] | list[str]):
+
+        # Set attributes using super to avoid recursion
+        #  would spawn from the overriden __getattr__ method
+
+        # Sympy expressions to solve for
+        self._super_setattr('eqs', [])
+        # User defined functions
+        self._super_setattr('funcs', [])
+
+        # Branches marked for pruning
+        self._super_setattr('contexts_to_prune', {})
+        # Advance branch flag -- used when a branch is pruned, and we need to advance to the next branch
+        self._super_setattr('advance_branch', BoolWrapper(False))
+        # Number of deletions for a current solve
+        # Important for determining if there are any valid solutions
+        self._super_setattr('deletions', IntWrapper(0))
+
+        # If the object has been solved
+        self._super_setattr('solved', BoolWrapper(False))
+
+        # If a bad solution was found
+        self._super_setattr('bad_solution', BoolWrapper(False))
+
+        # The minimum numerical quantity handled in the system
+        # Used to use as a reference if a value is compared to zero
+        # Ex. if the minimum number dealt ith is 5e-20, then technically 5e-15 is within the margin of error
+        self._super_setattr('min_float', MinFloatTracker())
+
+        if var_descriptions:
+            if isinstance(var_descriptions, dict):
+                self._super_setattr('context_stack', ContextStack(list(var_descriptions.keys())))
+                self._super_setattr('var_descriptions', var_descriptions)
+            elif isinstance(var_descriptions, list):
+                self._super_setattr('context_stack', ContextStack(var_descriptions))
+                self._super_setattr('var_descriptions', {name: '' for name in var_descriptions})
+        else:
+            raise ValueError('Must have at least one variable description')
+
+        # Get all methods defined in the class
+        methods = [getattr(self, name) for name in dir(self) if callable(getattr(self, name))]
+
+        # Add all methods that are decorated with @calc to the calculation_functions list
+        for method in methods:
+            if hasattr(method, '__equation__'):
+                self.eqs.append(method)
+            elif hasattr(method, '__user_func__'):
+                self.funcs.append(method)
+
+    @property
+    def num_branches(self) -> int:
+        """
+        Get the number of branches
+        :return: The number of branches
+        """
+
+        return self.context_stack.num_contexts
+
+    @property
+    def vars(self) -> list[dict[str, Symbol | Number]]:
+        """
+        Get the variables for all branches
+        :return: A list of dictionaries containing the variables for each branch
+        """
+
+        return self.context_stack.contexts
+
+    @property
+    def vars_decimal(self) -> list[dict[str, float]]:
+        """
+        Get the variables for all branches
+        Understandably could have this and the above be a function, but since these are used so often, it is
+        better to have them as a property
+        :return: A list of dictionaries containing the variables for each branch
+        """
+
+        non_decimal = self.vars
+        return [{key: N(value) for key, value in branch.items()} for branch in non_decimal]
+
+    @property
+    def locked(self) -> bool:
+        """
+        Get if the object is locked
+        :return: True if the object is locked, False otherwise
+        """
+
+        return self.context_stack.locked
+
+    def __getattr__(self, name):
+        """
+        Get the attribute for the current branch
+        This function is called when the attribute is not found, and therefore we should check the context stack
+        :param name: the attribute name
+        :return: the attribute value
+        """
+
+        # If the attribute is not in the context stack, raise an error
+        if name not in self.context_stack.variables:
+            raise AttributeError(f'Variable {name} does not exist')
+        else:
+            # Return the value of the attribute
+            return self.context_stack.get_value(name)
+
+    def __setattr__(self, name, value):
+        """
+        Set the attribute for all branches, if the attribute does not exist and the value is an int, float, or complex
+        :param name: the attribute name
+        :param value: the attribute value
+        :return: None
+        """
+
+        # If we have already solved the equations, raise a warning and do not set the attribute
+        if self.solved:
+            warn('Equations have already been solved. Cannot add new variables')
+            return
+
+        # If the value is an int, float, or complex, set the value for all branches
+        # (Also include the sympy types)
+        if isinstance(value, int | float | complex | Mul | Add | Pow | Symbol | Number):
+            # Check if the variables is in the context stack
+            if name in self.context_stack.variables:
+                # If it is, set the value for all branches
+                self.context_stack.set_value_all_contexts(name, value)
+            # Otherwise, raise an exception as the variable cannot be added
+            else:
+                raise AttributeError(f'Variable {name} cannot be added after initialization')
+
+        # Otherwise, use the default __setattr__ method for this branch
+        else:
+            self._super_setattr(name, value)
+
+    def add_variables(self, var_descriptions: dict[str, str] | list[str]) -> None:
+        """
+        Add variables to the context stack
+        Cannot be done after the context stack has branched
+        In this case, an exception will be raised
+        :param var_descriptions: The variable descriptions to add
+        :return: None
+        """
+
+        # If the variable descriptions are a dictionary, add them to the context stack
+        if isinstance(var_descriptions, dict):
+            self.context_stack.add_variables(list(var_descriptions.keys()))
+            self.var_descriptions.update(var_descriptions)
+        # Otherwise, if the variable descriptions are a list, add them to the context stack
+        elif isinstance(var_descriptions, list):
+            self.context_stack.add_variables(var_descriptions)
+            self.var_descriptions.update({name: '' for name in var_descriptions})
+
+    def _eval_funcs(self) -> None:
+        """
+        Evaluate all the user defined functions for the current branch
+        :return: None
+        """
+
+        # Loop through all the user-defined functions and evaluate them
+        for f in self.funcs:
+            try:
+                f()
+            except TypeError:
+                continue
+
+    def context_switch(self, target_branch: int) -> None:
+        """
+        Switch the current branch to the specified branch
+        :param target_branch: The branch number to switch to
+        :return: None
+        """
+
+        # If the branch number is out of range, throw an exception
+        if target_branch >= self.context_stack.num_contexts:
+            raise IndexError(f'Branch {target_branch} does not exist')
+
+        # Otherwise, set the current branch to the specified branch by moving it to the front of the list
+        self.context_stack.context_idx = target_branch
+
+    def rotate_context(self) -> None:
+        """
+        Rotate the current branch to the next branch
+        :return: None
+        """
+
+        self.context_stack.rotate_context()
+
+    def _verify_and_extract_solution(self, solution, target_variables) -> dict | None:
+        """
+        Check if the solution is a numeric solution
+        If multiple solutions, branch the solution set by adding contexts
+        :param solution: The solution to check
+        :param target_variables: The corresponding variables to check, match the order of the solution
+        :return: A dict containing the solution for the branch or None if the solution is not valid
+        """
+
+        if not bool(solution):
+            return None
+
+        # If solution is a list, it is not an individual solution
+        if isinstance(solution, list):
+            # If the solution has multiple elements, there are multiple solutions
+            # and a new solution branch should be created
+            if len(solution) > 1:
+                # [(solution 1), (solution 2), ...]
+                valid_sols = []
+
+                for sol in solution:
+                    add_flag = True
+                    # If the sol itself is composed of multiple variables, loop through them
+                    if isinstance(sol, tuple):
+                        # [(x, y, z), (x, y, z), ...]
+                        for variable in sol:
+                            # If the variable contains free symbols, it is not a numeric solution
+                            if bool(variable.free_symbols):
+                                add_flag = False
+                                break
+
+                    # Otherwise, for one variable, if the variable contains free symbols, it is not a numeric solution
+                    elif bool(sol.free_symbols):
+                        # [x, x, ...]
+                        add_flag = False
+                        break
+
+                    if add_flag:
+                        valid_sols.append(sol)
+
+                if len(valid_sols) == 0:
+                    return None
+
+                # With the valid solutions, create a new solution branch for each solution after the first
+                for sol in valid_sols[1:]:
+
+                    old_context_idx = self.context_stack.context_idx
+
+                    # Create a new branch (context)
+                    self.context_stack.add_context()
+
+                    # Switch to the new branch
+                    self.context_switch(self.context_stack.num_contexts - 1)
+
+                    # Set the values for the new branch
+                    for var, val in zip(target_variables, sol):
+                        self.context_stack.set_value(str(var), val)
+
+                    # Switch back to the old branch
+                    self.context_switch(old_context_idx)
+
+                # Return the first solution
+                # Create a dictionary to map the target variables to the solution
+                return dict(zip(target_variables, valid_sols[0]))
+
+            # If it is a list with one element, it is not a complete solution
+            else:
+                return None
+
+        elif isinstance(solution, dict):
+            # Trivial case, single solution for all variables
+            # Loop through the variables in the solution
+            for value in solution.values():
+                # If the value contains free symbols, it is not a numeric solution
+                if bool(value.free_symbols):
+                    return None
+
+            # In this case, we will already have a dictionary
+            return solution
+
+        else:
+            # Unknown type, not a valid solution. Throw an exception
+            raise RuntimeError(f'Unknown solution type {solution}')
+
+    def _mark_for_pruning(self, equations: list) -> None:
+        """
+        Mark the current context for pruning by adding a hash to the list of hashes to prune
+        Also carry the offending equation with the hash, so it can be printed if an exception is thrown
+        :return: None
+        """
+
+        # Generate a hash for the current context
+        current_context = self.context_stack.contexts[self.context_stack.context_idx]
+        # Specifically, we want to hash the values of the context, not the keys
+        context_hash = hash(tuple(sorted(current_context.items())))
+        # Add the context hash to the list of contexts to prune
+        # Also have the value be the equation that caused the contradiction, so it can be printed
+        # if an exception is thrown
+        self.contexts_to_prune[context_hash] = equations
+        # Mark that we can now advance to the next context
+        self.advance_branch.set(True)
+
+    def _observe_floats(self, equations: list) -> None:
+        """
+        Observe the specified floats and add them to the list of floats to observe
+        :param equations: The equations to observe
+        :return: None
+        """
+
+        for equation in equations:
+            # Extract the floats from the equation and add observe them
+            for num in Expr(equation).atoms(Number):
+                self.min_float.add(abs(num))
+
+    def _retrieve_equations(self) -> set:
+        """
+        Retrieve all the equations from the calculation functions
+        :return: A set of equations
+        """
+
+        equations = set()
+
+        for function in self.eqs:
+
+            # Call the function from the context of the branch
+            result = function()
+            if len(result) == 2:
+                # Simplify the results here to make all other operations faster
+                result = [simplify(e) for e in result]
+                # Check if the result is an equation that could produce a valid solution
+                # Also, handle the case where there is a contradiction (return -1)
+                can_compose = composes_equation(*result, self.min_float.value)
+                match can_compose:
+                    # Valid equation
+                    case 1:
+                        # Can only observe once we have samples of the magnitude of numbers that compose the solution
+                        self._observe_floats(result)
+                        resulting_eq = Eq(*result)
+                        equations.add(resulting_eq)
+                    # Invalid equation
+                    case 0:
+                        continue
+                    # Contradiction
+                    case -1:
+                        # Mark the current context for pruning
+                        # Note how a list type is passed, this is because this same function can be called elsewhere
+                        # with a list of equations that are all contradictory (but not necessarily on their own)
+                        self._mark_for_pruning([result])
+            else:
+                raise ValueError(f'Function does not return two elements {function}')
+
+        return equations
+
+    def _run_solver_this_branch(self) -> None:
+        """
+        Solve the equations by substituting solutions in place of unknown variables
+        Recursively attempts all combinations of equations
+        :return: None
+        """
+
+        # Evaluate all the user defined functions
+        self._eval_funcs()
+
+        # Gather all the equations from the calculation functions that have an unknown variable
+        # Remove any equations that are True as they are redundant
+        equations = self._retrieve_equations()
+
+        # If the advance_branch flag is set, return
+        # This means that a contradiction was found and the branch should be pruned
+        if self.advance_branch:
+            return
+
+        # Attempt to solve every subgroup of the equations
+        for r in range(1, len(equations) + 1):
+            for subgroup in combinations(equations, r):
+
+                target_variables = get_symbols(subgroup)
+
+                # Attempt to solve the subgroup of equations
+                solution = solve(subgroup, *target_variables)
+
+                # If solution == [], there is no solution for this subgroup
+                if not solution:
+                    # This branch shouldn't necessarily be pruned, but we need to throw special flag
+                    # Specifically, if the vars before solving and the vars after solving are the same, then
+                    # we should throw the flag. This is because some solutions may have branches that lead to this point
+                    # and we don't want to prune those branches because that set of equations could spawn a valid
+                    # solution. So, we need to check if the variables are the same before and after solving.
+                    # This would indicate that the equations are not solvable, and we should throw an exception.
+                    self.bad_solution.set(True)
+
+                # Verify the solution is valid; handle solution branching
+                sol = self._verify_and_extract_solution(solution, target_variables)
+
+                # If a solution was found, set the variables to the solution in this branch
+                if sol is not None:
+                    for key, value in sol.items():
+                        # Found a solution, set the variable to the solution
+                        self.context_stack.set_value(str(key), value)
+
+                    # If there are still unknown variables, attempt to solve again with the new information
+                    self._run_solver_this_branch()
+
+                    # Return to prevent further solving (want to utilize the most information possible)
+                    return
+
+        # Re-evaluate all the user defined functions in case of new information
+        self._eval_funcs()
+
+    def _prune_branches(self) -> None:
+        """
+        Prune the branches that are marked for pruning
+        :return: None
+        """
+
+        # If there are as many branches as there are contexts, raise an exception because there are no solutions
+        # Also need to offset the number of branches by the number of deletions
+        if self.num_branches - self.deletions.value == len(self.contexts_to_prune):
+
+            # Make quick-and-dirty pretty_equation function for use in just this exception throwing
+            # (Cannot have the second string be an f-string because that would mean nested f-strings)
+            def pretty_equation(equations):
+                s = ''
+                for eqn in equations:
+                    s += f'{eqn[0]} = {eqn[1]}, '
+                return s[:-2]
+
+            raise RuntimeError('Given equations have no consistent solutions. '
+                               'Please check your equations and try again. '
+                               'Contradiction(s) found: '
+                               f'{[pretty_equation(equations) for equations in self.contexts_to_prune.values()]}')
+
+        # Otherwise, prune the branches by finding the branches that match the hash
+        # Also, ensure that the context idx is not greater than the number of contexts
+        for context_hash, equation in self.contexts_to_prune.items():
+            for branch_idx, branch in enumerate(self.context_stack.contexts):
+                # If the branch matches the hash, prune it
+                if hash(tuple(sorted(branch.items()))) == context_hash:
+                    # Remove the context
+                    self.context_stack.remove_context(branch_idx)
+                    # Break out of the inner loop as we have found the branch to prune
+                    break
+
+        # Ensure that the actual idx pointer is not greater than the number of contexts
+        self.context_stack.context_idx = min(self.context_stack.context_idx, self.context_stack.num_contexts - 1)
+
+        # Reset the prune branches dictionary
+        self.contexts_to_prune.clear()
+
+    def solve(self) -> None:
+        """
+        Trigger the solver on all existing branches
+        Solver could branch into additional branches, of which the solver will also be triggered on
+        :return: None
+        """
+
+        # If the object has been solved before, throw a warning
+        if self.solved:
+            warn('This object has already been solved. '
+                 'Please create a new object to solve again.'
+                 'Solving multiple times could cause undetermined behavior in the branching behavior'
+                 'if variables are changed after the first solve.')
+
+        # Clear contexts_to_prune dictionary
+        self.contexts_to_prune.clear()
+
+        # Reset the bad_solution flag
+        self.bad_solution.set(False)
+
+        # Store the current context idx
+        old_context_idx = self.context_stack.context_idx
+
+        # Store the current solution as a copy of self.vars
+        old_solution = deepcopy(self.vars)
+
+        # Iterate through all the branches and solve them
+        # Iterate by rotating the context stack until we are back at where we started
+        # This accounts for new branches being added during the solving process
+
+        # Local function to run the solver on the current branch
+        def run_single():
+            # Run the solver on the current branch
+            self._run_solver_this_branch()
+            # Rotate off the first context
+            self.context_stack.rotate_context()
+            # Reset the advance_branch flag
+            self.advance_branch.set(False)
+            # Reset the number of deleted branches
+            self.deletions.set(0)
+
+        run_single()
+
+        # Wishing do-while loops were a thing in python...
+
+        # Continue rotating until we are back at the first context
+        while self.context_stack.context_idx != old_context_idx:
+            run_single()
+
+        # After solving, prune any branches that are marked for pruning
+        # Also check if there are no solutions and throw an exception accordingly
+        self._prune_branches()
+
+        # If the solution is bad and the branches did not change, throw an exception
+        if self.bad_solution and old_solution == self.vars:
+            raise RuntimeError('Given equations have no consistent solutions. '
+                               'Please check your equations and try again.')
+
+        # Mark the object as solved
+        self.solved.set(True)
+
+    def var_description(self, name: str) -> str:
+        """
+        Get the description of a variable
+        :param name: The name of the variable
+        :return: The description of the variable
+        """
+
+        # Raise an exception if the variable does not exist
+        if name not in self.var_descriptions:
+            raise KeyError(f'Variable {name} does not exist')
+
+        # Return the description of the variable
+        return self.var_descriptions[name]
+
+    def get_var_vals(self, name: str) -> list:
+        """
+        Get the value of a variable for each branch
+        :param name: The name of the variable
+        :return: A list of the values of the variable for each branch
+        """
+
+        # Raise an exception if the variable does not exist
+        if name not in self.context_stack.variables:
+            raise KeyError(f'Variable {name} does not exist')
+
+        # Return a list of the value of the variable for each branch
+        return list({self.context_stack.get_value(name, idx) for idx in range(self.context_stack.num_contexts)})
+
+    def get_var_vals_decimal(self, name: str) -> list:
+        """
+        Get the decimal value of a variable for each branch
+        :param name: The name of the variable
+        :return: A list of the values of the variable for each branch
+        """
+
+        # Raise an exception if the variable does not exist
+        if name not in self.context_stack.variables:
+            raise KeyError(f'Variable {name} does not exist')
+
+        # Return a list of the value of the variable for each branch
+        return list({N(self.context_stack.get_value(name, idx)) for idx in range(self.context_stack.num_contexts)})
+
+    def del_branch(self) -> None:
+        """
+        Delete the current branch of the current context
+        :return: None
+        """
+
+        # Delete the old context
+        # This handles updating the context idx
+        self.context_stack.remove_context(self.context_stack.context_idx)
+        # Note that we have deleted a branch
+        self.deletions.increment()
```

### Comparing `pyequations-0.1.0/pyequations/utils.py` & `pyequations-0.1.1/pyequations/utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-from sympy import Eq, Symbol, Number, Expr, N, Mul, Add, Pow, simplify
-from sympy.physics.units import Quantity, Unit
-
-from pyequations import EPSILON
-from pyequations.generate_units_subs import UnitSub
-
-
-def _is_solved(var) -> bool:
-    """
-    Check if the variable is solved
-    :param var: the attribute to check
-    :return: Whether the variable is solved
-    """
-
-    return not isinstance(var, Symbol)
-
-
-def solved(*variables) -> bool:
-    """
-    Check if all the variables are solved
-    :param variables: The variables to check
-    :return: Whether all the variables are solved
-    """
-
-    return all([_is_solved(var) for var in variables])
-
-
-def get_symbols(equations: [Eq]) -> tuple:
-    """
-    Get all the symbols in an equation
-    :param equations: The equations
-    :return: A tuple of all the symbols
-    """
-
-    # Return a tuple of all the symbols in the equation
-    # Cannot use sympy.atoms because that would return all the symbols PLUS the units
-    return tuple({sym for e in equations if isinstance(e, Eq) for sym in e.free_symbols})
-
-
-def remove_units(expr: Symbol | Number) -> Expr | Number | None:
-    """
-    Remove the units from a given expression
-    :param expr: An expression
-    :return: The expression with the units removed
-    """
-    if expr is None:
-        return None
-    if isinstance(expr, int | float | complex):
-        return expr
-    if not expr.has(Quantity):
-        return expr
-    units = expr.subs({x: 1 for x in expr.args if not x.has(Quantity)})
-    return expr / units
-
-
-def is_constant(expr) -> bool:
-    """
-    Check if the expression is constant
-    For example, 2 * cm is constant, but x * cm is not
-    Precondition: The expression must be simplified
-    :param expr: The expression to check
-    :return: Whether the expression is constant
-    """
-
-    # If the expression is a number, it is constant
-    if isinstance(expr, int | float | complex):
-        return True
-
-    # If the expression is a symbol, it is not constant
-    if isinstance(expr, Symbol):
-        return False
-
-    # If the expression is a unit, it is constant
-    if isinstance(expr, Quantity):
-        return True
-
-    # If the expression is a number, it is constant
-    if isinstance(expr, Number):
-        return True
-
-    # If calling N() on the expression is different from the expression, call is_constant on the result
-    if (result := N(expr)) != expr:
-        return is_constant(result)
-
-    # If the expression is an expression, check if it is constant
-    if isinstance(expr, Expr):
-
-        # If the expression is a Mul, check if all the args are constant
-        if isinstance(expr, Mul):
-            return all(is_constant(arg) for arg in expr.args)
-
-        # If the expression is an Add, check if all the args are constant
-        if isinstance(expr, Add):
-            return all(is_constant(arg) for arg in expr.args)
-
-        # If the expression is a Pow, check if the base and exponent are constant
-        if isinstance(expr, Pow):
-            return is_constant(expr.base) and is_constant(expr.exp)
-
-    # If the expression is not a number, symbol, or expression, it is not constant
-    return False
-
-
-def get_units(expr) -> set:
-    """
-    Get all the units in an expression
-    :param expr: The expression
-    :return: A set of all the units in the expression
-    """
-
-    if isinstance(expr, Expr):
-        return expr.atoms(Unit)
-    return set()
-
-
-def get_quantities(expr) -> set:
-    """
-    Get all the numerical quantities in an expression (ex. 7)
-    :param expr: The expression
-    :return: A set of all the quantities in the expression
-    """
-
-    if isinstance(expr, Expr):
-        return N(expr).atoms(Number)
-    return set()
-
-
-def composes_equation(lhs, rhs, min_float=1e-5) -> int:
-    """
-    Check if the two elements compose an equation
-    If there are no free symbols, it is not an equation
-    Otherwise, we check that the sides are 'close enough' to be considered equal
-    Precondition: The expressions must be simplified
-    :param lhs: The left hand side of the equation
-    :param rhs: The right hand side of the equation
-    :param min_float: The minimum float value observed elsewhere in the system. Used as a reference to zero.
-    :return: 1 if the elements compose an equation, 0 if they do not, or -1 if a contradiction is found
-    """
-
-    valid, invalid, contradiction = 1, 0, -1
-
-    lhs_constant = is_constant(lhs)
-    rhs_constant = is_constant(rhs)
-
-    # If both sides are expressions, check if they are equal
-    if not lhs_constant and not rhs_constant:
-        equal = False
-        # Need to simplify if either side contains units, otherwise the previous simplification is enough
-        if get_units(lhs) or get_units(rhs):
-            equal = simplify(lhs - rhs) == 0
-        else:
-            equal = lhs - rhs == 0
-        return invalid if equal else valid
-
-    # If either side contains free symbols, check if they are equal
-    elif not lhs_constant or not rhs_constant:
-        # Still need to check if they are equal
-        # Flip the sides if the rhs is an expression
-        if lhs_constant:
-            lhs, rhs = rhs, lhs
-        equal = False
-        # Need to simplify if either side contains units, otherwise the previous simplification is enough
-        if get_units(lhs) or get_units(rhs):
-            equal = simplify(lhs - rhs) == 0
-        else:
-            equal = lhs - rhs == 0
-        return invalid if equal else valid
-
-    # Final case: numeric values on both sides
-    # Check if the sides are 'close enough' to be considered equal
-    # This includes checking for unit correctness
-    # If lhs and rhs are both numbers, check if they are equal
-    else:
-
-        # The main things to be careful with here is units
-        # The workaround is to substitute all the units with random numbers around 1
-        # This is to avoid confusing the epsilon check
-        # Note that these random numbers are not the same for each unit
-
-        # Using randomness does have the potential to cause false positives
-        # However, this is unlikely to happen in practice and an incorrect result here will likely not cause issues
-        # This is because the system will likely be able to solve the system to the same extent, even if one equation is
-        # incorrectly considered to be not usable
-        # But, just to be sure, we check twice with two different mappings
-
-        # Get all the units in the lhs and rhs
-        lhs_units = get_units(lhs)
-        rhs_units = get_units(rhs)
-
-        # Make a list of the units, checking for None (no units)
-        units = []
-        if lhs_units is not None:
-            units.extend(lhs_units)
-        if rhs_units is not None:
-            units.extend(rhs_units)
-
-        # Reference the dictionaries of the units to substitute
-        for unit_dict in UnitSub.get_mappings():
-            # Test twice since there is the slightest probability that the random numbers will cause a false positive
-
-            # Substitute the units if they exist
-            if lhs_units:
-                lhs = lhs.subs(unit_dict)
-
-            if rhs_units:
-                rhs = rhs.subs(unit_dict)
-
-            sub = float(lhs - rhs)
-
-            # If one of the sides is 0, we can compare with the minimum float found elsewhere
-            if lhs == 0 or rhs == 0:
-                equal = abs(sub) <= min_float * EPSILON
-            else:
-                # Otherwise, re-check if the values are equal, scaled by the epsilon and the sum of the values
-                # This helps in the case when the numbers are smaller than the epsilon
-                equal = abs(sub) <= EPSILON * abs(lhs + rhs)
-
-            # This will only cause false positives -- i.e. we need to recheck only if the values are equal
-            if not equal:
-                break
-
-        return invalid if equal else contradiction
-
-
-class BoolWrapper:
-    """
-    A wrapper for a boolean value
-    This exists because we cannot re-initialize without the superclass in PyEquations
-    Provides simple functionality to set and get the value
-    """
-
-    def __init__(self, val: bool):
-        self.val = val
-
-    def __bool__(self):
-        return self.val
-
-    def set(self, val: bool):
-        self.val = val
-
-    def __repr__(self):
-        return str(self.val)
-
-
-class IntWrapper:
-    """
-    A wrapper for an integer value
-    This exists because we cannot re-initialize without the superclass in PyEquations
-    Provides simple functionality to set and get the value
-    """
-
-    def __init__(self, val: int):
-        self.val = val
-
-    @property
-    def value(self):
-        return self.val
-
-    def set(self, val: int):
-        self.val = val
-
-    def increment(self):
-        self.val += 1
-
-    def __repr__(self):
-        return str(self.val)
-
-
-class MinFloatTracker:
-    """
-    A wrapper for a float value representing the minimum (nonzero) value seen
-    """
-
-    def __init__(self):
-        self.val = float('inf')
-
-    @property
-    def value(self):
-        return self.val
-
-    def add(self, val: float):
-        """
-        Add a value to the tracker
-        :param val: The value to add
-        :return: None
-        """
-        if val != 0:
-            self.val = min(self.val, val)
-
-    def __repr__(self):
-        return str(self.val)
+from sympy import Eq, Symbol, Number, Expr, N, Mul, Add, Pow, simplify
+from sympy.physics.units import Quantity, Unit
+
+from pyequations import EPSILON
+from pyequations.generate_units_subs import UnitSub
+
+
+def _is_solved(var) -> bool:
+    """
+    Check if the variable is solved
+    :param var: the attribute to check
+    :return: Whether the variable is solved
+    """
+
+    return not isinstance(var, Symbol)
+
+
+def solved(*variables) -> bool:
+    """
+    Check if all the variables are solved
+    :param variables: The variables to check
+    :return: Whether all the variables are solved
+    """
+
+    return all([_is_solved(var) for var in variables])
+
+
+def get_symbols(equations: [Eq]) -> tuple:
+    """
+    Get all the symbols in an equation
+    :param equations: The equations
+    :return: A tuple of all the symbols
+    """
+
+    # Return a tuple of all the symbols in the equation
+    # Cannot use sympy.atoms because that would return all the symbols PLUS the units
+    return tuple({sym for e in equations if isinstance(e, Eq) for sym in e.free_symbols})
+
+
+def remove_units(expr: Symbol | Number) -> Expr | Number | None:
+    """
+    Remove the units from a given expression
+    :param expr: An expression
+    :return: The expression with the units removed
+    """
+    if expr is None:
+        return None
+    if isinstance(expr, int | float | complex):
+        return expr
+    if not expr.has(Quantity):
+        return expr
+    units = expr.subs({x: 1 for x in expr.args if not x.has(Quantity)})
+    return expr / units
+
+
+def is_constant(expr) -> bool:
+    """
+    Check if the expression is constant
+    For example, 2 * cm is constant, but x * cm is not
+    Precondition: The expression must be simplified
+    :param expr: The expression to check
+    :return: Whether the expression is constant
+    """
+
+    # If the expression is a number, it is constant
+    if isinstance(expr, int | float | complex):
+        return True
+
+    # If the expression is a symbol, it is not constant
+    if isinstance(expr, Symbol):
+        return False
+
+    # If the expression is a unit, it is constant
+    if isinstance(expr, Quantity):
+        return True
+
+    # If the expression is a number, it is constant
+    if isinstance(expr, Number):
+        return True
+
+    # If calling N() on the expression is different from the expression, call is_constant on the result
+    if (result := N(expr)) != expr:
+        return is_constant(result)
+
+    # If the expression is an expression, check if it is constant
+    if isinstance(expr, Expr):
+
+        # If the expression is a Mul, check if all the args are constant
+        if isinstance(expr, Mul):
+            return all(is_constant(arg) for arg in expr.args)
+
+        # If the expression is an Add, check if all the args are constant
+        if isinstance(expr, Add):
+            return all(is_constant(arg) for arg in expr.args)
+
+        # If the expression is a Pow, check if the base and exponent are constant
+        if isinstance(expr, Pow):
+            return is_constant(expr.base) and is_constant(expr.exp)
+
+    # If the expression is not a number, symbol, or expression, it is not constant
+    return False
+
+
+def get_units(expr) -> set:
+    """
+    Get all the units in an expression
+    :param expr: The expression
+    :return: A set of all the units in the expression
+    """
+
+    if isinstance(expr, Expr):
+        return expr.atoms(Unit)
+    return set()
+
+
+def get_quantities(expr) -> set:
+    """
+    Get all the numerical quantities in an expression (ex. 7)
+    :param expr: The expression
+    :return: A set of all the quantities in the expression
+    """
+
+    if isinstance(expr, Expr):
+        return N(expr).atoms(Number)
+    return set()
+
+
+def composes_equation(lhs, rhs, min_float=1e-5) -> int:
+    """
+    Check if the two elements compose an equation
+    If there are no free symbols, it is not an equation
+    Otherwise, we check that the sides are 'close enough' to be considered equal
+    Precondition: The expressions must be simplified
+    :param lhs: The left hand side of the equation
+    :param rhs: The right hand side of the equation
+    :param min_float: The minimum float value observed elsewhere in the system. Used as a reference to zero.
+    :return: 1 if the elements compose an equation, 0 if they do not, or -1 if a contradiction is found
+    """
+
+    valid, invalid, contradiction = 1, 0, -1
+
+    lhs_constant = is_constant(lhs)
+    rhs_constant = is_constant(rhs)
+
+    # If both sides are expressions, check if they are equal
+    if not lhs_constant and not rhs_constant:
+        equal = False
+        # Need to simplify if either side contains units, otherwise the previous simplification is enough
+        if get_units(lhs) or get_units(rhs):
+            equal = simplify(lhs - rhs) == 0
+        else:
+            equal = lhs - rhs == 0
+        return invalid if equal else valid
+
+    # If either side contains free symbols, check if they are equal
+    elif not lhs_constant or not rhs_constant:
+        # Still need to check if they are equal
+        # Flip the sides if the rhs is an expression
+        if lhs_constant:
+            lhs, rhs = rhs, lhs
+        equal = False
+        # Need to simplify if either side contains units, otherwise the previous simplification is enough
+        if get_units(lhs) or get_units(rhs):
+            equal = simplify(lhs - rhs) == 0
+        else:
+            equal = lhs - rhs == 0
+        return invalid if equal else valid
+
+    # Final case: numeric values on both sides
+    # Check if the sides are 'close enough' to be considered equal
+    # This includes checking for unit correctness
+    # If lhs and rhs are both numbers, check if they are equal
+    else:
+
+        # The main things to be careful with here is units
+        # The workaround is to substitute all the units with random numbers around 1
+        # This is to avoid confusing the epsilon check
+        # Note that these random numbers are not the same for each unit
+
+        # Using randomness does have the potential to cause false positives
+        # However, this is unlikely to happen in practice and an incorrect result here will likely not cause issues
+        # This is because the system will likely be able to solve the system to the same extent, even if one equation is
+        # incorrectly considered to be not usable
+        # But, just to be sure, we check twice with two different mappings
+
+        # Get all the units in the lhs and rhs
+        lhs_units = get_units(lhs)
+        rhs_units = get_units(rhs)
+
+        # Make a list of the units, checking for None (no units)
+        units = []
+        if lhs_units is not None:
+            units.extend(lhs_units)
+        if rhs_units is not None:
+            units.extend(rhs_units)
+
+        # Reference the dictionaries of the units to substitute
+        for unit_dict in UnitSub.get_mappings():
+            # Test twice since there is the slightest probability that the random numbers will cause a false positive
+
+            # Substitute the units if they exist
+            if lhs_units:
+                lhs = lhs.subs(unit_dict)
+
+            if rhs_units:
+                rhs = rhs.subs(unit_dict)
+
+            sub = float(lhs - rhs)
+
+            # If one of the sides is 0, we can compare with the minimum float found elsewhere
+            if lhs == 0 or rhs == 0:
+                equal = abs(sub) <= min_float * EPSILON
+            else:
+                # Otherwise, re-check if the values are equal, scaled by the epsilon and the sum of the values
+                # This helps in the case when the numbers are smaller than the epsilon
+                equal = abs(sub) <= EPSILON * abs(lhs + rhs)
+
+            # This will only cause false positives -- i.e. we need to recheck only if the values are equal
+            if not equal:
+                break
+
+        return invalid if equal else contradiction
+
+
+class BoolWrapper:
+    """
+    A wrapper for a boolean value
+    This exists because we cannot re-initialize without the superclass in PyEquations
+    Provides simple functionality to set and get the value
+    """
+
+    def __init__(self, val: bool):
+        self.val = val
+
+    def __bool__(self):
+        return self.val
+
+    def set(self, val: bool):
+        self.val = val
+
+    def __repr__(self):
+        return str(self.val)
+
+
+class IntWrapper:
+    """
+    A wrapper for an integer value
+    This exists because we cannot re-initialize without the superclass in PyEquations
+    Provides simple functionality to set and get the value
+    """
+
+    def __init__(self, val: int):
+        self.val = val
+
+    @property
+    def value(self):
+        return self.val
+
+    def set(self, val: int):
+        self.val = val
+
+    def increment(self):
+        self.val += 1
+
+    def __repr__(self):
+        return str(self.val)
+
+
+class MinFloatTracker:
+    """
+    A wrapper for a float value representing the minimum (nonzero) value seen
+    """
+
+    def __init__(self):
+        self.val = float('inf')
+
+    @property
+    def value(self):
+        return self.val
+
+    def add(self, val: float):
+        """
+        Add a value to the tracker
+        :param val: The value to add
+        :return: None
+        """
+        if val != 0:
+            self.val = min(self.val, val)
+
+    def __repr__(self):
+        return str(self.val)
```

