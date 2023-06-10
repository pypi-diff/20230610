# Comparing `tmp/mathslib-2.9.0.tar.gz` & `tmp/mathslib-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathslib-2.9.0.tar", last modified: Fri May 26 11:05:05 2023, max compression
+gzip compressed data, was "mathslib-3.0.0.tar", last modified: Sat Jun 10 05:31:22 2023, max compression
```

## Comparing `mathslib-2.9.0.tar` & `mathslib-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.681615 mathslib-2.9.0/
--rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-2.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0     6815 2023-05-26 11:05:05.681615 mathslib-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     5893 2023-05-26 11:03:53.000000 mathslib-2.9.0/README.rst
--rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-2.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       85 2023-05-26 11:05:05.689993 mathslib-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1560 2023-05-26 11:04:09.000000 mathslib-2.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.578900 mathslib-2.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.638984 mathslib-2.9.0/src/mathslib/
--rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-2.9.0/src/mathslib/__init__.py
--rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-2.9.0/src/mathslib/algorithms.py
--rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-2.9.0/src/mathslib/fib.py
--rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-2.9.0/src/mathslib/linalg.py
--rw-rw-rw-   0        0        0    21385 2023-05-26 11:01:11.000000 mathslib-2.9.0/src/mathslib/numtheory.py
--rw-rw-rw-   0        0        0    13999 2023-05-14 10:01:31.000000 mathslib-2.9.0/src/mathslib/primes.py
--rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-2.9.0/src/mathslib/simple.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:05:05.679357 mathslib-2.9.0/src/mathslib.egg-info/
--rw-rw-rw-   0        0        0     6815 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 11:05:05.000000 mathslib-2.9.0/src/mathslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.756217 mathslib-3.0.0/
+-rw-rw-rw-   0        0        0     1211 2022-05-22 14:55:29.000000 mathslib-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     7058 2023-06-10 05:31:22.759302 mathslib-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6133 2023-06-10 05:18:50.000000 mathslib-3.0.0/README.rst
+-rw-rw-rw-   0        0        0       85 2022-05-22 15:02:53.000000 mathslib-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       85 2023-06-10 05:31:22.767650 mathslib-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1560 2023-06-10 04:10:31.000000 mathslib-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.689290 mathslib-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.734510 mathslib-3.0.0/src/mathslib/
+-rw-rw-rw-   0        0        0     1543 2022-06-10 07:50:59.000000 mathslib-3.0.0/src/mathslib/__init__.py
+-rw-rw-rw-   0        0        0    15906 2023-05-14 09:39:13.000000 mathslib-3.0.0/src/mathslib/algorithms.py
+-rw-rw-rw-   0        0        0     5092 2023-06-10 05:27:26.000000 mathslib-3.0.0/src/mathslib/divisors.py
+-rw-rw-rw-   0        0        0     3314 2023-05-14 09:50:54.000000 mathslib-3.0.0/src/mathslib/fib.py
+-rw-rw-rw-   0        0        0     9961 2023-05-14 09:49:26.000000 mathslib-3.0.0/src/mathslib/linalg.py
+-rw-rw-rw-   0        0        0    19783 2023-06-10 04:09:38.000000 mathslib-3.0.0/src/mathslib/numtheory.py
+-rw-rw-rw-   0        0        0    14540 2023-06-10 04:36:27.000000 mathslib-3.0.0/src/mathslib/primes.py
+-rw-rw-rw-   0        0        0     5272 2023-05-14 09:45:48.000000 mathslib-3.0.0/src/mathslib/simple.py
+drwxrwxrwx   0        0        0        0 2023-06-10 05:31:22.756217 mathslib-3.0.0/src/mathslib.egg-info/
+-rw-rw-rw-   0        0        0     7058 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-10 05:31:22.000000 mathslib-3.0.0/src/mathslib.egg-info/top_level.txt
```

### Comparing `mathslib-2.9.0/LICENSE.txt` & `mathslib-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/PKG-INFO` & `mathslib-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.9.0
+Version: 3.0.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -38,42 +38,45 @@
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
 ---------
 +----------------+------------------------------------------------------------+
-|numtheory.py    | * divisors_of(x, include_x)                                |
-|                | * divisors(x, n)                                           |
-|                | * continued_fraction(x)                                    |
-|                | * overall_fraction(x)                                      |
-|                | * phi(x)                                                   |
+|numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
+|                | * continued_fraction(x)                                    |
+|                | * overall_fraction(x)                                      |
 +----------------+------------------------------------------------------------+
-|prime.py        | * prime_sieve(limit, block_size, segment, values)          |
+|primes.py       | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
+|                | * spf_sieve(x)                                             |
 |                | * primepi(x)                                               |
 |                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
 |                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
+|divisors.py     | * divisors(x, proper)                                      |
+|                | * divisor(x, n)                                            |
+|                | * divisor_sieve(x, n)                                      |
++----------------+------------------------------------------------------------+
 |linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
```

### Comparing `mathslib-2.9.0/README.rst` & `mathslib-3.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,42 +17,45 @@
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
 ---------
 +----------------+------------------------------------------------------------+
-|numtheory.py    | * divisors_of(x, include_x)                                |
-|                | * divisors(x, n)                                           |
-|                | * continued_fraction(x)                                    |
-|                | * overall_fraction(x)                                      |
-|                | * phi(x)                                                   |
+|numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
+|                | * continued_fraction(x)                                    |
+|                | * overall_fraction(x)                                      |
 +----------------+------------------------------------------------------------+
-|prime.py        | * prime_sieve(limit, block_size, segment, values)          |
+|primes.py       | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
+|                | * spf_sieve(x)                                             |
 |                | * primepi(x)                                               |
 |                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
 |                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
+|divisors.py     | * divisors(x, proper)                                      |
+|                | * divisor(x, n)                                            |
+|                | * divisor_sieve(x, n)                                      |
++----------------+------------------------------------------------------------+
 |linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
```

### Comparing `mathslib-2.9.0/setup.py` & `mathslib-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (here / "README.rst").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name = "mathslib",  # Required
-    version="2.9.0",  # Required
+    version="3.0.0",  # Required
     description="Library of Mathematical functions and Algorithms",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/x-rst",  # Optional
     url="https://github.com/igorvanloo/mathslib",  # Optional
     author="Igor van Loo",  # Optional
     author_email="igorvanloo@gmail.com",  # Optional
     classifiers=[  # Optional
```

### Comparing `mathslib-2.9.0/src/mathslib/__init__.py` & `mathslib-3.0.0/src/mathslib/__init__.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/src/mathslib/algorithms.py` & `mathslib-3.0.0/src/mathslib/algorithms.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/src/mathslib/fib.py` & `mathslib-3.0.0/src/mathslib/fib.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/src/mathslib/linalg.py` & `mathslib-3.0.0/src/mathslib/linalg.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/src/mathslib/numtheory.py` & `mathslib-3.0.0/src/mathslib/numtheory.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,133 +25,17 @@
 
 '''
 Various Number Theory functions
 
 Author: Igor van Loo
 '''
 import math
-from .primes import prime_factors, prime_sieve
+from .primes import prime_sieve
 from .simple import extended_euclidean_algorithm
 
-def divisors_of(x, include_x = True):
-    '''
-    Finds all the divisors of x
-
-    :param x: Integer to be checked
-    :param include_x: Optional boolean value, If true it will include x as a divisor of x
-
-    :returns: A list which contains all divisors of x
-    
-    .. code-block:: python
-    
-        print(divisors_of(15)) #[1, 3, 5, 15]
-        print(divisors_of(15, include_x = False)) #[1, 3, 5]
-
-    '''
-    if (type(x) != int):
-        return "All values must be integers"
-    divisors = []
-    for i in range(1, int(math.sqrt(x)) + 1):
-        if x % i == 0:
-            divisors.append(i)
-            divisors.append(int(x/i))
-    if include_x:
-        return sorted(divisors)
-    else:
-        divisors.remove(x)
-        return sorted(divisors)
-    
-def divisor(x, n):
-    '''
-    Implementation of `Divisor function 
-    <https://en.wikipedia.org/wiki/Divisor_function#Definition>`_ sigma(x, n) 
-    
-    :param x: An integer, denotes the power till which the divisors will be summed
-    :param n: An integer, denotes the number to find the divisors of
-    
-    :returns: An integer
-    
-    .. code-block:: python
-    
-        print(divisor(0, 9)) #3
-        print(divisor(1, 9)) #13
-        print(divisor(2, 9)) #91
-        
-    '''
-    if (type(n) != int) or (type(x) != int):
-        return "All values must be integers"
-    
-    pf = prime_factors(n)
-    total = 1
-    if x == 0:
-        for p in pf:
-            e = pf[p]
-            total *= (e + 1)
-    else:
-        for p in pf:
-            e = pf[p]
-            total *= ((pow(p, x*(e + 1)) - 1)//(pow(p, x) - 1))
-    return total
-
-def continued_fraction(x):
-    '''
-    Finds the `continued Fraction
-    <https://en.wikipedia.org/wiki/Continued_fraction>`_ of the sqrt(x)
-
-    :param x: An integer
-
-    :returns: A list containing the continued fraction of x
-    
-    .. code-block:: python
-    
-        print(continued_fraction(19)) #[4, 2, 1, 3, 1, 2, 8]
-    
-    .. note::
-        
-        The continued fraction may repeat forever, the code stops once it repeats, otherwise once we find the 100th number in the continued fraction
-    '''
-    if (type(x) != int):
-        return "All values must be integers"
-    m0 = 0
-    d0 = 1
-    a0 = math.floor(math.sqrt(x)) #These are the starting values
-    temp_list = [a0]
-    while True:
-        mn = int(d0*a0 - m0) 
-        dn = int((x - mn**2)/d0)
-        an = int(math.floor((math.sqrt(x) + mn) / dn)) #new values
-        temp_list.append(an)
-        if an == 2*math.floor(math.sqrt(x)):
-            break
-        if len(temp_list) == 100:
-            break
-        m0 = mn
-        d0 = dn
-        a0 = an #Replace values
-    return temp_list
-
-def overall_fraction(cf):
-    '''
-    :param cf: A list, this list represents the continued fraction of a number
-
-    :returns numerator: An integer, the numerator of the fraction
-    :returns denominator: An integer, the denominator of the fraction
-    
-    .. code-block:: python
-    
-        print(overall_fraction([4, 2, 6, 7])) #(415, 93)
-
-    '''
-    cf = cf[::-1]
-    denominator = 1
-    numerator = cf[0]
-    for x in range(1,len(cf)):
-        numerator, denominator = cf[x]*numerator + denominator, numerator
-    return numerator, denominator
-
 def phi(n):
     '''
     Implementation of `Eulers Totient Function
     <https://en.wikipedia.org/wiki/Euler%27s_totient_function>`_ counts the positive integers up to a given integer n that are relatively prime to n
 
     :param n: An integer
 
@@ -217,15 +101,15 @@
     :param n: An integer
 
     :returns: sum of phi(x) where x goes from 1 to n
     
     .. code-block:: python
     
         print(phi_sum(10**4)) #30397486
-        print(sum(phi(i) for i in range(1, 10**4))) #30397486
+        print(sum(phi(i) for i in range(1, 10**4 + 1))) #30397486
         print(sum(phi_sieve(10**4))) #30397486
         
     '''
     L = int(math.sqrt(n))
     v = [0]*(L + 1)
     bigV = [0]*(n//L + 1)
     
@@ -345,15 +229,15 @@
         print(count_k_free(2**50, 2)) #684465067343069
         
     '''
     sq = math.floor(n**(1/k))
     mobius_k = mobius_k_sieve(sq, 2)
     return sum([mobius_k[i]*(n//pow(i, k)) for i in range(1, sq + 1)])
 
-def ppt(limit, non_primitive = True):
+def pythagoren_triples(limit, non_primitive = True):
     '''
     Generates all `Pythagorean Triplets 
     <https://en.wikipedia.org/wiki/Pythagorean_triple>`_ up to the limit
 
     :param limit: An integer, will generate all Pythagorean Triplets such that no side is longer than the limit
     :param non_primitive: Optional boolean value, If True, returns all triplets, if False returns only primitive triplets
 
@@ -700,7 +584,63 @@
                 S[u] = w
                 P[u] = j
                 if u not in Q:
                     Q.append(u)
     #Step 3
     return max(S) - a1
 
+def continued_fraction(x):
+    '''
+    Finds the `continued Fraction
+    <https://en.wikipedia.org/wiki/Continued_fraction>`_ of the sqrt(x)
+
+    :param x: An integer
+
+    :returns: A list containing the continued fraction of x
+    
+    .. code-block:: python
+    
+        print(continued_fraction(19)) #[4, 2, 1, 3, 1, 2, 8]
+    
+    .. note::
+        
+        The continued fraction may repeat forever, the code stops once it repeats, otherwise once we find the 100th number in the continued fraction
+    '''
+    if (type(x) != int):
+        return "All values must be integers"
+    m0 = 0
+    d0 = 1
+    a0 = math.floor(math.sqrt(x)) #These are the starting values
+    temp_list = [a0]
+    while True:
+        mn = int(d0*a0 - m0) 
+        dn = int((x - mn**2)/d0)
+        an = int(math.floor((math.sqrt(x) + mn) / dn)) #new values
+        temp_list.append(an)
+        if an == 2*math.floor(math.sqrt(x)):
+            break
+        if len(temp_list) == 100:
+            break
+        m0 = mn
+        d0 = dn
+        a0 = an #Replace values
+    return temp_list
+
+def overall_fraction(cf):
+    '''
+    :param cf: A list, this list represents the continued fraction of a number
+
+    :returns numerator: An integer, the numerator of the fraction
+    :returns denominator: An integer, the denominator of the fraction
+    
+    .. code-block:: python
+    
+        print(overall_fraction([4, 2, 6, 7])) #(415, 93)
+
+    '''
+    cf = cf[::-1]
+    denominator = 1
+    numerator = cf[0]
+    for x in range(1,len(cf)):
+        numerator, denominator = cf[x]*numerator + denominator, numerator
+    return numerator, denominator
+
```

### Comparing `mathslib-2.9.0/src/mathslib/primes.py` & `mathslib-3.0.0/src/mathslib/primes.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,38 @@
                 if d in factors:
                     factors[n] += 1
                 else:
                     factors[n] = 1
             break
     return factors
 
+def spf_sieve(N):
+    '''
+    A smallest prime factor sieve. 
+
+    :param N: An integer
+
+    :returns: An array such that array[x] = smallest prime factor of x
+    
+    .. code-block:: python
+    
+        print(spf_sieve(10)) #[0, 1, 2, 3, 2, 5, 2, 7, 2, 3, 2]
+        
+    '''
+    if type(N) != int:
+        return "n must be an integer"
+    
+    spf = [i for i in range(N + 1)]
+    
+    for i in range(2, int(math.sqrt(N)) + 1):
+        if spf[i] == i:
+            for j in range(i*i, N + 1, i):
+                spf[j] = i
+    return spf
+
 def primepi(x):
     '''
     Primepi function is commonly known as `Prime Counting Function <https://en.wikipedia.org/wiki/Prime-counting_function>`_
     
     This function computes primepi(x) based on the `Meissel-Lehmer Method <https://mathworld.wolfram.com/LehmersFormula.html>`_
     
     The following `article <https://acgan.sh/posts/2016-12-23-prime-counting.html>`_ by Adithya Ganesh helped me a lot in understanding and implementing this function
```

### Comparing `mathslib-2.9.0/src/mathslib/simple.py` & `mathslib-3.0.0/src/mathslib/simple.py`

 * *Files identical despite different names*

### Comparing `mathslib-2.9.0/src/mathslib.egg-info/PKG-INFO` & `mathslib-3.0.0/src/mathslib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathslib
-Version: 2.9.0
+Version: 3.0.0
 Summary: Library of Mathematical functions and Algorithms
 Home-page: https://github.com/igorvanloo/mathslib
 Author: Igor van Loo
 Author-email: igorvanloo@gmail.com
 Project-URL: Bug Reports, https://github.com/igorvanloo/mathslib/issues
 Project-URL: Source, https://github.com/igorvanloo/mathslib
 Keywords: numbertheory,maths,algorithms
@@ -38,42 +38,45 @@
 See my website `ivl-projecteuler.com`_ for their implementation
 
 See the full documentation `here`_
 
 Breakdown
 ---------
 +----------------+------------------------------------------------------------+
-|numtheory.py    | * divisors_of(x, include_x)                                |
-|                | * divisors(x, n)                                           |
-|                | * continued_fraction(x)                                    |
-|                | * overall_fraction(x)                                      |
-|                | * phi(x)                                                   |
+|numtheory.py    | * phi(x)                                                   |
 |                | * phi_sieve(x)                                             |
 |                | * phi_sum(x)                                               |
 |                | * mobius(x)                                                |
 |                | * mobius_k_sieve(limit, k)                                 |
 |                | * count_k_free(n, k)                                       |
 |                | * ppt(limit, non_primitive)                                |
 |                | * k_smooth_numbers(max_prime, limit)                       |
 |                | * k_powerful(k, limit, count)                              |
 |                | * legendre_factorial(x)                                    |
 |                | * tonelli_shanks(a, p)                                     |
 |                | * chinese_remainder_theorem(a1, a2, n1, n2)                |
 |                | * generalised_CRT(a1, a2, n1, n2)                          |
 |                | * frobenius_number(\*integers)                             |
+|                | * continued_fraction(x)                                    |
+|                | * overall_fraction(x)                                      |
 +----------------+------------------------------------------------------------+
-|prime.py        | * prime_sieve(limit, block_size, segment, values)          |
+|primes.py       | * prime_sieve(limit, block_size, segment, values)          |
 |                | * is_prime(x)                                              |
 |                | * prime_factors(x)                                         |
+|                | * spf_sieve(x)                                             |
 |                | * primepi(x)                                               |
 |                | * primepi_sieve(x)                                         |
 |                | * sum_of_primes(x)                                         |
 |                | * fermat_primality_test(x)                                 |
 |                | * miller_primality_test(n, millerrabin, numoftests)        |
 +----------------+------------------------------------------------------------+
+|divisors.py     | * divisors(x, proper)                                      |
+|                | * divisor(x, n)                                            |
+|                | * divisor_sieve(x, n)                                      |
++----------------+------------------------------------------------------------+
 |linalg.py       | * gauss_jordan_elimination(matrix, augmentedpart)          |
 |                | * solve(M, b)                                              |
 |                | * inverse(matrix)                                          |
 |                | * determinant(matrix)                                      |
 |                | * matrix_addition(A, B, subtract)                          |
 |                | * identity(l, val)                                         |
 |                | * concatenate(A, B)                                        |
```

