# Comparing `tmp/graphene-django-filter-0.6.4.tar.gz` & `tmp/graphene_django_filter-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene-django-filter-0.6.4.tar", max compression
+gzip compressed data, was "graphene_django_filter-0.6.5.tar", max compression
```

## Comparing `graphene-django-filter-0.6.4.tar` & `graphene_django_filter-0.6.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1068 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/LICENSE
--rw-r--r--   0        0        0    10546 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/README.md
--rw-r--r--   0        0        0      168 2022-04-04 11:36:37.949880 graphene-django-filter-0.6.4/graphene_django_filter/__init__.py
--rw-r--r--   0        0        0     2230 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/conf.py
--rw-r--r--   0        0        0     4859 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/connection_field.py
--rw-r--r--   0        0        0     8890 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/filter_arguments_factory.py
--rw-r--r--   0        0        0     3397 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/filters.py
--rw-r--r--   0        0        0    11948 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/filterset.py
--rw-r--r--   0        0        0     1004 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/filterset_factories.py
--rw-r--r--   0        0        0     8530 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/input_data_factories.py
--rw-r--r--   0        0        0     5332 2022-04-04 11:36:36.913880 graphene-django-filter-0.6.4/graphene_django_filter/input_types.py
--rw-r--r--   0        0        0     1532 2022-04-04 11:36:37.949880 graphene-django-filter-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    11939 2022-04-04 11:36:49.482749 graphene-django-filter-0.6.4/setup.py
--rw-r--r--   0        0        0    11667 2022-04-04 11:36:49.483684 graphene-django-filter-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/LICENSE
+-rw-r--r--   0        0        0    10546 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/README.md
+-rw-r--r--   0        0        0      168 2023-06-10 10:28:37.703345 graphene_django_filter-0.6.5/graphene_django_filter/__init__.py
+-rw-r--r--   0        0        0     2230 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/conf.py
+-rw-r--r--   0        0        0     4859 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/connection_field.py
+-rw-r--r--   0        0        0     8888 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/filter_arguments_factory.py
+-rw-r--r--   0        0        0     3397 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/filters.py
+-rw-r--r--   0        0        0    11948 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/filterset.py
+-rw-r--r--   0        0        0     1004 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/filterset_factories.py
+-rw-r--r--   0        0        0     8530 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/input_data_factories.py
+-rw-r--r--   0        0        0     5332 2023-06-10 10:28:37.007343 graphene_django_filter-0.6.5/graphene_django_filter/input_types.py
+-rw-r--r--   0        0        0     1542 2023-06-10 10:28:37.703345 graphene_django_filter-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    11672 1970-01-01 00:00:00.000000 graphene_django_filter-0.6.5/PKG-INFO
```

### Comparing `graphene-django-filter-0.6.4/LICENSE` & `graphene_django_filter-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/README.md` & `graphene_django_filter-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/conf.py` & `graphene_django_filter-0.6.5/graphene_django_filter/conf.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/connection_field.py` & `graphene_django_filter-0.6.5/graphene_django_filter/connection_field.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/filter_arguments_factory.py` & `graphene_django_filter-0.6.5/graphene_django_filter/filter_arguments_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 
     @classmethod
     def filterset_to_trees(cls, filterset_class: Type[AdvancedFilterSet]) -> List[Node]:
         """Convert a FilterSet class to trees."""
         trees: List[Node] = []
         for filter_value in filterset_class.base_filters.values():
             values = (*filter_value.field_name.split(LOOKUP_SEP), filter_value.lookup_expr)
-            if len(trees) == 0 or not any([cls.try_add_sequence(tree, values) for tree in trees]):
+            if len(trees) == 0 or not any(cls.try_add_sequence(tree, values) for tree in trees):
                 trees.append(cls.sequence_to_tree(values))
         return trees
 
     @classmethod
     def try_add_sequence(cls, root: Node, values: Sequence[str]) -> bool:
         """Try to add a sequence to a tree.
```

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/filters.py` & `graphene_django_filter-0.6.5/graphene_django_filter/filters.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/filterset.py` & `graphene_django_filter-0.6.5/graphene_django_filter/filterset.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/filterset_factories.py` & `graphene_django_filter-0.6.5/graphene_django_filter/filterset_factories.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/input_data_factories.py` & `graphene_django_filter-0.6.5/graphene_django_filter/input_data_factories.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/graphene_django_filter/input_types.py` & `graphene_django_filter-0.6.5/graphene_django_filter/input_types.py`

 * *Files identical despite different names*

### Comparing `graphene-django-filter-0.6.4/pyproject.toml` & `graphene_django_filter-0.6.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-filter"
-version = "0.6.4"
+version = "0.6.5"
 description = "Advanced filters for Graphene"
 authors = ["devind-team <team@devind.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/devind-team/graphene-django-filter"
 repository = "https://github.com/devind-team/graphene-django-filter"
 keywords = ["django", "graphene", "filter"]
@@ -12,39 +12,39 @@
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Framework :: Django"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-Django = "^3"
-graphene = "2.1.9"
-graphene-django = "^2.15.0"
+python = ">=3.8,<4.0"
+Django = ">=3,<4.3"
+graphene = ">=2.1.9,<4"
+graphene-django = "^3.0.0"
 django-filter = "^21.1"
 psycopg2-binary = "^2.9.3"
 stringcase = "^1.2.0"
 anytree = "^2.8.0"
 wrapt = "^1.14.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 flake8-import-order = "^0.18.1"
 flake8-docstrings = "^1.6.0"
 flake8-builtins = "^1.5.3"
 flake8-quotes = "^3.3.1"
 flake8-comprehensions = "^3.8.0"
-flake8-eradicate = "^1.2.0"
+flake8-eradicate = "^1.2.1"
 flake8-simplify = "^0.19.2"
 flake8-use-fstring = "^1.3"
-flake8-annotations = "^2.8.0"
+flake8-annotations = "^2.9.0"
 pep8-naming = "^0.12.1"
 django-seed = "^0.3.1"
 python-dotenv = "^0.20.0"
-pre-commit = "^2.17.0"
+pre-commit = "^2.19.0"
 coveralls = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
```

### Comparing `graphene-django-filter-0.6.4/setup.py` & `graphene_django_filter-0.6.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,424 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: graphene-django-filter
+Version: 0.6.5
+Summary: Advanced filters for Graphene
+Home-page: https://github.com/devind-team/graphene-django-filter
+License: MIT
+Keywords: django,graphene,filter
+Author: devind-team
+Author-email: team@devind.ru
+Requires-Python: >=3.8,<4.0
+Classifier: Framework :: Django
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=3,<4.3)
+Requires-Dist: anytree (>=2.8.0,<3.0.0)
+Requires-Dist: django-filter (>=21.1,<22.0)
+Requires-Dist: graphene (>=2.1.9,<4)
+Requires-Dist: graphene-django (>=3.0.0,<4.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
+Requires-Dist: stringcase (>=1.2.0,<2.0.0)
+Requires-Dist: wrapt (>=1.14.0,<2.0.0)
+Project-URL: Repository, https://github.com/devind-team/graphene-django-filter
+Description-Content-Type: text/markdown
 
-packages = \
-['graphene_django_filter']
+# Graphene-Django-Filter
+[![CI](https://github.com/devind-team/graphene-django-filter/workflows/CI/badge.svg)](https://github.com/devind-team/graphene-django-filter/actions)
+[![Coverage Status](https://coveralls.io/repos/github/devind-team/graphene-django-filter/badge.svg?branch=main)](https://coveralls.io/github/devind-team/graphene-django-filter?branch=main)
+[![PyPI version](https://badge.fury.io/py/graphene-django-filter.svg)](https://badge.fury.io/py/graphene-django-filter)
+[![License: MIT](https://img.shields.io/badge/License-MIT-success.svg)](https://opensource.org/licenses/MIT)
 
-package_data = \
-{'': ['*']}
+This package contains advanced filters for [graphene-django](https://github.com/graphql-python/graphene-django).
+The standard filtering feature in graphene-django relies on the [django-filter](https://github.com/carltongibson/django-filter)
+library and therefore provides the flat API without the ability to use logical operators such as
+`and`, `or` and `not`. This library makes the API nested and adds logical expressions by extension
+of the `DjangoFilterConnectionField` field and the `FilterSet` class.
+Also, the library provides some other convenient filtering features.
 
-install_requires = \
-['Django>=3,<4',
- 'anytree>=2.8.0,<3.0.0',
- 'django-filter>=21.1,<22.0',
- 'graphene-django>=2.15.0,<3.0.0',
- 'graphene==2.1.9',
- 'psycopg2-binary>=2.9.3,<3.0.0',
- 'stringcase>=1.2.0,<2.0.0',
- 'wrapt>=1.14.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'graphene-django-filter',
-    'version': '0.6.4',
-    'description': 'Advanced filters for Graphene',
-    'long_description': '# Graphene-Django-Filter\n[![CI](https://github.com/devind-team/graphene-django-filter/workflows/CI/badge.svg)](https://github.com/devind-team/graphene-django-filter/actions)\n[![Coverage Status](https://coveralls.io/repos/github/devind-team/graphene-django-filter/badge.svg?branch=main)](https://coveralls.io/github/devind-team/graphene-django-filter?branch=main)\n[![PyPI version](https://badge.fury.io/py/graphene-django-filter.svg)](https://badge.fury.io/py/graphene-django-filter)\n[![License: MIT](https://img.shields.io/badge/License-MIT-success.svg)](https://opensource.org/licenses/MIT)\n\nThis package contains advanced filters for [graphene-django](https://github.com/graphql-python/graphene-django).\nThe standard filtering feature in graphene-django relies on the [django-filter](https://github.com/carltongibson/django-filter)\nlibrary and therefore provides the flat API without the ability to use logical operators such as\n`and`, `or` and `not`. This library makes the API nested and adds logical expressions by extension\nof the `DjangoFilterConnectionField` field and the `FilterSet` class.\nAlso, the library provides some other convenient filtering features.\n\n# Installation\n```shell\n# pip\npip install graphene-django-filter\n# poetry\npoetry add graphene-django-filter\n```\n\n# Requirements\n* Python (3.7, 3.8, 3.9, 3.10)\n* Graphene-Django (2.15)\n\n# Features\n\n## Nested API with the ability to use logical operators\nTo use, simply replace all `DjangoFilterConnectionField` fields with\n`AdvancedDjangoFilterConnectionField` fields in your queries.\nAlso,if you create custom FilterSets, replace the inheritance from the `FilterSet` class\nwith the inheritance from the `AdvancedFilterSet` class.\nFor example, the following task query exposes the old flat API.\n```python\nimport graphene\nfrom django_filters import FilterSet\nfrom graphene_django import DjangoObjectType\nfrom graphene_django.filter import DjangoFilterConnectionField\n\nclass TaskFilter(FilterSet):\n    class Meta:\n        model = Task\n        fields = {\n            \'name\': (\'exact\', \'contains\'),\n            \'user__email\': (\'exact\', \'contains\'),\n            \'user__first_name\': (\'exact\', \'contains\'),\n            \'user__last_name\': (\'exact\', \'contains\'),\n        }\n\nclass UserType(DjangoObjectType):\n    class Meta:\n        model = User\n        interfaces = (graphene.relay.Node,)\n        fields = \'__all__\'\n\nclass TaskType(DjangoObjectType):\n    user = graphene.Field(UserType)\n\n    class Meta:\n        model = Task\n        interfaces = (graphene.relay.Node,)\n        fields = \'__all__\'\n        filterset_class = TaskFilter\n\nclass Query(graphene.ObjectType):\n    tasks = DjangoFilterConnectionField(TaskType)\n```\nThe flat API in which all filters are applied using the `and` operator looks like this.\n```graphql\n{\n  tasks(\n    name_Contains: "important"\n    user_Email_Contains: "john"\n    user_FirstName: "John"\n    user_LastName: "Dou"\n  ){\n    edges {\n      node {\n        id\n        name\n      }\n    }\n  }\n}\n```\nAfter replacing the field class with the `AdvancedDjangoFilterConnectionField`\nand the `FilterSet` class with the `AdvancedFilterSet`\nthe API becomes nested with support for logical expressions.\n```python\nimport graphene\nfrom graphene_django_filter import AdvancedDjangoFilterConnectionField, AdvancedFilterSet\n\nclass TaskFilter(AdvancedFilterSet):\n    class Meta:\n        model = Task\n        fields = {\n            \'name\': (\'exact\', \'contains\'),\n            \'user__email\': (\'exact\', \'contains\'),\n            \'user__first_name\': (\'exact\', \'contains\'),\n            \'user__last_name\': (\'exact\', \'contains\'),\n        }\n\nclass Query(graphene.ObjectType):\n    tasks = AdvancedDjangoFilterConnectionField(TaskType)\n```\nFor example, the following query returns tasks which names contain the word "important"\nor the user\'s email address contains the word "john" and the user\'s last name is "Dou"\nand the first name is not "John".\nNote that the operators are applied to lookups\nsuch as `contains`, `exact`, etc. at the last level of nesting.\n```graphql\n{\n  tasks(\n    filter: {\n      or: [\n        {name: {contains: "important"}}\n        {\n            and: [\n              {user: {email: {contains: "john"}}}\n              {user: {lastName: {exact: "Dou"}}}\n            ]\n        }\n      ]\n      not: {\n        user: {firstName: {exact: "John"}}\n      }\n    }\n  ) {\n    edges {\n      node {\n        id\n        name\n      }\n    }\n  }\n}\n```\nThe same result can be achieved with an alternative query structure\nbecause within the same object the `and` operator is always used.\n```graphql\n{\n  tasks(\n    filter: {\n      or: [\n        {name: {contains: "important"}}\n        {\n          user: {\n            email: {contains: "john"}\n            lastName: {exact: "Dou"}\n          }\n        }\n      ]\n      not: {\n        user: {firstName: {exact: "John"}}\n      }\n    }\n  ){\n    edges {\n      node {\n        id\n        name\n      }\n    }\n  }\n}\n```\nThe filter input type has the following structure.\n```graphql\ninput FilterInputType {\n  and: [FilterInputType]\n  or: [FilterInputType]\n  not: FilterInputType\n  ...FieldLookups\n}\n```\nFor more examples, see [tests](https://github.com/devind-team/graphene-django-filter/blob/06ed0af8def8a4378b4c65a5d137ef17b6176cab/tests/test_queries_execution.py#L23).\n\n## Full text search\nDjango provides the [API](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/)\nfor PostgreSQL full text search. Graphene-Django-Filter inject this API into the GraphQL filter API.\nTo use, add `full_text_search` lookup to fields for which you want to enable full text search.\nFor example, the following type has full text search for\n`first_name` and `last_name` fields.\n```python\nimport graphene\nfrom graphene_django import DjangoObjectType\nfrom graphene_django_filter import AdvancedDjangoFilterConnectionField\n\nclass UserType(DjangoObjectType):\n    class Meta:\n        model = User\n        interfaces = (graphene.relay.Node,)\n        fields = \'__all__\'\n        filter_fields = {\n            \'email\': (\'exact\', \'startswith\', \'contains\'),\n            \'first_name\': (\'exact\', \'contains\', \'full_text_search\'),\n            \'last_name\': (\'exact\', \'contains\', \'full_text_search\'),\n        }\n\nclass Query(graphene.ObjectType):\n    users = AdvancedDjangoFilterConnectionField(UserType)\n```\nSince this feature belongs to the AdvancedFilterSet,\nit can be used in a custom FilterSet.\nThe following example will work exactly like the previous one.\n```python\nimport graphene\nfrom graphene_django import DjangoObjectType\nfrom graphene_django_filter import AdvancedDjangoFilterConnectionField, AdvancedFilterSet\n\nclass UserFilter(AdvancedFilterSet):\n    class Meta:\n        model = User\n        fields = {\n            \'email\': (\'exact\', \'startswith\', \'contains\'),\n            \'first_name\': (\'exact\', \'contains\', \'full_text_search\'),\n            \'last_name\': (\'exact\', \'contains\', \'full_text_search\'),\n        }\n\nclass UserType(DjangoObjectType):\n    class Meta:\n        model = User\n        interfaces = (graphene.relay.Node,)\n        fields = \'__all__\'\n        filterset_class = UserFilter\n\nclass Query(graphene.ObjectType):\n    users = AdvancedDjangoFilterConnectionField(UserType)\n```\nFull text search API includes SearchQuery, SearchRank, and Trigram filters.\nSearchQuery and SearchRank filters are at the top level.\nIf some field has been enabled for full text search then it can be included in the field array.\nThe following queries show an example of using the SearchQuery and SearchRank filters.\n```graphql\n{\n  users(\n    filter: {\n      searchQuery: {\n        vector: {\n          fields: ["first_name"]\n        }\n        query: {\n          or: [\n            {value: "Bob"}\n            {value: "Alice"}\n          ]\n        }\n      }\n    }\n  ){\n    edges {\n      node {\n        id\n        firstName\n        lastName  \n      }\n    }\n  }\n}\n```\n```graphql\n{\n  users(\n    filter: {\n      searchRank: {\n        vector: {fields: ["first_name", "last_name"]}\n        query: {value: "John Dou"}\n        lookups: {gte: 0.5}\n      }\n    }\n  ){\n    edges {\n      node {\n        id\n        firstName\n        lastName  \n      }\n    }\n  }\n}\n```\nTrigram filter belongs to the corresponding field.\nThe following query shows an example of using the Trigram filter.\n```graphql\n{\n  users(\n    filter: {\n      firstName: {\n        trigram: {\n          value: "john"\n          lookups: {gte: 0.85}\n        }\n      }\n    }\n  ){\n    edges {\n      node {\n        id\n        firstName\n        lastName  \n      }\n    }\n  }\n}\n```\nInput types have the following structure.\n```graphql\ninput SearchConfigInputType {\n  value: String!\n  isField: Boolean\n}\nenum SearchVectorWeight {\n  A\n  B\n  C\n  D\n}\ninput SearchVectorInputType {\n  fields: [String!]!\n  config: SearchConfigInputType\n  weight: SearchVectorWeight\n}\nenum SearchQueryType {\n  PLAIN\n  PHRASE\n  RAW\n  WEBSEARCH\n}\ninput SearchQueryInputType {\n  value: String\n  config: SearchConfigInputType\n  and: [SearchQueryInputType]\n  or: [SearchQueryInputType]\n  not: SearchQueryInputType\n}\ninput SearchQueryFilterInputType {\n  vector: SearchVectorInputType!\n  query: SearchQueryInputType!\n}\ninput FloatLookupsInputType {\n  exact: Float\n  gt: Float\n  gte: Float\n  lt: Float\n  lte: Float\n}\ninput SearchRankWeightsInputType {\n  D: Float\n  C: Float\n  B: Float\n  A: Float\n}\ninput SearchRankFilterInputType {\n  vector: SearchVectorInputType!\n  query: SearchQueryInputType!\n  lookups: FloatLookupsInputType!\n  weights: SearchRankWeightsInputType\n  coverDensity: Boolean\n  normalization: Int\n}\nenum TrigramSearchKind {\n  SIMILARITY\n  DISTANCE\n}\ninput TrigramFilterInputType {\n  kind: TrigramSearchKind\n  lookups: FloatLookupsInputType!\n  value: String!\n}\n```\nFor more examples, see [tests](https://github.com/devind-team/graphene-django-filter/blob/06ed0af8def8a4378b4c65a5d137ef17b6176cab/tests/test_queries_execution.py#L134).\n\n## Settings\nThe library can be customised using settings.\nTo add settings, create a dictionary\nwith name `GRAPHENE_DJANGO_FILTER` in the project’s `settings.py`.\nThe default settings are as follows.\n```python\nGRAPHENE_DJANGO_FILTER = {\n    \'FILTER_KEY\': \'filter\',\n    \'AND_KEY\': \'and\',\n    \'OR_KEY\': \'or\',\n    \'NOT_KEY\': \'not\',\n}\n```\nTo read the settings, import them from the `conf` module.\n```python\nfrom graphene_django_filter.conf import settings\n\nprint(settings.FILTER_KEY)\n```\nThe `settings` object also includes fixed settings, which depend on the user\'s environment.\n`IS_POSTGRESQL` determinate that current database is PostgreSQL\nand `HAS_TRIGRAM_EXTENSION` that `pg_trgm` extension is installed.\n',
-    'author': 'devind-team',
-    'author_email': 'team@devind.ru',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/devind-team/graphene-django-filter',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+# Installation
+```shell
+# pip
+pip install graphene-django-filter
+# poetry
+poetry add graphene-django-filter
+```
+
+# Requirements
+* Python (3.7, 3.8, 3.9, 3.10)
+* Graphene-Django (2.15)
+
+# Features
+
+## Nested API with the ability to use logical operators
+To use, simply replace all `DjangoFilterConnectionField` fields with
+`AdvancedDjangoFilterConnectionField` fields in your queries.
+Also,if you create custom FilterSets, replace the inheritance from the `FilterSet` class
+with the inheritance from the `AdvancedFilterSet` class.
+For example, the following task query exposes the old flat API.
+```python
+import graphene
+from django_filters import FilterSet
+from graphene_django import DjangoObjectType
+from graphene_django.filter import DjangoFilterConnectionField
+
+class TaskFilter(FilterSet):
+    class Meta:
+        model = Task
+        fields = {
+            'name': ('exact', 'contains'),
+            'user__email': ('exact', 'contains'),
+            'user__first_name': ('exact', 'contains'),
+            'user__last_name': ('exact', 'contains'),
+        }
+
+class UserType(DjangoObjectType):
+    class Meta:
+        model = User
+        interfaces = (graphene.relay.Node,)
+        fields = '__all__'
+
+class TaskType(DjangoObjectType):
+    user = graphene.Field(UserType)
+
+    class Meta:
+        model = Task
+        interfaces = (graphene.relay.Node,)
+        fields = '__all__'
+        filterset_class = TaskFilter
+
+class Query(graphene.ObjectType):
+    tasks = DjangoFilterConnectionField(TaskType)
+```
+The flat API in which all filters are applied using the `and` operator looks like this.
+```graphql
+{
+  tasks(
+    name_Contains: "important"
+    user_Email_Contains: "john"
+    user_FirstName: "John"
+    user_LastName: "Dou"
+  ){
+    edges {
+      node {
+        id
+        name
+      }
+    }
+  }
+}
+```
+After replacing the field class with the `AdvancedDjangoFilterConnectionField`
+and the `FilterSet` class with the `AdvancedFilterSet`
+the API becomes nested with support for logical expressions.
+```python
+import graphene
+from graphene_django_filter import AdvancedDjangoFilterConnectionField, AdvancedFilterSet
+
+class TaskFilter(AdvancedFilterSet):
+    class Meta:
+        model = Task
+        fields = {
+            'name': ('exact', 'contains'),
+            'user__email': ('exact', 'contains'),
+            'user__first_name': ('exact', 'contains'),
+            'user__last_name': ('exact', 'contains'),
+        }
+
+class Query(graphene.ObjectType):
+    tasks = AdvancedDjangoFilterConnectionField(TaskType)
+```
+For example, the following query returns tasks which names contain the word "important"
+or the user's email address contains the word "john" and the user's last name is "Dou"
+and the first name is not "John".
+Note that the operators are applied to lookups
+such as `contains`, `exact`, etc. at the last level of nesting.
+```graphql
+{
+  tasks(
+    filter: {
+      or: [
+        {name: {contains: "important"}}
+        {
+            and: [
+              {user: {email: {contains: "john"}}}
+              {user: {lastName: {exact: "Dou"}}}
+            ]
+        }
+      ]
+      not: {
+        user: {firstName: {exact: "John"}}
+      }
+    }
+  ) {
+    edges {
+      node {
+        id
+        name
+      }
+    }
+  }
+}
+```
+The same result can be achieved with an alternative query structure
+because within the same object the `and` operator is always used.
+```graphql
+{
+  tasks(
+    filter: {
+      or: [
+        {name: {contains: "important"}}
+        {
+          user: {
+            email: {contains: "john"}
+            lastName: {exact: "Dou"}
+          }
+        }
+      ]
+      not: {
+        user: {firstName: {exact: "John"}}
+      }
+    }
+  ){
+    edges {
+      node {
+        id
+        name
+      }
+    }
+  }
+}
+```
+The filter input type has the following structure.
+```graphql
+input FilterInputType {
+  and: [FilterInputType]
+  or: [FilterInputType]
+  not: FilterInputType
+  ...FieldLookups
+}
+```
+For more examples, see [tests](https://github.com/devind-team/graphene-django-filter/blob/06ed0af8def8a4378b4c65a5d137ef17b6176cab/tests/test_queries_execution.py#L23).
+
+## Full text search
+Django provides the [API](https://docs.djangoproject.com/en/3.2/ref/contrib/postgres/search/)
+for PostgreSQL full text search. Graphene-Django-Filter inject this API into the GraphQL filter API.
+To use, add `full_text_search` lookup to fields for which you want to enable full text search.
+For example, the following type has full text search for
+`first_name` and `last_name` fields.
+```python
+import graphene
+from graphene_django import DjangoObjectType
+from graphene_django_filter import AdvancedDjangoFilterConnectionField
+
+class UserType(DjangoObjectType):
+    class Meta:
+        model = User
+        interfaces = (graphene.relay.Node,)
+        fields = '__all__'
+        filter_fields = {
+            'email': ('exact', 'startswith', 'contains'),
+            'first_name': ('exact', 'contains', 'full_text_search'),
+            'last_name': ('exact', 'contains', 'full_text_search'),
+        }
+
+class Query(graphene.ObjectType):
+    users = AdvancedDjangoFilterConnectionField(UserType)
+```
+Since this feature belongs to the AdvancedFilterSet,
+it can be used in a custom FilterSet.
+The following example will work exactly like the previous one.
+```python
+import graphene
+from graphene_django import DjangoObjectType
+from graphene_django_filter import AdvancedDjangoFilterConnectionField, AdvancedFilterSet
+
+class UserFilter(AdvancedFilterSet):
+    class Meta:
+        model = User
+        fields = {
+            'email': ('exact', 'startswith', 'contains'),
+            'first_name': ('exact', 'contains', 'full_text_search'),
+            'last_name': ('exact', 'contains', 'full_text_search'),
+        }
+
+class UserType(DjangoObjectType):
+    class Meta:
+        model = User
+        interfaces = (graphene.relay.Node,)
+        fields = '__all__'
+        filterset_class = UserFilter
+
+class Query(graphene.ObjectType):
+    users = AdvancedDjangoFilterConnectionField(UserType)
+```
+Full text search API includes SearchQuery, SearchRank, and Trigram filters.
+SearchQuery and SearchRank filters are at the top level.
+If some field has been enabled for full text search then it can be included in the field array.
+The following queries show an example of using the SearchQuery and SearchRank filters.
+```graphql
+{
+  users(
+    filter: {
+      searchQuery: {
+        vector: {
+          fields: ["first_name"]
+        }
+        query: {
+          or: [
+            {value: "Bob"}
+            {value: "Alice"}
+          ]
+        }
+      }
+    }
+  ){
+    edges {
+      node {
+        id
+        firstName
+        lastName  
+      }
+    }
+  }
+}
+```
+```graphql
+{
+  users(
+    filter: {
+      searchRank: {
+        vector: {fields: ["first_name", "last_name"]}
+        query: {value: "John Dou"}
+        lookups: {gte: 0.5}
+      }
+    }
+  ){
+    edges {
+      node {
+        id
+        firstName
+        lastName  
+      }
+    }
+  }
+}
+```
+Trigram filter belongs to the corresponding field.
+The following query shows an example of using the Trigram filter.
+```graphql
+{
+  users(
+    filter: {
+      firstName: {
+        trigram: {
+          value: "john"
+          lookups: {gte: 0.85}
+        }
+      }
+    }
+  ){
+    edges {
+      node {
+        id
+        firstName
+        lastName  
+      }
+    }
+  }
+}
+```
+Input types have the following structure.
+```graphql
+input SearchConfigInputType {
+  value: String!
+  isField: Boolean
+}
+enum SearchVectorWeight {
+  A
+  B
+  C
+  D
+}
+input SearchVectorInputType {
+  fields: [String!]!
+  config: SearchConfigInputType
+  weight: SearchVectorWeight
+}
+enum SearchQueryType {
+  PLAIN
+  PHRASE
+  RAW
+  WEBSEARCH
+}
+input SearchQueryInputType {
+  value: String
+  config: SearchConfigInputType
+  and: [SearchQueryInputType]
+  or: [SearchQueryInputType]
+  not: SearchQueryInputType
+}
+input SearchQueryFilterInputType {
+  vector: SearchVectorInputType!
+  query: SearchQueryInputType!
+}
+input FloatLookupsInputType {
+  exact: Float
+  gt: Float
+  gte: Float
+  lt: Float
+  lte: Float
+}
+input SearchRankWeightsInputType {
+  D: Float
+  C: Float
+  B: Float
+  A: Float
+}
+input SearchRankFilterInputType {
+  vector: SearchVectorInputType!
+  query: SearchQueryInputType!
+  lookups: FloatLookupsInputType!
+  weights: SearchRankWeightsInputType
+  coverDensity: Boolean
+  normalization: Int
+}
+enum TrigramSearchKind {
+  SIMILARITY
+  DISTANCE
+}
+input TrigramFilterInputType {
+  kind: TrigramSearchKind
+  lookups: FloatLookupsInputType!
+  value: String!
+}
+```
+For more examples, see [tests](https://github.com/devind-team/graphene-django-filter/blob/06ed0af8def8a4378b4c65a5d137ef17b6176cab/tests/test_queries_execution.py#L134).
+
+## Settings
+The library can be customised using settings.
+To add settings, create a dictionary
+with name `GRAPHENE_DJANGO_FILTER` in the project’s `settings.py`.
+The default settings are as follows.
+```python
+GRAPHENE_DJANGO_FILTER = {
+    'FILTER_KEY': 'filter',
+    'AND_KEY': 'and',
+    'OR_KEY': 'or',
+    'NOT_KEY': 'not',
 }
+```
+To read the settings, import them from the `conf` module.
+```python
+from graphene_django_filter.conf import settings
 
+print(settings.FILTER_KEY)
+```
+The `settings` object also includes fixed settings, which depend on the user's environment.
+`IS_POSTGRESQL` determinate that current database is PostgreSQL
+and `HAS_TRIGRAM_EXTENSION` that `pg_trgm` extension is installed.
 
-setup(**setup_kwargs)
```

