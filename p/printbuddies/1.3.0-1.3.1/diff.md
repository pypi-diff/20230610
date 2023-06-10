# Comparing `tmp/printbuddies-1.3.0.tar.gz` & `tmp/printbuddies-1.3.1.tar.gz`

## Comparing `printbuddies-1.3.0.tar` & `printbuddies-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 printbuddies-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/index.html
--rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/printbuddies.html
--rw-r--r--   0        0        0    34898 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/search.js
--rw-r--r--   0        0        0   214063 2020-02-02 00:00:00.000000 printbuddies-1.3.0/docs/printbuddies/printbuddies.html
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 printbuddies-1.3.0/src/printbuddies/__init__.py
--rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 printbuddies-1.3.0/src/printbuddies/printbuddies.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 printbuddies-1.3.0/README.md
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 printbuddies-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 printbuddies-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 printbuddies-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.3.1/docs/index.html
+-rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 printbuddies-1.3.1/docs/printbuddies.html
+-rw-r--r--   0        0        0    34919 2020-02-02 00:00:00.000000 printbuddies-1.3.1/docs/search.js
+-rw-r--r--   0        0        0   226103 2020-02-02 00:00:00.000000 printbuddies-1.3.1/docs/printbuddies/printbuddies.html
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 printbuddies-1.3.1/src/printbuddies/__init__.py
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 printbuddies-1.3.1/src/printbuddies/printbuddies.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 printbuddies-1.3.1/README.md
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 printbuddies-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 printbuddies-1.3.1/PKG-INFO
```

### Comparing `printbuddies-1.3.0/CHANGELOG.md` & `printbuddies-1.3.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## v1.3.0 (2023-06-03)
+
+#### New Features
+
+* add movement to Spinner
+* sequence width will update when the terminal width changes
+#### Refactorings
+
+* default character sequence is assigned as parameter default
+* change width parameter to width_ratio
+#### Others
+
+* add missing version prefix
+
+
 ## v1.2.0 (2023-04-25)
 
 #### New Features
 
 * implement Spinner class
 * add context manager functionality
 * add runtime property to ProgBar
```

### Comparing `printbuddies-1.3.0/docs/printbuddies.html` & `printbuddies-1.3.1/docs/printbuddies.html`

 * *Files identical despite different names*

### Comparing `printbuddies-1.3.0/docs/search.js` & `printbuddies-1.3.1/docs/search.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -701,52 +701,52 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.print_in_place",
         "modulename": "printbuddies.printbuddies",
         "qualname": "print_in_place",
         "kind": "function",
-        "doc": "<p>Calls to print_in_place will overwrite\nthe previous line of text in the terminal\nwith the 'string' param.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>animate</strong>:  Will cause the string\nto be printed to the terminal\none character at a time.</p></li>\n<li><p><strong>animate_refresh</strong>:  Number of seconds\nbetween the addition of characters\nwhen 'animate' is True.</p></li>\n</ul>\n",
+        "doc": "<p>Calls to <code>print_in_place</code> will overwrite the previous line of text in the terminal with <code>string</code>.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>animate</code>: Will cause <code>string</code> to be printed to the terminal one character at a time.</p>\n\n<p><code>animate_refresh</code>: Number of seconds between the addition of characters when <code>animate</code> is <code>True</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">string</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">animate</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span>, </span><span class=\"param\"><span class=\"n\">animate_refresh</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">=</span> <span class=\"mf\">0.01</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.ticker",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ticker",
         "kind": "function",
-        "doc": "<p>Prints info to terminal with\ntop and bottom padding so that repeated\ncalls print info without showing previous\noutputs from ticker calls.</p>\n\n<p>Similar visually to print_in_place,\nbut for multiple lines.</p>\n",
+        "doc": "<p>Prints <code>info</code> to terminal with top and bottom padding so that previous text is not visible.</p>\n\n<p>Similar visually to <code>print_in_place</code>, but for multiple lines.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">info</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar",
         "kind": "class",
-        "doc": "<p>Self incrementing, dynamically sized progress bar.</p>\n\n<p>Includes an internal timer that starts when this object is created.\nIt can be easily added to the progress bar display by adding\nthe 'runtime' property to display's prefix or suffix param:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"n\">total</span><span class=\"o\">=</span><span class=\"mi\">100</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">time</span><span class=\"o\">.</span><span class=\"n\">sleep</span><span class=\"p\">(</span><span class=\"mi\">30</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">(</span><span class=\"n\">prefix</span><span class=\"o\">=</span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">runtime</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"s2\">&quot;runtime: 30s [_///////////////////]1.00%&quot;</span>\n</code></pre>\n</div>\n"
+        "doc": "<p>Self incrementing, dynamically sized progress bar.</p>\n\n<p>Includes an internal timer that starts when this object is created.</p>\n\n<p>Easily add runtime to progress display:</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"n\">total</span><span class=\"o\">=</span><span class=\"mi\">100</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">time</span><span class=\"o\">.</span><span class=\"n\">sleep</span><span class=\"p\">(</span><span class=\"mi\">30</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">(</span><span class=\"n\">prefix</span><span class=\"o\">=</span><span class=\"sa\">f</span><span class=\"s2\">&quot;Doin stuff ~ </span><span class=\"si\">{</span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">runtime</span><span class=\"si\">}</span><span class=\"s2\">&quot;</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"s2\">&quot;Doin stuff ~ runtime: 30s [_///////////////////]-1.00%&quot;</span>\n</code></pre>\n</div>\n"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar.__init__",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar.__init__",
         "kind": "function",
-        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>total</strong>:  The number of calls to reach 100% completion.</p></li>\n<li><p><strong>update_frequency</strong>:  The progress bar will only update once every this number of calls to display().\nThe larger the value, the less performance impact ProgBar has on the loop in which it is called.\ne.g.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"mi\">100</span><span class=\"p\">,</span> <span class=\"n\">update_frequency</span><span class=\"o\">=</span><span class=\"mi\">10</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">for</span> <span class=\"n\">_</span> <span class=\"ow\">in</span> <span class=\"nb\">range</span><span class=\"p\">(</span><span class=\"mi\">100</span><span class=\"p\">):</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">()</span>\n</code></pre>\n</div></li>\n</ul>\n\n<p>^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.\nNote: If 'total' is not a multiple of 'update_frequency', the display will not show 100% completion when the loop finishes.</p>\n\n<ul>\n<li><p><strong>fill_ch</strong>:  The character used to represent the completed part of the bar.</p></li>\n<li><p><strong>unfill_ch</strong>:  The character used to represent the uncompleted part of the bar.</p></li>\n<li><p><strong>width_ratio</strong>:  The width of the progress bar relative to the width of the terminal window.</p></li>\n<li><p><strong>new_line_after_completion</strong>:  Make a call to print() once self.counter &gt;= self.total.</p></li>\n<li><p><strong>clear_after_completion</strong>:  Make a call to printbuddies.clear() once self.counter &gt;= self.total.</p></li>\n</ul>\n\n<p>Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared\nthen a call to print() will be made.</p>\n",
-        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">total</span><span class=\"p\">:</span> <span class=\"nb\">float</span>,</span><span class=\"param\">\t<span class=\"n\">update_frequency</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"mi\">1</span>,</span><span class=\"param\">\t<span class=\"n\">fill_ch</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;_&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">unfill_ch</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;/&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">width_ratio</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">=</span> <span class=\"mf\">0.75</span>,</span><span class=\"param\">\t<span class=\"n\">new_line_after_completion</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">clear_after_completion</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span>)</span>"
+        "doc": "<h4 id=\"params\">:params:</h4>\n\n<p><code>total</code>: The number of calls to reach 100% completion.</p>\n\n<p><code>update_frequency</code>: The progress bar will only update once every this number of calls to <code>display()</code>.\nThe larger the value, the less performance impact <code>ProgBar</code> has on the loop in which it is called.\ne.g.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"mi\">100</span><span class=\"p\">,</span> <span class=\"n\">update_frequency</span><span class=\"o\">=</span><span class=\"mi\">10</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">for</span> <span class=\"n\">_</span> <span class=\"ow\">in</span> <span class=\"nb\">range</span><span class=\"p\">(</span><span class=\"mi\">100</span><span class=\"p\">):</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">()</span>\n</code></pre>\n</div>\n\n<p>^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.\nNote: If <code>total</code> is not a multiple of <code>update_frequency</code>, the display will not show 100% completion when the loop finishes.</p>\n\n<p><code>fill_ch</code>: The character used to represent the completed part of the bar.</p>\n\n<p><code>unfill_ch</code>: The character used to represent the incomplete part of the bar.</p>\n\n<p><code>width_ratio</code>: The width of the progress bar relative to the width of the terminal window.</p>\n\n<p><code>new_line_after_completion</code>: Make a call to <code>print()</code> once <code>self.counter &gt;= self.total</code>.</p>\n\n<p><code>clear_after_completion</code>: Make a call to <code>printbuddies.clear()</code> once <code>self.counter &gt;= self.total</code>.</p>\n\n<p>Note: if <code>new_line_after_completion</code> and <code>clear_after_completion</code> are both <code>True</code>, the line will be cleared\nthen a call to <code>print()</code> will be made.</p>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">total</span><span class=\"p\">:</span> <span class=\"nb\">float</span>,</span><span class=\"param\">\t<span class=\"n\">update_frequency</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">=</span> <span class=\"mi\">1</span>,</span><span class=\"param\">\t<span class=\"n\">fill_ch</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;_&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">unfill_ch</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;/&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">width_ratio</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">=</span> <span class=\"mf\">0.5</span>,</span><span class=\"param\">\t<span class=\"n\">new_line_after_completion</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">True</span>,</span><span class=\"param\">\t<span class=\"n\">clear_after_completion</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span>)</span>"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar.reset",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar.reset",
         "kind": "function",
         "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar.get_percent",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar.get_percent",
         "kind": "function",
-        "doc": "<p>Returns the percentage complete to two decimal places\nas a string without the %.</p>\n",
+        "doc": "<p>Returns the percentage completed to two decimal places as a string without the <code>%</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">str</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar.get_bar",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar.get_bar",
         "kind": "function",
@@ -754,29 +754,29 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.ProgBar.display",
         "modulename": "printbuddies.printbuddies",
         "qualname": "ProgBar.display",
         "kind": "function",
-        "doc": "<p>Writes the progress bar to the terminal.</p>\n\n<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>prefix</strong>:  String affixed to the front of the progress bar.</p></li>\n<li><p><strong>suffix</strong>:  String appended to the end of the progress bar.</p></li>\n<li><p><strong>counter_override</strong>:  When an externally incremented completion counter is needed.</p></li>\n<li><p><strong>total_override</strong>:  When an externally controlled bar total is needed.</p></li>\n<li><p><strong>return_object</strong>:  An object to be returned by display().</p></li>\n</ul>\n\n<p>Allows display() to be called within a comprehension:</p>\n\n<p>e.g.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"mi\">10</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">def</span> <span class=\"nf\">square</span><span class=\"p\">(</span><span class=\"n\">x</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"nb\">float</span><span class=\"p\">)</span><span class=\"o\">-&gt;</span><span class=\"nb\">int</span><span class=\"o\">|</span><span class=\"nb\">float</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">return</span> <span class=\"n\">x</span> <span class=\"o\">*</span> <span class=\"n\">x</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">myList</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">(</span><span class=\"n\">return_object</span><span class=\"o\">=</span><span class=\"n\">square</span><span class=\"p\">(</span><span class=\"n\">i</span><span class=\"p\">))</span> <span class=\"k\">for</span> <span class=\"n\">i</span> <span class=\"ow\">in</span> <span class=\"nb\">range</span><span class=\"p\">(</span><span class=\"mi\">10</span><span class=\"p\">)]</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"o\">&lt;</span><span class=\"n\">progress</span> <span class=\"n\">bar</span> <span class=\"n\">gets</span> <span class=\"n\">displayed</span><span class=\"o\">&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">myList</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"p\">[</span><span class=\"mi\">0</span><span class=\"p\">,</span> <span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"mi\">4</span><span class=\"p\">,</span> <span class=\"mi\">9</span><span class=\"p\">,</span> <span class=\"mi\">16</span><span class=\"p\">,</span> <span class=\"mi\">25</span><span class=\"p\">,</span> <span class=\"mi\">36</span><span class=\"p\">,</span> <span class=\"mi\">49</span><span class=\"p\">,</span> <span class=\"mi\">64</span><span class=\"p\">,</span> <span class=\"mi\">81</span><span class=\"p\">]</span>\n</code></pre>\n</div>\n",
+        "doc": "<p>Writes the progress bar to the terminal.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>prefix</code>: String affixed to the front of the progress bar.</p>\n\n<p><code>suffix</code>: String appended to the end of the progress bar.</p>\n\n<p><code>counter_override</code>: When an externally incremented completion counter is needed.</p>\n\n<p><code>total_override</code>: When an externally controlled bar total is needed.</p>\n\n<p><code>return_object</code>: An object to be returned by display().\nAllows <code>display()</code> to be called within a comprehension:</p>\n\n<p>e.g.</p>\n\n<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">bar</span> <span class=\"o\">=</span> <span class=\"n\">ProgBar</span><span class=\"p\">(</span><span class=\"mi\">10</span><span class=\"p\">)</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"k\">def</span> <span class=\"nf\">square</span><span class=\"p\">(</span><span class=\"n\">x</span><span class=\"p\">:</span> <span class=\"nb\">int</span> <span class=\"o\">|</span> <span class=\"nb\">float</span><span class=\"p\">)</span><span class=\"o\">-&gt;</span><span class=\"nb\">int</span><span class=\"o\">|</span><span class=\"nb\">float</span><span class=\"p\">:</span>\n<span class=\"gp\">&gt;&gt;&gt; </span>    <span class=\"k\">return</span> <span class=\"n\">x</span> <span class=\"o\">*</span> <span class=\"n\">x</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">myList</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"n\">bar</span><span class=\"o\">.</span><span class=\"n\">display</span><span class=\"p\">(</span><span class=\"n\">return_object</span><span class=\"o\">=</span><span class=\"n\">square</span><span class=\"p\">(</span><span class=\"n\">i</span><span class=\"p\">))</span> <span class=\"k\">for</span> <span class=\"n\">i</span> <span class=\"ow\">in</span> <span class=\"nb\">range</span><span class=\"p\">(</span><span class=\"mi\">10</span><span class=\"p\">)]</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"o\">&lt;</span><span class=\"n\">progress</span> <span class=\"n\">bar</span> <span class=\"n\">gets</span> <span class=\"n\">displayed</span><span class=\"o\">&gt;</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">myList</span>\n<span class=\"gp\">&gt;&gt;&gt; </span><span class=\"p\">[</span><span class=\"mi\">0</span><span class=\"p\">,</span> <span class=\"mi\">1</span><span class=\"p\">,</span> <span class=\"mi\">4</span><span class=\"p\">,</span> <span class=\"mi\">9</span><span class=\"p\">,</span> <span class=\"mi\">16</span><span class=\"p\">,</span> <span class=\"mi\">25</span><span class=\"p\">,</span> <span class=\"mi\">36</span><span class=\"p\">,</span> <span class=\"mi\">49</span><span class=\"p\">,</span> <span class=\"mi\">64</span><span class=\"p\">,</span> <span class=\"mi\">81</span><span class=\"p\">]</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"bp\">self</span>,</span><span class=\"param\">\t<span class=\"n\">prefix</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">suffix</span><span class=\"p\">:</span> <span class=\"nb\">str</span> <span class=\"o\">=</span> <span class=\"s1\">&#39;&#39;</span>,</span><span class=\"param\">\t<span class=\"n\">counter_override</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">total_override</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span>,</span><span class=\"param\">\t<span class=\"n\">return_object</span><span class=\"p\">:</span> <span class=\"n\">typing</span><span class=\"o\">.</span><span class=\"n\">Any</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">) -> <span class=\"n\">Any</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner",
         "kind": "class",
-        "doc": "<p>Prints one of a sequence of characters in order everytime display() is called.</p>\n\n<p>The display function writes the new character to the same line, overwriting the previous character.</p>\n\n<p>The sequence will be cycled through indefinitely.</p>\n\n<p>If used as a context manager, the last printed character will be cleared upon exiting.</p>\n"
+        "doc": "<p>Prints one of a sequence of characters in order everytime <code>display()</code> is called.</p>\n\n<p>The <code>display</code> function writes the new character to the same line, overwriting the previous character.</p>\n\n<p>The sequence will be cycled through indefinitely.</p>\n\n<p>If used as a context manager, the last printed character will be cleared upon exiting.</p>\n"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner.__init__",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner.__init__",
         "kind": "function",
-        "doc": "<h6 id=\"parameters\">Parameters</h6>\n\n<ul>\n<li><p><strong>sequence</strong>:  Override the built in spin sequence.</p></li>\n<li><p><strong>width</strong>:  The fractional amount of the terminal for characters to move across.</p></li>\n</ul>\n",
+        "doc": "<h4 id=\"params\">params:</h4>\n\n<p><code>sequence</code>: Override the built in spin sequence.</p>\n\n<p><code>width_ratio</code>: The fractional amount of the terminal for characters to move across.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">sequence</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">str</span><span class=\"p\">]</span> <span class=\"o\">=</span> <span class=\"p\">[</span><span class=\"s1\">&#39;/&#39;</span><span class=\"p\">,</span> <span class=\"s1\">&#39;-&#39;</span><span class=\"p\">,</span> <span class=\"s1\">&#39;</span><span class=\"se\">\\\\</span><span class=\"s1\">&#39;</span><span class=\"p\">]</span>, </span><span class=\"param\"><span class=\"n\">width_ratio</span><span class=\"p\">:</span> <span class=\"nb\">float</span> <span class=\"o\">=</span> <span class=\"mf\">0.25</span></span>)</span>"
     }, {
         "fullname": "printbuddies.printbuddies.Spinner.display",
         "modulename": "printbuddies.printbuddies",
         "qualname": "Spinner.display",
         "kind": "function",
         "doc": "<p>Print the next character in the sequence.</p>\n",
```

### Comparing `printbuddies-1.3.0/docs/printbuddies/printbuddies.html` & `printbuddies-1.3.1/docs/printbuddies/printbuddies.html`

 * *Files 2% similar despite different names*

```diff
@@ -98,290 +98,314 @@
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Any</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">noiftimer</span> <span class="kn">import</span> <span class="n">Timer</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a>
 </span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="k">def</span> <span class="nf">clear</span><span class="p">():</span>
 </span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a>    <span class="sd">&quot;&quot;&quot;Erase the current line from the terminal.&quot;&quot;&quot;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span><span class="p">),</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
-</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">print_in_place</span><span class="p">(</span><span class="n">string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">animate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">animate_refresh</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span><span class="p">):</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;Calls to print_in_place will overwrite</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a><span class="sd">    the previous line of text in the terminal</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a><span class="sd">    with the &#39;string&#39; param.</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span><span class="p">),</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>        <span class="o">...</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="sd">    :param animate: Will cause the string</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a><span class="sd">    to be printed to the terminal</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">    one character at a time.</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a><span class="sd">    :param animate_refresh: Number of seconds</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">    between the addition of characters</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="sd">    when &#39;animate&#39; is True.&quot;&quot;&quot;</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">clear</span><span class="p">()</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">string</span><span class="p">)</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="n">string</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">]</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="k">if</span> <span class="n">animate</span><span class="p">:</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">string</span><span class="p">)):</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">string</span><span class="p">[:</span><span class="n">i</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot; </span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>            <span class="n">sleep</span><span class="p">(</span><span class="n">animate_refresh</span><span class="p">)</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">string</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="k">def</span> <span class="nf">ticker</span><span class="p">(</span><span class="n">info</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="sd">&quot;&quot;&quot;Prints info to terminal with</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">    top and bottom padding so that repeated</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">    calls print info without showing previous</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">    outputs from ticker calls.</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">print_in_place</span><span class="p">(</span><span class="n">string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">animate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">animate_refresh</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span><span class="p">):</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="sd">&quot;&quot;&quot;Calls to `print_in_place` will overwrite the previous line of text in the terminal with `string`.</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">    `animate`: Will cause `string` to be printed to the terminal one character at a time.</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">    `animate_refresh`: Number of seconds between the addition of characters when `animate` is `True`.&quot;&quot;&quot;</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">string</span><span class="p">)</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="n">string</span> <span class="o">=</span> <span class="n">string</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">]</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="k">if</span> <span class="n">animate</span><span class="p">:</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">string</span><span class="p">)):</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">string</span><span class="p">[:</span><span class="n">i</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot; </span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>                <span class="n">sleep</span><span class="p">(</span><span class="n">animate_refresh</span><span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">string</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="o">...</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
 </span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="sd">    Similar visually to print_in_place,</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">    but for multiple lines.&quot;&quot;&quot;</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">info</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">line</span><span class="p">)[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">info</span><span class="p">]</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">height</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">lines</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">info</span><span class="p">)</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">height</span> <span class="o">*</span> <span class="mi">2</span><span class="p">),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">info</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="nb">int</span><span class="p">((</span><span class="n">height</span><span class="p">)</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">    It can be easily added to the progress bar display by adding</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">    the &#39;runtime&#39; property to display&#39;s prefix or suffix param:</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="k">def</span> <span class="nf">ticker</span><span class="p">(</span><span class="n">info</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="sd">&quot;&quot;&quot;Prints `info` to terminal with top and bottom padding so that previous text is not visible.</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">    Similar visually to `print_in_place`, but for multiple lines.&quot;&quot;&quot;</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">info</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">line</span><span class="p">)[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">info</span><span class="p">]</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">height</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">lines</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">info</span><span class="p">)</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">height</span> <span class="o">*</span> <span class="mi">2</span><span class="p">),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">info</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="nb">int</span><span class="p">((</span><span class="n">height</span><span class="p">)</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="o">...</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
 </span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=bar.runtime)</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    &gt;&gt;&gt; &quot;runtime: 30s [_///////////////////]1.00%&quot; &quot;&quot;&quot;</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
 </span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="p">):</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">        e.g.</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    Easily add runtime to progress display:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=f&quot;Doin stuff ~ {bar.runtime}&quot;)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">    &gt;&gt;&gt; &quot;Doin stuff ~ runtime: 30s [_///////////////////]-1.00%&quot; &quot;&quot;&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.5</span><span class="p">,</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="p">):</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">        `total`: The number of calls to reach 100% completion.</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">        `update_frequency`: The progress bar will only update once every this number of calls to `display()`.</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">        The larger the value, the less performance impact `ProgBar` has on the loop in which it is called.</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="sd">        e.g.</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">        Note: If `total` is not a multiple of `update_frequency`, the display will not show 100% completion when the loop finishes.</span>
 </span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>            <span class="n">clear</span><span class="p">()</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>            <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">        `fill_ch`: The character used to represent the completed part of the bar.</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">        `unfill_ch`: The character used to represent the incomplete part of the bar.</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">        `width_ratio`: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">        `new_line_after_completion`: Make a call to `print()` once `self.counter &gt;= self.total`.</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="sd">        `clear_after_completion`: Make a call to `printbuddies.clear()` once `self.counter &gt;= self.total`.</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">        Note: if `new_line_after_completion` and `clear_after_completion` are both `True`, the line will be cleared</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">        then a call to `print()` will be made.&quot;&quot;&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
 </span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>            <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>            <span class="nb">print</span><span class="p">()</span>
 </span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="nd">@property</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">return</span> <span class="n">percent</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="sd">        e.g.</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>                    <span class="n">clear</span><span class="p">()</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>                    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="k">return</span> <span class="n">return_object</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>    <span class="p">):</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="nd">@property</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="nd">@property</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">def</span> <span class="nf">bar</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage completed to two decimal places as a string without the `%`.&quot;&quot;&quot;</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="k">return</span> <span class="n">percent</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">        `prefix`: String affixed to the front of the progress bar.</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">        `suffix`: String appended to the end of the progress bar.</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">        `counter_override`: When an externally incremented completion counter is needed.</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">        `total_override`: When an externally controlled bar total is needed.</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">        `return_object`: An object to be returned by display().</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">        Allows `display()` to be called within a comprehension:</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">        e.g.</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>                <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>                <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                        <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>                        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>            <span class="o">...</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>            <span class="k">raise</span> <span class="n">e</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime `display()` is called.</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="sd">    The `display` function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
 </span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">    &quot;&quot;&quot;</span>
 </span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="nd">@property</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="p">):</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">        #### params:</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">        `sequence`: Override the built in spin sequence.</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">        `width_ratio`: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
 </span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="nd">@property</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="p">]</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence, append it to the end, and return the element.&quot;&quot;&quot;</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>    <span class="nd">@property</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
 </span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="nd">@property</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>        <span class="p">]</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of `self._sequence`, append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>            <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>            <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>            <span class="o">...</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>            <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
             </section>
                 <section id="clear">
                             <input id="clear-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -391,15 +415,20 @@
 
                 <label class="view-source-button" for="clear-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#clear"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="clear-9"><a href="#clear-9"><span class="linenos"> 9</span></a><span class="k">def</span> <span class="nf">clear</span><span class="p">():</span>
 </span><span id="clear-10"><a href="#clear-10"><span class="linenos">10</span></a>    <span class="sd">&quot;&quot;&quot;Erase the current line from the terminal.&quot;&quot;&quot;</span>
-</span><span id="clear-11"><a href="#clear-11"><span class="linenos">11</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span><span class="p">),</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="clear-11"><a href="#clear-11"><span class="linenos">11</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="clear-12"><a href="#clear-12"><span class="linenos">12</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span><span class="p">),</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="clear-13"><a href="#clear-13"><span class="linenos">13</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="clear-14"><a href="#clear-14"><span class="linenos">14</span></a>        <span class="o">...</span>
+</span><span id="clear-15"><a href="#clear-15"><span class="linenos">15</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="clear-16"><a href="#clear-16"><span class="linenos">16</span></a>        <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Erase the current line from the terminal.</p>
 </div>
 
 
@@ -411,53 +440,47 @@
         <span class="def">def</span>
         <span class="name">print_in_place</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">string</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">animate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span>, </span><span class="param"><span class="n">animate_refresh</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="print_in_place-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#print_in_place"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="print_in_place-14"><a href="#print_in_place-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">print_in_place</span><span class="p">(</span><span class="n">string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">animate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">animate_refresh</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span><span class="p">):</span>
-</span><span id="print_in_place-15"><a href="#print_in_place-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Calls to print_in_place will overwrite</span>
-</span><span id="print_in_place-16"><a href="#print_in_place-16"><span class="linenos">16</span></a><span class="sd">    the previous line of text in the terminal</span>
-</span><span id="print_in_place-17"><a href="#print_in_place-17"><span class="linenos">17</span></a><span class="sd">    with the &#39;string&#39; param.</span>
-</span><span id="print_in_place-18"><a href="#print_in_place-18"><span class="linenos">18</span></a>
-</span><span id="print_in_place-19"><a href="#print_in_place-19"><span class="linenos">19</span></a><span class="sd">    :param animate: Will cause the string</span>
-</span><span id="print_in_place-20"><a href="#print_in_place-20"><span class="linenos">20</span></a><span class="sd">    to be printed to the terminal</span>
-</span><span id="print_in_place-21"><a href="#print_in_place-21"><span class="linenos">21</span></a><span class="sd">    one character at a time.</span>
-</span><span id="print_in_place-22"><a href="#print_in_place-22"><span class="linenos">22</span></a>
-</span><span id="print_in_place-23"><a href="#print_in_place-23"><span class="linenos">23</span></a><span class="sd">    :param animate_refresh: Number of seconds</span>
-</span><span id="print_in_place-24"><a href="#print_in_place-24"><span class="linenos">24</span></a><span class="sd">    between the addition of characters</span>
-</span><span id="print_in_place-25"><a href="#print_in_place-25"><span class="linenos">25</span></a><span class="sd">    when &#39;animate&#39; is True.&quot;&quot;&quot;</span>
-</span><span id="print_in_place-26"><a href="#print_in_place-26"><span class="linenos">26</span></a>    <span class="n">clear</span><span class="p">()</span>
-</span><span id="print_in_place-27"><a href="#print_in_place-27"><span class="linenos">27</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">string</span><span class="p">)</span>
-</span><span id="print_in_place-28"><a href="#print_in_place-28"><span class="linenos">28</span></a>    <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="print_in_place-29"><a href="#print_in_place-29"><span class="linenos">29</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="n">string</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">]</span>
-</span><span id="print_in_place-30"><a href="#print_in_place-30"><span class="linenos">30</span></a>    <span class="k">if</span> <span class="n">animate</span><span class="p">:</span>
-</span><span id="print_in_place-31"><a href="#print_in_place-31"><span class="linenos">31</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">string</span><span class="p">)):</span>
-</span><span id="print_in_place-32"><a href="#print_in_place-32"><span class="linenos">32</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">string</span><span class="p">[:</span><span class="n">i</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot; </span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="print_in_place-33"><a href="#print_in_place-33"><span class="linenos">33</span></a>            <span class="n">sleep</span><span class="p">(</span><span class="n">animate_refresh</span><span class="p">)</span>
-</span><span id="print_in_place-34"><a href="#print_in_place-34"><span class="linenos">34</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="print_in_place-35"><a href="#print_in_place-35"><span class="linenos">35</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">string</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="print_in_place-19"><a href="#print_in_place-19"><span class="linenos">19</span></a><span class="k">def</span> <span class="nf">print_in_place</span><span class="p">(</span><span class="n">string</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">animate</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">animate_refresh</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.01</span><span class="p">):</span>
+</span><span id="print_in_place-20"><a href="#print_in_place-20"><span class="linenos">20</span></a>    <span class="sd">&quot;&quot;&quot;Calls to `print_in_place` will overwrite the previous line of text in the terminal with `string`.</span>
+</span><span id="print_in_place-21"><a href="#print_in_place-21"><span class="linenos">21</span></a>
+</span><span id="print_in_place-22"><a href="#print_in_place-22"><span class="linenos">22</span></a><span class="sd">    #### :params:</span>
+</span><span id="print_in_place-23"><a href="#print_in_place-23"><span class="linenos">23</span></a>
+</span><span id="print_in_place-24"><a href="#print_in_place-24"><span class="linenos">24</span></a><span class="sd">    `animate`: Will cause `string` to be printed to the terminal one character at a time.</span>
+</span><span id="print_in_place-25"><a href="#print_in_place-25"><span class="linenos">25</span></a>
+</span><span id="print_in_place-26"><a href="#print_in_place-26"><span class="linenos">26</span></a><span class="sd">    `animate_refresh`: Number of seconds between the addition of characters when `animate` is `True`.&quot;&quot;&quot;</span>
+</span><span id="print_in_place-27"><a href="#print_in_place-27"><span class="linenos">27</span></a>    <span class="n">clear</span><span class="p">()</span>
+</span><span id="print_in_place-28"><a href="#print_in_place-28"><span class="linenos">28</span></a>    <span class="n">string</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">string</span><span class="p">)</span>
+</span><span id="print_in_place-29"><a href="#print_in_place-29"><span class="linenos">29</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="print_in_place-30"><a href="#print_in_place-30"><span class="linenos">30</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="print_in_place-31"><a href="#print_in_place-31"><span class="linenos">31</span></a>        <span class="n">string</span> <span class="o">=</span> <span class="n">string</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">]</span>
+</span><span id="print_in_place-32"><a href="#print_in_place-32"><span class="linenos">32</span></a>        <span class="k">if</span> <span class="n">animate</span><span class="p">:</span>
+</span><span id="print_in_place-33"><a href="#print_in_place-33"><span class="linenos">33</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">string</span><span class="p">)):</span>
+</span><span id="print_in_place-34"><a href="#print_in_place-34"><span class="linenos">34</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">string</span><span class="p">[:</span><span class="n">i</span><span class="o">+</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot; </span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="print_in_place-35"><a href="#print_in_place-35"><span class="linenos">35</span></a>                <span class="n">sleep</span><span class="p">(</span><span class="n">animate_refresh</span><span class="p">)</span>
+</span><span id="print_in_place-36"><a href="#print_in_place-36"><span class="linenos">36</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="print_in_place-37"><a href="#print_in_place-37"><span class="linenos">37</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">string</span><span class="p">,</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="print_in_place-38"><a href="#print_in_place-38"><span class="linenos">38</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="print_in_place-39"><a href="#print_in_place-39"><span class="linenos">39</span></a>        <span class="o">...</span>
+</span><span id="print_in_place-40"><a href="#print_in_place-40"><span class="linenos">40</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="print_in_place-41"><a href="#print_in_place-41"><span class="linenos">41</span></a>        <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Calls to print_in_place will overwrite
-the previous line of text in the terminal
-with the 'string' param.</p>
-
-<h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><p><strong>animate</strong>:  Will cause the string
-to be printed to the terminal
-one character at a time.</p></li>
-<li><p><strong>animate_refresh</strong>:  Number of seconds
-between the addition of characters
-when 'animate' is True.</p></li>
-</ul>
+            <div class="docstring"><p>Calls to <code><a href="#print_in_place">print_in_place</a></code> will overwrite the previous line of text in the terminal with <code>string</code>.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>animate</code>: Will cause <code>string</code> to be printed to the terminal one character at a time.</p>
+
+<p><code>animate_refresh</code>: Number of seconds between the addition of characters when <code>animate</code> is <code>True</code>.</p>
 </div>
 
 
                 </section>
                 <section id="ticker">
                             <input id="ticker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -465,38 +488,35 @@
         <span class="def">def</span>
         <span class="name">ticker</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">info</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ticker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ticker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ticker-38"><a href="#ticker-38"><span class="linenos">38</span></a><span class="k">def</span> <span class="nf">ticker</span><span class="p">(</span><span class="n">info</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
-</span><span id="ticker-39"><a href="#ticker-39"><span class="linenos">39</span></a>    <span class="sd">&quot;&quot;&quot;Prints info to terminal with</span>
-</span><span id="ticker-40"><a href="#ticker-40"><span class="linenos">40</span></a><span class="sd">    top and bottom padding so that repeated</span>
-</span><span id="ticker-41"><a href="#ticker-41"><span class="linenos">41</span></a><span class="sd">    calls print info without showing previous</span>
-</span><span id="ticker-42"><a href="#ticker-42"><span class="linenos">42</span></a><span class="sd">    outputs from ticker calls.</span>
-</span><span id="ticker-43"><a href="#ticker-43"><span class="linenos">43</span></a>
-</span><span id="ticker-44"><a href="#ticker-44"><span class="linenos">44</span></a><span class="sd">    Similar visually to print_in_place,</span>
-</span><span id="ticker-45"><a href="#ticker-45"><span class="linenos">45</span></a><span class="sd">    but for multiple lines.&quot;&quot;&quot;</span>
-</span><span id="ticker-46"><a href="#ticker-46"><span class="linenos">46</span></a>    <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="ticker-47"><a href="#ticker-47"><span class="linenos">47</span></a>    <span class="n">info</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">line</span><span class="p">)[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">info</span><span class="p">]</span>
-</span><span id="ticker-48"><a href="#ticker-48"><span class="linenos">48</span></a>    <span class="n">height</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">lines</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">info</span><span class="p">)</span>
-</span><span id="ticker-49"><a href="#ticker-49"><span class="linenos">49</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">height</span> <span class="o">*</span> <span class="mi">2</span><span class="p">),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="ticker-50"><a href="#ticker-50"><span class="linenos">50</span></a>    <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">info</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
-</span><span id="ticker-51"><a href="#ticker-51"><span class="linenos">51</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="nb">int</span><span class="p">((</span><span class="n">height</span><span class="p">)</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ticker-44"><a href="#ticker-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">ticker</span><span class="p">(</span><span class="n">info</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
+</span><span id="ticker-45"><a href="#ticker-45"><span class="linenos">45</span></a>    <span class="sd">&quot;&quot;&quot;Prints `info` to terminal with top and bottom padding so that previous text is not visible.</span>
+</span><span id="ticker-46"><a href="#ticker-46"><span class="linenos">46</span></a>
+</span><span id="ticker-47"><a href="#ticker-47"><span class="linenos">47</span></a><span class="sd">    Similar visually to `print_in_place`, but for multiple lines.&quot;&quot;&quot;</span>
+</span><span id="ticker-48"><a href="#ticker-48"><span class="linenos">48</span></a>    <span class="k">try</span><span class="p">:</span>
+</span><span id="ticker-49"><a href="#ticker-49"><span class="linenos">49</span></a>        <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="ticker-50"><a href="#ticker-50"><span class="linenos">50</span></a>        <span class="n">info</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">line</span><span class="p">)[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span> <span class="k">for</span> <span class="n">line</span> <span class="ow">in</span> <span class="n">info</span><span class="p">]</span>
+</span><span id="ticker-51"><a href="#ticker-51"><span class="linenos">51</span></a>        <span class="n">height</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">lines</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="n">info</span><span class="p">)</span>
+</span><span id="ticker-52"><a href="#ticker-52"><span class="linenos">52</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="n">height</span> <span class="o">*</span> <span class="mi">2</span><span class="p">),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="ticker-53"><a href="#ticker-53"><span class="linenos">53</span></a>        <span class="nb">print</span><span class="p">(</span><span class="o">*</span><span class="n">info</span><span class="p">,</span> <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="ticker-54"><a href="#ticker-54"><span class="linenos">54</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span> <span class="o">*</span> <span class="p">(</span><span class="nb">int</span><span class="p">((</span><span class="n">height</span><span class="p">)</span> <span class="o">/</span> <span class="mi">2</span><span class="p">)),</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">)</span>
+</span><span id="ticker-55"><a href="#ticker-55"><span class="linenos">55</span></a>    <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="ticker-56"><a href="#ticker-56"><span class="linenos">56</span></a>        <span class="o">...</span>
+</span><span id="ticker-57"><a href="#ticker-57"><span class="linenos">57</span></a>    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="ticker-58"><a href="#ticker-58"><span class="linenos">58</span></a>        <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Prints info to terminal with
-top and bottom padding so that repeated
-calls print info without showing previous
-outputs from ticker calls.</p>
+            <div class="docstring"><p>Prints <code>info</code> to terminal with top and bottom padding so that previous text is not visible.</p>
 
-<p>Similar visually to print_in_place,
-but for multiple lines.</p>
+<p>Similar visually to <code><a href="#print_in_place">print_in_place</a></code>, but for multiple lines.</p>
 </div>
 
 
                 </section>
                 <section id="ProgBar">
                             <input id="ProgBar-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -504,284 +524,298 @@
     <span class="def">class</span>
     <span class="name">ProgBar</span>:
 
                 <label class="view-source-button" for="ProgBar-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar-54"><a href="#ProgBar-54"><span class="linenos"> 54</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
-</span><span id="ProgBar-55"><a href="#ProgBar-55"><span class="linenos"> 55</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
-</span><span id="ProgBar-56"><a href="#ProgBar-56"><span class="linenos"> 56</span></a>
-</span><span id="ProgBar-57"><a href="#ProgBar-57"><span class="linenos"> 57</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
-</span><span id="ProgBar-58"><a href="#ProgBar-58"><span class="linenos"> 58</span></a><span class="sd">    It can be easily added to the progress bar display by adding</span>
-</span><span id="ProgBar-59"><a href="#ProgBar-59"><span class="linenos"> 59</span></a><span class="sd">    the &#39;runtime&#39; property to display&#39;s prefix or suffix param:</span>
-</span><span id="ProgBar-60"><a href="#ProgBar-60"><span class="linenos"> 60</span></a>
-</span><span id="ProgBar-61"><a href="#ProgBar-61"><span class="linenos"> 61</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
-</span><span id="ProgBar-62"><a href="#ProgBar-62"><span class="linenos"> 62</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
-</span><span id="ProgBar-63"><a href="#ProgBar-63"><span class="linenos"> 63</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=bar.runtime)</span>
-</span><span id="ProgBar-64"><a href="#ProgBar-64"><span class="linenos"> 64</span></a><span class="sd">    &gt;&gt;&gt; &quot;runtime: 30s [_///////////////////]1.00%&quot; &quot;&quot;&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar-61"><a href="#ProgBar-61"><span class="linenos"> 61</span></a><span class="k">class</span> <span class="nc">ProgBar</span><span class="p">:</span>
+</span><span id="ProgBar-62"><a href="#ProgBar-62"><span class="linenos"> 62</span></a>    <span class="sd">&quot;&quot;&quot;Self incrementing, dynamically sized progress bar.</span>
+</span><span id="ProgBar-63"><a href="#ProgBar-63"><span class="linenos"> 63</span></a>
+</span><span id="ProgBar-64"><a href="#ProgBar-64"><span class="linenos"> 64</span></a><span class="sd">    Includes an internal timer that starts when this object is created.</span>
 </span><span id="ProgBar-65"><a href="#ProgBar-65"><span class="linenos"> 65</span></a>
-</span><span id="ProgBar-66"><a href="#ProgBar-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="ProgBar-67"><a href="#ProgBar-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar-68"><a href="#ProgBar-68"><span class="linenos"> 68</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
-</span><span id="ProgBar-69"><a href="#ProgBar-69"><span class="linenos"> 69</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
-</span><span id="ProgBar-70"><a href="#ProgBar-70"><span class="linenos"> 70</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-71"><a href="#ProgBar-71"><span class="linenos"> 71</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-72"><a href="#ProgBar-72"><span class="linenos"> 72</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
-</span><span id="ProgBar-73"><a href="#ProgBar-73"><span class="linenos"> 73</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="ProgBar-74"><a href="#ProgBar-74"><span class="linenos"> 74</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="ProgBar-75"><a href="#ProgBar-75"><span class="linenos"> 75</span></a>    <span class="p">):</span>
-</span><span id="ProgBar-76"><a href="#ProgBar-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
-</span><span id="ProgBar-77"><a href="#ProgBar-77"><span class="linenos"> 77</span></a>
-</span><span id="ProgBar-78"><a href="#ProgBar-78"><span class="linenos"> 78</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
-</span><span id="ProgBar-79"><a href="#ProgBar-79"><span class="linenos"> 79</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
-</span><span id="ProgBar-80"><a href="#ProgBar-80"><span class="linenos"> 80</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar-81"><a href="#ProgBar-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
-</span><span id="ProgBar-82"><a href="#ProgBar-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
-</span><span id="ProgBar-83"><a href="#ProgBar-83"><span class="linenos"> 83</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
-</span><span id="ProgBar-84"><a href="#ProgBar-84"><span class="linenos"> 84</span></a>
-</span><span id="ProgBar-85"><a href="#ProgBar-85"><span class="linenos"> 85</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
-</span><span id="ProgBar-86"><a href="#ProgBar-86"><span class="linenos"> 86</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
+</span><span id="ProgBar-66"><a href="#ProgBar-66"><span class="linenos"> 66</span></a><span class="sd">    Easily add runtime to progress display:</span>
+</span><span id="ProgBar-67"><a href="#ProgBar-67"><span class="linenos"> 67</span></a>
+</span><span id="ProgBar-68"><a href="#ProgBar-68"><span class="linenos"> 68</span></a><span class="sd">    &gt;&gt;&gt; bar = ProgBar(total=100)</span>
+</span><span id="ProgBar-69"><a href="#ProgBar-69"><span class="linenos"> 69</span></a><span class="sd">    &gt;&gt;&gt; time.sleep(30)</span>
+</span><span id="ProgBar-70"><a href="#ProgBar-70"><span class="linenos"> 70</span></a><span class="sd">    &gt;&gt;&gt; bar.display(prefix=f&quot;Doin stuff ~ {bar.runtime}&quot;)</span>
+</span><span id="ProgBar-71"><a href="#ProgBar-71"><span class="linenos"> 71</span></a><span class="sd">    &gt;&gt;&gt; &quot;Doin stuff ~ runtime: 30s [_///////////////////]-1.00%&quot; &quot;&quot;&quot;</span>
+</span><span id="ProgBar-72"><a href="#ProgBar-72"><span class="linenos"> 72</span></a>
+</span><span id="ProgBar-73"><a href="#ProgBar-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="ProgBar-74"><a href="#ProgBar-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar-75"><a href="#ProgBar-75"><span class="linenos"> 75</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="ProgBar-76"><a href="#ProgBar-76"><span class="linenos"> 76</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
+</span><span id="ProgBar-77"><a href="#ProgBar-77"><span class="linenos"> 77</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-78"><a href="#ProgBar-78"><span class="linenos"> 78</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-79"><a href="#ProgBar-79"><span class="linenos"> 79</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.5</span><span class="p">,</span>
+</span><span id="ProgBar-80"><a href="#ProgBar-80"><span class="linenos"> 80</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="ProgBar-81"><a href="#ProgBar-81"><span class="linenos"> 81</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="ProgBar-82"><a href="#ProgBar-82"><span class="linenos"> 82</span></a>    <span class="p">):</span>
+</span><span id="ProgBar-83"><a href="#ProgBar-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="ProgBar-84"><a href="#ProgBar-84"><span class="linenos"> 84</span></a><span class="sd">        #### :params:</span>
+</span><span id="ProgBar-85"><a href="#ProgBar-85"><span class="linenos"> 85</span></a>
+</span><span id="ProgBar-86"><a href="#ProgBar-86"><span class="linenos"> 86</span></a><span class="sd">        `total`: The number of calls to reach 100% completion.</span>
 </span><span id="ProgBar-87"><a href="#ProgBar-87"><span class="linenos"> 87</span></a>
-</span><span id="ProgBar-88"><a href="#ProgBar-88"><span class="linenos"> 88</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="ProgBar-89"><a href="#ProgBar-89"><span class="linenos"> 89</span></a>
-</span><span id="ProgBar-90"><a href="#ProgBar-90"><span class="linenos"> 90</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="ProgBar-91"><a href="#ProgBar-91"><span class="linenos"> 91</span></a>
-</span><span id="ProgBar-92"><a href="#ProgBar-92"><span class="linenos"> 92</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="ProgBar-93"><a href="#ProgBar-93"><span class="linenos"> 93</span></a>
-</span><span id="ProgBar-94"><a href="#ProgBar-94"><span class="linenos"> 94</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="ProgBar-95"><a href="#ProgBar-95"><span class="linenos"> 95</span></a>
-</span><span id="ProgBar-96"><a href="#ProgBar-96"><span class="linenos"> 96</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar-88"><a href="#ProgBar-88"><span class="linenos"> 88</span></a><span class="sd">        `update_frequency`: The progress bar will only update once every this number of calls to `display()`.</span>
+</span><span id="ProgBar-89"><a href="#ProgBar-89"><span class="linenos"> 89</span></a><span class="sd">        The larger the value, the less performance impact `ProgBar` has on the loop in which it is called.</span>
+</span><span id="ProgBar-90"><a href="#ProgBar-90"><span class="linenos"> 90</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar-91"><a href="#ProgBar-91"><span class="linenos"> 91</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="ProgBar-92"><a href="#ProgBar-92"><span class="linenos"> 92</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="ProgBar-93"><a href="#ProgBar-93"><span class="linenos"> 93</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="ProgBar-94"><a href="#ProgBar-94"><span class="linenos"> 94</span></a>
+</span><span id="ProgBar-95"><a href="#ProgBar-95"><span class="linenos"> 95</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="ProgBar-96"><a href="#ProgBar-96"><span class="linenos"> 96</span></a><span class="sd">        Note: If `total` is not a multiple of `update_frequency`, the display will not show 100% completion when the loop finishes.</span>
 </span><span id="ProgBar-97"><a href="#ProgBar-97"><span class="linenos"> 97</span></a>
-</span><span id="ProgBar-98"><a href="#ProgBar-98"><span class="linenos"> 98</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="ProgBar-99"><a href="#ProgBar-99"><span class="linenos"> 99</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="ProgBar-100"><a href="#ProgBar-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="ProgBar-101"><a href="#ProgBar-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
-</span><span id="ProgBar-102"><a href="#ProgBar-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar-103"><a href="#ProgBar-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar-104"><a href="#ProgBar-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="ProgBar-105"><a href="#ProgBar-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="ProgBar-106"><a href="#ProgBar-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="ProgBar-107"><a href="#ProgBar-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
-</span><span id="ProgBar-108"><a href="#ProgBar-108"><span class="linenos">108</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="ProgBar-109"><a href="#ProgBar-109"><span class="linenos">109</span></a>
-</span><span id="ProgBar-110"><a href="#ProgBar-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-111"><a href="#ProgBar-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="ProgBar-112"><a href="#ProgBar-112"><span class="linenos">112</span></a>        <span class="k">return</span> <span class="bp">self</span>
-</span><span id="ProgBar-113"><a href="#ProgBar-113"><span class="linenos">113</span></a>
-</span><span id="ProgBar-114"><a href="#ProgBar-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="ProgBar-115"><a href="#ProgBar-115"><span class="linenos">115</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar-116"><a href="#ProgBar-116"><span class="linenos">116</span></a>            <span class="n">clear</span><span class="p">()</span>
-</span><span id="ProgBar-117"><a href="#ProgBar-117"><span class="linenos">117</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="ProgBar-118"><a href="#ProgBar-118"><span class="linenos">118</span></a>            <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar-98"><a href="#ProgBar-98"><span class="linenos"> 98</span></a><span class="sd">        `fill_ch`: The character used to represent the completed part of the bar.</span>
+</span><span id="ProgBar-99"><a href="#ProgBar-99"><span class="linenos"> 99</span></a>
+</span><span id="ProgBar-100"><a href="#ProgBar-100"><span class="linenos">100</span></a><span class="sd">        `unfill_ch`: The character used to represent the incomplete part of the bar.</span>
+</span><span id="ProgBar-101"><a href="#ProgBar-101"><span class="linenos">101</span></a>
+</span><span id="ProgBar-102"><a href="#ProgBar-102"><span class="linenos">102</span></a><span class="sd">        `width_ratio`: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="ProgBar-103"><a href="#ProgBar-103"><span class="linenos">103</span></a>
+</span><span id="ProgBar-104"><a href="#ProgBar-104"><span class="linenos">104</span></a><span class="sd">        `new_line_after_completion`: Make a call to `print()` once `self.counter &gt;= self.total`.</span>
+</span><span id="ProgBar-105"><a href="#ProgBar-105"><span class="linenos">105</span></a>
+</span><span id="ProgBar-106"><a href="#ProgBar-106"><span class="linenos">106</span></a><span class="sd">        `clear_after_completion`: Make a call to `printbuddies.clear()` once `self.counter &gt;= self.total`.</span>
+</span><span id="ProgBar-107"><a href="#ProgBar-107"><span class="linenos">107</span></a>
+</span><span id="ProgBar-108"><a href="#ProgBar-108"><span class="linenos">108</span></a><span class="sd">        Note: if `new_line_after_completion` and `clear_after_completion` are both `True`, the line will be cleared</span>
+</span><span id="ProgBar-109"><a href="#ProgBar-109"><span class="linenos">109</span></a><span class="sd">        then a call to `print()` will be made.&quot;&quot;&quot;</span>
+</span><span id="ProgBar-110"><a href="#ProgBar-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="ProgBar-111"><a href="#ProgBar-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="ProgBar-112"><a href="#ProgBar-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar-113"><a href="#ProgBar-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar-114"><a href="#ProgBar-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="ProgBar-115"><a href="#ProgBar-115"><span class="linenos">115</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="ProgBar-116"><a href="#ProgBar-116"><span class="linenos">116</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="ProgBar-117"><a href="#ProgBar-117"><span class="linenos">117</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="ProgBar-118"><a href="#ProgBar-118"><span class="linenos">118</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
 </span><span id="ProgBar-119"><a href="#ProgBar-119"><span class="linenos">119</span></a>
-</span><span id="ProgBar-120"><a href="#ProgBar-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-121"><a href="#ProgBar-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="ProgBar-122"><a href="#ProgBar-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-123"><a href="#ProgBar-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-124"><a href="#ProgBar-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-125"><a href="#ProgBar-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-126"><a href="#ProgBar-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-127"><a href="#ProgBar-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar-128"><a href="#ProgBar-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar-120"><a href="#ProgBar-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-121"><a href="#ProgBar-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="ProgBar-122"><a href="#ProgBar-122"><span class="linenos">122</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="ProgBar-123"><a href="#ProgBar-123"><span class="linenos">123</span></a>
+</span><span id="ProgBar-124"><a href="#ProgBar-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="ProgBar-125"><a href="#ProgBar-125"><span class="linenos">125</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-126"><a href="#ProgBar-126"><span class="linenos">126</span></a>            <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar-127"><a href="#ProgBar-127"><span class="linenos">127</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="ProgBar-128"><a href="#ProgBar-128"><span class="linenos">128</span></a>            <span class="nb">print</span><span class="p">()</span>
 </span><span id="ProgBar-129"><a href="#ProgBar-129"><span class="linenos">129</span></a>
-</span><span id="ProgBar-130"><a href="#ProgBar-130"><span class="linenos">130</span></a>    <span class="nd">@property</span>
-</span><span id="ProgBar-131"><a href="#ProgBar-131"><span class="linenos">131</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="ProgBar-132"><a href="#ProgBar-132"><span class="linenos">132</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="ProgBar-133"><a href="#ProgBar-133"><span class="linenos">133</span></a>
-</span><span id="ProgBar-134"><a href="#ProgBar-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="ProgBar-135"><a href="#ProgBar-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="ProgBar-136"><a href="#ProgBar-136"><span class="linenos">136</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="ProgBar-137"><a href="#ProgBar-137"><span class="linenos">137</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="ProgBar-138"><a href="#ProgBar-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar-139"><a href="#ProgBar-139"><span class="linenos">139</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="ProgBar-140"><a href="#ProgBar-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar-141"><a href="#ProgBar-141"><span class="linenos">141</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="ProgBar-142"><a href="#ProgBar-142"><span class="linenos">142</span></a>        <span class="k">return</span> <span class="n">percent</span>
-</span><span id="ProgBar-143"><a href="#ProgBar-143"><span class="linenos">143</span></a>
-</span><span id="ProgBar-144"><a href="#ProgBar-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-145"><a href="#ProgBar-145"><span class="linenos">145</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
-</span><span id="ProgBar-146"><a href="#ProgBar-146"><span class="linenos">146</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
-</span><span id="ProgBar-147"><a href="#ProgBar-147"><span class="linenos">147</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
-</span><span id="ProgBar-148"><a href="#ProgBar-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
-</span><span id="ProgBar-149"><a href="#ProgBar-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
-</span><span id="ProgBar-150"><a href="#ProgBar-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
-</span><span id="ProgBar-151"><a href="#ProgBar-151"><span class="linenos">151</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_bar</span><span class="p">()</span>
-</span><span id="ProgBar-152"><a href="#ProgBar-152"><span class="linenos">152</span></a>
-</span><span id="ProgBar-153"><a href="#ProgBar-153"><span class="linenos">153</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-154"><a href="#ProgBar-154"><span class="linenos">154</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
-</span><span id="ProgBar-155"><a href="#ProgBar-155"><span class="linenos">155</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar-156"><a href="#ProgBar-156"><span class="linenos">156</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
-</span><span id="ProgBar-157"><a href="#ProgBar-157"><span class="linenos">157</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar-158"><a href="#ProgBar-158"><span class="linenos">158</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
-</span><span id="ProgBar-159"><a href="#ProgBar-159"><span class="linenos">159</span></a>
-</span><span id="ProgBar-160"><a href="#ProgBar-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar-161"><a href="#ProgBar-161"><span class="linenos">161</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="ProgBar-162"><a href="#ProgBar-162"><span class="linenos">162</span></a>
-</span><span id="ProgBar-163"><a href="#ProgBar-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="ProgBar-164"><a href="#ProgBar-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar-165"><a href="#ProgBar-165"><span class="linenos">165</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-166"><a href="#ProgBar-166"><span class="linenos">166</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar-167"><a href="#ProgBar-167"><span class="linenos">167</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-168"><a href="#ProgBar-168"><span class="linenos">168</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-169"><a href="#ProgBar-169"><span class="linenos">169</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar-170"><a href="#ProgBar-170"><span class="linenos">170</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="ProgBar-171"><a href="#ProgBar-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="ProgBar-172"><a href="#ProgBar-172"><span class="linenos">172</span></a>
-</span><span id="ProgBar-173"><a href="#ProgBar-173"><span class="linenos">173</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="ProgBar-174"><a href="#ProgBar-174"><span class="linenos">174</span></a>
-</span><span id="ProgBar-175"><a href="#ProgBar-175"><span class="linenos">175</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="ProgBar-176"><a href="#ProgBar-176"><span class="linenos">176</span></a>
-</span><span id="ProgBar-177"><a href="#ProgBar-177"><span class="linenos">177</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
-</span><span id="ProgBar-178"><a href="#ProgBar-178"><span class="linenos">178</span></a>
-</span><span id="ProgBar-179"><a href="#ProgBar-179"><span class="linenos">179</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="ProgBar-180"><a href="#ProgBar-180"><span class="linenos">180</span></a>
-</span><span id="ProgBar-181"><a href="#ProgBar-181"><span class="linenos">181</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="ProgBar-182"><a href="#ProgBar-182"><span class="linenos">182</span></a>
-</span><span id="ProgBar-183"><a href="#ProgBar-183"><span class="linenos">183</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="ProgBar-184"><a href="#ProgBar-184"><span class="linenos">184</span></a>
-</span><span id="ProgBar-185"><a href="#ProgBar-185"><span class="linenos">185</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar-186"><a href="#ProgBar-186"><span class="linenos">186</span></a>
-</span><span id="ProgBar-187"><a href="#ProgBar-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
-</span><span id="ProgBar-188"><a href="#ProgBar-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
-</span><span id="ProgBar-189"><a href="#ProgBar-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
-</span><span id="ProgBar-190"><a href="#ProgBar-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
-</span><span id="ProgBar-191"><a href="#ProgBar-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
-</span><span id="ProgBar-192"><a href="#ProgBar-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
-</span><span id="ProgBar-193"><a href="#ProgBar-193"><span class="linenos">193</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
-</span><span id="ProgBar-194"><a href="#ProgBar-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="ProgBar-195"><a href="#ProgBar-195"><span class="linenos">195</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="ProgBar-196"><a href="#ProgBar-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ProgBar-197"><a href="#ProgBar-197"><span class="linenos">197</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="ProgBar-198"><a href="#ProgBar-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="ProgBar-199"><a href="#ProgBar-199"><span class="linenos">199</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="ProgBar-200"><a href="#ProgBar-200"><span class="linenos">200</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="ProgBar-201"><a href="#ProgBar-201"><span class="linenos">201</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar-202"><a href="#ProgBar-202"><span class="linenos">202</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar-203"><a href="#ProgBar-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar-204"><a href="#ProgBar-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="ProgBar-205"><a href="#ProgBar-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="ProgBar-206"><a href="#ProgBar-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar-207"><a href="#ProgBar-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="ProgBar-208"><a href="#ProgBar-208"><span class="linenos">208</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="ProgBar-209"><a href="#ProgBar-209"><span class="linenos">209</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="ProgBar-210"><a href="#ProgBar-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ProgBar-211"><a href="#ProgBar-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="ProgBar-212"><a href="#ProgBar-212"><span class="linenos">212</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="ProgBar-213"><a href="#ProgBar-213"><span class="linenos">213</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
-</span><span id="ProgBar-214"><a href="#ProgBar-214"><span class="linenos">214</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar-215"><a href="#ProgBar-215"><span class="linenos">215</span></a>                    <span class="n">clear</span><span class="p">()</span>
-</span><span id="ProgBar-216"><a href="#ProgBar-216"><span class="linenos">216</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar-217"><a href="#ProgBar-217"><span class="linenos">217</span></a>                    <span class="nb">print</span><span class="p">()</span>
-</span><span id="ProgBar-218"><a href="#ProgBar-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar-219"><a href="#ProgBar-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+</span><span id="ProgBar-130"><a href="#ProgBar-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-131"><a href="#ProgBar-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="ProgBar-132"><a href="#ProgBar-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-133"><a href="#ProgBar-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-134"><a href="#ProgBar-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-135"><a href="#ProgBar-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-136"><a href="#ProgBar-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar-137"><a href="#ProgBar-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar-138"><a href="#ProgBar-138"><span class="linenos">138</span></a>
+</span><span id="ProgBar-139"><a href="#ProgBar-139"><span class="linenos">139</span></a>    <span class="nd">@property</span>
+</span><span id="ProgBar-140"><a href="#ProgBar-140"><span class="linenos">140</span></a>    <span class="k">def</span> <span class="nf">runtime</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar-141"><a href="#ProgBar-141"><span class="linenos">141</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;runtime:</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="ProgBar-142"><a href="#ProgBar-142"><span class="linenos">142</span></a>
+</span><span id="ProgBar-143"><a href="#ProgBar-143"><span class="linenos">143</span></a>    <span class="nd">@property</span>
+</span><span id="ProgBar-144"><a href="#ProgBar-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">bar</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar-145"><a href="#ProgBar-145"><span class="linenos">145</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="ProgBar-146"><a href="#ProgBar-146"><span class="linenos">146</span></a>
+</span><span id="ProgBar-147"><a href="#ProgBar-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar-148"><a href="#ProgBar-148"><span class="linenos">148</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage completed to two decimal places as a string without the `%`.&quot;&quot;&quot;</span>
+</span><span id="ProgBar-149"><a href="#ProgBar-149"><span class="linenos">149</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="ProgBar-150"><a href="#ProgBar-150"><span class="linenos">150</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar-151"><a href="#ProgBar-151"><span class="linenos">151</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="ProgBar-152"><a href="#ProgBar-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar-153"><a href="#ProgBar-153"><span class="linenos">153</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="ProgBar-154"><a href="#ProgBar-154"><span class="linenos">154</span></a>        <span class="k">return</span> <span class="n">percent</span>
+</span><span id="ProgBar-155"><a href="#ProgBar-155"><span class="linenos">155</span></a>
+</span><span id="ProgBar-156"><a href="#ProgBar-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">_prepare_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-157"><a href="#ProgBar-157"><span class="linenos">157</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">-</span> <span class="mi">1</span>
+</span><span id="ProgBar-158"><a href="#ProgBar-158"><span class="linenos">158</span></a>        <span class="n">bar_length</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="ProgBar-159"><a href="#ProgBar-159"><span class="linenos">159</span></a>        <span class="n">progress</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">bar_length</span> <span class="o">*</span> <span class="nb">min</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mf">1.0</span><span class="p">))</span>
+</span><span id="ProgBar-160"><a href="#ProgBar-160"><span class="linenos">160</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">*</span> <span class="n">progress</span>
+</span><span id="ProgBar-161"><a href="#ProgBar-161"><span class="linenos">161</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">*</span> <span class="p">(</span><span class="n">bar_length</span> <span class="o">-</span> <span class="n">progress</span><span class="p">)</span>
+</span><span id="ProgBar-162"><a href="#ProgBar-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_percent</span><span class="p">()</span>
+</span><span id="ProgBar-163"><a href="#ProgBar-163"><span class="linenos">163</span></a>
+</span><span id="ProgBar-164"><a href="#ProgBar-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">_trim_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-165"><a href="#ProgBar-165"><span class="linenos">165</span></a>        <span class="n">original_width</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span>
+</span><span id="ProgBar-166"><a href="#ProgBar-166"><span class="linenos">166</span></a>        <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">)</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-167"><a href="#ProgBar-167"><span class="linenos">167</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">-=</span> <span class="mf">0.01</span>
+</span><span id="ProgBar-168"><a href="#ProgBar-168"><span class="linenos">168</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar-169"><a href="#ProgBar-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">original_width</span>
+</span><span id="ProgBar-170"><a href="#ProgBar-170"><span class="linenos">170</span></a>
+</span><span id="ProgBar-171"><a href="#ProgBar-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar-172"><a href="#ProgBar-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="ProgBar-173"><a href="#ProgBar-173"><span class="linenos">173</span></a>
+</span><span id="ProgBar-174"><a href="#ProgBar-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="ProgBar-175"><a href="#ProgBar-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar-176"><a href="#ProgBar-176"><span class="linenos">176</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-177"><a href="#ProgBar-177"><span class="linenos">177</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar-178"><a href="#ProgBar-178"><span class="linenos">178</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-179"><a href="#ProgBar-179"><span class="linenos">179</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-180"><a href="#ProgBar-180"><span class="linenos">180</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar-181"><a href="#ProgBar-181"><span class="linenos">181</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="ProgBar-182"><a href="#ProgBar-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="ProgBar-183"><a href="#ProgBar-183"><span class="linenos">183</span></a>
+</span><span id="ProgBar-184"><a href="#ProgBar-184"><span class="linenos">184</span></a><span class="sd">        #### :params:</span>
+</span><span id="ProgBar-185"><a href="#ProgBar-185"><span class="linenos">185</span></a>
+</span><span id="ProgBar-186"><a href="#ProgBar-186"><span class="linenos">186</span></a><span class="sd">        `prefix`: String affixed to the front of the progress bar.</span>
+</span><span id="ProgBar-187"><a href="#ProgBar-187"><span class="linenos">187</span></a>
+</span><span id="ProgBar-188"><a href="#ProgBar-188"><span class="linenos">188</span></a><span class="sd">        `suffix`: String appended to the end of the progress bar.</span>
+</span><span id="ProgBar-189"><a href="#ProgBar-189"><span class="linenos">189</span></a>
+</span><span id="ProgBar-190"><a href="#ProgBar-190"><span class="linenos">190</span></a><span class="sd">        `counter_override`: When an externally incremented completion counter is needed.</span>
+</span><span id="ProgBar-191"><a href="#ProgBar-191"><span class="linenos">191</span></a>
+</span><span id="ProgBar-192"><a href="#ProgBar-192"><span class="linenos">192</span></a><span class="sd">        `total_override`: When an externally controlled bar total is needed.</span>
+</span><span id="ProgBar-193"><a href="#ProgBar-193"><span class="linenos">193</span></a>
+</span><span id="ProgBar-194"><a href="#ProgBar-194"><span class="linenos">194</span></a><span class="sd">        `return_object`: An object to be returned by display().</span>
+</span><span id="ProgBar-195"><a href="#ProgBar-195"><span class="linenos">195</span></a><span class="sd">        Allows `display()` to be called within a comprehension:</span>
+</span><span id="ProgBar-196"><a href="#ProgBar-196"><span class="linenos">196</span></a>
+</span><span id="ProgBar-197"><a href="#ProgBar-197"><span class="linenos">197</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar-198"><a href="#ProgBar-198"><span class="linenos">198</span></a>
+</span><span id="ProgBar-199"><a href="#ProgBar-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="ProgBar-200"><a href="#ProgBar-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="ProgBar-201"><a href="#ProgBar-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="ProgBar-202"><a href="#ProgBar-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="ProgBar-203"><a href="#ProgBar-203"><span class="linenos">203</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="ProgBar-204"><a href="#ProgBar-204"><span class="linenos">204</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="ProgBar-205"><a href="#ProgBar-205"><span class="linenos">205</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="ProgBar-206"><a href="#ProgBar-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="ProgBar-207"><a href="#ProgBar-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar-208"><a href="#ProgBar-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ProgBar-209"><a href="#ProgBar-209"><span class="linenos">209</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="ProgBar-210"><a href="#ProgBar-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="ProgBar-211"><a href="#ProgBar-211"><span class="linenos">211</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="ProgBar-212"><a href="#ProgBar-212"><span class="linenos">212</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="ProgBar-213"><a href="#ProgBar-213"><span class="linenos">213</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-214"><a href="#ProgBar-214"><span class="linenos">214</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar-215"><a href="#ProgBar-215"><span class="linenos">215</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="ProgBar-216"><a href="#ProgBar-216"><span class="linenos">216</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar-217"><a href="#ProgBar-217"><span class="linenos">217</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="ProgBar-218"><a href="#ProgBar-218"><span class="linenos">218</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="ProgBar-219"><a href="#ProgBar-219"><span class="linenos">219</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar-220"><a href="#ProgBar-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="ProgBar-221"><a href="#ProgBar-221"><span class="linenos">221</span></a>                <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="ProgBar-222"><a href="#ProgBar-222"><span class="linenos">222</span></a>                <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="ProgBar-223"><a href="#ProgBar-223"><span class="linenos">223</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ProgBar-224"><a href="#ProgBar-224"><span class="linenos">224</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="ProgBar-225"><a href="#ProgBar-225"><span class="linenos">225</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="ProgBar-226"><a href="#ProgBar-226"><span class="linenos">226</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="ProgBar-227"><a href="#ProgBar-227"><span class="linenos">227</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-228"><a href="#ProgBar-228"><span class="linenos">228</span></a>                        <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar-229"><a href="#ProgBar-229"><span class="linenos">229</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar-230"><a href="#ProgBar-230"><span class="linenos">230</span></a>                        <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar-231"><a href="#ProgBar-231"><span class="linenos">231</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar-232"><a href="#ProgBar-232"><span class="linenos">232</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="ProgBar-233"><a href="#ProgBar-233"><span class="linenos">233</span></a>            <span class="o">...</span>
+</span><span id="ProgBar-234"><a href="#ProgBar-234"><span class="linenos">234</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="ProgBar-235"><a href="#ProgBar-235"><span class="linenos">235</span></a>            <span class="k">raise</span> <span class="n">e</span>
+</span><span id="ProgBar-236"><a href="#ProgBar-236"><span class="linenos">236</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Self incrementing, dynamically sized progress bar.</p>
 
-<p>Includes an internal timer that starts when this object is created.
-It can be easily added to the progress bar display by adding
-the 'runtime' property to display's prefix or suffix param:</p>
+<p>Includes an internal timer that starts when this object is created.</p>
+
+<p>Easily add runtime to progress display:</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="n">total</span><span class="o">=</span><span class="mi">100</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mi">30</span><span class="p">)</span>
-<span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">prefix</span><span class="o">=</span><span class="n">bar</span><span class="o">.</span><span class="n">runtime</span><span class="p">)</span>
-<span class="gp">&gt;&gt;&gt; </span><span class="s2">&quot;runtime: 30s [_///////////////////]1.00%&quot;</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">prefix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Doin stuff ~ </span><span class="si">{</span><span class="n">bar</span><span class="o">.</span><span class="n">runtime</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="s2">&quot;Doin stuff ~ runtime: 30s [_///////////////////]-1.00%&quot;</span>
 </code></pre>
 </div>
 </div>
 
 
                             <div id="ProgBar.__init__" class="classattr">
                                         <input id="ProgBar.__init__-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
-        <span class="name">ProgBar</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">total</span><span class="p">:</span> <span class="nb">float</span>,</span><span class="param">	<span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span>,</span><span class="param">	<span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;_&#39;</span>,</span><span class="param">	<span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;/&#39;</span>,</span><span class="param">	<span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span>,</span><span class="param">	<span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
+        <span class="name">ProgBar</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">total</span><span class="p">:</span> <span class="nb">float</span>,</span><span class="param">	<span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span>,</span><span class="param">	<span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;_&#39;</span>,</span><span class="param">	<span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;/&#39;</span>,</span><span class="param">	<span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.5</span>,</span><span class="param">	<span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>,</span><span class="param">	<span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span>)</span>
 
                 <label class="view-source-button" for="ProgBar.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.__init__-66"><a href="#ProgBar.__init__-66"><span class="linenos"> 66</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="ProgBar.__init__-67"><a href="#ProgBar.__init__-67"><span class="linenos"> 67</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-68"><a href="#ProgBar.__init__-68"><span class="linenos"> 68</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-69"><a href="#ProgBar.__init__-69"><span class="linenos"> 69</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-70"><a href="#ProgBar.__init__-70"><span class="linenos"> 70</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-71"><a href="#ProgBar.__init__-71"><span class="linenos"> 71</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-72"><a href="#ProgBar.__init__-72"><span class="linenos"> 72</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-73"><a href="#ProgBar.__init__-73"><span class="linenos"> 73</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-74"><a href="#ProgBar.__init__-74"><span class="linenos"> 74</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-</span><span id="ProgBar.__init__-75"><a href="#ProgBar.__init__-75"><span class="linenos"> 75</span></a>    <span class="p">):</span>
-</span><span id="ProgBar.__init__-76"><a href="#ProgBar.__init__-76"><span class="linenos"> 76</span></a>        <span class="sd">&quot;&quot;&quot;:param total: The number of calls to reach 100% completion.</span>
-</span><span id="ProgBar.__init__-77"><a href="#ProgBar.__init__-77"><span class="linenos"> 77</span></a>
-</span><span id="ProgBar.__init__-78"><a href="#ProgBar.__init__-78"><span class="linenos"> 78</span></a><span class="sd">        :param update_frequency: The progress bar will only update once every this number of calls to display().</span>
-</span><span id="ProgBar.__init__-79"><a href="#ProgBar.__init__-79"><span class="linenos"> 79</span></a><span class="sd">        The larger the value, the less performance impact ProgBar has on the loop in which it is called.</span>
-</span><span id="ProgBar.__init__-80"><a href="#ProgBar.__init__-80"><span class="linenos"> 80</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar.__init__-81"><a href="#ProgBar.__init__-81"><span class="linenos"> 81</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
-</span><span id="ProgBar.__init__-82"><a href="#ProgBar.__init__-82"><span class="linenos"> 82</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
-</span><span id="ProgBar.__init__-83"><a href="#ProgBar.__init__-83"><span class="linenos"> 83</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
-</span><span id="ProgBar.__init__-84"><a href="#ProgBar.__init__-84"><span class="linenos"> 84</span></a>
-</span><span id="ProgBar.__init__-85"><a href="#ProgBar.__init__-85"><span class="linenos"> 85</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
-</span><span id="ProgBar.__init__-86"><a href="#ProgBar.__init__-86"><span class="linenos"> 86</span></a><span class="sd">        Note: If &#39;total&#39; is not a multiple of &#39;update_frequency&#39;, the display will not show 100% completion when the loop finishes.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.__init__-73"><a href="#ProgBar.__init__-73"><span class="linenos"> 73</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="ProgBar.__init__-74"><a href="#ProgBar.__init__-74"><span class="linenos"> 74</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-75"><a href="#ProgBar.__init__-75"><span class="linenos"> 75</span></a>        <span class="n">total</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-76"><a href="#ProgBar.__init__-76"><span class="linenos"> 76</span></a>        <span class="n">update_frequency</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">1</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-77"><a href="#ProgBar.__init__-77"><span class="linenos"> 77</span></a>        <span class="n">fill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;_&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-78"><a href="#ProgBar.__init__-78"><span class="linenos"> 78</span></a>        <span class="n">unfill_ch</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;/&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-79"><a href="#ProgBar.__init__-79"><span class="linenos"> 79</span></a>        <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.5</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-80"><a href="#ProgBar.__init__-80"><span class="linenos"> 80</span></a>        <span class="n">new_line_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-81"><a href="#ProgBar.__init__-81"><span class="linenos"> 81</span></a>        <span class="n">clear_after_completion</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+</span><span id="ProgBar.__init__-82"><a href="#ProgBar.__init__-82"><span class="linenos"> 82</span></a>    <span class="p">):</span>
+</span><span id="ProgBar.__init__-83"><a href="#ProgBar.__init__-83"><span class="linenos"> 83</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="ProgBar.__init__-84"><a href="#ProgBar.__init__-84"><span class="linenos"> 84</span></a><span class="sd">        #### :params:</span>
+</span><span id="ProgBar.__init__-85"><a href="#ProgBar.__init__-85"><span class="linenos"> 85</span></a>
+</span><span id="ProgBar.__init__-86"><a href="#ProgBar.__init__-86"><span class="linenos"> 86</span></a><span class="sd">        `total`: The number of calls to reach 100% completion.</span>
 </span><span id="ProgBar.__init__-87"><a href="#ProgBar.__init__-87"><span class="linenos"> 87</span></a>
-</span><span id="ProgBar.__init__-88"><a href="#ProgBar.__init__-88"><span class="linenos"> 88</span></a><span class="sd">        :param fill_ch: The character used to represent the completed part of the bar.</span>
-</span><span id="ProgBar.__init__-89"><a href="#ProgBar.__init__-89"><span class="linenos"> 89</span></a>
-</span><span id="ProgBar.__init__-90"><a href="#ProgBar.__init__-90"><span class="linenos"> 90</span></a><span class="sd">        :param unfill_ch: The character used to represent the uncompleted part of the bar.</span>
-</span><span id="ProgBar.__init__-91"><a href="#ProgBar.__init__-91"><span class="linenos"> 91</span></a>
-</span><span id="ProgBar.__init__-92"><a href="#ProgBar.__init__-92"><span class="linenos"> 92</span></a><span class="sd">        :param width_ratio: The width of the progress bar relative to the width of the terminal window.</span>
-</span><span id="ProgBar.__init__-93"><a href="#ProgBar.__init__-93"><span class="linenos"> 93</span></a>
-</span><span id="ProgBar.__init__-94"><a href="#ProgBar.__init__-94"><span class="linenos"> 94</span></a><span class="sd">        :param new_line_after_completion: Make a call to print() once self.counter &gt;= self.total.</span>
-</span><span id="ProgBar.__init__-95"><a href="#ProgBar.__init__-95"><span class="linenos"> 95</span></a>
-</span><span id="ProgBar.__init__-96"><a href="#ProgBar.__init__-96"><span class="linenos"> 96</span></a><span class="sd">        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter &gt;= self.total.</span>
+</span><span id="ProgBar.__init__-88"><a href="#ProgBar.__init__-88"><span class="linenos"> 88</span></a><span class="sd">        `update_frequency`: The progress bar will only update once every this number of calls to `display()`.</span>
+</span><span id="ProgBar.__init__-89"><a href="#ProgBar.__init__-89"><span class="linenos"> 89</span></a><span class="sd">        The larger the value, the less performance impact `ProgBar` has on the loop in which it is called.</span>
+</span><span id="ProgBar.__init__-90"><a href="#ProgBar.__init__-90"><span class="linenos"> 90</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar.__init__-91"><a href="#ProgBar.__init__-91"><span class="linenos"> 91</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(100, update_frequency=10)</span>
+</span><span id="ProgBar.__init__-92"><a href="#ProgBar.__init__-92"><span class="linenos"> 92</span></a><span class="sd">        &gt;&gt;&gt; for _ in range(100):</span>
+</span><span id="ProgBar.__init__-93"><a href="#ProgBar.__init__-93"><span class="linenos"> 93</span></a><span class="sd">        &gt;&gt;&gt;     bar.display()</span>
+</span><span id="ProgBar.__init__-94"><a href="#ProgBar.__init__-94"><span class="linenos"> 94</span></a>
+</span><span id="ProgBar.__init__-95"><a href="#ProgBar.__init__-95"><span class="linenos"> 95</span></a><span class="sd">        ^The progress bar in the terminal will only update once every ten calls, going from 0%-&gt;100% in 10% increments.</span>
+</span><span id="ProgBar.__init__-96"><a href="#ProgBar.__init__-96"><span class="linenos"> 96</span></a><span class="sd">        Note: If `total` is not a multiple of `update_frequency`, the display will not show 100% completion when the loop finishes.</span>
 </span><span id="ProgBar.__init__-97"><a href="#ProgBar.__init__-97"><span class="linenos"> 97</span></a>
-</span><span id="ProgBar.__init__-98"><a href="#ProgBar.__init__-98"><span class="linenos"> 98</span></a><span class="sd">        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared</span>
-</span><span id="ProgBar.__init__-99"><a href="#ProgBar.__init__-99"><span class="linenos"> 99</span></a><span class="sd">        then a call to print() will be made.&quot;&quot;&quot;</span>
-</span><span id="ProgBar.__init__-100"><a href="#ProgBar.__init__-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
-</span><span id="ProgBar.__init__-101"><a href="#ProgBar.__init__-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
-</span><span id="ProgBar.__init__-102"><a href="#ProgBar.__init__-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar.__init__-103"><a href="#ProgBar.__init__-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="ProgBar.__init__-104"><a href="#ProgBar.__init__-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="ProgBar.__init__-105"><a href="#ProgBar.__init__-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
-</span><span id="ProgBar.__init__-106"><a href="#ProgBar.__init__-106"><span class="linenos">106</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
-</span><span id="ProgBar.__init__-107"><a href="#ProgBar.__init__-107"><span class="linenos">107</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
-</span><span id="ProgBar.__init__-108"><a href="#ProgBar.__init__-108"><span class="linenos">108</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="ProgBar.__init__-98"><a href="#ProgBar.__init__-98"><span class="linenos"> 98</span></a><span class="sd">        `fill_ch`: The character used to represent the completed part of the bar.</span>
+</span><span id="ProgBar.__init__-99"><a href="#ProgBar.__init__-99"><span class="linenos"> 99</span></a>
+</span><span id="ProgBar.__init__-100"><a href="#ProgBar.__init__-100"><span class="linenos">100</span></a><span class="sd">        `unfill_ch`: The character used to represent the incomplete part of the bar.</span>
+</span><span id="ProgBar.__init__-101"><a href="#ProgBar.__init__-101"><span class="linenos">101</span></a>
+</span><span id="ProgBar.__init__-102"><a href="#ProgBar.__init__-102"><span class="linenos">102</span></a><span class="sd">        `width_ratio`: The width of the progress bar relative to the width of the terminal window.</span>
+</span><span id="ProgBar.__init__-103"><a href="#ProgBar.__init__-103"><span class="linenos">103</span></a>
+</span><span id="ProgBar.__init__-104"><a href="#ProgBar.__init__-104"><span class="linenos">104</span></a><span class="sd">        `new_line_after_completion`: Make a call to `print()` once `self.counter &gt;= self.total`.</span>
+</span><span id="ProgBar.__init__-105"><a href="#ProgBar.__init__-105"><span class="linenos">105</span></a>
+</span><span id="ProgBar.__init__-106"><a href="#ProgBar.__init__-106"><span class="linenos">106</span></a><span class="sd">        `clear_after_completion`: Make a call to `printbuddies.clear()` once `self.counter &gt;= self.total`.</span>
+</span><span id="ProgBar.__init__-107"><a href="#ProgBar.__init__-107"><span class="linenos">107</span></a>
+</span><span id="ProgBar.__init__-108"><a href="#ProgBar.__init__-108"><span class="linenos">108</span></a><span class="sd">        Note: if `new_line_after_completion` and `clear_after_completion` are both `True`, the line will be cleared</span>
+</span><span id="ProgBar.__init__-109"><a href="#ProgBar.__init__-109"><span class="linenos">109</span></a><span class="sd">        then a call to `print()` will be made.&quot;&quot;&quot;</span>
+</span><span id="ProgBar.__init__-110"><a href="#ProgBar.__init__-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total</span>
+</span><span id="ProgBar.__init__-111"><a href="#ProgBar.__init__-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">=</span> <span class="n">update_frequency</span>
+</span><span id="ProgBar.__init__-112"><a href="#ProgBar.__init__-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">fill_ch</span> <span class="o">=</span> <span class="n">fill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar.__init__-113"><a href="#ProgBar.__init__-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfill_ch</span> <span class="o">=</span> <span class="n">unfill_ch</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="ProgBar.__init__-114"><a href="#ProgBar.__init__-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="ProgBar.__init__-115"><a href="#ProgBar.__init__-115"><span class="linenos">115</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span> <span class="o">=</span> <span class="n">new_line_after_completion</span>
+</span><span id="ProgBar.__init__-116"><a href="#ProgBar.__init__-116"><span class="linenos">116</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span> <span class="o">=</span> <span class="n">clear_after_completion</span>
+</span><span id="ProgBar.__init__-117"><a href="#ProgBar.__init__-117"><span class="linenos">117</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">reset</span><span class="p">()</span>
+</span><span id="ProgBar.__init__-118"><a href="#ProgBar.__init__-118"><span class="linenos">118</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span> <span class="o">=</span> <span class="kc">False</span>
 </span></pre></div>
 
 
-            <div class="docstring"><h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><p><strong>total</strong>:  The number of calls to reach 100% completion.</p></li>
-<li><p><strong>update_frequency</strong>:  The progress bar will only update once every this number of calls to display().
-The larger the value, the less performance impact ProgBar has on the loop in which it is called.
+            <div class="docstring"><h4 id="params">:params:</h4>
+
+<p><code>total</code>: The number of calls to reach 100% completion.</p>
+
+<p><code>update_frequency</code>: The progress bar will only update once every this number of calls to <code><a href="#ProgBar.display">display()</a></code>.
+The larger the value, the less performance impact <code><a href="#ProgBar">ProgBar</a></code> has on the loop in which it is called.
 e.g.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="mi">100</span><span class="p">,</span> <span class="n">update_frequency</span><span class="o">=</span><span class="mi">10</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">100</span><span class="p">):</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
 </code></pre>
-</div></li>
-</ul>
+</div>
 
 <p>^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.
-Note: If 'total' is not a multiple of 'update_frequency', the display will not show 100% completion when the loop finishes.</p>
+Note: If <code>total</code> is not a multiple of <code>update_frequency</code>, the display will not show 100% completion when the loop finishes.</p>
+
+<p><code>fill_ch</code>: The character used to represent the completed part of the bar.</p>
 
-<ul>
-<li><p><strong>fill_ch</strong>:  The character used to represent the completed part of the bar.</p></li>
-<li><p><strong>unfill_ch</strong>:  The character used to represent the uncompleted part of the bar.</p></li>
-<li><p><strong>width_ratio</strong>:  The width of the progress bar relative to the width of the terminal window.</p></li>
-<li><p><strong>new_line_after_completion</strong>:  Make a call to print() once self.counter &gt;= self.total.</p></li>
-<li><p><strong>clear_after_completion</strong>:  Make a call to printbuddies.clear() once self.counter &gt;= self.total.</p></li>
-</ul>
+<p><code>unfill_ch</code>: The character used to represent the incomplete part of the bar.</p>
 
-<p>Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared
-then a call to print() will be made.</p>
+<p><code>width_ratio</code>: The width of the progress bar relative to the width of the terminal window.</p>
+
+<p><code>new_line_after_completion</code>: Make a call to <code>print()</code> once <code>self.counter &gt;= self.total</code>.</p>
+
+<p><code>clear_after_completion</code>: Make a call to <code>printbuddies.clear()</code> once <code>self.counter &gt;= self.total</code>.</p>
+
+<p>Note: if <code>new_line_after_completion</code> and <code>clear_after_completion</code> are both <code>True</code>, the line will be cleared
+then a call to <code>print()</code> will be made.</p>
 </div>
 
 
                             </div>
                             <div id="ProgBar.reset" class="classattr">
                                         <input id="ProgBar.reset-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -789,23 +823,22 @@
         <span class="def">def</span>
         <span class="name">reset</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProgBar.reset-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.reset"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.reset-120"><a href="#ProgBar.reset-120"><span class="linenos">120</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar.reset-121"><a href="#ProgBar.reset-121"><span class="linenos">121</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
-</span><span id="ProgBar.reset-122"><a href="#ProgBar.reset-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-123"><a href="#ProgBar.reset-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-124"><a href="#ProgBar.reset-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-125"><a href="#ProgBar.reset-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-126"><a href="#ProgBar.reset-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-127"><a href="#ProgBar.reset-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">bar</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
-</span><span id="ProgBar.reset-128"><a href="#ProgBar.reset-128"><span class="linenos">128</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.reset-130"><a href="#ProgBar.reset-130"><span class="linenos">130</span></a>    <span class="k">def</span> <span class="nf">reset</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar.reset-131"><a href="#ProgBar.reset-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="mi">1</span>
+</span><span id="ProgBar.reset-132"><a href="#ProgBar.reset-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-133"><a href="#ProgBar.reset-133"><span class="linenos">133</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-134"><a href="#ProgBar.reset-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-135"><a href="#ProgBar.reset-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">filled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-136"><a href="#ProgBar.reset-136"><span class="linenos">136</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
+</span><span id="ProgBar.reset-137"><a href="#ProgBar.reset-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">(</span><span class="n">subsecond_resolution</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ProgBar.get_percent" class="classattr">
@@ -815,28 +848,26 @@
         <span class="def">def</span>
         <span class="name">get_percent</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="ProgBar.get_percent-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.get_percent"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_percent-134"><a href="#ProgBar.get_percent-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-135"><a href="#ProgBar.get_percent-135"><span class="linenos">135</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage complete to two decimal places</span>
-</span><span id="ProgBar.get_percent-136"><a href="#ProgBar.get_percent-136"><span class="linenos">136</span></a><span class="sd">        as a string without the %.&quot;&quot;&quot;</span>
-</span><span id="ProgBar.get_percent-137"><a href="#ProgBar.get_percent-137"><span class="linenos">137</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
-</span><span id="ProgBar.get_percent-138"><a href="#ProgBar.get_percent-138"><span class="linenos">138</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-139"><a href="#ProgBar.get_percent-139"><span class="linenos">139</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
-</span><span id="ProgBar.get_percent-140"><a href="#ProgBar.get_percent-140"><span class="linenos">140</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="ProgBar.get_percent-141"><a href="#ProgBar.get_percent-141"><span class="linenos">141</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
-</span><span id="ProgBar.get_percent-142"><a href="#ProgBar.get_percent-142"><span class="linenos">142</span></a>        <span class="k">return</span> <span class="n">percent</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_percent-147"><a href="#ProgBar.get_percent-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">get_percent</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-148"><a href="#ProgBar.get_percent-148"><span class="linenos">148</span></a>        <span class="sd">&quot;&quot;&quot;Returns the percentage completed to two decimal places as a string without the `%`.&quot;&quot;&quot;</span>
+</span><span id="ProgBar.get_percent-149"><a href="#ProgBar.get_percent-149"><span class="linenos">149</span></a>        <span class="n">percent</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="mf">100.0</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">,</span> <span class="mi">2</span><span class="p">))</span>
+</span><span id="ProgBar.get_percent-150"><a href="#ProgBar.get_percent-150"><span class="linenos">150</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">1</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-151"><a href="#ProgBar.get_percent-151"><span class="linenos">151</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="n">percent</span> <span class="o">+</span> <span class="s2">&quot;0&quot;</span>
+</span><span id="ProgBar.get_percent-152"><a href="#ProgBar.get_percent-152"><span class="linenos">152</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">percent</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">])</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="ProgBar.get_percent-153"><a href="#ProgBar.get_percent-153"><span class="linenos">153</span></a>            <span class="n">percent</span> <span class="o">=</span> <span class="s2">&quot;0&quot;</span> <span class="o">+</span> <span class="n">percent</span>
+</span><span id="ProgBar.get_percent-154"><a href="#ProgBar.get_percent-154"><span class="linenos">154</span></a>        <span class="k">return</span> <span class="n">percent</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Returns the percentage complete to two decimal places
-as a string without the %.</p>
+            <div class="docstring"><p>Returns the percentage completed to two decimal places as a string without the <code>%</code>.</p>
 </div>
 
 
                             </div>
                             <div id="ProgBar.get_bar" class="classattr">
                                         <input id="ProgBar.get_bar-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -844,16 +875,16 @@
         <span class="def">def</span>
         <span class="name">get_bar</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProgBar.get_bar-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.get_bar"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_bar-160"><a href="#ProgBar.get_bar-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="ProgBar.get_bar-161"><a href="#ProgBar.get_bar-161"><span class="linenos">161</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.get_bar-171"><a href="#ProgBar.get_bar-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">get_bar</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="ProgBar.get_bar-172"><a href="#ProgBar.get_bar-172"><span class="linenos">172</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">prefix</span><span class="p">)</span><span class="si">}</span><span class="s2">[</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">filled</span><span class="si">}{</span><span class="bp">self</span><span class="o">.</span><span class="n">unfilled</span><span class="si">}</span><span class="s2">]-</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">percent</span><span class="si">}</span><span class="s2">% </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">suffix</span><span class="si">}</span><span class="s2">&quot;</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ProgBar.display" class="classattr">
@@ -863,87 +894,94 @@
         <span class="def">def</span>
         <span class="name">display</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="bp">self</span>,</span><span class="param">	<span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span>,</span><span class="param">	<span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">return_object</span><span class="p">:</span> <span class="n">typing</span><span class="o">.</span><span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">) -> <span class="n">Any</span>:</span></span>
 
                 <label class="view-source-button" for="ProgBar.display-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProgBar.display"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.display-163"><a href="#ProgBar.display-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
-</span><span id="ProgBar.display-164"><a href="#ProgBar.display-164"><span class="linenos">164</span></a>        <span class="bp">self</span><span class="p">,</span>
-</span><span id="ProgBar.display-165"><a href="#ProgBar.display-165"><span class="linenos">165</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.display-166"><a href="#ProgBar.display-166"><span class="linenos">166</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-</span><span id="ProgBar.display-167"><a href="#ProgBar.display-167"><span class="linenos">167</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-168"><a href="#ProgBar.display-168"><span class="linenos">168</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-169"><a href="#ProgBar.display-169"><span class="linenos">169</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-</span><span id="ProgBar.display-170"><a href="#ProgBar.display-170"><span class="linenos">170</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
-</span><span id="ProgBar.display-171"><a href="#ProgBar.display-171"><span class="linenos">171</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
-</span><span id="ProgBar.display-172"><a href="#ProgBar.display-172"><span class="linenos">172</span></a>
-</span><span id="ProgBar.display-173"><a href="#ProgBar.display-173"><span class="linenos">173</span></a><span class="sd">        :param prefix: String affixed to the front of the progress bar.</span>
-</span><span id="ProgBar.display-174"><a href="#ProgBar.display-174"><span class="linenos">174</span></a>
-</span><span id="ProgBar.display-175"><a href="#ProgBar.display-175"><span class="linenos">175</span></a><span class="sd">        :param suffix: String appended to the end of the progress bar.</span>
-</span><span id="ProgBar.display-176"><a href="#ProgBar.display-176"><span class="linenos">176</span></a>
-</span><span id="ProgBar.display-177"><a href="#ProgBar.display-177"><span class="linenos">177</span></a><span class="sd">        :param counter_override: When an externally incremented completion counter is needed.</span>
-</span><span id="ProgBar.display-178"><a href="#ProgBar.display-178"><span class="linenos">178</span></a>
-</span><span id="ProgBar.display-179"><a href="#ProgBar.display-179"><span class="linenos">179</span></a><span class="sd">        :param total_override: When an externally controlled bar total is needed.</span>
-</span><span id="ProgBar.display-180"><a href="#ProgBar.display-180"><span class="linenos">180</span></a>
-</span><span id="ProgBar.display-181"><a href="#ProgBar.display-181"><span class="linenos">181</span></a><span class="sd">        :param return_object: An object to be returned by display().</span>
-</span><span id="ProgBar.display-182"><a href="#ProgBar.display-182"><span class="linenos">182</span></a>
-</span><span id="ProgBar.display-183"><a href="#ProgBar.display-183"><span class="linenos">183</span></a><span class="sd">        Allows display() to be called within a comprehension:</span>
-</span><span id="ProgBar.display-184"><a href="#ProgBar.display-184"><span class="linenos">184</span></a>
-</span><span id="ProgBar.display-185"><a href="#ProgBar.display-185"><span class="linenos">185</span></a><span class="sd">        e.g.</span>
-</span><span id="ProgBar.display-186"><a href="#ProgBar.display-186"><span class="linenos">186</span></a>
-</span><span id="ProgBar.display-187"><a href="#ProgBar.display-187"><span class="linenos">187</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
-</span><span id="ProgBar.display-188"><a href="#ProgBar.display-188"><span class="linenos">188</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
-</span><span id="ProgBar.display-189"><a href="#ProgBar.display-189"><span class="linenos">189</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
-</span><span id="ProgBar.display-190"><a href="#ProgBar.display-190"><span class="linenos">190</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
-</span><span id="ProgBar.display-191"><a href="#ProgBar.display-191"><span class="linenos">191</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
-</span><span id="ProgBar.display-192"><a href="#ProgBar.display-192"><span class="linenos">192</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
-</span><span id="ProgBar.display-193"><a href="#ProgBar.display-193"><span class="linenos">193</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
-</span><span id="ProgBar.display-194"><a href="#ProgBar.display-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
-</span><span id="ProgBar.display-195"><a href="#ProgBar.display-195"><span class="linenos">195</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
-</span><span id="ProgBar.display-196"><a href="#ProgBar.display-196"><span class="linenos">196</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-</span><span id="ProgBar.display-197"><a href="#ProgBar.display-197"><span class="linenos">197</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
-</span><span id="ProgBar.display-198"><a href="#ProgBar.display-198"><span class="linenos">198</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
-</span><span id="ProgBar.display-199"><a href="#ProgBar.display-199"><span class="linenos">199</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
-</span><span id="ProgBar.display-200"><a href="#ProgBar.display-200"><span class="linenos">200</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
-</span><span id="ProgBar.display-201"><a href="#ProgBar.display-201"><span class="linenos">201</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar.display-202"><a href="#ProgBar.display-202"><span class="linenos">202</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar.display-203"><a href="#ProgBar.display-203"><span class="linenos">203</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="ProgBar.display-204"><a href="#ProgBar.display-204"><span class="linenos">204</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
-</span><span id="ProgBar.display-205"><a href="#ProgBar.display-205"><span class="linenos">205</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
-</span><span id="ProgBar.display-206"><a href="#ProgBar.display-206"><span class="linenos">206</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
-</span><span id="ProgBar.display-207"><a href="#ProgBar.display-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
-</span><span id="ProgBar.display-208"><a href="#ProgBar.display-208"><span class="linenos">208</span></a>            <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
-</span><span id="ProgBar.display-209"><a href="#ProgBar.display-209"><span class="linenos">209</span></a>            <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="ProgBar.display-210"><a href="#ProgBar.display-210"><span class="linenos">210</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="ProgBar.display-211"><a href="#ProgBar.display-211"><span class="linenos">211</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
-</span><span id="ProgBar.display-212"><a href="#ProgBar.display-212"><span class="linenos">212</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
-</span><span id="ProgBar.display-213"><a href="#ProgBar.display-213"><span class="linenos">213</span></a>            <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
-</span><span id="ProgBar.display-214"><a href="#ProgBar.display-214"><span class="linenos">214</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar.display-215"><a href="#ProgBar.display-215"><span class="linenos">215</span></a>                    <span class="n">clear</span><span class="p">()</span>
-</span><span id="ProgBar.display-216"><a href="#ProgBar.display-216"><span class="linenos">216</span></a>                <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
-</span><span id="ProgBar.display-217"><a href="#ProgBar.display-217"><span class="linenos">217</span></a>                    <span class="nb">print</span><span class="p">()</span>
-</span><span id="ProgBar.display-218"><a href="#ProgBar.display-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
-</span><span id="ProgBar.display-219"><a href="#ProgBar.display-219"><span class="linenos">219</span></a>        <span class="k">return</span> <span class="n">return_object</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProgBar.display-174"><a href="#ProgBar.display-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span>
+</span><span id="ProgBar.display-175"><a href="#ProgBar.display-175"><span class="linenos">175</span></a>        <span class="bp">self</span><span class="p">,</span>
+</span><span id="ProgBar.display-176"><a href="#ProgBar.display-176"><span class="linenos">176</span></a>        <span class="n">prefix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.display-177"><a href="#ProgBar.display-177"><span class="linenos">177</span></a>        <span class="n">suffix</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+</span><span id="ProgBar.display-178"><a href="#ProgBar.display-178"><span class="linenos">178</span></a>        <span class="n">counter_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-179"><a href="#ProgBar.display-179"><span class="linenos">179</span></a>        <span class="n">total_override</span><span class="p">:</span> <span class="nb">float</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-180"><a href="#ProgBar.display-180"><span class="linenos">180</span></a>        <span class="n">return_object</span><span class="p">:</span> <span class="n">Any</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+</span><span id="ProgBar.display-181"><a href="#ProgBar.display-181"><span class="linenos">181</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Any</span><span class="p">:</span>
+</span><span id="ProgBar.display-182"><a href="#ProgBar.display-182"><span class="linenos">182</span></a>        <span class="sd">&quot;&quot;&quot;Writes the progress bar to the terminal.</span>
+</span><span id="ProgBar.display-183"><a href="#ProgBar.display-183"><span class="linenos">183</span></a>
+</span><span id="ProgBar.display-184"><a href="#ProgBar.display-184"><span class="linenos">184</span></a><span class="sd">        #### :params:</span>
+</span><span id="ProgBar.display-185"><a href="#ProgBar.display-185"><span class="linenos">185</span></a>
+</span><span id="ProgBar.display-186"><a href="#ProgBar.display-186"><span class="linenos">186</span></a><span class="sd">        `prefix`: String affixed to the front of the progress bar.</span>
+</span><span id="ProgBar.display-187"><a href="#ProgBar.display-187"><span class="linenos">187</span></a>
+</span><span id="ProgBar.display-188"><a href="#ProgBar.display-188"><span class="linenos">188</span></a><span class="sd">        `suffix`: String appended to the end of the progress bar.</span>
+</span><span id="ProgBar.display-189"><a href="#ProgBar.display-189"><span class="linenos">189</span></a>
+</span><span id="ProgBar.display-190"><a href="#ProgBar.display-190"><span class="linenos">190</span></a><span class="sd">        `counter_override`: When an externally incremented completion counter is needed.</span>
+</span><span id="ProgBar.display-191"><a href="#ProgBar.display-191"><span class="linenos">191</span></a>
+</span><span id="ProgBar.display-192"><a href="#ProgBar.display-192"><span class="linenos">192</span></a><span class="sd">        `total_override`: When an externally controlled bar total is needed.</span>
+</span><span id="ProgBar.display-193"><a href="#ProgBar.display-193"><span class="linenos">193</span></a>
+</span><span id="ProgBar.display-194"><a href="#ProgBar.display-194"><span class="linenos">194</span></a><span class="sd">        `return_object`: An object to be returned by display().</span>
+</span><span id="ProgBar.display-195"><a href="#ProgBar.display-195"><span class="linenos">195</span></a><span class="sd">        Allows `display()` to be called within a comprehension:</span>
+</span><span id="ProgBar.display-196"><a href="#ProgBar.display-196"><span class="linenos">196</span></a>
+</span><span id="ProgBar.display-197"><a href="#ProgBar.display-197"><span class="linenos">197</span></a><span class="sd">        e.g.</span>
+</span><span id="ProgBar.display-198"><a href="#ProgBar.display-198"><span class="linenos">198</span></a>
+</span><span id="ProgBar.display-199"><a href="#ProgBar.display-199"><span class="linenos">199</span></a><span class="sd">        &gt;&gt;&gt; bar = ProgBar(10)</span>
+</span><span id="ProgBar.display-200"><a href="#ProgBar.display-200"><span class="linenos">200</span></a><span class="sd">        &gt;&gt;&gt; def square(x: int | float)-&gt;int|float:</span>
+</span><span id="ProgBar.display-201"><a href="#ProgBar.display-201"><span class="linenos">201</span></a><span class="sd">        &gt;&gt;&gt;     return x * x</span>
+</span><span id="ProgBar.display-202"><a href="#ProgBar.display-202"><span class="linenos">202</span></a><span class="sd">        &gt;&gt;&gt; myList = [bar.display(return_object=square(i)) for i in range(10)]</span>
+</span><span id="ProgBar.display-203"><a href="#ProgBar.display-203"><span class="linenos">203</span></a><span class="sd">        &gt;&gt;&gt; &lt;progress bar gets displayed&gt;</span>
+</span><span id="ProgBar.display-204"><a href="#ProgBar.display-204"><span class="linenos">204</span></a><span class="sd">        &gt;&gt;&gt; myList</span>
+</span><span id="ProgBar.display-205"><a href="#ProgBar.display-205"><span class="linenos">205</span></a><span class="sd">        &gt;&gt;&gt; [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]&quot;&quot;&quot;</span>
+</span><span id="ProgBar.display-206"><a href="#ProgBar.display-206"><span class="linenos">206</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">started</span><span class="p">:</span>
+</span><span id="ProgBar.display-207"><a href="#ProgBar.display-207"><span class="linenos">207</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="ProgBar.display-208"><a href="#ProgBar.display-208"><span class="linenos">208</span></a>        <span class="k">if</span> <span class="n">counter_override</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+</span><span id="ProgBar.display-209"><a href="#ProgBar.display-209"><span class="linenos">209</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">=</span> <span class="n">counter_override</span>
+</span><span id="ProgBar.display-210"><a href="#ProgBar.display-210"><span class="linenos">210</span></a>        <span class="k">if</span> <span class="n">total_override</span><span class="p">:</span>
+</span><span id="ProgBar.display-211"><a href="#ProgBar.display-211"><span class="linenos">211</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">=</span> <span class="n">total_override</span>
+</span><span id="ProgBar.display-212"><a href="#ProgBar.display-212"><span class="linenos">212</span></a>        <span class="c1"># Don&#39;t wanna divide by 0 there, pal</span>
+</span><span id="ProgBar.display-213"><a href="#ProgBar.display-213"><span class="linenos">213</span></a>        <span class="k">while</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">&lt;=</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar.display-214"><a href="#ProgBar.display-214"><span class="linenos">214</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">total</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar.display-215"><a href="#ProgBar.display-215"><span class="linenos">215</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="ProgBar.display-216"><a href="#ProgBar.display-216"><span class="linenos">216</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">%</span> <span class="bp">self</span><span class="o">.</span><span class="n">update_frequency</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="ProgBar.display-217"><a href="#ProgBar.display-217"><span class="linenos">217</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">prefix</span> <span class="o">=</span> <span class="n">prefix</span>
+</span><span id="ProgBar.display-218"><a href="#ProgBar.display-218"><span class="linenos">218</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">suffix</span> <span class="o">=</span> <span class="n">suffix</span>
+</span><span id="ProgBar.display-219"><a href="#ProgBar.display-219"><span class="linenos">219</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_prepare_bar</span><span class="p">()</span>
+</span><span id="ProgBar.display-220"><a href="#ProgBar.display-220"><span class="linenos">220</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_trim_bar</span><span class="p">()</span>
+</span><span id="ProgBar.display-221"><a href="#ProgBar.display-221"><span class="linenos">221</span></a>                <span class="n">pad</span> <span class="o">=</span> <span class="s2">&quot; &quot;</span> <span class="o">*</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">terminal_width</span> <span class="o">-</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="p">))</span>
+</span><span id="ProgBar.display-222"><a href="#ProgBar.display-222"><span class="linenos">222</span></a>                <span class="n">width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="ProgBar.display-223"><a href="#ProgBar.display-223"><span class="linenos">223</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">bar</span><span class="si">}{</span><span class="n">pad</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">[:</span> <span class="n">width</span> <span class="o">-</span> <span class="mi">2</span><span class="p">],</span> <span class="n">flush</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">end</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\r</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="ProgBar.display-224"><a href="#ProgBar.display-224"><span class="linenos">224</span></a>            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">&gt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">total</span><span class="p">:</span>
+</span><span id="ProgBar.display-225"><a href="#ProgBar.display-225"><span class="linenos">225</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="ProgBar.display-226"><a href="#ProgBar.display-226"><span class="linenos">226</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">with_context</span><span class="p">:</span>
+</span><span id="ProgBar.display-227"><a href="#ProgBar.display-227"><span class="linenos">227</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">clear_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar.display-228"><a href="#ProgBar.display-228"><span class="linenos">228</span></a>                        <span class="n">clear</span><span class="p">()</span>
+</span><span id="ProgBar.display-229"><a href="#ProgBar.display-229"><span class="linenos">229</span></a>                    <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">new_line_after_completion</span><span class="p">:</span>
+</span><span id="ProgBar.display-230"><a href="#ProgBar.display-230"><span class="linenos">230</span></a>                        <span class="nb">print</span><span class="p">()</span>
+</span><span id="ProgBar.display-231"><a href="#ProgBar.display-231"><span class="linenos">231</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">counter</span> <span class="o">+=</span> <span class="mi">1</span>
+</span><span id="ProgBar.display-232"><a href="#ProgBar.display-232"><span class="linenos">232</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="ProgBar.display-233"><a href="#ProgBar.display-233"><span class="linenos">233</span></a>            <span class="o">...</span>
+</span><span id="ProgBar.display-234"><a href="#ProgBar.display-234"><span class="linenos">234</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="ProgBar.display-235"><a href="#ProgBar.display-235"><span class="linenos">235</span></a>            <span class="k">raise</span> <span class="n">e</span>
+</span><span id="ProgBar.display-236"><a href="#ProgBar.display-236"><span class="linenos">236</span></a>        <span class="k">return</span> <span class="n">return_object</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Writes the progress bar to the terminal.</p>
 
-<h6 id="parameters">Parameters</h6>
+<h4 id="params">:params:</h4>
+
+<p><code>prefix</code>: String affixed to the front of the progress bar.</p>
 
-<ul>
-<li><p><strong>prefix</strong>:  String affixed to the front of the progress bar.</p></li>
-<li><p><strong>suffix</strong>:  String appended to the end of the progress bar.</p></li>
-<li><p><strong>counter_override</strong>:  When an externally incremented completion counter is needed.</p></li>
-<li><p><strong>total_override</strong>:  When an externally controlled bar total is needed.</p></li>
-<li><p><strong>return_object</strong>:  An object to be returned by display().</p></li>
-</ul>
+<p><code>suffix</code>: String appended to the end of the progress bar.</p>
 
-<p>Allows display() to be called within a comprehension:</p>
+<p><code>counter_override</code>: When an externally incremented completion counter is needed.</p>
+
+<p><code>total_override</code>: When an externally controlled bar total is needed.</p>
+
+<p><code>return_object</code>: An object to be returned by display().
+Allows <code><a href="#ProgBar.display">display()</a></code> to be called within a comprehension:</p>
 
 <p>e.g.</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="k">def</span> <span class="nf">square</span><span class="p">(</span><span class="n">x</span><span class="p">:</span> <span class="nb">int</span> <span class="o">|</span> <span class="nb">float</span><span class="p">)</span><span class="o">-&gt;</span><span class="nb">int</span><span class="o">|</span><span class="nb">float</span><span class="p">:</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="k">return</span> <span class="n">x</span> <span class="o">*</span> <span class="n">x</span>
@@ -965,85 +1003,92 @@
     <span class="def">class</span>
     <span class="name">Spinner</span>:
 
                 <label class="view-source-button" for="Spinner-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner-222"><a href="#Spinner-222"><span class="linenos">222</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
-</span><span id="Spinner-223"><a href="#Spinner-223"><span class="linenos">223</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime display() is called.</span>
-</span><span id="Spinner-224"><a href="#Spinner-224"><span class="linenos">224</span></a>
-</span><span id="Spinner-225"><a href="#Spinner-225"><span class="linenos">225</span></a><span class="sd">    The display function writes the new character to the same line, overwriting the previous character.</span>
-</span><span id="Spinner-226"><a href="#Spinner-226"><span class="linenos">226</span></a>
-</span><span id="Spinner-227"><a href="#Spinner-227"><span class="linenos">227</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
-</span><span id="Spinner-228"><a href="#Spinner-228"><span class="linenos">228</span></a>
-</span><span id="Spinner-229"><a href="#Spinner-229"><span class="linenos">229</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
-</span><span id="Spinner-230"><a href="#Spinner-230"><span class="linenos">230</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Spinner-231"><a href="#Spinner-231"><span class="linenos">231</span></a>
-</span><span id="Spinner-232"><a href="#Spinner-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Spinner-233"><a href="#Spinner-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
-</span><span id="Spinner-234"><a href="#Spinner-234"><span class="linenos">234</span></a>    <span class="p">):</span>
-</span><span id="Spinner-235"><a href="#Spinner-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Spinner-236"><a href="#Spinner-236"><span class="linenos">236</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
-</span><span id="Spinner-237"><a href="#Spinner-237"><span class="linenos">237</span></a>
-</span><span id="Spinner-238"><a href="#Spinner-238"><span class="linenos">238</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
-</span><span id="Spinner-239"><a href="#Spinner-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="Spinner-240"><a href="#Spinner-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="Spinner-241"><a href="#Spinner-241"><span class="linenos">241</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
-</span><span id="Spinner-242"><a href="#Spinner-242"><span class="linenos">242</span></a>
-</span><span id="Spinner-243"><a href="#Spinner-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner-244"><a href="#Spinner-244"><span class="linenos">244</span></a>        <span class="k">return</span> <span class="bp">self</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner-239"><a href="#Spinner-239"><span class="linenos">239</span></a><span class="k">class</span> <span class="nc">Spinner</span><span class="p">:</span>
+</span><span id="Spinner-240"><a href="#Spinner-240"><span class="linenos">240</span></a>    <span class="sd">&quot;&quot;&quot;Prints one of a sequence of characters in order everytime `display()` is called.</span>
+</span><span id="Spinner-241"><a href="#Spinner-241"><span class="linenos">241</span></a>
+</span><span id="Spinner-242"><a href="#Spinner-242"><span class="linenos">242</span></a><span class="sd">    The `display` function writes the new character to the same line, overwriting the previous character.</span>
+</span><span id="Spinner-243"><a href="#Spinner-243"><span class="linenos">243</span></a>
+</span><span id="Spinner-244"><a href="#Spinner-244"><span class="linenos">244</span></a><span class="sd">    The sequence will be cycled through indefinitely.</span>
 </span><span id="Spinner-245"><a href="#Spinner-245"><span class="linenos">245</span></a>
-</span><span id="Spinner-246"><a href="#Spinner-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-</span><span id="Spinner-247"><a href="#Spinner-247"><span class="linenos">247</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="Spinner-246"><a href="#Spinner-246"><span class="linenos">246</span></a><span class="sd">    If used as a context manager, the last printed character will be cleared upon exiting.</span>
+</span><span id="Spinner-247"><a href="#Spinner-247"><span class="linenos">247</span></a><span class="sd">    &quot;&quot;&quot;</span>
 </span><span id="Spinner-248"><a href="#Spinner-248"><span class="linenos">248</span></a>
-</span><span id="Spinner-249"><a href="#Spinner-249"><span class="linenos">249</span></a>    <span class="nd">@property</span>
-</span><span id="Spinner-250"><a href="#Spinner-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-</span><span id="Spinner-251"><a href="#Spinner-251"><span class="linenos">251</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
-</span><span id="Spinner-252"><a href="#Spinner-252"><span class="linenos">252</span></a>
-</span><span id="Spinner-253"><a href="#Spinner-253"><span class="linenos">253</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Spinner-254"><a href="#Spinner-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
-</span><span id="Spinner-255"><a href="#Spinner-255"><span class="linenos">255</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
-</span><span id="Spinner-256"><a href="#Spinner-256"><span class="linenos">256</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
-</span><span id="Spinner-257"><a href="#Spinner-257"><span class="linenos">257</span></a>
-</span><span id="Spinner-258"><a href="#Spinner-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner-259"><a href="#Spinner-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="Spinner-260"><a href="#Spinner-260"><span class="linenos">260</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
+</span><span id="Spinner-249"><a href="#Spinner-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Spinner-250"><a href="#Spinner-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="Spinner-251"><a href="#Spinner-251"><span class="linenos">251</span></a>    <span class="p">):</span>
+</span><span id="Spinner-252"><a href="#Spinner-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner-253"><a href="#Spinner-253"><span class="linenos">253</span></a><span class="sd">        #### params:</span>
+</span><span id="Spinner-254"><a href="#Spinner-254"><span class="linenos">254</span></a>
+</span><span id="Spinner-255"><a href="#Spinner-255"><span class="linenos">255</span></a><span class="sd">        `sequence`: Override the built in spin sequence.</span>
+</span><span id="Spinner-256"><a href="#Spinner-256"><span class="linenos">256</span></a>
+</span><span id="Spinner-257"><a href="#Spinner-257"><span class="linenos">257</span></a><span class="sd">        `width_ratio`: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="Spinner-258"><a href="#Spinner-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner-259"><a href="#Spinner-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="Spinner-260"><a href="#Spinner-260"><span class="linenos">260</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
 </span><span id="Spinner-261"><a href="#Spinner-261"><span class="linenos">261</span></a>
-</span><span id="Spinner-262"><a href="#Spinner-262"><span class="linenos">262</span></a>    <span class="nd">@property</span>
-</span><span id="Spinner-263"><a href="#Spinner-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
-</span><span id="Spinner-264"><a href="#Spinner-264"><span class="linenos">264</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
-</span><span id="Spinner-265"><a href="#Spinner-265"><span class="linenos">265</span></a>
-</span><span id="Spinner-266"><a href="#Spinner-266"><span class="linenos">266</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
-</span><span id="Spinner-267"><a href="#Spinner-267"><span class="linenos">267</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
-</span><span id="Spinner-268"><a href="#Spinner-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="Spinner-269"><a href="#Spinner-269"><span class="linenos">269</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="Spinner-270"><a href="#Spinner-270"><span class="linenos">270</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
-</span><span id="Spinner-271"><a href="#Spinner-271"><span class="linenos">271</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
-</span><span id="Spinner-272"><a href="#Spinner-272"><span class="linenos">272</span></a>        <span class="p">]</span>
-</span><span id="Spinner-273"><a href="#Spinner-273"><span class="linenos">273</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="Spinner-274"><a href="#Spinner-274"><span class="linenos">274</span></a>
-</span><span id="Spinner-275"><a href="#Spinner-275"><span class="linenos">275</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="Spinner-276"><a href="#Spinner-276"><span class="linenos">276</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of self._sequence, append it to the end, and return the element.&quot;&quot;&quot;</span>
-</span><span id="Spinner-277"><a href="#Spinner-277"><span class="linenos">277</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-</span><span id="Spinner-278"><a href="#Spinner-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
-</span><span id="Spinner-279"><a href="#Spinner-279"><span class="linenos">279</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="Spinner-262"><a href="#Spinner-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="fm">__enter__</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-263"><a href="#Spinner-263"><span class="linenos">263</span></a>        <span class="k">return</span> <span class="bp">self</span>
+</span><span id="Spinner-264"><a href="#Spinner-264"><span class="linenos">264</span></a>
+</span><span id="Spinner-265"><a href="#Spinner-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="fm">__exit__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
+</span><span id="Spinner-266"><a href="#Spinner-266"><span class="linenos">266</span></a>        <span class="n">clear</span><span class="p">()</span>
+</span><span id="Spinner-267"><a href="#Spinner-267"><span class="linenos">267</span></a>
+</span><span id="Spinner-268"><a href="#Spinner-268"><span class="linenos">268</span></a>    <span class="nd">@property</span>
+</span><span id="Spinner-269"><a href="#Spinner-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
+</span><span id="Spinner-270"><a href="#Spinner-270"><span class="linenos">270</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span>
+</span><span id="Spinner-271"><a href="#Spinner-271"><span class="linenos">271</span></a>
+</span><span id="Spinner-272"><a href="#Spinner-272"><span class="linenos">272</span></a>    <span class="nd">@width_ratio</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Spinner-273"><a href="#Spinner-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">width_ratio</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ratio</span><span class="p">:</span> <span class="nb">float</span><span class="p">):</span>
+</span><span id="Spinner-274"><a href="#Spinner-274"><span class="linenos">274</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width_ratio</span> <span class="o">=</span> <span class="n">ratio</span>
+</span><span id="Spinner-275"><a href="#Spinner-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner-276"><a href="#Spinner-276"><span class="linenos">276</span></a>
+</span><span id="Spinner-277"><a href="#Spinner-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">_update_width</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-278"><a href="#Spinner-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">=</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="Spinner-279"><a href="#Spinner-279"><span class="linenos">279</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_width</span> <span class="o">=</span> <span class="nb">int</span><span class="p">((</span><span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span><span class="p">)</span>
 </span><span id="Spinner-280"><a href="#Spinner-280"><span class="linenos">280</span></a>
-</span><span id="Spinner-281"><a href="#Spinner-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner-282"><a href="#Spinner-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner-283"><a href="#Spinner-283"><span class="linenos">283</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
-</span><span id="Spinner-284"><a href="#Spinner-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
-</span><span id="Spinner-285"><a href="#Spinner-285"><span class="linenos">285</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
-</span><span id="Spinner-286"><a href="#Spinner-286"><span class="linenos">286</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="Spinner-281"><a href="#Spinner-281"><span class="linenos">281</span></a>    <span class="nd">@property</span>
+</span><span id="Spinner-282"><a href="#Spinner-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
+</span><span id="Spinner-283"><a href="#Spinner-283"><span class="linenos">283</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span>
+</span><span id="Spinner-284"><a href="#Spinner-284"><span class="linenos">284</span></a>
+</span><span id="Spinner-285"><a href="#Spinner-285"><span class="linenos">285</span></a>    <span class="nd">@sequence</span><span class="o">.</span><span class="n">setter</span>
+</span><span id="Spinner-286"><a href="#Spinner-286"><span class="linenos">286</span></a>    <span class="k">def</span> <span class="nf">sequence</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">character_list</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]):</span>
+</span><span id="Spinner-287"><a href="#Spinner-287"><span class="linenos">287</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="Spinner-288"><a href="#Spinner-288"><span class="linenos">288</span></a>            <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
+</span><span id="Spinner-289"><a href="#Spinner-289"><span class="linenos">289</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">_width</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">character_list</span><span class="p">))</span>
+</span><span id="Spinner-290"><a href="#Spinner-290"><span class="linenos">290</span></a>            <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">character_list</span><span class="p">)</span>
+</span><span id="Spinner-291"><a href="#Spinner-291"><span class="linenos">291</span></a>        <span class="p">]</span>
+</span><span id="Spinner-292"><a href="#Spinner-292"><span class="linenos">292</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_sequence</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
+</span><span id="Spinner-293"><a href="#Spinner-293"><span class="linenos">293</span></a>
+</span><span id="Spinner-294"><a href="#Spinner-294"><span class="linenos">294</span></a>    <span class="k">def</span> <span class="nf">_get_next</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="Spinner-295"><a href="#Spinner-295"><span class="linenos">295</span></a>        <span class="sd">&quot;&quot;&quot;Pop the first element of `self._sequence`, append it to the end, and return the element.&quot;&quot;&quot;</span>
+</span><span id="Spinner-296"><a href="#Spinner-296"><span class="linenos">296</span></a>        <span class="n">ch</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
+</span><span id="Spinner-297"><a href="#Spinner-297"><span class="linenos">297</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">ch</span><span class="p">)</span>
+</span><span id="Spinner-298"><a href="#Spinner-298"><span class="linenos">298</span></a>        <span class="k">return</span> <span class="n">ch</span>
+</span><span id="Spinner-299"><a href="#Spinner-299"><span class="linenos">299</span></a>
+</span><span id="Spinner-300"><a href="#Spinner-300"><span class="linenos">300</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner-301"><a href="#Spinner-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner-302"><a href="#Spinner-302"><span class="linenos">302</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Spinner-303"><a href="#Spinner-303"><span class="linenos">303</span></a>            <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="Spinner-304"><a href="#Spinner-304"><span class="linenos">304</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner-305"><a href="#Spinner-305"><span class="linenos">305</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="Spinner-306"><a href="#Spinner-306"><span class="linenos">306</span></a>            <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="Spinner-307"><a href="#Spinner-307"><span class="linenos">307</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="Spinner-308"><a href="#Spinner-308"><span class="linenos">308</span></a>            <span class="o">...</span>
+</span><span id="Spinner-309"><a href="#Spinner-309"><span class="linenos">309</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Spinner-310"><a href="#Spinner-310"><span class="linenos">310</span></a>            <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Prints one of a sequence of characters in order everytime display() is called.</p>
+            <div class="docstring"><p>Prints one of a sequence of characters in order everytime <code><a href="#Spinner.display">display()</a></code> is called.</p>
 
-<p>The display function writes the new character to the same line, overwriting the previous character.</p>
+<p>The <code><a href="#Spinner.display">display</a></code> function writes the new character to the same line, overwriting the previous character.</p>
 
 <p>The sequence will be cycled through indefinitely.</p>
 
 <p>If used as a context manager, the last printed character will be cleared upon exiting.</p>
 </div>
 
 
@@ -1053,33 +1098,34 @@
             
         <span class="name">Spinner</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;/&#39;</span><span class="p">,</span> <span class="s1">&#39;-&#39;</span><span class="p">,</span> <span class="s1">&#39;</span><span class="se">\\</span><span class="s1">&#39;</span><span class="p">]</span>, </span><span class="param"><span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span></span>)</span>
 
                 <label class="view-source-button" for="Spinner.__init__-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner.__init__"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.__init__-232"><a href="#Spinner.__init__-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
-</span><span id="Spinner.__init__-233"><a href="#Spinner.__init__-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
-</span><span id="Spinner.__init__-234"><a href="#Spinner.__init__-234"><span class="linenos">234</span></a>    <span class="p">):</span>
-</span><span id="Spinner.__init__-235"><a href="#Spinner.__init__-235"><span class="linenos">235</span></a>        <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Spinner.__init__-236"><a href="#Spinner.__init__-236"><span class="linenos">236</span></a><span class="sd">        :param sequence: Override the built in spin sequence.</span>
-</span><span id="Spinner.__init__-237"><a href="#Spinner.__init__-237"><span class="linenos">237</span></a>
-</span><span id="Spinner.__init__-238"><a href="#Spinner.__init__-238"><span class="linenos">238</span></a><span class="sd">        :param width: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
-</span><span id="Spinner.__init__-239"><a href="#Spinner.__init__-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
-</span><span id="Spinner.__init__-240"><a href="#Spinner.__init__-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
-</span><span id="Spinner.__init__-241"><a href="#Spinner.__init__-241"><span class="linenos">241</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.__init__-249"><a href="#Spinner.__init__-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span>
+</span><span id="Spinner.__init__-250"><a href="#Spinner.__init__-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="p">,</span> <span class="n">sequence</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">],</span> <span class="n">width_ratio</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mf">0.25</span>
+</span><span id="Spinner.__init__-251"><a href="#Spinner.__init__-251"><span class="linenos">251</span></a>    <span class="p">):</span>
+</span><span id="Spinner.__init__-252"><a href="#Spinner.__init__-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-253"><a href="#Spinner.__init__-253"><span class="linenos">253</span></a><span class="sd">        #### params:</span>
+</span><span id="Spinner.__init__-254"><a href="#Spinner.__init__-254"><span class="linenos">254</span></a>
+</span><span id="Spinner.__init__-255"><a href="#Spinner.__init__-255"><span class="linenos">255</span></a><span class="sd">        `sequence`: Override the built in spin sequence.</span>
+</span><span id="Spinner.__init__-256"><a href="#Spinner.__init__-256"><span class="linenos">256</span></a>
+</span><span id="Spinner.__init__-257"><a href="#Spinner.__init__-257"><span class="linenos">257</span></a><span class="sd">        `width_ratio`: The fractional amount of the terminal for characters to move across.&quot;&quot;&quot;</span>
+</span><span id="Spinner.__init__-258"><a href="#Spinner.__init__-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span> <span class="o">=</span> <span class="n">sequence</span>
+</span><span id="Spinner.__init__-259"><a href="#Spinner.__init__-259"><span class="linenos">259</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">width_ratio</span> <span class="o">=</span> <span class="n">width_ratio</span>
+</span><span id="Spinner.__init__-260"><a href="#Spinner.__init__-260"><span class="linenos">260</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
 </span></pre></div>
 
 
-            <div class="docstring"><h6 id="parameters">Parameters</h6>
-
-<ul>
-<li><p><strong>sequence</strong>:  Override the built in spin sequence.</p></li>
-<li><p><strong>width</strong>:  The fractional amount of the terminal for characters to move across.</p></li>
-</ul>
+            <div class="docstring"><h4 id="params">params:</h4>
+
+<p><code>sequence</code>: Override the built in spin sequence.</p>
+
+<p><code>width_ratio</code>: The fractional amount of the terminal for characters to move across.</p>
 </div>
 
 
                             </div>
                             <div id="Spinner.display" class="classattr">
                                         <input id="Spinner.display-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1087,20 +1133,25 @@
         <span class="def">def</span>
         <span class="name">display</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="Spinner.display-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Spinner.display"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.display-281"><a href="#Spinner.display-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="Spinner.display-282"><a href="#Spinner.display-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
-</span><span id="Spinner.display-283"><a href="#Spinner.display-283"><span class="linenos">283</span></a>        <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
-</span><span id="Spinner.display-284"><a href="#Spinner.display-284"><span class="linenos">284</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
-</span><span id="Spinner.display-285"><a href="#Spinner.display-285"><span class="linenos">285</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
-</span><span id="Spinner.display-286"><a href="#Spinner.display-286"><span class="linenos">286</span></a>        <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Spinner.display-300"><a href="#Spinner.display-300"><span class="linenos">300</span></a>    <span class="k">def</span> <span class="nf">display</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="Spinner.display-301"><a href="#Spinner.display-301"><span class="linenos">301</span></a>        <span class="sd">&quot;&quot;&quot;Print the next character in the sequence.&quot;&quot;&quot;</span>
+</span><span id="Spinner.display-302"><a href="#Spinner.display-302"><span class="linenos">302</span></a>        <span class="k">try</span><span class="p">:</span>
+</span><span id="Spinner.display-303"><a href="#Spinner.display-303"><span class="linenos">303</span></a>            <span class="k">if</span> <span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span> <span class="o">!=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_current_terminal_width</span><span class="p">:</span>
+</span><span id="Spinner.display-304"><a href="#Spinner.display-304"><span class="linenos">304</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">_update_width</span><span class="p">()</span>
+</span><span id="Spinner.display-305"><a href="#Spinner.display-305"><span class="linenos">305</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">sequence</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_base_sequence</span>
+</span><span id="Spinner.display-306"><a href="#Spinner.display-306"><span class="linenos">306</span></a>            <span class="n">print_in_place</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_next</span><span class="p">())</span>
+</span><span id="Spinner.display-307"><a href="#Spinner.display-307"><span class="linenos">307</span></a>        <span class="k">except</span> <span class="ne">OSError</span><span class="p">:</span>
+</span><span id="Spinner.display-308"><a href="#Spinner.display-308"><span class="linenos">308</span></a>            <span class="o">...</span>
+</span><span id="Spinner.display-309"><a href="#Spinner.display-309"><span class="linenos">309</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="Spinner.display-310"><a href="#Spinner.display-310"><span class="linenos">310</span></a>            <span class="k">raise</span> <span class="n">e</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print the next character in the sequence.</p>
 </div>
```

#### html2text {}

```diff
@@ -24,861 +24,930 @@
 __3from typing import Any
 __4
 __5from noiftimer import Timer
 __6
 __7
 __8def clear():
 __9    """Erase the current line from the terminal."""
-_10    print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
-_11
-_12
-_13def print_in_place(string: str, animate: bool = False, animate_refresh:
-float = 0.01):
-_14    """Calls to print_in_place will overwrite
-_15    the previous line of text in the terminal
-_16    with the 'string' param.
+_10    try:
+_11        print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
+_12    except OSError:
+_13        ...
+_14    except Exception as e:
+_15        raise e
+_16
 _17
-_18    :param animate: Will cause the string
-_19    to be printed to the terminal
-_20    one character at a time.
-_21
-_22    :param animate_refresh: Number of seconds
-_23    between the addition of characters
-_24    when 'animate' is True."""
-_25    clear()
-_26    string = str(string)
-_27    width = get_terminal_size().columns
-_28    string = string[: width - 2]
-_29    if animate:
-_30        for i in range(len(string)):
-_31            print(f"{string[:i+1]}", flush=True, end=" \r")
-_32            sleep(animate_refresh)
-_33    else:
-_34        print(string, flush=True, end="\r")
-_35
-_36
-_37def ticker(info: list[str]):
-_38    """Prints info to terminal with
-_39    top and bottom padding so that repeated
-_40    calls print info without showing previous
-_41    outputs from ticker calls.
+_18def print_in_place(string: str, animate: bool = False, animate_refresh:
+float = 0.01):
+_19    """Calls to `print_in_place` will overwrite the previous line of text in
+the terminal with `string`.
+_20
+_21    #### :params:
+_22
+_23    `animate`: Will cause `string` to be printed to the terminal one
+character at a time.
+_24
+_25    `animate_refresh`: Number of seconds between the addition of characters
+when `animate` is `True`."""
+_26    clear()
+_27    string = str(string)
+_28    try:
+_29        width = get_terminal_size().columns
+_30        string = string[: width - 2]
+_31        if animate:
+_32            for i in range(len(string)):
+_33                print(f"{string[:i+1]}", flush=True, end=" \r")
+_34                sleep(animate_refresh)
+_35        else:
+_36            print(string, flush=True, end="\r")
+_37    except OSError:
+_38        ...
+_39    except Exception as e:
+_40        raise e
+_41
 _42
-_43    Similar visually to print_in_place,
-_44    but for multiple lines."""
-_45    width = get_terminal_size().columns
-_46    info = [str(line)[: width - 1] for line in info]
-_47    height = get_terminal_size().lines - len(info)
-_48    print("\n" * (height * 2), end="")
-_49    print(*info, sep="\n", end="")
-_50    print("\n" * (int((height) / 2)), end="")
-_51
-_52
-_53class ProgBar:
-_54    """Self incrementing, dynamically sized progress bar.
-_55
-_56    Includes an internal timer that starts when this object is created.
-_57    It can be easily added to the progress bar display by adding
-_58    the 'runtime' property to display's prefix or suffix param:
+_43def ticker(info: list[str]):
+_44    """Prints `info` to terminal with top and bottom padding so that
+previous text is not visible.
+_45
+_46    Similar visually to `print_in_place`, but for multiple lines."""
+_47    try:
+_48        width = get_terminal_size().columns
+_49        info = [str(line)[: width - 1] for line in info]
+_50        height = get_terminal_size().lines - len(info)
+_51        print("\n" * (height * 2), end="")
+_52        print(*info, sep="\n", end="")
+_53        print("\n" * (int((height) / 2)), end="")
+_54    except OSError:
+_55        ...
+_56    except Exception as e:
+_57        raise e
+_58
 _59
-_60    >>> bar = ProgBar(total=100)
-_61    >>> time.sleep(30)
-_62    >>> bar.display(prefix=bar.runtime)
-_63    >>> "runtime: 30s [_///////////////////]1.00%" """
+_60class ProgBar:
+_61    """Self incrementing, dynamically sized progress bar.
+_62
+_63    Includes an internal timer that starts when this object is created.
 _64
-_65    def __init__(
-_66        self,
-_67        total: float,
-_68        update_frequency: int = 1,
-_69        fill_ch: str = "_",
-_70        unfill_ch: str = "/",
-_71        width_ratio: float = 0.75,
-_72        new_line_after_completion: bool = True,
-_73        clear_after_completion: bool = False,
-_74    ):
-_75        """:param total: The number of calls to reach 100% completion.
-_76
-_77        :param update_frequency: The progress bar will only update once
-every this number of calls to display().
-_78        The larger the value, the less performance impact ProgBar has on the
-loop in which it is called.
-_79        e.g.
-_80        >>> bar = ProgBar(100, update_frequency=10)
-_81        >>> for _ in range(100):
-_82        >>>     bar.display()
-_83
-_84        ^The progress bar in the terminal will only update once every ten
+_65    Easily add runtime to progress display:
+_66
+_67    >>> bar = ProgBar(total=100)
+_68    >>> time.sleep(30)
+_69    >>> bar.display(prefix=f"Doin stuff ~ {bar.runtime}")
+_70    >>> "Doin stuff ~ runtime: 30s [_///////////////////]-1.00%" """
+_71
+_72    def __init__(
+_73        self,
+_74        total: float,
+_75        update_frequency: int = 1,
+_76        fill_ch: str = "_",
+_77        unfill_ch: str = "/",
+_78        width_ratio: float = 0.5,
+_79        new_line_after_completion: bool = True,
+_80        clear_after_completion: bool = False,
+_81    ):
+_82        """
+_83        #### :params:
+_84
+_85        `total`: The number of calls to reach 100% completion.
+_86
+_87        `update_frequency`: The progress bar will only update once every
+this number of calls to `display()`.
+_88        The larger the value, the less performance impact `ProgBar` has on
+the loop in which it is called.
+_89        e.g.
+_90        >>> bar = ProgBar(100, update_frequency=10)
+_91        >>> for _ in range(100):
+_92        >>>     bar.display()
+_93
+_94        ^The progress bar in the terminal will only update once every ten
 calls, going from 0%->100% in 10% increments.
-_85        Note: If 'total' is not a multiple of 'update_frequency', the
+_95        Note: If `total` is not a multiple of `update_frequency`, the
 display will not show 100% completion when the loop finishes.
-_86
-_87        :param fill_ch: The character used to represent the completed part
-of the bar.
-_88
-_89        :param unfill_ch: The character used to represent the uncompleted
-part of the bar.
-_90
-_91        :param width_ratio: The width of the progress bar relative to the
-width of the terminal window.
-_92
-_93        :param new_line_after_completion: Make a call to print() once
-self.counter >= self.total.
-_94
-_95        :param clear_after_completion: Make a call to printbuddies.clear()
-once self.counter >= self.total.
 _96
-_97        Note: if new_line_after_completion and clear_after_completion are
-both True, the line will be cleared
-_98        then a call to print() will be made."""
-_99        self.total = total
-100        self.update_frequency = update_frequency
-101        self.fill_ch = fill_ch[0]
-102        self.unfill_ch = unfill_ch[0]
-103        self.width_ratio = width_ratio
-104        self.new_line_after_completion = new_line_after_completion
-105        self.clear_after_completion = clear_after_completion
-106        self.reset()
-107        self.with_context = False
-108
-109    def __enter__(self):
-110        self.with_context = True
-111        return self
-112
-113    def __exit__(self, *args, **kwargs):
-114        if self.clear_after_completion:
-115            clear()
-116        else:
-117            print()
+_97        `fill_ch`: The character used to represent the completed part of the
+bar.
+_98
+_99        `unfill_ch`: The character used to represent the incomplete part of
+the bar.
+100
+101        `width_ratio`: The width of the progress bar relative to the width
+of the terminal window.
+102
+103        `new_line_after_completion`: Make a call to `print()` once
+`self.counter >= self.total`.
+104
+105        `clear_after_completion`: Make a call to `printbuddies.clear()` once
+`self.counter >= self.total`.
+106
+107        Note: if `new_line_after_completion` and `clear_after_completion`
+are both `True`, the line will be cleared
+108        then a call to `print()` will be made."""
+109        self.total = total
+110        self.update_frequency = update_frequency
+111        self.fill_ch = fill_ch[0]
+112        self.unfill_ch = unfill_ch[0]
+113        self.width_ratio = width_ratio
+114        self.new_line_after_completion = new_line_after_completion
+115        self.clear_after_completion = clear_after_completion
+116        self.reset()
+117        self.with_context = False
 118
-119    def reset(self):
-120        self.counter = 1
-121        self.percent = ""
-122        self.prefix = ""
-123        self.suffix = ""
-124        self.filled = ""
-125        self.unfilled = ""
-126        self.bar = ""
-127        self.timer = Timer(subsecond_resolution=False).start()
+119    def __enter__(self):
+120        self.with_context = True
+121        return self
+122
+123    def __exit__(self, *args, **kwargs):
+124        if self.clear_after_completion:
+125            clear()
+126        else:
+127            print()
 128
-129    @property
-130    def runtime(self) -> str:
-131        return f"runtime:{self.timer.elapsed_str}"
-132
-133    def get_percent(self) -> str:
-134        """Returns the percentage complete to two decimal places
-135        as a string without the %."""
-136        percent = str(round(100.0 * self.counter / self.total, 2))
-137        if len(percent.split(".")[1]) == 1:
-138            percent = percent + "0"
-139        if len(percent.split(".")[0]) == 1:
-140            percent = "0" + percent
-141        return percent
-142
-143    def _prepare_bar(self):
-144        self.terminal_width = get_terminal_size().columns - 1
-145        bar_length = int(self.terminal_width * self.width_ratio)
-146        progress = int(bar_length * min(self.counter / self.total, 1.0))
-147        self.filled = self.fill_ch * progress
-148        self.unfilled = self.unfill_ch * (bar_length - progress)
-149        self.percent = self.get_percent()
-150        self.bar = self.get_bar()
-151
-152    def _trim_bar(self):
-153        original_width = self.width_ratio
-154        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
-155            self.width_ratio -= 0.01
-156            self._prepare_bar()
-157        self.width_ratio = original_width
-158
-159    def get_bar(self):
-160        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+129    def reset(self):
+130        self.counter = 1
+131        self.percent = ""
+132        self.prefix = ""
+133        self.suffix = ""
+134        self.filled = ""
+135        self.unfilled = ""
+136        self.timer = Timer(subsecond_resolution=False).start()
+137
+138    @property
+139    def runtime(self) -> str:
+140        return f"runtime:{self.timer.elapsed_str}"
+141
+142    @property
+143    def bar(self) -> str:
+144        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
 {self.unfilled}]-{self.percent}% {self.suffix}"
-161
-162    def display(
-163        self,
-164        prefix: str = "",
-165        suffix: str = "",
-166        counter_override: float | None = None,
-167        total_override: float | None = None,
-168        return_object: Any | None = None,
-169    ) -> Any:
-170        """Writes the progress bar to the terminal.
-171
-172        :param prefix: String affixed to the front of the progress bar.
-173
-174        :param suffix: String appended to the end of the progress bar.
-175
-176        :param counter_override: When an externally incremented completion
+145
+146    def get_percent(self) -> str:
+147        """Returns the percentage completed to two decimal places as a
+string without the `%`."""
+148        percent = str(round(100.0 * self.counter / self.total, 2))
+149        if len(percent.split(".")[1]) == 1:
+150            percent = percent + "0"
+151        if len(percent.split(".")[0]) == 1:
+152            percent = "0" + percent
+153        return percent
+154
+155    def _prepare_bar(self):
+156        self.terminal_width = get_terminal_size().columns - 1
+157        bar_length = int(self.terminal_width * self.width_ratio)
+158        progress = int(bar_length * min(self.counter / self.total, 1.0))
+159        self.filled = self.fill_ch * progress
+160        self.unfilled = self.unfill_ch * (bar_length - progress)
+161        self.percent = self.get_percent()
+162
+163    def _trim_bar(self):
+164        original_width = self.width_ratio
+165        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
+166            self.width_ratio -= 0.01
+167            self._prepare_bar()
+168        self.width_ratio = original_width
+169
+170    def get_bar(self):
+171        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+{self.unfilled}]-{self.percent}% {self.suffix}"
+172
+173    def display(
+174        self,
+175        prefix: str = "",
+176        suffix: str = "",
+177        counter_override: float | None = None,
+178        total_override: float | None = None,
+179        return_object: Any | None = None,
+180    ) -> Any:
+181        """Writes the progress bar to the terminal.
+182
+183        #### :params:
+184
+185        `prefix`: String affixed to the front of the progress bar.
+186
+187        `suffix`: String appended to the end of the progress bar.
+188
+189        `counter_override`: When an externally incremented completion
 counter is needed.
-177
-178        :param total_override: When an externally controlled bar total is
-needed.
-179
-180        :param return_object: An object to be returned by display().
-181
-182        Allows display() to be called within a comprehension:
-183
-184        e.g.
-185
-186        >>> bar = ProgBar(10)
-187        >>> def square(x: int | float)->int|float:
-188        >>>     return x * x
-189        >>> myList = [bar.display(return_object=square(i)) for i in range
+190
+191        `total_override`: When an externally controlled bar total is needed.
+192
+193        `return_object`: An object to be returned by display().
+194        Allows `display()` to be called within a comprehension:
+195
+196        e.g.
+197
+198        >>> bar = ProgBar(10)
+199        >>> def square(x: int | float)->int|float:
+200        >>>     return x * x
+201        >>> myList = [bar.display(return_object=square(i)) for i in range
 (10)]
-190        >>> <progress bar gets displayed>
-191        >>> myList
-192        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
-193        if not self.timer.started:
-194            self.timer.start()
-195        if counter_override is not None:
-196            self.counter = counter_override
-197        if total_override:
-198            self.total = total_override
-199        # Don't wanna divide by 0 there, pal
-200        while self.total <= 0:
-201            self.total += 1
-202        if self.counter % self.update_frequency == 0:
-203            self.prefix = prefix
-204            self.suffix = suffix
-205            self._prepare_bar()
-206            self._trim_bar()
-207            pad = " " * (self.terminal_width - len(self.bar))
-208            width = get_terminal_size().columns
-209            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-210        if self.counter >= self.total:
-211            self.timer.stop()
-212            if not self.with_context:
-213                if self.clear_after_completion:
-214                    clear()
-215                if self.new_line_after_completion:
-216                    print()
-217        self.counter += 1
-218        return return_object
-219
-220
-221class Spinner:
-222    """Prints one of a sequence of characters in order everytime display()
+202        >>> <progress bar gets displayed>
+203        >>> myList
+204        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+205        if not self.timer.started:
+206            self.timer.start()
+207        if counter_override is not None:
+208            self.counter = counter_override
+209        if total_override:
+210            self.total = total_override
+211        # Don't wanna divide by 0 there, pal
+212        while self.total <= 0:
+213            self.total += 1
+214        try:
+215            if self.counter % self.update_frequency == 0:
+216                self.prefix = prefix
+217                self.suffix = suffix
+218                self._prepare_bar()
+219                self._trim_bar()
+220                pad = " " * (self.terminal_width - len(self.bar))
+221                width = get_terminal_size().columns
+222                print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+223            if self.counter >= self.total:
+224                self.timer.stop()
+225                if not self.with_context:
+226                    if self.clear_after_completion:
+227                        clear()
+228                    if self.new_line_after_completion:
+229                        print()
+230            self.counter += 1
+231        except OSError:
+232            ...
+233        except Exception as e:
+234            raise e
+235        return return_object
+236
+237
+238class Spinner:
+239    """Prints one of a sequence of characters in order everytime `display()`
 is called.
-223
-224    The display function writes the new character to the same line,
+240
+241    The `display` function writes the new character to the same line,
 overwriting the previous character.
-225
-226    The sequence will be cycled through indefinitely.
-227
-228    If used as a context manager, the last printed character will be cleared
+242
+243    The sequence will be cycled through indefinitely.
+244
+245    If used as a context manager, the last printed character will be cleared
 upon exiting.
-229    """
-230
-231    def __init__(
-232        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+246    """
+247
+248    def __init__(
+249        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
 0.25
-233    ):
-234        """
-235        :param sequence: Override the built in spin sequence.
-236
-237        :param width: The fractional amount of the terminal for characters
+250    ):
+251        """
+252        #### params:
+253
+254        `sequence`: Override the built in spin sequence.
+255
+256        `width_ratio`: The fractional amount of the terminal for characters
 to move across."""
-238        self._base_sequence = sequence
-239        self.width_ratio = width_ratio
-240        self.sequence = self._base_sequence
-241
-242    def __enter__(self):
-243        return self
-244
-245    def __exit__(self, *args, **kwargs):
-246        clear()
-247
-248    @property
-249    def width_ratio(self) -> float:
-250        return self._width_ratio
-251
-252    @width_ratio.setter
-253    def width_ratio(self, ratio: float):
-254        self._width_ratio = ratio
-255        self._update_width()
-256
-257    def _update_width(self):
-258        self._current_terminal_width = get_terminal_size().columns
-259        self._width = int((self._current_terminal_width - 1) *
-self.width_ratio)
+257        self._base_sequence = sequence
+258        self.width_ratio = width_ratio
+259        self.sequence = self._base_sequence
 260
-261    @property
-262    def sequence(self) -> list[Any]:
-263        return self._sequence
-264
-265    @sequence.setter
-266    def sequence(self, character_list: list[Any]):
-267        self._sequence = [
-268            ch.rjust(i + j)
-269            for i in range(1, self._width, len(character_list))
-270            for j, ch in enumerate(character_list)
-271        ]
-272        self._sequence += self._sequence[::-1]
-273
-274    def _get_next(self) -> str:
-275        """Pop the first element of self._sequence, append it to the end,
-and return the element."""
-276        ch = self.sequence.pop(0)
-277        self.sequence.append(ch)
-278        return ch
+261    def __enter__(self):
+262        return self
+263
+264    def __exit__(self, *args, **kwargs):
+265        clear()
+266
+267    @property
+268    def width_ratio(self) -> float:
+269        return self._width_ratio
+270
+271    @width_ratio.setter
+272    def width_ratio(self, ratio: float):
+273        self._width_ratio = ratio
+274        self._update_width()
+275
+276    def _update_width(self):
+277        self._current_terminal_width = get_terminal_size().columns
+278        self._width = int((self._current_terminal_width - 1) *
+self.width_ratio)
 279
-280    def display(self):
-281        """Print the next character in the sequence."""
-282        if get_terminal_size().columns != self._current_terminal_width:
-283            self._update_width()
-284            self.sequence = self._base_sequence
-285        print_in_place(self._get_next())
+280    @property
+281    def sequence(self) -> list[Any]:
+282        return self._sequence
+283
+284    @sequence.setter
+285    def sequence(self, character_list: list[Any]):
+286        self._sequence = [
+287            ch.rjust(i + j)
+288            for i in range(1, self._width, len(character_list))
+289            for j, ch in enumerate(character_list)
+290        ]
+291        self._sequence += self._sequence[::-1]
+292
+293    def _get_next(self) -> str:
+294        """Pop the first element of `self._sequence`, append it to the end,
+and return the element."""
+295        ch = self.sequence.pop(0)
+296        self.sequence.append(ch)
+297        return ch
+298
+299    def display(self):
+300        """Print the next character in the sequence."""
+301        try:
+302            if get_terminal_size().columns != self._current_terminal_width:
+303                self._update_width()
+304                self.sequence = self._base_sequence
+305            print_in_place(self._get_next())
+306        except OSError:
+307            ...
+308        except Exception as e:
+309            raise e
   ⁰
 def clear(): View Source
 _9def clear():
 10    """Erase the current line from the terminal."""
-11    print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
+11    try:
+12        print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
+13    except OSError:
+14        ...
+15    except Exception as e:
+16        raise e
 Erase the current line from the terminal.
   ⁰
 def print_in_place(string: str, animate: bool = False, animate_refresh: float =
 0.01): View Source
-14def print_in_place(string: str, animate: bool = False, animate_refresh: float
+19def print_in_place(string: str, animate: bool = False, animate_refresh: float
 = 0.01):
-15    """Calls to print_in_place will overwrite
-16    the previous line of text in the terminal
-17    with the 'string' param.
-18
-19    :param animate: Will cause the string
-20    to be printed to the terminal
-21    one character at a time.
-22
-23    :param animate_refresh: Number of seconds
-24    between the addition of characters
-25    when 'animate' is True."""
-26    clear()
-27    string = str(string)
-28    width = get_terminal_size().columns
-29    string = string[: width - 2]
-30    if animate:
-31        for i in range(len(string)):
-32            print(f"{string[:i+1]}", flush=True, end=" \r")
-33            sleep(animate_refresh)
-34    else:
-35        print(string, flush=True, end="\r")
+20    """Calls to `print_in_place` will overwrite the previous line of text in
+the terminal with `string`.
+21
+22    #### :params:
+23
+24    `animate`: Will cause `string` to be printed to the terminal one
+character at a time.
+25
+26    `animate_refresh`: Number of seconds between the addition of characters
+when `animate` is `True`."""
+27    clear()
+28    string = str(string)
+29    try:
+30        width = get_terminal_size().columns
+31        string = string[: width - 2]
+32        if animate:
+33            for i in range(len(string)):
+34                print(f"{string[:i+1]}", flush=True, end=" \r")
+35                sleep(animate_refresh)
+36        else:
+37            print(string, flush=True, end="\r")
+38    except OSError:
+39        ...
+40    except Exception as e:
+41        raise e
 Calls to print_in_place will overwrite the previous line of text in the
-terminal with the 'string' param.
-* Parameters *
-    * animate: Will cause the string to be printed to the terminal one
-      character at a time.
-    * animate_refresh: Number of seconds between the addition of characters
-      when 'animate' is True.
+terminal with string.
+*** :params: ***
+animate: Will cause string to be printed to the terminal one character at a
+time.
+animate_refresh: Number of seconds between the addition of characters when
+animate is True.
   ⁰
 def ticker(info: list[str]): View Source
-38def ticker(info: list[str]):
-39    """Prints info to terminal with
-40    top and bottom padding so that repeated
-41    calls print info without showing previous
-42    outputs from ticker calls.
-43
-44    Similar visually to print_in_place,
-45    but for multiple lines."""
-46    width = get_terminal_size().columns
-47    info = [str(line)[: width - 1] for line in info]
-48    height = get_terminal_size().lines - len(info)
-49    print("\n" * (height * 2), end="")
-50    print(*info, sep="\n", end="")
-51    print("\n" * (int((height) / 2)), end="")
-Prints info to terminal with top and bottom padding so that repeated calls
-print info without showing previous outputs from ticker calls.
+44def ticker(info: list[str]):
+45    """Prints `info` to terminal with top and bottom padding so that previous
+text is not visible.
+46
+47    Similar visually to `print_in_place`, but for multiple lines."""
+48    try:
+49        width = get_terminal_size().columns
+50        info = [str(line)[: width - 1] for line in info]
+51        height = get_terminal_size().lines - len(info)
+52        print("\n" * (height * 2), end="")
+53        print(*info, sep="\n", end="")
+54        print("\n" * (int((height) / 2)), end="")
+55    except OSError:
+56        ...
+57    except Exception as e:
+58        raise e
+Prints info to terminal with top and bottom padding so that previous text is
+not visible.
 Similar visually to print_in_place, but for multiple lines.
   ⁰
 class ProgBar: View Source
-_54class ProgBar:
-_55    """Self incrementing, dynamically sized progress bar.
-_56
-_57    Includes an internal timer that starts when this object is created.
-_58    It can be easily added to the progress bar display by adding
-_59    the 'runtime' property to display's prefix or suffix param:
-_60
-_61    >>> bar = ProgBar(total=100)
-_62    >>> time.sleep(30)
-_63    >>> bar.display(prefix=bar.runtime)
-_64    >>> "runtime: 30s [_///////////////////]1.00%" """
+_61class ProgBar:
+_62    """Self incrementing, dynamically sized progress bar.
+_63
+_64    Includes an internal timer that starts when this object is created.
 _65
-_66    def __init__(
-_67        self,
-_68        total: float,
-_69        update_frequency: int = 1,
-_70        fill_ch: str = "_",
-_71        unfill_ch: str = "/",
-_72        width_ratio: float = 0.75,
-_73        new_line_after_completion: bool = True,
-_74        clear_after_completion: bool = False,
-_75    ):
-_76        """:param total: The number of calls to reach 100% completion.
-_77
-_78        :param update_frequency: The progress bar will only update once
-every this number of calls to display().
-_79        The larger the value, the less performance impact ProgBar has on the
-loop in which it is called.
-_80        e.g.
-_81        >>> bar = ProgBar(100, update_frequency=10)
-_82        >>> for _ in range(100):
-_83        >>>     bar.display()
-_84
-_85        ^The progress bar in the terminal will only update once every ten
+_66    Easily add runtime to progress display:
+_67
+_68    >>> bar = ProgBar(total=100)
+_69    >>> time.sleep(30)
+_70    >>> bar.display(prefix=f"Doin stuff ~ {bar.runtime}")
+_71    >>> "Doin stuff ~ runtime: 30s [_///////////////////]-1.00%" """
+_72
+_73    def __init__(
+_74        self,
+_75        total: float,
+_76        update_frequency: int = 1,
+_77        fill_ch: str = "_",
+_78        unfill_ch: str = "/",
+_79        width_ratio: float = 0.5,
+_80        new_line_after_completion: bool = True,
+_81        clear_after_completion: bool = False,
+_82    ):
+_83        """
+_84        #### :params:
+_85
+_86        `total`: The number of calls to reach 100% completion.
+_87
+_88        `update_frequency`: The progress bar will only update once every
+this number of calls to `display()`.
+_89        The larger the value, the less performance impact `ProgBar` has on
+the loop in which it is called.
+_90        e.g.
+_91        >>> bar = ProgBar(100, update_frequency=10)
+_92        >>> for _ in range(100):
+_93        >>>     bar.display()
+_94
+_95        ^The progress bar in the terminal will only update once every ten
 calls, going from 0%->100% in 10% increments.
-_86        Note: If 'total' is not a multiple of 'update_frequency', the
+_96        Note: If `total` is not a multiple of `update_frequency`, the
 display will not show 100% completion when the loop finishes.
-_87
-_88        :param fill_ch: The character used to represent the completed part
-of the bar.
-_89
-_90        :param unfill_ch: The character used to represent the uncompleted
-part of the bar.
-_91
-_92        :param width_ratio: The width of the progress bar relative to the
-width of the terminal window.
-_93
-_94        :param new_line_after_completion: Make a call to print() once
-self.counter >= self.total.
-_95
-_96        :param clear_after_completion: Make a call to printbuddies.clear()
-once self.counter >= self.total.
 _97
-_98        Note: if new_line_after_completion and clear_after_completion are
-both True, the line will be cleared
-_99        then a call to print() will be made."""
-100        self.total = total
-101        self.update_frequency = update_frequency
-102        self.fill_ch = fill_ch[0]
-103        self.unfill_ch = unfill_ch[0]
-104        self.width_ratio = width_ratio
-105        self.new_line_after_completion = new_line_after_completion
-106        self.clear_after_completion = clear_after_completion
-107        self.reset()
-108        self.with_context = False
-109
-110    def __enter__(self):
-111        self.with_context = True
-112        return self
-113
-114    def __exit__(self, *args, **kwargs):
-115        if self.clear_after_completion:
-116            clear()
-117        else:
-118            print()
+_98        `fill_ch`: The character used to represent the completed part of the
+bar.
+_99
+100        `unfill_ch`: The character used to represent the incomplete part of
+the bar.
+101
+102        `width_ratio`: The width of the progress bar relative to the width
+of the terminal window.
+103
+104        `new_line_after_completion`: Make a call to `print()` once
+`self.counter >= self.total`.
+105
+106        `clear_after_completion`: Make a call to `printbuddies.clear()` once
+`self.counter >= self.total`.
+107
+108        Note: if `new_line_after_completion` and `clear_after_completion`
+are both `True`, the line will be cleared
+109        then a call to `print()` will be made."""
+110        self.total = total
+111        self.update_frequency = update_frequency
+112        self.fill_ch = fill_ch[0]
+113        self.unfill_ch = unfill_ch[0]
+114        self.width_ratio = width_ratio
+115        self.new_line_after_completion = new_line_after_completion
+116        self.clear_after_completion = clear_after_completion
+117        self.reset()
+118        self.with_context = False
 119
-120    def reset(self):
-121        self.counter = 1
-122        self.percent = ""
-123        self.prefix = ""
-124        self.suffix = ""
-125        self.filled = ""
-126        self.unfilled = ""
-127        self.bar = ""
-128        self.timer = Timer(subsecond_resolution=False).start()
+120    def __enter__(self):
+121        self.with_context = True
+122        return self
+123
+124    def __exit__(self, *args, **kwargs):
+125        if self.clear_after_completion:
+126            clear()
+127        else:
+128            print()
 129
-130    @property
-131    def runtime(self) -> str:
-132        return f"runtime:{self.timer.elapsed_str}"
-133
-134    def get_percent(self) -> str:
-135        """Returns the percentage complete to two decimal places
-136        as a string without the %."""
-137        percent = str(round(100.0 * self.counter / self.total, 2))
-138        if len(percent.split(".")[1]) == 1:
-139            percent = percent + "0"
-140        if len(percent.split(".")[0]) == 1:
-141            percent = "0" + percent
-142        return percent
-143
-144    def _prepare_bar(self):
-145        self.terminal_width = get_terminal_size().columns - 1
-146        bar_length = int(self.terminal_width * self.width_ratio)
-147        progress = int(bar_length * min(self.counter / self.total, 1.0))
-148        self.filled = self.fill_ch * progress
-149        self.unfilled = self.unfill_ch * (bar_length - progress)
-150        self.percent = self.get_percent()
-151        self.bar = self.get_bar()
-152
-153    def _trim_bar(self):
-154        original_width = self.width_ratio
-155        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
-156            self.width_ratio -= 0.01
-157            self._prepare_bar()
-158        self.width_ratio = original_width
-159
-160    def get_bar(self):
-161        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+130    def reset(self):
+131        self.counter = 1
+132        self.percent = ""
+133        self.prefix = ""
+134        self.suffix = ""
+135        self.filled = ""
+136        self.unfilled = ""
+137        self.timer = Timer(subsecond_resolution=False).start()
+138
+139    @property
+140    def runtime(self) -> str:
+141        return f"runtime:{self.timer.elapsed_str}"
+142
+143    @property
+144    def bar(self) -> str:
+145        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
 {self.unfilled}]-{self.percent}% {self.suffix}"
-162
-163    def display(
-164        self,
-165        prefix: str = "",
-166        suffix: str = "",
-167        counter_override: float | None = None,
-168        total_override: float | None = None,
-169        return_object: Any | None = None,
-170    ) -> Any:
-171        """Writes the progress bar to the terminal.
-172
-173        :param prefix: String affixed to the front of the progress bar.
-174
-175        :param suffix: String appended to the end of the progress bar.
-176
-177        :param counter_override: When an externally incremented completion
+146
+147    def get_percent(self) -> str:
+148        """Returns the percentage completed to two decimal places as a
+string without the `%`."""
+149        percent = str(round(100.0 * self.counter / self.total, 2))
+150        if len(percent.split(".")[1]) == 1:
+151            percent = percent + "0"
+152        if len(percent.split(".")[0]) == 1:
+153            percent = "0" + percent
+154        return percent
+155
+156    def _prepare_bar(self):
+157        self.terminal_width = get_terminal_size().columns - 1
+158        bar_length = int(self.terminal_width * self.width_ratio)
+159        progress = int(bar_length * min(self.counter / self.total, 1.0))
+160        self.filled = self.fill_ch * progress
+161        self.unfilled = self.unfill_ch * (bar_length - progress)
+162        self.percent = self.get_percent()
+163
+164    def _trim_bar(self):
+165        original_width = self.width_ratio
+166        while len(self.bar) > self.terminal_width and self.width_ratio > 0:
+167            self.width_ratio -= 0.01
+168            self._prepare_bar()
+169        self.width_ratio = original_width
+170
+171    def get_bar(self):
+172        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+{self.unfilled}]-{self.percent}% {self.suffix}"
+173
+174    def display(
+175        self,
+176        prefix: str = "",
+177        suffix: str = "",
+178        counter_override: float | None = None,
+179        total_override: float | None = None,
+180        return_object: Any | None = None,
+181    ) -> Any:
+182        """Writes the progress bar to the terminal.
+183
+184        #### :params:
+185
+186        `prefix`: String affixed to the front of the progress bar.
+187
+188        `suffix`: String appended to the end of the progress bar.
+189
+190        `counter_override`: When an externally incremented completion
 counter is needed.
-178
-179        :param total_override: When an externally controlled bar total is
-needed.
-180
-181        :param return_object: An object to be returned by display().
-182
-183        Allows display() to be called within a comprehension:
-184
-185        e.g.
-186
-187        >>> bar = ProgBar(10)
-188        >>> def square(x: int | float)->int|float:
-189        >>>     return x * x
-190        >>> myList = [bar.display(return_object=square(i)) for i in range
+191
+192        `total_override`: When an externally controlled bar total is needed.
+193
+194        `return_object`: An object to be returned by display().
+195        Allows `display()` to be called within a comprehension:
+196
+197        e.g.
+198
+199        >>> bar = ProgBar(10)
+200        >>> def square(x: int | float)->int|float:
+201        >>>     return x * x
+202        >>> myList = [bar.display(return_object=square(i)) for i in range
 (10)]
-191        >>> <progress bar gets displayed>
-192        >>> myList
-193        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
-194        if not self.timer.started:
-195            self.timer.start()
-196        if counter_override is not None:
-197            self.counter = counter_override
-198        if total_override:
-199            self.total = total_override
-200        # Don't wanna divide by 0 there, pal
-201        while self.total <= 0:
-202            self.total += 1
-203        if self.counter % self.update_frequency == 0:
-204            self.prefix = prefix
-205            self.suffix = suffix
-206            self._prepare_bar()
-207            self._trim_bar()
-208            pad = " " * (self.terminal_width - len(self.bar))
-209            width = get_terminal_size().columns
-210            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-211        if self.counter >= self.total:
-212            self.timer.stop()
-213            if not self.with_context:
-214                if self.clear_after_completion:
-215                    clear()
-216                if self.new_line_after_completion:
-217                    print()
-218        self.counter += 1
-219        return return_object
+203        >>> <progress bar gets displayed>
+204        >>> myList
+205        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+206        if not self.timer.started:
+207            self.timer.start()
+208        if counter_override is not None:
+209            self.counter = counter_override
+210        if total_override:
+211            self.total = total_override
+212        # Don't wanna divide by 0 there, pal
+213        while self.total <= 0:
+214            self.total += 1
+215        try:
+216            if self.counter % self.update_frequency == 0:
+217                self.prefix = prefix
+218                self.suffix = suffix
+219                self._prepare_bar()
+220                self._trim_bar()
+221                pad = " " * (self.terminal_width - len(self.bar))
+222                width = get_terminal_size().columns
+223                print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+224            if self.counter >= self.total:
+225                self.timer.stop()
+226                if not self.with_context:
+227                    if self.clear_after_completion:
+228                        clear()
+229                    if self.new_line_after_completion:
+230                        print()
+231            self.counter += 1
+232        except OSError:
+233            ...
+234        except Exception as e:
+235            raise e
+236        return return_object
 Self incrementing, dynamically sized progress bar.
-Includes an internal timer that starts when this object is created. It can be
-easily added to the progress bar display by adding the 'runtime' property to
-display's prefix or suffix param:
+Includes an internal timer that starts when this object is created.
+Easily add runtime to progress display:
 >>> bar = ProgBar(total=100)
 >>> time.sleep(30)
->>> bar.display(prefix=bar.runtime)
->>> "runtime: 30s [_///////////////////]1.00%"
+>>> bar.display(prefix=f"Doin stuff ~ {bar.runtime}")
+>>> "Doin stuff ~ runtime: 30s [_///////////////////]-1.00%"
 ⁰
 ProgBar(
 total: float,
 update_frequency: int = 1,
 fill_ch: str = '_',
 unfill_ch: str = '/',
-width_ratio: float = 0.75,
+width_ratio: float = 0.5,
 new_line_after_completion: bool = True,
 clear_after_completion: bool = False) View Source
-_66    def __init__(
-_67        self,
-_68        total: float,
-_69        update_frequency: int = 1,
-_70        fill_ch: str = "_",
-_71        unfill_ch: str = "/",
-_72        width_ratio: float = 0.75,
-_73        new_line_after_completion: bool = True,
-_74        clear_after_completion: bool = False,
-_75    ):
-_76        """:param total: The number of calls to reach 100% completion.
-_77
-_78        :param update_frequency: The progress bar will only update once
-every this number of calls to display().
-_79        The larger the value, the less performance impact ProgBar has on the
-loop in which it is called.
-_80        e.g.
-_81        >>> bar = ProgBar(100, update_frequency=10)
-_82        >>> for _ in range(100):
-_83        >>>     bar.display()
-_84
-_85        ^The progress bar in the terminal will only update once every ten
+_73    def __init__(
+_74        self,
+_75        total: float,
+_76        update_frequency: int = 1,
+_77        fill_ch: str = "_",
+_78        unfill_ch: str = "/",
+_79        width_ratio: float = 0.5,
+_80        new_line_after_completion: bool = True,
+_81        clear_after_completion: bool = False,
+_82    ):
+_83        """
+_84        #### :params:
+_85
+_86        `total`: The number of calls to reach 100% completion.
+_87
+_88        `update_frequency`: The progress bar will only update once every
+this number of calls to `display()`.
+_89        The larger the value, the less performance impact `ProgBar` has on
+the loop in which it is called.
+_90        e.g.
+_91        >>> bar = ProgBar(100, update_frequency=10)
+_92        >>> for _ in range(100):
+_93        >>>     bar.display()
+_94
+_95        ^The progress bar in the terminal will only update once every ten
 calls, going from 0%->100% in 10% increments.
-_86        Note: If 'total' is not a multiple of 'update_frequency', the
+_96        Note: If `total` is not a multiple of `update_frequency`, the
 display will not show 100% completion when the loop finishes.
-_87
-_88        :param fill_ch: The character used to represent the completed part
-of the bar.
-_89
-_90        :param unfill_ch: The character used to represent the uncompleted
-part of the bar.
-_91
-_92        :param width_ratio: The width of the progress bar relative to the
-width of the terminal window.
-_93
-_94        :param new_line_after_completion: Make a call to print() once
-self.counter >= self.total.
-_95
-_96        :param clear_after_completion: Make a call to printbuddies.clear()
-once self.counter >= self.total.
 _97
-_98        Note: if new_line_after_completion and clear_after_completion are
-both True, the line will be cleared
-_99        then a call to print() will be made."""
-100        self.total = total
-101        self.update_frequency = update_frequency
-102        self.fill_ch = fill_ch[0]
-103        self.unfill_ch = unfill_ch[0]
-104        self.width_ratio = width_ratio
-105        self.new_line_after_completion = new_line_after_completion
-106        self.clear_after_completion = clear_after_completion
-107        self.reset()
-108        self.with_context = False
-* Parameters *
-    * total: The number of calls to reach 100% completion.
-    * update_frequency: The progress bar will only update once every this
-      number of calls to display(). The larger the value, the less performance
-      impact ProgBar has on the loop in which it is called. e.g.
-      >>> bar = ProgBar(100, update_frequency=10)
-      >>> for _ in range(100):
-      >>>     bar.display()
+_98        `fill_ch`: The character used to represent the completed part of the
+bar.
+_99
+100        `unfill_ch`: The character used to represent the incomplete part of
+the bar.
+101
+102        `width_ratio`: The width of the progress bar relative to the width
+of the terminal window.
+103
+104        `new_line_after_completion`: Make a call to `print()` once
+`self.counter >= self.total`.
+105
+106        `clear_after_completion`: Make a call to `printbuddies.clear()` once
+`self.counter >= self.total`.
+107
+108        Note: if `new_line_after_completion` and `clear_after_completion`
+are both `True`, the line will be cleared
+109        then a call to `print()` will be made."""
+110        self.total = total
+111        self.update_frequency = update_frequency
+112        self.fill_ch = fill_ch[0]
+113        self.unfill_ch = unfill_ch[0]
+114        self.width_ratio = width_ratio
+115        self.new_line_after_completion = new_line_after_completion
+116        self.clear_after_completion = clear_after_completion
+117        self.reset()
+118        self.with_context = False
+*** :params: ***
+total: The number of calls to reach 100% completion.
+update_frequency: The progress bar will only update once every this number of
+calls to display(). The larger the value, the less performance impact ProgBar
+has on the loop in which it is called. e.g.
+>>> bar = ProgBar(100, update_frequency=10)
+>>> for _ in range(100):
+>>>     bar.display()
 ^The progress bar in the terminal will only update once every ten calls, going
-from 0%->100% in 10% increments. Note: If 'total' is not a multiple of
-'update_frequency', the display will not show 100% completion when the loop
+from 0%->100% in 10% increments. Note: If total is not a multiple of
+update_frequency, the display will not show 100% completion when the loop
 finishes.
-    * fill_ch: The character used to represent the completed part of the bar.
-    * unfill_ch: The character used to represent the uncompleted part of the
-      bar.
-    * width_ratio: The width of the progress bar relative to the width of the
-      terminal window.
-    * new_line_after_completion: Make a call to print() once self.counter >=
-      self.total.
-    * clear_after_completion: Make a call to printbuddies.clear() once
-      self.counter >= self.total.
+fill_ch: The character used to represent the completed part of the bar.
+unfill_ch: The character used to represent the incomplete part of the bar.
+width_ratio: The width of the progress bar relative to the width of the
+terminal window.
+new_line_after_completion: Make a call to print() once self.counter >=
+self.total.
+clear_after_completion: Make a call to printbuddies.clear() once self.counter
+>= self.total.
 Note: if new_line_after_completion and clear_after_completion are both True,
 the line will be cleared then a call to print() will be made.
 ⁰
 def reset(self): View Source
-120    def reset(self):
-121        self.counter = 1
-122        self.percent = ""
-123        self.prefix = ""
-124        self.suffix = ""
-125        self.filled = ""
-126        self.unfilled = ""
-127        self.bar = ""
-128        self.timer = Timer(subsecond_resolution=False).start()
+130    def reset(self):
+131        self.counter = 1
+132        self.percent = ""
+133        self.prefix = ""
+134        self.suffix = ""
+135        self.filled = ""
+136        self.unfilled = ""
+137        self.timer = Timer(subsecond_resolution=False).start()
 ⁰
 def get_percent(self) -> str: View Source
-134    def get_percent(self) -> str:
-135        """Returns the percentage complete to two decimal places
-136        as a string without the %."""
-137        percent = str(round(100.0 * self.counter / self.total, 2))
-138        if len(percent.split(".")[1]) == 1:
-139            percent = percent + "0"
-140        if len(percent.split(".")[0]) == 1:
-141            percent = "0" + percent
-142        return percent
-Returns the percentage complete to two decimal places as a string without the
+147    def get_percent(self) -> str:
+148        """Returns the percentage completed to two decimal places as a
+string without the `%`."""
+149        percent = str(round(100.0 * self.counter / self.total, 2))
+150        if len(percent.split(".")[1]) == 1:
+151            percent = percent + "0"
+152        if len(percent.split(".")[0]) == 1:
+153            percent = "0" + percent
+154        return percent
+Returns the percentage completed to two decimal places as a string without the
 %.
 ⁰
 def get_bar(self): View Source
-160    def get_bar(self):
-161        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
+171    def get_bar(self):
+172        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}
 {self.unfilled}]-{self.percent}% {self.suffix}"
 ⁰
 def display(
 self,
 prefix: str = '',
 suffix: str = '',
 counter_override: float | None = None,
 total_override: float | None = None,
 return_object: typing.Any | None = None) -> Any: View Source
-163    def display(
-164        self,
-165        prefix: str = "",
-166        suffix: str = "",
-167        counter_override: float | None = None,
-168        total_override: float | None = None,
-169        return_object: Any | None = None,
-170    ) -> Any:
-171        """Writes the progress bar to the terminal.
-172
-173        :param prefix: String affixed to the front of the progress bar.
-174
-175        :param suffix: String appended to the end of the progress bar.
-176
-177        :param counter_override: When an externally incremented completion
+174    def display(
+175        self,
+176        prefix: str = "",
+177        suffix: str = "",
+178        counter_override: float | None = None,
+179        total_override: float | None = None,
+180        return_object: Any | None = None,
+181    ) -> Any:
+182        """Writes the progress bar to the terminal.
+183
+184        #### :params:
+185
+186        `prefix`: String affixed to the front of the progress bar.
+187
+188        `suffix`: String appended to the end of the progress bar.
+189
+190        `counter_override`: When an externally incremented completion
 counter is needed.
-178
-179        :param total_override: When an externally controlled bar total is
-needed.
-180
-181        :param return_object: An object to be returned by display().
-182
-183        Allows display() to be called within a comprehension:
-184
-185        e.g.
-186
-187        >>> bar = ProgBar(10)
-188        >>> def square(x: int | float)->int|float:
-189        >>>     return x * x
-190        >>> myList = [bar.display(return_object=square(i)) for i in range
+191
+192        `total_override`: When an externally controlled bar total is needed.
+193
+194        `return_object`: An object to be returned by display().
+195        Allows `display()` to be called within a comprehension:
+196
+197        e.g.
+198
+199        >>> bar = ProgBar(10)
+200        >>> def square(x: int | float)->int|float:
+201        >>>     return x * x
+202        >>> myList = [bar.display(return_object=square(i)) for i in range
 (10)]
-191        >>> <progress bar gets displayed>
-192        >>> myList
-193        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
-194        if not self.timer.started:
-195            self.timer.start()
-196        if counter_override is not None:
-197            self.counter = counter_override
-198        if total_override:
-199            self.total = total_override
-200        # Don't wanna divide by 0 there, pal
-201        while self.total <= 0:
-202            self.total += 1
-203        if self.counter % self.update_frequency == 0:
-204            self.prefix = prefix
-205            self.suffix = suffix
-206            self._prepare_bar()
-207            self._trim_bar()
-208            pad = " " * (self.terminal_width - len(self.bar))
-209            width = get_terminal_size().columns
-210            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-211        if self.counter >= self.total:
-212            self.timer.stop()
-213            if not self.with_context:
-214                if self.clear_after_completion:
-215                    clear()
-216                if self.new_line_after_completion:
-217                    print()
-218        self.counter += 1
-219        return return_object
+203        >>> <progress bar gets displayed>
+204        >>> myList
+205        >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]"""
+206        if not self.timer.started:
+207            self.timer.start()
+208        if counter_override is not None:
+209            self.counter = counter_override
+210        if total_override:
+211            self.total = total_override
+212        # Don't wanna divide by 0 there, pal
+213        while self.total <= 0:
+214            self.total += 1
+215        try:
+216            if self.counter % self.update_frequency == 0:
+217                self.prefix = prefix
+218                self.suffix = suffix
+219                self._prepare_bar()
+220                self._trim_bar()
+221                pad = " " * (self.terminal_width - len(self.bar))
+222                width = get_terminal_size().columns
+223                print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+224            if self.counter >= self.total:
+225                self.timer.stop()
+226                if not self.with_context:
+227                    if self.clear_after_completion:
+228                        clear()
+229                    if self.new_line_after_completion:
+230                        print()
+231            self.counter += 1
+232        except OSError:
+233            ...
+234        except Exception as e:
+235            raise e
+236        return return_object
 Writes the progress bar to the terminal.
-* Parameters *
-    * prefix: String affixed to the front of the progress bar.
-    * suffix: String appended to the end of the progress bar.
-    * counter_override: When an externally incremented completion counter is
-      needed.
-    * total_override: When an externally controlled bar total is needed.
-    * return_object: An object to be returned by display().
-Allows display() to be called within a comprehension:
+*** :params: ***
+prefix: String affixed to the front of the progress bar.
+suffix: String appended to the end of the progress bar.
+counter_override: When an externally incremented completion counter is needed.
+total_override: When an externally controlled bar total is needed.
+return_object: An object to be returned by display(). Allows display() to be
+called within a comprehension:
 e.g.
 >>> bar = ProgBar(10)
 >>> def square(x: int | float)->int|float:
 >>>     return x * x
 >>> myList = [bar.display(return_object=square(i)) for i in range(10)]
 >>> <progress bar gets displayed>
 >>> myList
 >>> [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
   ⁰
 class Spinner: View Source
-222class Spinner:
-223    """Prints one of a sequence of characters in order everytime display()
+239class Spinner:
+240    """Prints one of a sequence of characters in order everytime `display()`
 is called.
-224
-225    The display function writes the new character to the same line,
+241
+242    The `display` function writes the new character to the same line,
 overwriting the previous character.
-226
-227    The sequence will be cycled through indefinitely.
-228
-229    If used as a context manager, the last printed character will be cleared
+243
+244    The sequence will be cycled through indefinitely.
+245
+246    If used as a context manager, the last printed character will be cleared
 upon exiting.
-230    """
-231
-232    def __init__(
-233        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+247    """
+248
+249    def __init__(
+250        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
 0.25
-234    ):
-235        """
-236        :param sequence: Override the built in spin sequence.
-237
-238        :param width: The fractional amount of the terminal for characters
+251    ):
+252        """
+253        #### params:
+254
+255        `sequence`: Override the built in spin sequence.
+256
+257        `width_ratio`: The fractional amount of the terminal for characters
 to move across."""
-239        self._base_sequence = sequence
-240        self.width_ratio = width_ratio
-241        self.sequence = self._base_sequence
-242
-243    def __enter__(self):
-244        return self
-245
-246    def __exit__(self, *args, **kwargs):
-247        clear()
-248
-249    @property
-250    def width_ratio(self) -> float:
-251        return self._width_ratio
-252
-253    @width_ratio.setter
-254    def width_ratio(self, ratio: float):
-255        self._width_ratio = ratio
-256        self._update_width()
-257
-258    def _update_width(self):
-259        self._current_terminal_width = get_terminal_size().columns
-260        self._width = int((self._current_terminal_width - 1) *
-self.width_ratio)
+258        self._base_sequence = sequence
+259        self.width_ratio = width_ratio
+260        self.sequence = self._base_sequence
 261
-262    @property
-263    def sequence(self) -> list[Any]:
-264        return self._sequence
-265
-266    @sequence.setter
-267    def sequence(self, character_list: list[Any]):
-268        self._sequence = [
-269            ch.rjust(i + j)
-270            for i in range(1, self._width, len(character_list))
-271            for j, ch in enumerate(character_list)
-272        ]
-273        self._sequence += self._sequence[::-1]
-274
-275    def _get_next(self) -> str:
-276        """Pop the first element of self._sequence, append it to the end,
-and return the element."""
-277        ch = self.sequence.pop(0)
-278        self.sequence.append(ch)
-279        return ch
+262    def __enter__(self):
+263        return self
+264
+265    def __exit__(self, *args, **kwargs):
+266        clear()
+267
+268    @property
+269    def width_ratio(self) -> float:
+270        return self._width_ratio
+271
+272    @width_ratio.setter
+273    def width_ratio(self, ratio: float):
+274        self._width_ratio = ratio
+275        self._update_width()
+276
+277    def _update_width(self):
+278        self._current_terminal_width = get_terminal_size().columns
+279        self._width = int((self._current_terminal_width - 1) *
+self.width_ratio)
 280
-281    def display(self):
-282        """Print the next character in the sequence."""
-283        if get_terminal_size().columns != self._current_terminal_width:
-284            self._update_width()
-285            self.sequence = self._base_sequence
-286        print_in_place(self._get_next())
+281    @property
+282    def sequence(self) -> list[Any]:
+283        return self._sequence
+284
+285    @sequence.setter
+286    def sequence(self, character_list: list[Any]):
+287        self._sequence = [
+288            ch.rjust(i + j)
+289            for i in range(1, self._width, len(character_list))
+290            for j, ch in enumerate(character_list)
+291        ]
+292        self._sequence += self._sequence[::-1]
+293
+294    def _get_next(self) -> str:
+295        """Pop the first element of `self._sequence`, append it to the end,
+and return the element."""
+296        ch = self.sequence.pop(0)
+297        self.sequence.append(ch)
+298        return ch
+299
+300    def display(self):
+301        """Print the next character in the sequence."""
+302        try:
+303            if get_terminal_size().columns != self._current_terminal_width:
+304                self._update_width()
+305                self.sequence = self._base_sequence
+306            print_in_place(self._get_next())
+307        except OSError:
+308            ...
+309        except Exception as e:
+310            raise e
 Prints one of a sequence of characters in order everytime display() is called.
 The display function writes the new character to the same line, overwriting the
 previous character.
 The sequence will be cycled through indefinitely.
 If used as a context manager, the last printed character will be cleared upon
 exiting.
 ⁰
 Spinner(sequence: list[str] = ['/', '-', '\\'], width_ratio: float = 0.25) View
 Source
-232    def __init__(
-233        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
+249    def __init__(
+250        self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float =
 0.25
-234    ):
-235        """
-236        :param sequence: Override the built in spin sequence.
-237
-238        :param width: The fractional amount of the terminal for characters
+251    ):
+252        """
+253        #### params:
+254
+255        `sequence`: Override the built in spin sequence.
+256
+257        `width_ratio`: The fractional amount of the terminal for characters
 to move across."""
-239        self._base_sequence = sequence
-240        self.width_ratio = width_ratio
-241        self.sequence = self._base_sequence
-* Parameters *
-    * sequence: Override the built in spin sequence.
-    * width: The fractional amount of the terminal for characters to move
-      across.
+258        self._base_sequence = sequence
+259        self.width_ratio = width_ratio
+260        self.sequence = self._base_sequence
+*** params: ***
+sequence: Override the built in spin sequence.
+width_ratio: The fractional amount of the terminal for characters to move
+across.
 ⁰
 def display(self): View Source
-281    def display(self):
-282        """Print the next character in the sequence."""
-283        if get_terminal_size().columns != self._current_terminal_width:
-284            self._update_width()
-285            self.sequence = self._base_sequence
-286        print_in_place(self._get_next())
+300    def display(self):
+301        """Print the next character in the sequence."""
+302        try:
+303            if get_terminal_size().columns != self._current_terminal_width:
+304                self._update_width()
+305                self.sequence = self._base_sequence
+306            print_in_place(self._get_next())
+307        except OSError:
+308            ...
+309        except Exception as e:
+310            raise e
 Print the next character in the sequence.
```

### Comparing `printbuddies-1.3.0/src/printbuddies/printbuddies.py` & `printbuddies-1.3.1/src/printbuddies/printbuddies.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,103 +3,113 @@
 from typing import Any
 
 from noiftimer import Timer
 
 
 def clear():
     """Erase the current line from the terminal."""
-    print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
+    try:
+        print(" " * (get_terminal_size().columns - 1), flush=True, end="\r")
+    except OSError:
+        ...
+    except Exception as e:
+        raise e
 
 
 def print_in_place(string: str, animate: bool = False, animate_refresh: float = 0.01):
-    """Calls to print_in_place will overwrite
-    the previous line of text in the terminal
-    with the 'string' param.
-
-    :param animate: Will cause the string
-    to be printed to the terminal
-    one character at a time.
-
-    :param animate_refresh: Number of seconds
-    between the addition of characters
-    when 'animate' is True."""
+    """Calls to `print_in_place` will overwrite the previous line of text in the terminal with `string`.
+
+    #### :params:
+
+    `animate`: Will cause `string` to be printed to the terminal one character at a time.
+
+    `animate_refresh`: Number of seconds between the addition of characters when `animate` is `True`."""
     clear()
     string = str(string)
-    width = get_terminal_size().columns
-    string = string[: width - 2]
-    if animate:
-        for i in range(len(string)):
-            print(f"{string[:i+1]}", flush=True, end=" \r")
-            sleep(animate_refresh)
-    else:
-        print(string, flush=True, end="\r")
+    try:
+        width = get_terminal_size().columns
+        string = string[: width - 2]
+        if animate:
+            for i in range(len(string)):
+                print(f"{string[:i+1]}", flush=True, end=" \r")
+                sleep(animate_refresh)
+        else:
+            print(string, flush=True, end="\r")
+    except OSError:
+        ...
+    except Exception as e:
+        raise e
 
 
 def ticker(info: list[str]):
-    """Prints info to terminal with
-    top and bottom padding so that repeated
-    calls print info without showing previous
-    outputs from ticker calls.
-
-    Similar visually to print_in_place,
-    but for multiple lines."""
-    width = get_terminal_size().columns
-    info = [str(line)[: width - 1] for line in info]
-    height = get_terminal_size().lines - len(info)
-    print("\n" * (height * 2), end="")
-    print(*info, sep="\n", end="")
-    print("\n" * (int((height) / 2)), end="")
+    """Prints `info` to terminal with top and bottom padding so that previous text is not visible.
+
+    Similar visually to `print_in_place`, but for multiple lines."""
+    try:
+        width = get_terminal_size().columns
+        info = [str(line)[: width - 1] for line in info]
+        height = get_terminal_size().lines - len(info)
+        print("\n" * (height * 2), end="")
+        print(*info, sep="\n", end="")
+        print("\n" * (int((height) / 2)), end="")
+    except OSError:
+        ...
+    except Exception as e:
+        raise e
 
 
 class ProgBar:
     """Self incrementing, dynamically sized progress bar.
 
     Includes an internal timer that starts when this object is created.
-    It can be easily added to the progress bar display by adding
-    the 'runtime' property to display's prefix or suffix param:
+
+    Easily add runtime to progress display:
 
     >>> bar = ProgBar(total=100)
     >>> time.sleep(30)
-    >>> bar.display(prefix=bar.runtime)
-    >>> "runtime: 30s [_///////////////////]1.00%" """
+    >>> bar.display(prefix=f"Doin stuff ~ {bar.runtime}")
+    >>> "Doin stuff ~ runtime: 30s [_///////////////////]-1.00%" """
 
     def __init__(
         self,
         total: float,
         update_frequency: int = 1,
         fill_ch: str = "_",
         unfill_ch: str = "/",
-        width_ratio: float = 0.75,
+        width_ratio: float = 0.5,
         new_line_after_completion: bool = True,
         clear_after_completion: bool = False,
     ):
-        """:param total: The number of calls to reach 100% completion.
+        """
+        #### :params:
 
-        :param update_frequency: The progress bar will only update once every this number of calls to display().
-        The larger the value, the less performance impact ProgBar has on the loop in which it is called.
+        `total`: The number of calls to reach 100% completion.
+
+        `update_frequency`: The progress bar will only update once every this number of calls to `display()`.
+        The larger the value, the less performance impact `ProgBar` has on the loop in which it is called.
         e.g.
         >>> bar = ProgBar(100, update_frequency=10)
         >>> for _ in range(100):
         >>>     bar.display()
 
         ^The progress bar in the terminal will only update once every ten calls, going from 0%->100% in 10% increments.
-        Note: If 'total' is not a multiple of 'update_frequency', the display will not show 100% completion when the loop finishes.
+        Note: If `total` is not a multiple of `update_frequency`, the display will not show 100% completion when the loop finishes.
 
-        :param fill_ch: The character used to represent the completed part of the bar.
+        `fill_ch`: The character used to represent the completed part of the bar.
 
-        :param unfill_ch: The character used to represent the uncompleted part of the bar.
+        `unfill_ch`: The character used to represent the incomplete part of the bar.
 
-        :param width_ratio: The width of the progress bar relative to the width of the terminal window.
+        `width_ratio`: The width of the progress bar relative to the width of the terminal window.
 
-        :param new_line_after_completion: Make a call to print() once self.counter >= self.total.
+        `new_line_after_completion`: Make a call to `print()` once `self.counter >= self.total`.
 
-        :param clear_after_completion: Make a call to printbuddies.clear() once self.counter >= self.total.
+        `clear_after_completion`: Make a call to `printbuddies.clear()` once `self.counter >= self.total`.
 
-        Note: if new_line_after_completion and clear_after_completion are both True, the line will be cleared
-        then a call to print() will be made."""
+        Note: if `new_line_after_completion` and `clear_after_completion` are both `True`, the line will be cleared
+        then a call to `print()` will be made."""
         self.total = total
         self.update_frequency = update_frequency
         self.fill_ch = fill_ch[0]
         self.unfill_ch = unfill_ch[0]
         self.width_ratio = width_ratio
         self.new_line_after_completion = new_line_after_completion
         self.clear_after_completion = clear_after_completion
@@ -119,39 +129,40 @@
     def reset(self):
         self.counter = 1
         self.percent = ""
         self.prefix = ""
         self.suffix = ""
         self.filled = ""
         self.unfilled = ""
-        self.bar = ""
         self.timer = Timer(subsecond_resolution=False).start()
 
     @property
     def runtime(self) -> str:
         return f"runtime:{self.timer.elapsed_str}"
 
+    @property
+    def bar(self) -> str:
+        return f"{self.prefix}{' '*bool(self.prefix)}[{self.filled}{self.unfilled}]-{self.percent}% {self.suffix}"
+
     def get_percent(self) -> str:
-        """Returns the percentage complete to two decimal places
-        as a string without the %."""
+        """Returns the percentage completed to two decimal places as a string without the `%`."""
         percent = str(round(100.0 * self.counter / self.total, 2))
         if len(percent.split(".")[1]) == 1:
             percent = percent + "0"
         if len(percent.split(".")[0]) == 1:
             percent = "0" + percent
         return percent
 
     def _prepare_bar(self):
         self.terminal_width = get_terminal_size().columns - 1
         bar_length = int(self.terminal_width * self.width_ratio)
         progress = int(bar_length * min(self.counter / self.total, 1.0))
         self.filled = self.fill_ch * progress
         self.unfilled = self.unfill_ch * (bar_length - progress)
         self.percent = self.get_percent()
-        self.bar = self.get_bar()
 
     def _trim_bar(self):
         original_width = self.width_ratio
         while len(self.bar) > self.terminal_width and self.width_ratio > 0:
             self.width_ratio -= 0.01
             self._prepare_bar()
         self.width_ratio = original_width
@@ -165,25 +176,26 @@
         suffix: str = "",
         counter_override: float | None = None,
         total_override: float | None = None,
         return_object: Any | None = None,
     ) -> Any:
         """Writes the progress bar to the terminal.
 
-        :param prefix: String affixed to the front of the progress bar.
+        #### :params:
 
-        :param suffix: String appended to the end of the progress bar.
+        `prefix`: String affixed to the front of the progress bar.
 
-        :param counter_override: When an externally incremented completion counter is needed.
+        `suffix`: String appended to the end of the progress bar.
 
-        :param total_override: When an externally controlled bar total is needed.
+        `counter_override`: When an externally incremented completion counter is needed.
 
-        :param return_object: An object to be returned by display().
+        `total_override`: When an externally controlled bar total is needed.
 
-        Allows display() to be called within a comprehension:
+        `return_object`: An object to be returned by display().
+        Allows `display()` to be called within a comprehension:
 
         e.g.
 
         >>> bar = ProgBar(10)
         >>> def square(x: int | float)->int|float:
         >>>     return x * x
         >>> myList = [bar.display(return_object=square(i)) for i in range(10)]
@@ -195,50 +207,57 @@
         if counter_override is not None:
             self.counter = counter_override
         if total_override:
             self.total = total_override
         # Don't wanna divide by 0 there, pal
         while self.total <= 0:
             self.total += 1
-        if self.counter % self.update_frequency == 0:
-            self.prefix = prefix
-            self.suffix = suffix
-            self._prepare_bar()
-            self._trim_bar()
-            pad = " " * (self.terminal_width - len(self.bar))
-            width = get_terminal_size().columns
-            print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
-        if self.counter >= self.total:
-            self.timer.stop()
-            if not self.with_context:
-                if self.clear_after_completion:
-                    clear()
-                if self.new_line_after_completion:
-                    print()
-        self.counter += 1
+        try:
+            if self.counter % self.update_frequency == 0:
+                self.prefix = prefix
+                self.suffix = suffix
+                self._prepare_bar()
+                self._trim_bar()
+                pad = " " * (self.terminal_width - len(self.bar))
+                width = get_terminal_size().columns
+                print(f"{self.bar}{pad}"[: width - 2], flush=True, end="\r")
+            if self.counter >= self.total:
+                self.timer.stop()
+                if not self.with_context:
+                    if self.clear_after_completion:
+                        clear()
+                    if self.new_line_after_completion:
+                        print()
+            self.counter += 1
+        except OSError:
+            ...
+        except Exception as e:
+            raise e
         return return_object
 
 
 class Spinner:
-    """Prints one of a sequence of characters in order everytime display() is called.
+    """Prints one of a sequence of characters in order everytime `display()` is called.
 
-    The display function writes the new character to the same line, overwriting the previous character.
+    The `display` function writes the new character to the same line, overwriting the previous character.
 
     The sequence will be cycled through indefinitely.
 
     If used as a context manager, the last printed character will be cleared upon exiting.
     """
 
     def __init__(
         self, sequence: list[str] = ["/", "-", "\\"], width_ratio: float = 0.25
     ):
         """
-        :param sequence: Override the built in spin sequence.
+        #### params:
+
+        `sequence`: Override the built in spin sequence.
 
-        :param width: The fractional amount of the terminal for characters to move across."""
+        `width_ratio`: The fractional amount of the terminal for characters to move across."""
         self._base_sequence = sequence
         self.width_ratio = width_ratio
         self.sequence = self._base_sequence
 
     def __enter__(self):
         return self
 
@@ -268,18 +287,23 @@
             ch.rjust(i + j)
             for i in range(1, self._width, len(character_list))
             for j, ch in enumerate(character_list)
         ]
         self._sequence += self._sequence[::-1]
 
     def _get_next(self) -> str:
-        """Pop the first element of self._sequence, append it to the end, and return the element."""
+        """Pop the first element of `self._sequence`, append it to the end, and return the element."""
         ch = self.sequence.pop(0)
         self.sequence.append(ch)
         return ch
 
     def display(self):
         """Print the next character in the sequence."""
-        if get_terminal_size().columns != self._current_terminal_width:
-            self._update_width()
-            self.sequence = self._base_sequence
-        print_in_place(self._get_next())
+        try:
+            if get_terminal_size().columns != self._current_terminal_width:
+                self._update_width()
+                self.sequence = self._base_sequence
+            print_in_place(self._get_next())
+        except OSError:
+            ...
+        except Exception as e:
+            raise e
```

### Comparing `printbuddies-1.3.0/LICENSE.txt` & `printbuddies-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `printbuddies-1.3.0/README.md` & `printbuddies-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # printbuddies
 
 A few utilities to do terminal printing tricks. <br>
 Install with:
 <pre>pip install printbuddies</pre>
 
-Contains one class and three functions: ProgBar, print_in_place, ticker, and clear.<br>
+Contains two classes and three functions: ProgBar, Spinner, print_in_place, ticker, and clear.<br>
 
 ### ProgBar
 
 ProgBar is a self-incrementing, dynamically sized progress bar.<br>
 The progress counter and completion values can be manually overriden if desired.<br>
 The width of the progress bar is set according to a ratio of the terminal width
 so it will be resized automatically if the terminal width is changed.<br>
```

### Comparing `printbuddies-1.3.0/pyproject.toml` & `printbuddies-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "printbuddies"
 authors = [{name="Matt Manes"}]
 description = "Handful of utilities to do printing tricks to the terminal."
-version = "1.3.0"
+version = "1.3.1"
 requires-python = ">=3.10"
 dependencies = ["noiftimer", "pytest"]
 readme = "README.md"
 keywords = [
     "terminal",
     "print",
     "printing",
```

### Comparing `printbuddies-1.3.0/PKG-INFO` & `printbuddies-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: printbuddies
-Version: 1.3.0
+Version: 1.3.1
 Summary: Handful of utilities to do printing tricks to the terminal.
 Project-URL: Homepage, https://github.com/matt-manes/printbuddies
 Project-URL: Documentation, https://github.com/matt-manes/printbuddies/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/printbuddies/tree/main/src/printbuddies
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: print,printing,progressbar,terminal
@@ -18,15 +18,15 @@
 
 # printbuddies
 
 A few utilities to do terminal printing tricks. <br>
 Install with:
 <pre>pip install printbuddies</pre>
 
-Contains one class and three functions: ProgBar, print_in_place, ticker, and clear.<br>
+Contains two classes and three functions: ProgBar, Spinner, print_in_place, ticker, and clear.<br>
 
 ### ProgBar
 
 ProgBar is a self-incrementing, dynamically sized progress bar.<br>
 The progress counter and completion values can be manually overriden if desired.<br>
 The width of the progress bar is set according to a ratio of the terminal width
 so it will be resized automatically if the terminal width is changed.<br>
```

