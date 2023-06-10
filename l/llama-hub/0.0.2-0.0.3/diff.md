# Comparing `tmp/llama_hub-0.0.2.tar.gz` & `tmp/llama_hub-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_hub-0.0.2.tar", max compression
+gzip compressed data, was "llama_hub-0.0.3.tar", max compression
```

## Comparing `llama_hub-0.0.2.tar` & `llama_hub-0.0.3.tar`

### file list

```diff
@@ -1,439 +1,447 @@
--rw-r--r--   0        0        0     1064 2023-04-18 06:55:56.425923 llama_hub-0.0.2/LICENSE
--rw-r--r--   0        0        0     6505 2023-05-31 00:19:23.700889 llama_hub-0.0.2/README.md
--rw-r--r--   0        0        0      247 2023-05-31 00:19:23.701017 llama_hub-0.0.2/llama_hub/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701087 llama_hub-0.0.2/llama_hub/__init__.py
--rwxr-xr-x   0        0        0      119 2023-05-31 00:19:23.701156 llama_hub-0.0.2/llama_hub/add_loader.sh
--rw-r--r--   0        0        0      826 2023-05-31 00:19:23.701312 llama_hub-0.0.2/llama_hub/airtable/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701382 llama_hub-0.0.2/llama_hub/airtable/__init__.py
--rw-r--r--   0        0        0      901 2023-05-31 00:19:23.701488 llama_hub-0.0.2/llama_hub/airtable/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.701580 llama_hub-0.0.2/llama_hub/airtable/requirements.txt
--rw-r--r--   0        0        0     1839 2023-05-31 00:19:23.701803 llama_hub-0.0.2/llama_hub/apify/actor/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701871 llama_hub-0.0.2/llama_hub/apify/actor/__init__.py
--rw-r--r--   0        0        0     2474 2023-05-31 00:19:23.702257 llama_hub-0.0.2/llama_hub/apify/actor/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702389 llama_hub-0.0.2/llama_hub/apify/actor/requirements.txt
--rw-r--r--   0        0        0     1499 2023-05-31 00:19:23.702551 llama_hub-0.0.2/llama_hub/apify/dataset/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.702623 llama_hub-0.0.2/llama_hub/apify/dataset/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-31 00:19:23.702732 llama_hub-0.0.2/llama_hub/apify/dataset/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702829 llama_hub-0.0.2/llama_hub/apify/dataset/requirements.txt
--rw-r--r--   0        0        0      778 2023-05-31 00:19:23.702978 llama_hub-0.0.2/llama_hub/asana/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703048 llama_hub-0.0.2/llama_hub/asana/__init__.py
--rw-r--r--   0        0        0     1856 2023-05-31 00:19:23.703120 llama_hub-0.0.2/llama_hub/asana/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.703184 llama_hub-0.0.2/llama_hub/asana/requirements.txt
--rw-r--r--   0        0        0     2200 2023-05-31 00:19:23.703343 llama_hub-0.0.2/llama_hub/azcognitive_search/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703413 llama_hub-0.0.2/llama_hub/azcognitive_search/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-31 00:19:23.703514 llama_hub-0.0.2/llama_hub/azcognitive_search/base.py
--rw-r--r--   0        0        0       37 2023-05-31 00:19:23.703715 llama_hub-0.0.2/llama_hub/azcognitive_search/requirements.txt
--rw-r--r--   0        0        0     2542 2023-05-31 00:19:23.703897 llama_hub-0.0.2/llama_hub/azstorage_blob/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703969 llama_hub-0.0.2/llama_hub/azstorage_blob/__init__.py
--rw-r--r--   0        0        0     5419 2023-05-31 00:19:23.704197 llama_hub-0.0.2/llama_hub/azstorage_blob/base.py
--rw-r--r--   0        0        0       34 2023-05-31 00:19:23.704302 llama_hub-0.0.2/llama_hub/azstorage_blob/requirements.txt
--rw-r--r--   0        0        0     1077 2023-05-31 00:19:23.704450 llama_hub-0.0.2/llama_hub/bilibili/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.704513 llama_hub-0.0.2/llama_hub/bilibili/__init__.py
--rw-r--r--   0        0        0     2374 2023-05-31 00:19:23.704590 llama_hub-0.0.2/llama_hub/bilibili/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.704655 llama_hub-0.0.2/llama_hub/bilibili/requirements.txt
--rw-r--r--   0        0        0     3373 2023-05-31 00:19:23.705017 llama_hub-0.0.2/llama_hub/boarddocs/BoardDocsReader.ipynb
--rw-r--r--   0        0        0     1402 2023-05-31 00:19:23.705098 llama_hub-0.0.2/llama_hub/boarddocs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.705155 llama_hub-0.0.2/llama_hub/boarddocs/__init__.py
--rw-r--r--   0        0        0     4430 2023-05-31 00:19:23.705233 llama_hub-0.0.2/llama_hub/boarddocs/base.py
--rw-r--r--   0        0        0    19752 2023-05-31 00:19:23.705373 llama_hub-0.0.2/llama_hub/boarddocs/crawl.ipynb
--rw-r--r--   0        0        0       22 2023-05-31 00:19:23.705450 llama_hub-0.0.2/llama_hub/boarddocs/requirements.txt
--rw-r--r--   0        0        0      921 2023-05-31 00:19:23.705605 llama_hub-0.0.2/llama_hub/chatgpt_plugin/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.705665 llama_hub-0.0.2/llama_hub/chatgpt_plugin/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-31 00:19:23.705774 llama_hub-0.0.2/llama_hub/chatgpt_plugin/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705804 llama_hub-0.0.2/llama_hub/chatgpt_plugin/requirements.txt
--rw-r--r--   0        0        0     1056 2023-05-31 00:19:23.705957 llama_hub-0.0.2/llama_hub/chroma/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705990 llama_hub-0.0.2/llama_hub/chroma/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-31 00:19:23.706083 llama_hub-0.0.2/llama_hub/chroma/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.706141 llama_hub-0.0.2/llama_hub/chroma/requirements.txt
--rw-r--r--   0        0        0     2288 2023-05-31 00:19:23.706281 llama_hub-0.0.2/llama_hub/confluence/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706342 llama_hub-0.0.2/llama_hub/confluence/__init__.py
--rw-r--r--   0        0        0    11384 2023-05-31 00:19:23.706436 llama_hub-0.0.2/llama_hub/confluence/base.py
--rw-r--r--   0        0        0       80 2023-05-31 00:19:23.706544 llama_hub-0.0.2/llama_hub/confluence/requirements.txt
--rw-r--r--   0        0        0     1052 2023-05-31 00:19:23.706689 llama_hub-0.0.2/llama_hub/couchdb/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706764 llama_hub-0.0.2/llama_hub/couchdb/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-31 00:19:23.706867 llama_hub-0.0.2/llama_hub/couchdb/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.706940 llama_hub-0.0.2/llama_hub/couchdb/requirements.txt
--rw-r--r--   0        0        0      582 2023-05-31 00:19:23.707023 llama_hub-0.0.2/llama_hub/dad_jokes/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707074 llama_hub-0.0.2/llama_hub/dad_jokes/__init__.py
--rw-r--r--   0        0        0      715 2023-05-31 00:19:23.707121 llama_hub-0.0.2/llama_hub/dad_jokes/base.py
--rw-r--r--   0        0        0     1259 2023-05-31 00:19:23.707209 llama_hub-0.0.2/llama_hub/database/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707265 llama_hub-0.0.2/llama_hub/database/__init__.py
--rw-r--r--   0        0        0     3328 2023-05-31 00:19:23.707352 llama_hub-0.0.2/llama_hub/database/base.py
--rw-r--r--   0        0        0     1096 2023-05-31 00:19:23.707478 llama_hub-0.0.2/llama_hub/deeplake/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.707559 llama_hub-0.0.2/llama_hub/deeplake/__init__.py
--rw-r--r--   0        0        0     3457 2023-05-31 00:19:23.707661 llama_hub-0.0.2/llama_hub/deeplake/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.707752 llama_hub-0.0.2/llama_hub/deeplake/requirements.txt
--rw-r--r--   0        0        0      851 2023-05-31 00:19:23.707833 llama_hub-0.0.2/llama_hub/discord/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707879 llama_hub-0.0.2/llama_hub/discord/__init__.py
--rw-r--r--   0        0        0     4650 2023-05-31 00:19:23.707939 llama_hub-0.0.2/llama_hub/discord/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.707985 llama_hub-0.0.2/llama_hub/discord/requirements.txt
--rw-r--r--   0        0        0     4153 2023-05-31 00:19:23.708074 llama_hub-0.0.2/llama_hub/docugami/README.md
--rw-r--r--   0        0        0        4 2023-05-31 00:19:23.708125 llama_hub-0.0.2/llama_hub/docugami/__init__.py
--rw-r--r--   0        0        0    12075 2023-05-31 00:19:23.708201 llama_hub-0.0.2/llama_hub/docugami/base.py
--rw-r--r--   0        0        0    65833 2023-05-31 00:19:23.708412 llama_hub-0.0.2/llama_hub/docugami/docugami.ipynb
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.708465 llama_hub-0.0.2/llama_hub/docugami/requirements.txt
--rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.708545 llama_hub-0.0.2/llama_hub/elasticsearch/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.708572 llama_hub-0.0.2/llama_hub/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2301 2023-05-31 00:19:23.708639 llama_hub-0.0.2/llama_hub/elasticsearch/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708699 llama_hub-0.0.2/llama_hub/elasticsearch/requirements.txt
--rw-r--r--   0        0        0     1319 2023-05-31 00:19:23.708825 llama_hub-0.0.2/llama_hub/faiss/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.708885 llama_hub-0.0.2/llama_hub/faiss/__init__.py
--rw-r--r--   0        0        0     2126 2023-05-31 00:19:23.708943 llama_hub-0.0.2/llama_hub/faiss/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708986 llama_hub-0.0.2/llama_hub/faiss/requirements.txt
--rw-r--r--   0        0        0      585 2023-05-31 00:19:23.709108 llama_hub-0.0.2/llama_hub/feedly_rss/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.709136 llama_hub-0.0.2/llama_hub/feedly_rss/__init__.py
--rw-r--r--   0        0        0     2100 2023-05-31 00:19:23.709219 llama_hub-0.0.2/llama_hub/feedly_rss/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.709288 llama_hub-0.0.2/llama_hub/feedly_rss/requirements.txt
--rw-r--r--   0        0        0     2829 2023-05-31 00:19:23.709504 llama_hub-0.0.2/llama_hub/file/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709559 llama_hub-0.0.2/llama_hub/file/__init__.py
--rw-r--r--   0        0        0      858 2023-05-31 00:19:23.709669 llama_hub-0.0.2/llama_hub/file/audio/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709737 llama_hub-0.0.2/llama_hub/file/audio/__init__.py
--rw-r--r--   0        0        0     1486 2023-05-31 00:19:23.709814 llama_hub-0.0.2/llama_hub/file/audio/base.py
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.709874 llama_hub-0.0.2/llama_hub/file/audio/requirements.txt
--rw-r--r--   0        0        0     1241 2023-05-31 00:19:23.710011 llama_hub-0.0.2/llama_hub/file/audio_gladia/README.md
--rw-r--r--   0        0        0       19 2023-05-31 00:19:23.710082 llama_hub-0.0.2/llama_hub/file/audio_gladia/__init__.py
--rw-r--r--   0        0        0     3274 2023-05-31 00:19:23.710177 llama_hub-0.0.2/llama_hub/file/audio_gladia/base.py
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.710239 llama_hub-0.0.2/llama_hub/file/audio_gladia/requirements.txt
--rw-r--r--   0        0        0     5552 2023-05-31 00:19:23.710436 llama_hub-0.0.2/llama_hub/file/base.py
--rw-r--r--   0        0        0     1069 2023-05-31 00:19:23.710517 llama_hub-0.0.2/llama_hub/file/cjk_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.710563 llama_hub-0.0.2/llama_hub/file/cjk_pdf/__init__.py
--rw-r--r--   0        0        0     2584 2023-05-31 00:19:23.710634 llama_hub-0.0.2/llama_hub/file/cjk_pdf/base.py
--rw-r--r--   0        0        0       12 2023-05-31 00:19:23.710693 llama_hub-0.0.2/llama_hub/file/cjk_pdf/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-31 00:19:23.710812 llama_hub-0.0.2/llama_hub/file/deepdoctection/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.710846 llama_hub-0.0.2/llama_hub/file/deepdoctection/__init__.py
--rw-r--r--   0        0        0     1188 2023-05-31 00:19:23.710944 llama_hub-0.0.2/llama_hub/file/deepdoctection/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.711015 llama_hub-0.0.2/llama_hub/file/deepdoctection/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-31 00:19:23.711097 llama_hub-0.0.2/llama_hub/file/docx/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711148 llama_hub-0.0.2/llama_hub/file/docx/__init__.py
--rw-r--r--   0        0        0      624 2023-05-31 00:19:23.711197 llama_hub-0.0.2/llama_hub/file/docx/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.711264 llama_hub-0.0.2/llama_hub/file/docx/requirements.txt
--rw-r--r--   0        0        0      724 2023-05-31 00:19:23.711407 llama_hub-0.0.2/llama_hub/file/epub/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711459 llama_hub-0.0.2/llama_hub/file/epub/__init__.py
--rw-r--r--   0        0        0     1000 2023-05-31 00:19:23.711525 llama_hub-0.0.2/llama_hub/file/epub/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.711579 llama_hub-0.0.2/llama_hub/file/epub/requirements.txt
--rw-r--r--   0        0        0     1087 2023-05-31 00:19:23.711703 llama_hub-0.0.2/llama_hub/file/flat_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711756 llama_hub-0.0.2/llama_hub/file/flat_pdf/__init__.py
--rw-r--r--   0        0        0     2837 2023-05-31 00:19:23.711854 llama_hub-0.0.2/llama_hub/file/flat_pdf/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.711939 llama_hub-0.0.2/llama_hub/file/flat_pdf/requirements.txt
--rw-r--r--   0        0        0     1359 2023-05-31 00:19:23.712052 llama_hub-0.0.2/llama_hub/file/image/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.712114 llama_hub-0.0.2/llama_hub/file/image/__init__.py
--rw-r--r--   0        0        0     3888 2023-05-31 00:19:23.712184 llama_hub-0.0.2/llama_hub/file/image/base.py
--rw-r--r--   0        0        0       63 2023-05-31 00:19:23.712235 llama_hub-0.0.2/llama_hub/file/image/requirements.txt
--rw-r--r--   0        0        0      373 2023-05-31 00:19:23.712359 llama_hub-0.0.2/llama_hub/file/image_blip/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712384 llama_hub-0.0.2/llama_hub/file/image_blip/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-03 03:50:30.194383 llama_hub-0.0.2/llama_hub/file/image_blip/base.py
--rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712578 llama_hub-0.0.2/llama_hub/file/image_blip/requirements.txt
--rw-r--r--   0        0        0      422 2023-05-31 00:19:23.712697 llama_hub-0.0.2/llama_hub/file/image_blip2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712725 llama_hub-0.0.2/llama_hub/file/image_blip2/__init__.py
--rw-r--r--   0        0        0     3331 2023-06-03 03:50:30.194545 llama_hub-0.0.2/llama_hub/file/image_blip2/base.py
--rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712933 llama_hub-0.0.2/llama_hub/file/image_blip2/requirements.txt
--rw-r--r--   0        0        0      457 2023-05-31 00:19:23.713074 llama_hub-0.0.2/llama_hub/file/ipynb/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713111 llama_hub-0.0.2/llama_hub/file/ipynb/__init__.py
--rw-r--r--   0        0        0     1296 2023-05-31 00:19:23.713224 llama_hub-0.0.2/llama_hub/file/ipynb/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.713320 llama_hub-0.0.2/llama_hub/file/ipynb/requirements.txt
--rw-r--r--   0        0        0      735 2023-05-31 00:19:23.713712 llama_hub-0.0.2/llama_hub/file/json/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.713821 llama_hub-0.0.2/llama_hub/file/json/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-31 00:19:23.713925 llama_hub-0.0.2/llama_hub/file/json/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713956 llama_hub-0.0.2/llama_hub/file/json/requirements.txt
--rw-r--r--   0        0        0      744 2023-05-31 00:19:23.714073 llama_hub-0.0.2/llama_hub/file/markdown/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714150 llama_hub-0.0.2/llama_hub/file/markdown/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-31 00:19:23.714275 llama_hub-0.0.2/llama_hub/file/markdown/base.py
--rw-r--r--   0        0        0      680 2023-05-31 00:19:23.714381 llama_hub-0.0.2/llama_hub/file/mbox/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714447 llama_hub-0.0.2/llama_hub/file/mbox/__init__.py
--rw-r--r--   0        0        0     3604 2023-05-31 00:19:23.714680 llama_hub-0.0.2/llama_hub/file/mbox/base.py
--rw-r--r--   0        0        0       14 2023-05-31 00:19:23.714754 llama_hub-0.0.2/llama_hub/file/mbox/requirements.txt
--rw-r--r--   0        0        0      929 2023-05-31 00:19:23.714899 llama_hub-0.0.2/llama_hub/file/paged_csv/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.714940 llama_hub-0.0.2/llama_hub/file/paged_csv/__init__.py
--rw-r--r--   0        0        0      929 2023-05-31 00:19:23.715096 llama_hub-0.0.2/llama_hub/file/paged_csv/base.py
--rw-r--r--   0        0        0      786 2023-05-31 00:19:23.715234 llama_hub-0.0.2/llama_hub/file/pandas_csv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715305 llama_hub-0.0.2/llama_hub/file/pandas_csv/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-31 00:19:23.715402 llama_hub-0.0.2/llama_hub/file/pandas_csv/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715462 llama_hub-0.0.2/llama_hub/file/pandas_csv/requirements.txt
--rw-r--r--   0        0        0     1334 2023-05-31 00:19:23.715614 llama_hub-0.0.2/llama_hub/file/pandas_excel/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715680 llama_hub-0.0.2/llama_hub/file/pandas_excel/__init__.py
--rw-r--r--   0        0        0     2219 2023-05-31 00:19:23.715753 llama_hub-0.0.2/llama_hub/file/pandas_excel/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715809 llama_hub-0.0.2/llama_hub/file/pandas_excel/requirements.txt
--rw-r--r--   0        0        0      790 2023-05-31 00:19:23.715925 llama_hub-0.0.2/llama_hub/file/pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715984 llama_hub-0.0.2/llama_hub/file/pdf/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-31 00:19:23.716042 llama_hub-0.0.2/llama_hub/file/pdf/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.716096 llama_hub-0.0.2/llama_hub/file/pdf/requirements.txt
--rw-r--r--   0        0        0     1120 2023-05-31 00:19:23.716188 llama_hub-0.0.2/llama_hub/file/pptx/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716252 llama_hub-0.0.2/llama_hub/file/pptx/__init__.py
--rw-r--r--   0        0        0     3447 2023-05-31 00:19:23.716338 llama_hub-0.0.2/llama_hub/file/pptx/base.py
--rw-r--r--   0        0        0       49 2023-05-31 00:19:23.716404 llama_hub-0.0.2/llama_hub/file/pptx/requirements.txt
--rw-r--r--   0        0        0     1160 2023-05-31 00:19:23.716683 llama_hub-0.0.2/llama_hub/file/pymu_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716754 llama_hub-0.0.2/llama_hub/file/pymu_pdf/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-31 00:19:23.716819 llama_hub-0.0.2/llama_hub/file/pymu_pdf/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.716870 llama_hub-0.0.2/llama_hub/file/pymu_pdf/requirements.txt
--rw-r--r--   0        0        0      890 2023-05-31 00:19:23.716967 llama_hub-0.0.2/llama_hub/file/rdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717033 llama_hub-0.0.2/llama_hub/file/rdf/__init__.py
--rw-r--r--   0        0        0     2203 2023-05-31 00:19:23.717110 llama_hub-0.0.2/llama_hub/file/rdf/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.717167 llama_hub-0.0.2/llama_hub/file/rdf/requirements.txt
--rw-r--r--   0        0        0      792 2023-05-31 00:19:23.717279 llama_hub-0.0.2/llama_hub/file/simple_csv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717342 llama_hub-0.0.2/llama_hub/file/simple_csv/__init__.py
--rw-r--r--   0        0        0     1234 2023-05-31 00:19:23.717441 llama_hub-0.0.2/llama_hub/file/simple_csv/base.py
--rw-r--r--   0        0        0     2531 2023-05-31 00:19:23.717561 llama_hub-0.0.2/llama_hub/file/unstructured/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717635 llama_hub-0.0.2/llama_hub/file/unstructured/__init__.py
--rw-r--r--   0        0        0     1305 2023-05-31 00:19:23.717707 llama_hub-0.0.2/llama_hub/file/unstructured/base.py
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717763 llama_hub-0.0.2/llama_hub/file/unstructured/requirements.txt
--rw-r--r--   0        0        0     3068 2023-06-03 03:50:30.194696 llama_hub-0.0.2/llama_hub/github_repo/README.md
--rw-r--r--   0        0        0      153 2023-05-31 00:19:23.717979 llama_hub-0.0.2/llama_hub/github_repo/__init__.py
--rw-r--r--   0        0        0    20914 2023-06-03 03:50:30.194900 llama_hub-0.0.2/llama_hub/github_repo/base.py
--rw-r--r--   0        0        0    12721 2023-05-31 00:19:23.718674 llama_hub-0.0.2/llama_hub/github_repo/github_client.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.718740 llama_hub-0.0.2/llama_hub/github_repo/requirements.txt
--rw-r--r--   0        0        0     5709 2023-06-03 03:50:30.195070 llama_hub-0.0.2/llama_hub/github_repo/utils.py
--rw-r--r--   0        0        0      948 2023-05-31 00:19:23.719165 llama_hub-0.0.2/llama_hub/gmail/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719238 llama_hub-0.0.2/llama_hub/gmail/__init__.py
--rw-r--r--   0        0        0     5302 2023-05-31 00:19:23.719342 llama_hub-0.0.2/llama_hub/gmail/base.py
--rw-r--r--   0        0        0       81 2023-05-31 00:19:23.719438 llama_hub-0.0.2/llama_hub/gmail/requirements.txt
--rw-r--r--   0        0        0     1364 2023-05-31 00:19:23.719568 llama_hub-0.0.2/llama_hub/google_calendar/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719630 llama_hub-0.0.2/llama_hub/google_calendar/__init__.py
--rw-r--r--   0        0        0     4755 2023-05-31 00:19:23.719707 llama_hub-0.0.2/llama_hub/google_calendar/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.719771 llama_hub-0.0.2/llama_hub/google_calendar/requirements.txt
--rw-r--r--   0        0        0     2571 2023-05-31 00:19:23.719884 llama_hub-0.0.2/llama_hub/google_docs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719942 llama_hub-0.0.2/llama_hub/google_docs/__init__.py
--rw-r--r--   0        0        0     5019 2023-05-31 00:19:23.720018 llama_hub-0.0.2/llama_hub/google_docs/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720074 llama_hub-0.0.2/llama_hub/google_docs/requirements.txt
--rw-r--r--   0        0        0     1807 2023-05-31 00:19:23.720187 llama_hub-0.0.2/llama_hub/google_drive/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720244 llama_hub-0.0.2/llama_hub/google_drive/__init__.py
--rw-r--r--   0        0        0    13454 2023-06-03 03:50:30.195254 llama_hub-0.0.2/llama_hub/google_drive/base.py
--rw-r--r--   0        0        0       76 2023-05-31 00:19:23.720583 llama_hub-0.0.2/llama_hub/google_drive/requirements.txt
--rw-r--r--   0        0        0     1150 2023-05-31 00:19:23.720701 llama_hub-0.0.2/llama_hub/google_sheets/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720755 llama_hub-0.0.2/llama_hub/google_sheets/__init__.py
--rw-r--r--   0        0        0     4989 2023-05-31 00:19:23.720863 llama_hub-0.0.2/llama_hub/google_sheets/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720914 llama_hub-0.0.2/llama_hub/google_sheets/requirements.txt
--rw-r--r--   0        0        0      809 2023-05-31 00:19:23.721050 llama_hub-0.0.2/llama_hub/gpt_repo/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.721109 llama_hub-0.0.2/llama_hub/gpt_repo/__init__.py
--rw-r--r--   0        0        0     5488 2023-05-31 00:19:23.721217 llama_hub-0.0.2/llama_hub/gpt_repo/base.py
--rw-r--r--   0        0        0     1595 2023-05-31 00:19:23.721376 llama_hub-0.0.2/llama_hub/graphdb_cypher/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721443 llama_hub-0.0.2/llama_hub/graphdb_cypher/__init__.py
--rw-r--r--   0        0        0     1788 2023-05-31 00:19:23.721561 llama_hub-0.0.2/llama_hub/graphdb_cypher/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.721683 llama_hub-0.0.2/llama_hub/graphdb_cypher/requirements.txt
--rw-r--r--   0        0        0     1215 2023-05-31 00:19:23.721834 llama_hub-0.0.2/llama_hub/graphql/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721886 llama_hub-0.0.2/llama_hub/graphql/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-31 00:19:23.721979 llama_hub-0.0.2/llama_hub/graphql/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.722048 llama_hub-0.0.2/llama_hub/graphql/requirements.txt
--rw-r--r--   0        0        0      969 2023-05-31 00:19:23.722173 llama_hub-0.0.2/llama_hub/hatena_blog/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722225 llama_hub-0.0.2/llama_hub/hatena_blog/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-31 00:19:23.722316 llama_hub-0.0.2/llama_hub/hatena_blog/base.py
--rw-r--r--   0        0        0       28 2023-05-31 00:19:23.722405 llama_hub-0.0.2/llama_hub/hatena_blog/requirements.txt
--rw-r--r--   0        0        0      916 2023-05-31 00:19:23.722570 llama_hub-0.0.2/llama_hub/hubspot/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722654 llama_hub-0.0.2/llama_hub/hubspot/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-31 00:19:23.722744 llama_hub-0.0.2/llama_hub/hubspot/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.722823 llama_hub-0.0.2/llama_hub/hubspot/requirements.txt
--rw-r--r--   0        0        0     1035 2023-05-31 00:19:23.722974 llama_hub-0.0.2/llama_hub/huggingface/fs/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.723070 llama_hub-0.0.2/llama_hub/huggingface/fs/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-31 00:19:23.723162 llama_hub-0.0.2/llama_hub/huggingface/fs/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.723269 llama_hub-0.0.2/llama_hub/huggingface/fs/requirements.txt
--rw-r--r--   0        0        0      797 2023-05-31 00:19:23.723369 llama_hub-0.0.2/llama_hub/intercom/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.723425 llama_hub-0.0.2/llama_hub/intercom/__init__.py
--rw-r--r--   0        0        0     2416 2023-05-31 00:19:23.723490 llama_hub-0.0.2/llama_hub/intercom/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.723542 llama_hub-0.0.2/llama_hub/intercom/requirements.txt
--rw-r--r--   0        0        0      533 2023-05-31 00:19:23.723674 llama_hub-0.0.2/llama_hub/jira/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.723719 llama_hub-0.0.2/llama_hub/jira/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-31 00:19:23.723801 llama_hub-0.0.2/llama_hub/jira/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.723892 llama_hub-0.0.2/llama_hub/jira/requirements.txt
--rw-r--r--   0        0        0     1362 2023-05-31 00:19:23.724041 llama_hub-0.0.2/llama_hub/joplin/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724074 llama_hub-0.0.2/llama_hub/joplin/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-31 00:19:23.724310 llama_hub-0.0.2/llama_hub/joplin/base.py
--rw-r--r--   0        0        0      698 2023-05-31 00:19:23.724418 llama_hub-0.0.2/llama_hub/jsondata/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.724463 llama_hub-0.0.2/llama_hub/jsondata/__init__.py
--rw-r--r--   0        0        0     1633 2023-05-31 00:19:23.724551 llama_hub-0.0.2/llama_hub/jsondata/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724577 llama_hub-0.0.2/llama_hub/jsondata/requirements.txt
--rw-r--r--   0        0        0     7206 2023-05-31 00:19:23.724774 llama_hub-0.0.2/llama_hub/kaltura/esearch/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.724845 llama_hub-0.0.2/llama_hub/kaltura/esearch/__init__.py
--rw-r--r--   0        0        0    12019 2023-05-31 00:19:23.724953 llama_hub-0.0.2/llama_hub/kaltura/esearch/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.725038 llama_hub-0.0.2/llama_hub/kaltura/esearch/requirements.txt
--rw-r--r--   0        0        0    11434 2023-05-31 00:19:23.725176 llama_hub-0.0.2/llama_hub/library.json
--rw-r--r--   0        0        0     1117 2023-05-31 00:19:23.725289 llama_hub-0.0.2/llama_hub/make_com/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725348 llama_hub-0.0.2/llama_hub/make_com/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-31 00:19:23.725434 llama_hub-0.0.2/llama_hub/make_com/base.py
--rw-r--r--   0        0        0      810 2023-05-31 00:19:23.725515 llama_hub-0.0.2/llama_hub/mangoapps_guides/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725566 llama_hub-0.0.2/llama_hub/mangoapps_guides/__init__.py
--rw-r--r--   0        0        0     4752 2023-05-31 00:19:23.725645 llama_hub-0.0.2/llama_hub/mangoapps_guides/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.725706 llama_hub-0.0.2/llama_hub/mangoapps_guides/requirements.txt
--rw-r--r--   0        0        0     2740 2023-05-31 00:19:23.725850 llama_hub-0.0.2/llama_hub/maps/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.725903 llama_hub-0.0.2/llama_hub/maps/__init__.py
--rw-r--r--   0        0        0     4599 2023-05-31 00:19:23.726215 llama_hub-0.0.2/llama_hub/maps/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.726327 llama_hub-0.0.2/llama_hub/maps/requirements.txt
--rw-r--r--   0        0        0      870 2023-05-31 00:19:23.726449 llama_hub-0.0.2/llama_hub/memos/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726502 llama_hub-0.0.2/llama_hub/memos/__init__.py
--rw-r--r--   0        0        0     1465 2023-05-31 00:19:23.726557 llama_hub-0.0.2/llama_hub/memos/base.py
--rw-r--r--   0        0        0      952 2023-05-31 00:19:23.726641 llama_hub-0.0.2/llama_hub/metal/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726693 llama_hub-0.0.2/llama_hub/metal/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-31 00:19:23.726764 llama_hub-0.0.2/llama_hub/metal/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.726825 llama_hub-0.0.2/llama_hub/metal/requirements.txt
--rw-r--r--   0        0        0     1174 2023-05-31 00:19:23.726943 llama_hub-0.0.2/llama_hub/milvus/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.727017 llama_hub-0.0.2/llama_hub/milvus/__init__.py
--rw-r--r--   0        0        0     4588 2023-05-31 00:19:23.727112 llama_hub-0.0.2/llama_hub/milvus/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727182 llama_hub-0.0.2/llama_hub/milvus/requirements.txt
--rw-r--r--   0        0        0      853 2023-05-31 00:19:23.727268 llama_hub-0.0.2/llama_hub/mondaydotcom/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727321 llama_hub-0.0.2/llama_hub/mondaydotcom/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-31 00:19:23.727383 llama_hub-0.0.2/llama_hub/mondaydotcom/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727432 llama_hub-0.0.2/llama_hub/mondaydotcom/requirements.txt
--rw-r--r--   0        0        0      973 2023-05-31 00:19:23.727516 llama_hub-0.0.2/llama_hub/mongo/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727566 llama_hub-0.0.2/llama_hub/mongo/__init__.py
--rw-r--r--   0        0        0     2260 2023-05-31 00:19:23.727656 llama_hub-0.0.2/llama_hub/mongo/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.727743 llama_hub-0.0.2/llama_hub/mongo/requirements.txt
--rw-r--r--   0        0        0      916 2023-05-31 00:19:23.727849 llama_hub-0.0.2/llama_hub/notion/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727909 llama_hub-0.0.2/llama_hub/notion/__init__.py
--rw-r--r--   0        0        0     6102 2023-05-31 00:19:23.727971 llama_hub-0.0.2/llama_hub/notion/base.py
--rw-r--r--   0        0        0      395 2023-06-01 05:01:36.458116 llama_hub-0.0.2/llama_hub/notion/tool.py
--rw-r--r--   0        0        0      688 2023-05-31 00:19:23.728057 llama_hub-0.0.2/llama_hub/obsidian/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728106 llama_hub-0.0.2/llama_hub/obsidian/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-31 00:19:23.728167 llama_hub-0.0.2/llama_hub/obsidian/base.py
--rw-r--r--   0        0        0     1050 2023-05-31 00:19:23.728304 llama_hub-0.0.2/llama_hub/opendal_reader/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.728335 llama_hub-0.0.2/llama_hub/opendal_reader/__init__.py
--rw-r--r--   0        0        0      980 2023-05-31 00:19:23.728466 llama_hub-0.0.2/llama_hub/opendal_reader/azblob/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728521 llama_hub-0.0.2/llama_hub/opendal_reader/azblob/__init__.py
--rw-r--r--   0        0        0     2476 2023-05-31 00:19:23.728643 llama_hub-0.0.2/llama_hub/opendal_reader/azblob/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.728751 llama_hub-0.0.2/llama_hub/opendal_reader/azblob/requirements.txt
--rw-r--r--   0        0        0     2979 2023-05-31 00:19:23.728891 llama_hub-0.0.2/llama_hub/opendal_reader/base.py
--rw-r--r--   0        0        0      999 2023-05-31 00:19:23.729020 llama_hub-0.0.2/llama_hub/opendal_reader/gcs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729087 llama_hub-0.0.2/llama_hub/opendal_reader/gcs/__init__.py
--rw-r--r--   0        0        0     2294 2023-05-31 00:19:23.729212 llama_hub-0.0.2/llama_hub/opendal_reader/gcs/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729283 llama_hub-0.0.2/llama_hub/opendal_reader/gcs/requirements.txt
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729358 llama_hub-0.0.2/llama_hub/opendal_reader/requirements.txt
--rw-r--r--   0        0        0     1397 2023-05-31 00:19:23.729481 llama_hub-0.0.2/llama_hub/opendal_reader/s3/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729530 llama_hub-0.0.2/llama_hub/opendal_reader/s3/__init__.py
--rw-r--r--   0        0        0     2605 2023-05-31 00:19:23.729641 llama_hub-0.0.2/llama_hub/opendal_reader/s3/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729714 llama_hub-0.0.2/llama_hub/opendal_reader/s3/requirements.txt
--rw-r--r--   0        0        0     2147 2023-05-31 00:19:23.729798 llama_hub-0.0.2/llama_hub/outlook_localcalendar/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729846 llama_hub-0.0.2/llama_hub/outlook_localcalendar/__init__,py
--rw-r--r--   0        0        0     3838 2023-05-31 00:19:23.729934 llama_hub-0.0.2/llama_hub/outlook_localcalendar/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730022 llama_hub-0.0.2/llama_hub/outlook_localcalendar/requirements.txt
--rw-r--r--   0        0        0     1801 2023-05-31 00:19:23.730149 llama_hub-0.0.2/llama_hub/pandas_ai/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.730219 llama_hub-0.0.2/llama_hub/pandas_ai/__init__.py
--rw-r--r--   0        0        0     3932 2023-05-31 00:19:23.730347 llama_hub-0.0.2/llama_hub/pandas_ai/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730434 llama_hub-0.0.2/llama_hub/pandas_ai/requirements.txt
--rw-r--r--   0        0        0     1484 2023-05-31 00:19:23.730555 llama_hub-0.0.2/llama_hub/papers/arxiv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730614 llama_hub-0.0.2/llama_hub/papers/arxiv/__init__.py
--rw-r--r--   0        0        0     6441 2023-05-31 00:19:23.730749 llama_hub-0.0.2/llama_hub/papers/arxiv/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.730795 llama_hub-0.0.2/llama_hub/papers/arxiv/requirements.txt
--rw-r--r--   0        0        0      931 2023-05-31 00:19:23.730889 llama_hub-0.0.2/llama_hub/papers/pubmed/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730947 llama_hub-0.0.2/llama_hub/papers/pubmed/__init__.py
--rw-r--r--   0        0        0     6168 2023-05-31 00:19:23.731053 llama_hub-0.0.2/llama_hub/papers/pubmed/base.py
--rw-r--r--   0        0        0     1279 2023-05-31 00:19:23.731154 llama_hub-0.0.2/llama_hub/pinecone/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731210 llama_hub-0.0.2/llama_hub/pinecone/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-31 00:19:23.731290 llama_hub-0.0.2/llama_hub/pinecone/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.731346 llama_hub-0.0.2/llama_hub/pinecone/requirements.txt
--rw-r--r--   0        0        0     1157 2023-05-31 00:19:23.731448 llama_hub-0.0.2/llama_hub/qdrant/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731505 llama_hub-0.0.2/llama_hub/qdrant/__init__.py
--rw-r--r--   0        0        0     6920 2023-05-31 00:19:23.731618 llama_hub-0.0.2/llama_hub/qdrant/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.731674 llama_hub-0.0.2/llama_hub/qdrant/requirements.txt
--rw-r--r--   0        0        0     1551 2023-05-31 00:19:23.731776 llama_hub-0.0.2/llama_hub/readwise/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731833 llama_hub-0.0.2/llama_hub/readwise/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-31 00:19:23.731903 llama_hub-0.0.2/llama_hub/readwise/base.py
--rw-r--r--   0        0        0     2707 2023-05-31 00:19:23.732014 llama_hub-0.0.2/llama_hub/reddit/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732079 llama_hub-0.0.2/llama_hub/reddit/__init__.py
--rw-r--r--   0        0        0     1914 2023-05-31 00:19:23.732143 llama_hub-0.0.2/llama_hub/reddit/base.py
--rw-r--r--   0        0        0       81 2023-05-31 00:19:23.732202 llama_hub-0.0.2/llama_hub/reddit/requirements.txt
--rw-r--r--   0        0        0     1330 2023-05-31 00:19:23.732308 llama_hub-0.0.2/llama_hub/remote/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732382 llama_hub-0.0.2/llama_hub/remote/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-31 00:19:23.732529 llama_hub-0.0.2/llama_hub/remote/base.py
--rw-r--r--   0        0        0     1383 2023-05-31 00:19:23.732627 llama_hub-0.0.2/llama_hub/remote_depth/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.732655 llama_hub-0.0.2/llama_hub/remote_depth/__init__.py
--rw-r--r--   0        0        0     3829 2023-05-31 00:19:23.732820 llama_hub-0.0.2/llama_hub/remote_depth/base.py
--rw-r--r--   0        0        0       31 2023-05-31 00:19:23.732887 llama_hub-0.0.2/llama_hub/remote_depth/requirements.txt
--rw-r--r--   0        0        0     1669 2023-05-31 00:19:23.732997 llama_hub-0.0.2/llama_hub/s3/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733053 llama_hub-0.0.2/llama_hub/s3/__init__.py
--rw-r--r--   0        0        0     3985 2023-05-31 00:19:23.733196 llama_hub-0.0.2/llama_hub/s3/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.733253 llama_hub-0.0.2/llama_hub/s3/requirements.txt
--rw-r--r--   0        0        0      821 2023-05-31 00:19:23.733394 llama_hub-0.0.2/llama_hub/slack/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733459 llama_hub-0.0.2/llama_hub/slack/__init__.py
--rw-r--r--   0        0        0     7499 2023-05-31 00:19:23.733536 llama_hub-0.0.2/llama_hub/slack/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.733594 llama_hub-0.0.2/llama_hub/slack/requirements.txt
--rw-r--r--   0        0        0      690 2023-05-31 00:19:23.733754 llama_hub-0.0.2/llama_hub/snscrape_twitter/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733815 llama_hub-0.0.2/llama_hub/snscrape_twitter/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-31 00:19:23.733911 llama_hub-0.0.2/llama_hub/snscrape_twitter/base.py
--rw-r--r--   0        0        0       56 2023-05-31 00:19:23.734041 llama_hub-0.0.2/llama_hub/snscrape_twitter/requirements.txt
--rw-r--r--   0        0        0     1662 2023-05-31 00:19:23.734145 llama_hub-0.0.2/llama_hub/spotify/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734204 llama_hub-0.0.2/llama_hub/spotify/__init__.py
--rw-r--r--   0        0        0     2287 2023-05-31 00:19:23.734275 llama_hub-0.0.2/llama_hub/spotify/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.734331 llama_hub-0.0.2/llama_hub/spotify/requirements.txt
--rw-r--r--   0        0        0      846 2023-05-31 00:19:23.734458 llama_hub-0.0.2/llama_hub/stackoverflow/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734518 llama_hub-0.0.2/llama_hub/stackoverflow/__init__.py
--rw-r--r--   0        0        0     6263 2023-05-31 00:19:23.734626 llama_hub-0.0.2/llama_hub/stackoverflow/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.734708 llama_hub-0.0.2/llama_hub/stackoverflow/requirements.txt
--rw-r--r--   0        0        0      936 2023-05-31 00:19:23.734832 llama_hub-0.0.2/llama_hub/steamship/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.734866 llama_hub-0.0.2/llama_hub/steamship/__init__.py
--rw-r--r--   0        0        0     3498 2023-05-31 00:19:23.734974 llama_hub-0.0.2/llama_hub/steamship/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.735057 llama_hub-0.0.2/llama_hub/steamship/requirements.txt
--rw-r--r--   0        0        0      726 2023-05-31 00:19:23.735154 llama_hub-0.0.2/llama_hub/string_iterable/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735234 llama_hub-0.0.2/llama_hub/string_iterable/__init__.py
--rw-r--r--   0        0        0      969 2023-05-31 00:19:23.735290 llama_hub-0.0.2/llama_hub/string_iterable/base.py
--rw-r--r--   0        0        0      676 2023-05-31 00:19:23.735435 llama_hub-0.0.2/llama_hub/trello/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735493 llama_hub-0.0.2/llama_hub/trello/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-31 00:19:23.735587 llama_hub-0.0.2/llama_hub/trello/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.735672 llama_hub-0.0.2/llama_hub/trello/requirements.txt
--rw-r--r--   0        0        0      924 2023-05-31 00:19:23.735778 llama_hub-0.0.2/llama_hub/twitter/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735847 llama_hub-0.0.2/llama_hub/twitter/__init__.py
--rw-r--r--   0        0        0     1777 2023-05-31 00:19:23.735917 llama_hub-0.0.2/llama_hub/twitter/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.735976 llama_hub-0.0.2/llama_hub/twitter/requirements.txt
--rw-r--r--   0        0        0      637 2023-05-31 00:19:23.736279 llama_hub-0.0.2/llama_hub/utils.py
--rw-r--r--   0        0        0     1162 2023-05-31 00:19:23.736420 llama_hub-0.0.2/llama_hub/weather/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.736481 llama_hub-0.0.2/llama_hub/weather/__init__.py
--rw-r--r--   0        0        0     2779 2023-05-31 00:19:23.736578 llama_hub-0.0.2/llama_hub/weather/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.736662 llama_hub-0.0.2/llama_hub/weather/requirements.txt
--rw-r--r--   0        0        0     1525 2023-05-31 00:19:23.736765 llama_hub-0.0.2/llama_hub/weaviate/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.736823 llama_hub-0.0.2/llama_hub/weaviate/__init__.py
--rw-r--r--   0        0        0     3697 2023-05-31 00:19:23.736889 llama_hub-0.0.2/llama_hub/weaviate/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.736940 llama_hub-0.0.2/llama_hub/weaviate/requirements.txt
--rw-r--r--   0        0        0      415 2023-05-31 00:19:23.737101 llama_hub-0.0.2/llama_hub/web/async_web/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.737136 llama_hub-0.0.2/llama_hub/web/async_web/__init__.py
--rw-r--r--   0        0        0     2554 2023-05-31 00:19:23.737236 llama_hub-0.0.2/llama_hub/web/async_web/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.737325 llama_hub-0.0.2/llama_hub/web/async_web/requirements.txt
--rw-r--r--   0        0        0     3446 2023-05-31 00:19:23.737437 llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.737504 llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/__init__.py
--rw-r--r--   0        0        0     6747 2023-05-31 00:19:23.737610 llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/base.py
--rw-r--r--   0        0        0       31 2023-05-31 00:19:23.737666 llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/requirements.txt
--rw-r--r--   0        0        0     3672 2023-05-31 00:19:23.737782 llama_hub-0.0.2/llama_hub/web/knowledge_base/README.md
--rw-r--r--   0        0        0        1 2023-05-31 00:19:23.737843 llama_hub-0.0.2/llama_hub/web/knowledge_base/__init__.py
--rw-r--r--   0        0        0     5611 2023-05-31 00:19:23.737918 llama_hub-0.0.2/llama_hub/web/knowledge_base/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.737968 llama_hub-0.0.2/llama_hub/web/knowledge_base/requirements.txt
--rw-r--r--   0        0        0     2681 2023-05-31 00:19:23.738073 llama_hub-0.0.2/llama_hub/web/readability_web/README.md
--rw-r--r--   0        0        0    83319 2023-05-31 00:19:23.738443 llama_hub-0.0.2/llama_hub/web/readability_web/Readability.js
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738513 llama_hub-0.0.2/llama_hub/web/readability_web/__init__.py
--rw-r--r--   0        0        0     4531 2023-05-31 00:19:23.738613 llama_hub-0.0.2/llama_hub/web/readability_web/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.738660 llama_hub-0.0.2/llama_hub/web/readability_web/requirements.txt
--rw-r--r--   0        0        0      489 2023-05-31 00:19:23.738734 llama_hub-0.0.2/llama_hub/web/rss/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738780 llama_hub-0.0.2/llama_hub/web/rss/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-31 00:19:23.738829 llama_hub-0.0.2/llama_hub/web/rss/base.py
--rw-r--r--   0        0        0     1994 2023-05-31 00:19:23.738914 llama_hub-0.0.2/llama_hub/web/simple_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738959 llama_hub-0.0.2/llama_hub/web/simple_web/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-31 00:19:23.739036 llama_hub-0.0.2/llama_hub/web/simple_web/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.739081 llama_hub-0.0.2/llama_hub/web/simple_web/requirements.txt
--rw-r--r--   0        0        0     2009 2023-05-31 00:19:23.739158 llama_hub-0.0.2/llama_hub/web/trafilatura_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739207 llama_hub-0.0.2/llama_hub/web/trafilatura_web/__init__.py
--rw-r--r--   0        0        0      889 2023-05-31 00:19:23.739262 llama_hub-0.0.2/llama_hub/web/trafilatura_web/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.739305 llama_hub-0.0.2/llama_hub/web/trafilatura_web/requirements.txt
--rw-r--r--   0        0        0     1075 2023-05-31 00:19:23.739438 llama_hub-0.0.2/llama_hub/web/unstructured_web/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.739468 llama_hub-0.0.2/llama_hub/web/unstructured_web/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-31 00:19:23.739541 llama_hub-0.0.2/llama_hub/web/unstructured_web/base.py
--rw-r--r--   0        0        0       12 2023-05-31 00:19:23.739609 llama_hub-0.0.2/llama_hub/web/unstructured_web/requirements.txt
--rw-r--r--   0        0        0     1315 2023-05-31 00:19:23.739686 llama_hub-0.0.2/llama_hub/whatsapp/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739729 llama_hub-0.0.2/llama_hub/whatsapp/__init__.py
--rw-r--r--   0        0        0     1509 2023-05-31 00:19:23.739776 llama_hub-0.0.2/llama_hub/whatsapp/base.py
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739818 llama_hub-0.0.2/llama_hub/whatsapp/requirements.txt
--rw-r--r--   0        0        0      895 2023-05-31 00:19:23.739897 llama_hub-0.0.2/llama_hub/wikipedia/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739946 llama_hub-0.0.2/llama_hub/wikipedia/__init__.py
--rw-r--r--   0        0        0      818 2023-05-31 00:19:23.740017 llama_hub-0.0.2/llama_hub/wikipedia/base.py
--rw-r--r--   0        0        0       14 2023-05-31 00:19:23.740060 llama_hub-0.0.2/llama_hub/wikipedia/requirements.txt
--rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.740135 llama_hub-0.0.2/llama_hub/wordpress/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740190 llama_hub-0.0.2/llama_hub/wordpress/__init__.py
--rw-r--r--   0        0        0     2546 2023-05-31 00:19:23.740248 llama_hub-0.0.2/llama_hub/wordpress/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.740291 llama_hub-0.0.2/llama_hub/wordpress/requirements.txt
--rw-r--r--   0        0        0      774 2023-05-31 00:19:23.740378 llama_hub-0.0.2/llama_hub/youtube_transcript/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740429 llama_hub-0.0.2/llama_hub/youtube_transcript/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-31 00:19:23.740509 llama_hub-0.0.2/llama_hub/youtube_transcript/base.py
--rw-r--r--   0        0        0       29 2023-05-31 00:19:23.740552 llama_hub-0.0.2/llama_hub/youtube_transcript/requirements.txt
--rw-r--r--   0        0        0      884 2023-05-31 00:19:23.740654 llama_hub-0.0.2/llama_hub/zendesk/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740708 llama_hub-0.0.2/llama_hub/zendesk/__init__.py
--rw-r--r--   0        0        0     2323 2023-05-31 00:19:23.740795 llama_hub-0.0.2/llama_hub/zendesk/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.740869 llama_hub-0.0.2/llama_hub/zendesk/requirements.txt
--rw-r--r--   0        0        0     1304 2023-05-31 00:19:23.740971 llama_hub-0.0.2/llama_hub/zulip/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.741018 llama_hub-0.0.2/llama_hub/zulip/__init__.py
--rw-r--r--   0        0        0     2432 2023-05-31 00:19:23.741092 llama_hub-0.0.2/llama_hub/zulip/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.741155 llama_hub-0.0.2/llama_hub/zulip/requirements.txt
--rw-r--r--   0        0        0      868 2023-06-03 03:50:43.975884 llama_hub-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 llama_hub-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 06:55:56.425923 llama_hub-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6505 2023-05-31 00:19:23.700889 llama_hub-0.0.3/README.md
+-rw-r--r--   0        0        0      247 2023-05-31 00:19:23.701017 llama_hub-0.0.3/llama_hub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701087 llama_hub-0.0.3/llama_hub/__init__.py
+-rwxr-xr-x   0        0        0      119 2023-05-31 00:19:23.701156 llama_hub-0.0.3/llama_hub/add_loader.sh
+-rw-r--r--   0        0        0      826 2023-05-31 00:19:23.701312 llama_hub-0.0.3/llama_hub/airtable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701382 llama_hub-0.0.3/llama_hub/airtable/__init__.py
+-rw-r--r--   0        0        0      901 2023-05-31 00:19:23.701488 llama_hub-0.0.3/llama_hub/airtable/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.701580 llama_hub-0.0.3/llama_hub/airtable/requirements.txt
+-rw-r--r--   0        0        0     1839 2023-05-31 00:19:23.701803 llama_hub-0.0.3/llama_hub/apify/actor/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701871 llama_hub-0.0.3/llama_hub/apify/actor/__init__.py
+-rw-r--r--   0        0        0     2474 2023-05-31 00:19:23.702257 llama_hub-0.0.3/llama_hub/apify/actor/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702389 llama_hub-0.0.3/llama_hub/apify/actor/requirements.txt
+-rw-r--r--   0        0        0     1499 2023-05-31 00:19:23.702551 llama_hub-0.0.3/llama_hub/apify/dataset/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.702623 llama_hub-0.0.3/llama_hub/apify/dataset/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-31 00:19:23.702732 llama_hub-0.0.3/llama_hub/apify/dataset/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702829 llama_hub-0.0.3/llama_hub/apify/dataset/requirements.txt
+-rw-r--r--   0        0        0      778 2023-05-31 00:19:23.702978 llama_hub-0.0.3/llama_hub/asana/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703048 llama_hub-0.0.3/llama_hub/asana/__init__.py
+-rw-r--r--   0        0        0     1856 2023-05-31 00:19:23.703120 llama_hub-0.0.3/llama_hub/asana/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.703184 llama_hub-0.0.3/llama_hub/asana/requirements.txt
+-rw-r--r--   0        0        0     2200 2023-05-31 00:19:23.703343 llama_hub-0.0.3/llama_hub/azcognitive_search/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703413 llama_hub-0.0.3/llama_hub/azcognitive_search/__init__.py
+-rw-r--r--   0        0        0     2080 2023-05-31 00:19:23.703514 llama_hub-0.0.3/llama_hub/azcognitive_search/base.py
+-rw-r--r--   0        0        0       37 2023-05-31 00:19:23.703715 llama_hub-0.0.3/llama_hub/azcognitive_search/requirements.txt
+-rw-r--r--   0        0        0     2542 2023-05-31 00:19:23.703897 llama_hub-0.0.3/llama_hub/azstorage_blob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703969 llama_hub-0.0.3/llama_hub/azstorage_blob/__init__.py
+-rw-r--r--   0        0        0     5419 2023-05-31 00:19:23.704197 llama_hub-0.0.3/llama_hub/azstorage_blob/base.py
+-rw-r--r--   0        0        0       34 2023-05-31 00:19:23.704302 llama_hub-0.0.3/llama_hub/azstorage_blob/requirements.txt
+-rw-r--r--   0        0        0     1077 2023-05-31 00:19:23.704450 llama_hub-0.0.3/llama_hub/bilibili/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.704513 llama_hub-0.0.3/llama_hub/bilibili/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-31 00:19:23.704590 llama_hub-0.0.3/llama_hub/bilibili/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.704655 llama_hub-0.0.3/llama_hub/bilibili/requirements.txt
+-rw-r--r--   0        0        0     3373 2023-05-31 00:19:23.705017 llama_hub-0.0.3/llama_hub/boarddocs/BoardDocsReader.ipynb
+-rw-r--r--   0        0        0     1402 2023-05-31 00:19:23.705098 llama_hub-0.0.3/llama_hub/boarddocs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.705155 llama_hub-0.0.3/llama_hub/boarddocs/__init__.py
+-rw-r--r--   0        0        0     4430 2023-05-31 00:19:23.705233 llama_hub-0.0.3/llama_hub/boarddocs/base.py
+-rw-r--r--   0        0        0    19752 2023-05-31 00:19:23.705373 llama_hub-0.0.3/llama_hub/boarddocs/crawl.ipynb
+-rw-r--r--   0        0        0       22 2023-05-31 00:19:23.705450 llama_hub-0.0.3/llama_hub/boarddocs/requirements.txt
+-rw-r--r--   0        0        0      921 2023-05-31 00:19:23.705605 llama_hub-0.0.3/llama_hub/chatgpt_plugin/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.705665 llama_hub-0.0.3/llama_hub/chatgpt_plugin/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-31 00:19:23.705774 llama_hub-0.0.3/llama_hub/chatgpt_plugin/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705804 llama_hub-0.0.3/llama_hub/chatgpt_plugin/requirements.txt
+-rw-r--r--   0        0        0     1056 2023-05-31 00:19:23.705957 llama_hub-0.0.3/llama_hub/chroma/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705990 llama_hub-0.0.3/llama_hub/chroma/__init__.py
+-rw-r--r--   0        0        0     1918 2023-05-31 00:19:23.706083 llama_hub-0.0.3/llama_hub/chroma/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.706141 llama_hub-0.0.3/llama_hub/chroma/requirements.txt
+-rw-r--r--   0        0        0     2288 2023-05-31 00:19:23.706281 llama_hub-0.0.3/llama_hub/confluence/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706342 llama_hub-0.0.3/llama_hub/confluence/__init__.py
+-rw-r--r--   0        0        0    11384 2023-05-31 00:19:23.706436 llama_hub-0.0.3/llama_hub/confluence/base.py
+-rw-r--r--   0        0        0       80 2023-05-31 00:19:23.706544 llama_hub-0.0.3/llama_hub/confluence/requirements.txt
+-rw-r--r--   0        0        0     1052 2023-05-31 00:19:23.706689 llama_hub-0.0.3/llama_hub/couchdb/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706764 llama_hub-0.0.3/llama_hub/couchdb/__init__.py
+-rw-r--r--   0        0        0     2564 2023-05-31 00:19:23.706867 llama_hub-0.0.3/llama_hub/couchdb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.706940 llama_hub-0.0.3/llama_hub/couchdb/requirements.txt
+-rw-r--r--   0        0        0      582 2023-05-31 00:19:23.707023 llama_hub-0.0.3/llama_hub/dad_jokes/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707074 llama_hub-0.0.3/llama_hub/dad_jokes/__init__.py
+-rw-r--r--   0        0        0      715 2023-05-31 00:19:23.707121 llama_hub-0.0.3/llama_hub/dad_jokes/base.py
+-rw-r--r--   0        0        0     1259 2023-05-31 00:19:23.707209 llama_hub-0.0.3/llama_hub/database/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707265 llama_hub-0.0.3/llama_hub/database/__init__.py
+-rw-r--r--   0        0        0     3328 2023-05-31 00:19:23.707352 llama_hub-0.0.3/llama_hub/database/base.py
+-rw-r--r--   0        0        0     1096 2023-05-31 00:19:23.707478 llama_hub-0.0.3/llama_hub/deeplake/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.707559 llama_hub-0.0.3/llama_hub/deeplake/__init__.py
+-rw-r--r--   0        0        0     3457 2023-05-31 00:19:23.707661 llama_hub-0.0.3/llama_hub/deeplake/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.707752 llama_hub-0.0.3/llama_hub/deeplake/requirements.txt
+-rw-r--r--   0        0        0      851 2023-05-31 00:19:23.707833 llama_hub-0.0.3/llama_hub/discord/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707879 llama_hub-0.0.3/llama_hub/discord/__init__.py
+-rw-r--r--   0        0        0     4650 2023-05-31 00:19:23.707939 llama_hub-0.0.3/llama_hub/discord/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.707985 llama_hub-0.0.3/llama_hub/discord/requirements.txt
+-rw-r--r--   0        0        0     4153 2023-05-31 00:19:23.708074 llama_hub-0.0.3/llama_hub/docugami/README.md
+-rw-r--r--   0        0        0        4 2023-05-31 00:19:23.708125 llama_hub-0.0.3/llama_hub/docugami/__init__.py
+-rw-r--r--   0        0        0    12075 2023-05-31 00:19:23.708201 llama_hub-0.0.3/llama_hub/docugami/base.py
+-rw-r--r--   0        0        0    65833 2023-05-31 00:19:23.708412 llama_hub-0.0.3/llama_hub/docugami/docugami.ipynb
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.708465 llama_hub-0.0.3/llama_hub/docugami/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.708545 llama_hub-0.0.3/llama_hub/elasticsearch/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.708572 llama_hub-0.0.3/llama_hub/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2301 2023-05-31 00:19:23.708639 llama_hub-0.0.3/llama_hub/elasticsearch/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708699 llama_hub-0.0.3/llama_hub/elasticsearch/requirements.txt
+-rw-r--r--   0        0        0     1319 2023-05-31 00:19:23.708825 llama_hub-0.0.3/llama_hub/faiss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.708885 llama_hub-0.0.3/llama_hub/faiss/__init__.py
+-rw-r--r--   0        0        0     2126 2023-05-31 00:19:23.708943 llama_hub-0.0.3/llama_hub/faiss/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708986 llama_hub-0.0.3/llama_hub/faiss/requirements.txt
+-rw-r--r--   0        0        0      585 2023-05-31 00:19:23.709108 llama_hub-0.0.3/llama_hub/feedly_rss/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.709136 llama_hub-0.0.3/llama_hub/feedly_rss/__init__.py
+-rw-r--r--   0        0        0     2100 2023-05-31 00:19:23.709219 llama_hub-0.0.3/llama_hub/feedly_rss/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.709288 llama_hub-0.0.3/llama_hub/feedly_rss/requirements.txt
+-rw-r--r--   0        0        0     2829 2023-05-31 00:19:23.709504 llama_hub-0.0.3/llama_hub/file/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709559 llama_hub-0.0.3/llama_hub/file/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-31 00:19:23.709669 llama_hub-0.0.3/llama_hub/file/audio/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709737 llama_hub-0.0.3/llama_hub/file/audio/__init__.py
+-rw-r--r--   0        0        0     1486 2023-05-31 00:19:23.709814 llama_hub-0.0.3/llama_hub/file/audio/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.709874 llama_hub-0.0.3/llama_hub/file/audio/requirements.txt
+-rw-r--r--   0        0        0     1241 2023-05-31 00:19:23.710011 llama_hub-0.0.3/llama_hub/file/audio_gladia/README.md
+-rw-r--r--   0        0        0       19 2023-05-31 00:19:23.710082 llama_hub-0.0.3/llama_hub/file/audio_gladia/__init__.py
+-rw-r--r--   0        0        0     3274 2023-05-31 00:19:23.710177 llama_hub-0.0.3/llama_hub/file/audio_gladia/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.710239 llama_hub-0.0.3/llama_hub/file/audio_gladia/requirements.txt
+-rw-r--r--   0        0        0     5552 2023-05-31 00:19:23.710436 llama_hub-0.0.3/llama_hub/file/base.py
+-rw-r--r--   0        0        0     1069 2023-05-31 00:19:23.710517 llama_hub-0.0.3/llama_hub/file/cjk_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.710563 llama_hub-0.0.3/llama_hub/file/cjk_pdf/__init__.py
+-rw-r--r--   0        0        0     2584 2023-05-31 00:19:23.710634 llama_hub-0.0.3/llama_hub/file/cjk_pdf/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:19:23.710693 llama_hub-0.0.3/llama_hub/file/cjk_pdf/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:19:23.710812 llama_hub-0.0.3/llama_hub/file/deepdoctection/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.710846 llama_hub-0.0.3/llama_hub/file/deepdoctection/__init__.py
+-rw-r--r--   0        0        0     1188 2023-05-31 00:19:23.710944 llama_hub-0.0.3/llama_hub/file/deepdoctection/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.711015 llama_hub-0.0.3/llama_hub/file/deepdoctection/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:19:23.711097 llama_hub-0.0.3/llama_hub/file/docx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711148 llama_hub-0.0.3/llama_hub/file/docx/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-31 00:19:23.711197 llama_hub-0.0.3/llama_hub/file/docx/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.711264 llama_hub-0.0.3/llama_hub/file/docx/requirements.txt
+-rw-r--r--   0        0        0      724 2023-05-31 00:19:23.711407 llama_hub-0.0.3/llama_hub/file/epub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711459 llama_hub-0.0.3/llama_hub/file/epub/__init__.py
+-rw-r--r--   0        0        0     1000 2023-05-31 00:19:23.711525 llama_hub-0.0.3/llama_hub/file/epub/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.711579 llama_hub-0.0.3/llama_hub/file/epub/requirements.txt
+-rw-r--r--   0        0        0     1087 2023-05-31 00:19:23.711703 llama_hub-0.0.3/llama_hub/file/flat_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711756 llama_hub-0.0.3/llama_hub/file/flat_pdf/__init__.py
+-rw-r--r--   0        0        0     2837 2023-05-31 00:19:23.711854 llama_hub-0.0.3/llama_hub/file/flat_pdf/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.711939 llama_hub-0.0.3/llama_hub/file/flat_pdf/requirements.txt
+-rw-r--r--   0        0        0     1359 2023-05-31 00:19:23.712052 llama_hub-0.0.3/llama_hub/file/image/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.712114 llama_hub-0.0.3/llama_hub/file/image/__init__.py
+-rw-r--r--   0        0        0     3888 2023-05-31 00:19:23.712184 llama_hub-0.0.3/llama_hub/file/image/base.py
+-rw-r--r--   0        0        0       63 2023-05-31 00:19:23.712235 llama_hub-0.0.3/llama_hub/file/image/requirements.txt
+-rw-r--r--   0        0        0      373 2023-05-31 00:19:23.712359 llama_hub-0.0.3/llama_hub/file/image_blip/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712384 llama_hub-0.0.3/llama_hub/file/image_blip/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-03 03:50:30.194383 llama_hub-0.0.3/llama_hub/file/image_blip/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712578 llama_hub-0.0.3/llama_hub/file/image_blip/requirements.txt
+-rw-r--r--   0        0        0      422 2023-05-31 00:19:23.712697 llama_hub-0.0.3/llama_hub/file/image_blip2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712725 llama_hub-0.0.3/llama_hub/file/image_blip2/__init__.py
+-rw-r--r--   0        0        0     3331 2023-06-03 03:50:30.194545 llama_hub-0.0.3/llama_hub/file/image_blip2/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712933 llama_hub-0.0.3/llama_hub/file/image_blip2/requirements.txt
+-rw-r--r--   0        0        0      457 2023-05-31 00:19:23.713074 llama_hub-0.0.3/llama_hub/file/ipynb/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713111 llama_hub-0.0.3/llama_hub/file/ipynb/__init__.py
+-rw-r--r--   0        0        0     1296 2023-05-31 00:19:23.713224 llama_hub-0.0.3/llama_hub/file/ipynb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.713320 llama_hub-0.0.3/llama_hub/file/ipynb/requirements.txt
+-rw-r--r--   0        0        0      735 2023-05-31 00:19:23.713712 llama_hub-0.0.3/llama_hub/file/json/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.713821 llama_hub-0.0.3/llama_hub/file/json/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-31 00:19:23.713925 llama_hub-0.0.3/llama_hub/file/json/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713956 llama_hub-0.0.3/llama_hub/file/json/requirements.txt
+-rw-r--r--   0        0        0      744 2023-05-31 00:19:23.714073 llama_hub-0.0.3/llama_hub/file/markdown/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714150 llama_hub-0.0.3/llama_hub/file/markdown/__init__.py
+-rw-r--r--   0        0        0     3633 2023-05-31 00:19:23.714275 llama_hub-0.0.3/llama_hub/file/markdown/base.py
+-rw-r--r--   0        0        0      680 2023-05-31 00:19:23.714381 llama_hub-0.0.3/llama_hub/file/mbox/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714447 llama_hub-0.0.3/llama_hub/file/mbox/__init__.py
+-rw-r--r--   0        0        0     3604 2023-05-31 00:19:23.714680 llama_hub-0.0.3/llama_hub/file/mbox/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:19:23.714754 llama_hub-0.0.3/llama_hub/file/mbox/requirements.txt
+-rw-r--r--   0        0        0      929 2023-05-31 00:19:23.714899 llama_hub-0.0.3/llama_hub/file/paged_csv/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.714940 llama_hub-0.0.3/llama_hub/file/paged_csv/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-31 00:19:23.715096 llama_hub-0.0.3/llama_hub/file/paged_csv/base.py
+-rw-r--r--   0        0        0      786 2023-05-31 00:19:23.715234 llama_hub-0.0.3/llama_hub/file/pandas_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715305 llama_hub-0.0.3/llama_hub/file/pandas_csv/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-31 00:19:23.715402 llama_hub-0.0.3/llama_hub/file/pandas_csv/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715462 llama_hub-0.0.3/llama_hub/file/pandas_csv/requirements.txt
+-rw-r--r--   0        0        0     1334 2023-05-31 00:19:23.715614 llama_hub-0.0.3/llama_hub/file/pandas_excel/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715680 llama_hub-0.0.3/llama_hub/file/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     2219 2023-05-31 00:19:23.715753 llama_hub-0.0.3/llama_hub/file/pandas_excel/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715809 llama_hub-0.0.3/llama_hub/file/pandas_excel/requirements.txt
+-rw-r--r--   0        0        0      790 2023-05-31 00:19:23.715925 llama_hub-0.0.3/llama_hub/file/pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715984 llama_hub-0.0.3/llama_hub/file/pdf/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-31 00:19:23.716042 llama_hub-0.0.3/llama_hub/file/pdf/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.716096 llama_hub-0.0.3/llama_hub/file/pdf/requirements.txt
+-rw-r--r--   0        0        0      904 2023-06-10 07:58:38.772384 llama_hub-0.0.3/llama_hub/file/pdf_miner/README.md
+-rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772474 llama_hub-0.0.3/llama_hub/file/pdf_miner/__init__.py
+-rw-r--r--   0        0        0     2005 2023-06-10 07:58:38.772566 llama_hub-0.0.3/llama_hub/file/pdf_miner/base.py
+-rw-r--r--   0        0        0       13 2023-06-10 07:58:38.772654 llama_hub-0.0.3/llama_hub/file/pdf_miner/requirements.txt
+-rw-r--r--   0        0        0     1120 2023-05-31 00:19:23.716188 llama_hub-0.0.3/llama_hub/file/pptx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716252 llama_hub-0.0.3/llama_hub/file/pptx/__init__.py
+-rw-r--r--   0        0        0     3447 2023-05-31 00:19:23.716338 llama_hub-0.0.3/llama_hub/file/pptx/base.py
+-rw-r--r--   0        0        0       49 2023-05-31 00:19:23.716404 llama_hub-0.0.3/llama_hub/file/pptx/requirements.txt
+-rw-r--r--   0        0        0     1160 2023-05-31 00:19:23.716683 llama_hub-0.0.3/llama_hub/file/pymu_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716754 llama_hub-0.0.3/llama_hub/file/pymu_pdf/__init__.py
+-rw-r--r--   0        0        0     2415 2023-05-31 00:19:23.716819 llama_hub-0.0.3/llama_hub/file/pymu_pdf/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.716870 llama_hub-0.0.3/llama_hub/file/pymu_pdf/requirements.txt
+-rw-r--r--   0        0        0      890 2023-05-31 00:19:23.716967 llama_hub-0.0.3/llama_hub/file/rdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717033 llama_hub-0.0.3/llama_hub/file/rdf/__init__.py
+-rw-r--r--   0        0        0     2203 2023-05-31 00:19:23.717110 llama_hub-0.0.3/llama_hub/file/rdf/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.717167 llama_hub-0.0.3/llama_hub/file/rdf/requirements.txt
+-rw-r--r--   0        0        0      792 2023-05-31 00:19:23.717279 llama_hub-0.0.3/llama_hub/file/simple_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717342 llama_hub-0.0.3/llama_hub/file/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1234 2023-05-31 00:19:23.717441 llama_hub-0.0.3/llama_hub/file/simple_csv/base.py
+-rw-r--r--   0        0        0     2531 2023-05-31 00:19:23.717561 llama_hub-0.0.3/llama_hub/file/unstructured/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717635 llama_hub-0.0.3/llama_hub/file/unstructured/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-31 00:19:23.717707 llama_hub-0.0.3/llama_hub/file/unstructured/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717763 llama_hub-0.0.3/llama_hub/file/unstructured/requirements.txt
+-rw-r--r--   0        0        0     1498 2023-06-10 07:58:38.772778 llama_hub-0.0.3/llama_hub/firestore/README.md
+-rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772830 llama_hub-0.0.3/llama_hub/firestore/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-10 07:58:38.772918 llama_hub-0.0.3/llama_hub/firestore/base.py
+-rw-r--r--   0        0        0       23 2023-06-10 07:58:38.772997 llama_hub-0.0.3/llama_hub/firestore/requirements.txt
+-rw-r--r--   0        0        0     3141 2023-06-10 07:58:38.773157 llama_hub-0.0.3/llama_hub/github_repo/README.md
+-rw-r--r--   0        0        0      153 2023-05-31 00:19:23.717979 llama_hub-0.0.3/llama_hub/github_repo/__init__.py
+-rw-r--r--   0        0        0    20914 2023-06-03 03:50:30.194900 llama_hub-0.0.3/llama_hub/github_repo/base.py
+-rw-r--r--   0        0        0    12721 2023-05-31 00:19:23.718674 llama_hub-0.0.3/llama_hub/github_repo/github_client.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.718740 llama_hub-0.0.3/llama_hub/github_repo/requirements.txt
+-rw-r--r--   0        0        0     5709 2023-06-03 03:50:30.195070 llama_hub-0.0.3/llama_hub/github_repo/utils.py
+-rw-r--r--   0        0        0      948 2023-05-31 00:19:23.719165 llama_hub-0.0.3/llama_hub/gmail/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719238 llama_hub-0.0.3/llama_hub/gmail/__init__.py
+-rw-r--r--   0        0        0     5302 2023-05-31 00:19:23.719342 llama_hub-0.0.3/llama_hub/gmail/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:19:23.719438 llama_hub-0.0.3/llama_hub/gmail/requirements.txt
+-rw-r--r--   0        0        0     1364 2023-05-31 00:19:23.719568 llama_hub-0.0.3/llama_hub/google_calendar/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719630 llama_hub-0.0.3/llama_hub/google_calendar/__init__.py
+-rw-r--r--   0        0        0     4755 2023-05-31 00:19:23.719707 llama_hub-0.0.3/llama_hub/google_calendar/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.719771 llama_hub-0.0.3/llama_hub/google_calendar/requirements.txt
+-rw-r--r--   0        0        0     2571 2023-05-31 00:19:23.719884 llama_hub-0.0.3/llama_hub/google_docs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719942 llama_hub-0.0.3/llama_hub/google_docs/__init__.py
+-rw-r--r--   0        0        0     5019 2023-05-31 00:19:23.720018 llama_hub-0.0.3/llama_hub/google_docs/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720074 llama_hub-0.0.3/llama_hub/google_docs/requirements.txt
+-rw-r--r--   0        0        0     1807 2023-05-31 00:19:23.720187 llama_hub-0.0.3/llama_hub/google_drive/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720244 llama_hub-0.0.3/llama_hub/google_drive/__init__.py
+-rw-r--r--   0        0        0    13454 2023-06-03 03:50:30.195254 llama_hub-0.0.3/llama_hub/google_drive/base.py
+-rw-r--r--   0        0        0       76 2023-05-31 00:19:23.720583 llama_hub-0.0.3/llama_hub/google_drive/requirements.txt
+-rw-r--r--   0        0        0     1150 2023-05-31 00:19:23.720701 llama_hub-0.0.3/llama_hub/google_sheets/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720755 llama_hub-0.0.3/llama_hub/google_sheets/__init__.py
+-rw-r--r--   0        0        0     4989 2023-05-31 00:19:23.720863 llama_hub-0.0.3/llama_hub/google_sheets/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720914 llama_hub-0.0.3/llama_hub/google_sheets/requirements.txt
+-rw-r--r--   0        0        0      809 2023-05-31 00:19:23.721050 llama_hub-0.0.3/llama_hub/gpt_repo/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.721109 llama_hub-0.0.3/llama_hub/gpt_repo/__init__.py
+-rw-r--r--   0        0        0     5488 2023-05-31 00:19:23.721217 llama_hub-0.0.3/llama_hub/gpt_repo/base.py
+-rw-r--r--   0        0        0     1595 2023-05-31 00:19:23.721376 llama_hub-0.0.3/llama_hub/graphdb_cypher/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721443 llama_hub-0.0.3/llama_hub/graphdb_cypher/__init__.py
+-rw-r--r--   0        0        0     1788 2023-05-31 00:19:23.721561 llama_hub-0.0.3/llama_hub/graphdb_cypher/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.721683 llama_hub-0.0.3/llama_hub/graphdb_cypher/requirements.txt
+-rw-r--r--   0        0        0     1215 2023-05-31 00:19:23.721834 llama_hub-0.0.3/llama_hub/graphql/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721886 llama_hub-0.0.3/llama_hub/graphql/__init__.py
+-rw-r--r--   0        0        0     2204 2023-05-31 00:19:23.721979 llama_hub-0.0.3/llama_hub/graphql/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.722048 llama_hub-0.0.3/llama_hub/graphql/requirements.txt
+-rw-r--r--   0        0        0      969 2023-05-31 00:19:23.722173 llama_hub-0.0.3/llama_hub/hatena_blog/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722225 llama_hub-0.0.3/llama_hub/hatena_blog/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-31 00:19:23.722316 llama_hub-0.0.3/llama_hub/hatena_blog/base.py
+-rw-r--r--   0        0        0       28 2023-05-31 00:19:23.722405 llama_hub-0.0.3/llama_hub/hatena_blog/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:19:23.722570 llama_hub-0.0.3/llama_hub/hubspot/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722654 llama_hub-0.0.3/llama_hub/hubspot/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-31 00:19:23.722744 llama_hub-0.0.3/llama_hub/hubspot/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.722823 llama_hub-0.0.3/llama_hub/hubspot/requirements.txt
+-rw-r--r--   0        0        0     1035 2023-05-31 00:19:23.722974 llama_hub-0.0.3/llama_hub/huggingface/fs/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.723070 llama_hub-0.0.3/llama_hub/huggingface/fs/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-31 00:19:23.723162 llama_hub-0.0.3/llama_hub/huggingface/fs/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.723269 llama_hub-0.0.3/llama_hub/huggingface/fs/requirements.txt
+-rw-r--r--   0        0        0      797 2023-05-31 00:19:23.723369 llama_hub-0.0.3/llama_hub/intercom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.723425 llama_hub-0.0.3/llama_hub/intercom/__init__.py
+-rw-r--r--   0        0        0     2416 2023-05-31 00:19:23.723490 llama_hub-0.0.3/llama_hub/intercom/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.723542 llama_hub-0.0.3/llama_hub/intercom/requirements.txt
+-rw-r--r--   0        0        0      808 2023-06-10 07:58:38.773924 llama_hub-0.0.3/llama_hub/jira/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.723719 llama_hub-0.0.3/llama_hub/jira/__init__.py
+-rw-r--r--   0        0        0     3383 2023-05-31 00:19:23.723801 llama_hub-0.0.3/llama_hub/jira/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.723892 llama_hub-0.0.3/llama_hub/jira/requirements.txt
+-rw-r--r--   0        0        0     1362 2023-05-31 00:19:23.724041 llama_hub-0.0.3/llama_hub/joplin/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724074 llama_hub-0.0.3/llama_hub/joplin/__init__.py
+-rw-r--r--   0        0        0     5183 2023-05-31 00:19:23.724310 llama_hub-0.0.3/llama_hub/joplin/base.py
+-rw-r--r--   0        0        0      698 2023-05-31 00:19:23.724418 llama_hub-0.0.3/llama_hub/jsondata/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.724463 llama_hub-0.0.3/llama_hub/jsondata/__init__.py
+-rw-r--r--   0        0        0     1633 2023-05-31 00:19:23.724551 llama_hub-0.0.3/llama_hub/jsondata/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724577 llama_hub-0.0.3/llama_hub/jsondata/requirements.txt
+-rw-r--r--   0        0        0     7206 2023-05-31 00:19:23.724774 llama_hub-0.0.3/llama_hub/kaltura/esearch/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.724845 llama_hub-0.0.3/llama_hub/kaltura/esearch/__init__.py
+-rw-r--r--   0        0        0    12019 2023-05-31 00:19:23.724953 llama_hub-0.0.3/llama_hub/kaltura/esearch/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.725038 llama_hub-0.0.3/llama_hub/kaltura/esearch/requirements.txt
+-rw-r--r--   0        0        0    11665 2023-06-10 07:58:38.774117 llama_hub-0.0.3/llama_hub/library.json
+-rw-r--r--   0        0        0     1117 2023-05-31 00:19:23.725289 llama_hub-0.0.3/llama_hub/make_com/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725348 llama_hub-0.0.3/llama_hub/make_com/__init__.py
+-rw-r--r--   0        0        0     1721 2023-05-31 00:19:23.725434 llama_hub-0.0.3/llama_hub/make_com/base.py
+-rw-r--r--   0        0        0      810 2023-05-31 00:19:23.725515 llama_hub-0.0.3/llama_hub/mangoapps_guides/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725566 llama_hub-0.0.3/llama_hub/mangoapps_guides/__init__.py
+-rw-r--r--   0        0        0     4752 2023-05-31 00:19:23.725645 llama_hub-0.0.3/llama_hub/mangoapps_guides/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.725706 llama_hub-0.0.3/llama_hub/mangoapps_guides/requirements.txt
+-rw-r--r--   0        0        0     2740 2023-05-31 00:19:23.725850 llama_hub-0.0.3/llama_hub/maps/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.725903 llama_hub-0.0.3/llama_hub/maps/__init__.py
+-rw-r--r--   0        0        0     4599 2023-05-31 00:19:23.726215 llama_hub-0.0.3/llama_hub/maps/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.726327 llama_hub-0.0.3/llama_hub/maps/requirements.txt
+-rw-r--r--   0        0        0      870 2023-05-31 00:19:23.726449 llama_hub-0.0.3/llama_hub/memos/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726502 llama_hub-0.0.3/llama_hub/memos/__init__.py
+-rw-r--r--   0        0        0     1465 2023-05-31 00:19:23.726557 llama_hub-0.0.3/llama_hub/memos/base.py
+-rw-r--r--   0        0        0      952 2023-05-31 00:19:23.726641 llama_hub-0.0.3/llama_hub/metal/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726693 llama_hub-0.0.3/llama_hub/metal/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-31 00:19:23.726764 llama_hub-0.0.3/llama_hub/metal/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.726825 llama_hub-0.0.3/llama_hub/metal/requirements.txt
+-rw-r--r--   0        0        0     1174 2023-05-31 00:19:23.726943 llama_hub-0.0.3/llama_hub/milvus/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.727017 llama_hub-0.0.3/llama_hub/milvus/__init__.py
+-rw-r--r--   0        0        0     4588 2023-05-31 00:19:23.727112 llama_hub-0.0.3/llama_hub/milvus/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727182 llama_hub-0.0.3/llama_hub/milvus/requirements.txt
+-rw-r--r--   0        0        0      853 2023-05-31 00:19:23.727268 llama_hub-0.0.3/llama_hub/mondaydotcom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727321 llama_hub-0.0.3/llama_hub/mondaydotcom/__init__.py
+-rw-r--r--   0        0        0     2658 2023-05-31 00:19:23.727383 llama_hub-0.0.3/llama_hub/mondaydotcom/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727432 llama_hub-0.0.3/llama_hub/mondaydotcom/requirements.txt
+-rw-r--r--   0        0        0      973 2023-05-31 00:19:23.727516 llama_hub-0.0.3/llama_hub/mongo/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727566 llama_hub-0.0.3/llama_hub/mongo/__init__.py
+-rw-r--r--   0        0        0     2260 2023-05-31 00:19:23.727656 llama_hub-0.0.3/llama_hub/mongo/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.727743 llama_hub-0.0.3/llama_hub/mongo/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:19:23.727849 llama_hub-0.0.3/llama_hub/notion/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727909 llama_hub-0.0.3/llama_hub/notion/__init__.py
+-rw-r--r--   0        0        0     6102 2023-05-31 00:19:23.727971 llama_hub-0.0.3/llama_hub/notion/base.py
+-rw-r--r--   0        0        0      395 2023-06-01 05:01:36.458116 llama_hub-0.0.3/llama_hub/notion/tool.py
+-rw-r--r--   0        0        0      688 2023-05-31 00:19:23.728057 llama_hub-0.0.3/llama_hub/obsidian/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728106 llama_hub-0.0.3/llama_hub/obsidian/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-31 00:19:23.728167 llama_hub-0.0.3/llama_hub/obsidian/base.py
+-rw-r--r--   0        0        0     1050 2023-05-31 00:19:23.728304 llama_hub-0.0.3/llama_hub/opendal_reader/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.728335 llama_hub-0.0.3/llama_hub/opendal_reader/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-31 00:19:23.728466 llama_hub-0.0.3/llama_hub/opendal_reader/azblob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728521 llama_hub-0.0.3/llama_hub/opendal_reader/azblob/__init__.py
+-rw-r--r--   0        0        0     2476 2023-05-31 00:19:23.728643 llama_hub-0.0.3/llama_hub/opendal_reader/azblob/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.728751 llama_hub-0.0.3/llama_hub/opendal_reader/azblob/requirements.txt
+-rw-r--r--   0        0        0     2979 2023-05-31 00:19:23.728891 llama_hub-0.0.3/llama_hub/opendal_reader/base.py
+-rw-r--r--   0        0        0      999 2023-05-31 00:19:23.729020 llama_hub-0.0.3/llama_hub/opendal_reader/gcs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729087 llama_hub-0.0.3/llama_hub/opendal_reader/gcs/__init__.py
+-rw-r--r--   0        0        0     2294 2023-05-31 00:19:23.729212 llama_hub-0.0.3/llama_hub/opendal_reader/gcs/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729283 llama_hub-0.0.3/llama_hub/opendal_reader/gcs/requirements.txt
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729358 llama_hub-0.0.3/llama_hub/opendal_reader/requirements.txt
+-rw-r--r--   0        0        0     1397 2023-05-31 00:19:23.729481 llama_hub-0.0.3/llama_hub/opendal_reader/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729530 llama_hub-0.0.3/llama_hub/opendal_reader/s3/__init__.py
+-rw-r--r--   0        0        0     2605 2023-05-31 00:19:23.729641 llama_hub-0.0.3/llama_hub/opendal_reader/s3/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729714 llama_hub-0.0.3/llama_hub/opendal_reader/s3/requirements.txt
+-rw-r--r--   0        0        0     2147 2023-05-31 00:19:23.729798 llama_hub-0.0.3/llama_hub/outlook_localcalendar/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729846 llama_hub-0.0.3/llama_hub/outlook_localcalendar/__init__,py
+-rw-r--r--   0        0        0     3838 2023-05-31 00:19:23.729934 llama_hub-0.0.3/llama_hub/outlook_localcalendar/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730022 llama_hub-0.0.3/llama_hub/outlook_localcalendar/requirements.txt
+-rw-r--r--   0        0        0     1801 2023-05-31 00:19:23.730149 llama_hub-0.0.3/llama_hub/pandas_ai/README.md
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.730219 llama_hub-0.0.3/llama_hub/pandas_ai/__init__.py
+-rw-r--r--   0        0        0     3932 2023-05-31 00:19:23.730347 llama_hub-0.0.3/llama_hub/pandas_ai/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730434 llama_hub-0.0.3/llama_hub/pandas_ai/requirements.txt
+-rw-r--r--   0        0        0     1484 2023-05-31 00:19:23.730555 llama_hub-0.0.3/llama_hub/papers/arxiv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730614 llama_hub-0.0.3/llama_hub/papers/arxiv/__init__.py
+-rw-r--r--   0        0        0     6441 2023-05-31 00:19:23.730749 llama_hub-0.0.3/llama_hub/papers/arxiv/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.730795 llama_hub-0.0.3/llama_hub/papers/arxiv/requirements.txt
+-rw-r--r--   0        0        0      931 2023-05-31 00:19:23.730889 llama_hub-0.0.3/llama_hub/papers/pubmed/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730947 llama_hub-0.0.3/llama_hub/papers/pubmed/__init__.py
+-rw-r--r--   0        0        0     6168 2023-05-31 00:19:23.731053 llama_hub-0.0.3/llama_hub/papers/pubmed/base.py
+-rw-r--r--   0        0        0     1279 2023-05-31 00:19:23.731154 llama_hub-0.0.3/llama_hub/pinecone/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731210 llama_hub-0.0.3/llama_hub/pinecone/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-31 00:19:23.731290 llama_hub-0.0.3/llama_hub/pinecone/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.731346 llama_hub-0.0.3/llama_hub/pinecone/requirements.txt
+-rw-r--r--   0        0        0     1157 2023-05-31 00:19:23.731448 llama_hub-0.0.3/llama_hub/qdrant/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731505 llama_hub-0.0.3/llama_hub/qdrant/__init__.py
+-rw-r--r--   0        0        0     6920 2023-05-31 00:19:23.731618 llama_hub-0.0.3/llama_hub/qdrant/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.731674 llama_hub-0.0.3/llama_hub/qdrant/requirements.txt
+-rw-r--r--   0        0        0     1551 2023-05-31 00:19:23.731776 llama_hub-0.0.3/llama_hub/readwise/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731833 llama_hub-0.0.3/llama_hub/readwise/__init__.py
+-rw-r--r--   0        0        0     1800 2023-05-31 00:19:23.731903 llama_hub-0.0.3/llama_hub/readwise/base.py
+-rw-r--r--   0        0        0     2707 2023-05-31 00:19:23.732014 llama_hub-0.0.3/llama_hub/reddit/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732079 llama_hub-0.0.3/llama_hub/reddit/__init__.py
+-rw-r--r--   0        0        0     1914 2023-05-31 00:19:23.732143 llama_hub-0.0.3/llama_hub/reddit/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:19:23.732202 llama_hub-0.0.3/llama_hub/reddit/requirements.txt
+-rw-r--r--   0        0        0     1330 2023-05-31 00:19:23.732308 llama_hub-0.0.3/llama_hub/remote/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732382 llama_hub-0.0.3/llama_hub/remote/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-31 00:19:23.732529 llama_hub-0.0.3/llama_hub/remote/base.py
+-rw-r--r--   0        0        0     1383 2023-05-31 00:19:23.732627 llama_hub-0.0.3/llama_hub/remote_depth/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.732655 llama_hub-0.0.3/llama_hub/remote_depth/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-31 00:19:23.732820 llama_hub-0.0.3/llama_hub/remote_depth/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:19:23.732887 llama_hub-0.0.3/llama_hub/remote_depth/requirements.txt
+-rw-r--r--   0        0        0     1669 2023-05-31 00:19:23.732997 llama_hub-0.0.3/llama_hub/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733053 llama_hub-0.0.3/llama_hub/s3/__init__.py
+-rw-r--r--   0        0        0     3985 2023-05-31 00:19:23.733196 llama_hub-0.0.3/llama_hub/s3/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.733253 llama_hub-0.0.3/llama_hub/s3/requirements.txt
+-rw-r--r--   0        0        0      821 2023-05-31 00:19:23.733394 llama_hub-0.0.3/llama_hub/slack/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733459 llama_hub-0.0.3/llama_hub/slack/__init__.py
+-rw-r--r--   0        0        0     7499 2023-05-31 00:19:23.733536 llama_hub-0.0.3/llama_hub/slack/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.733594 llama_hub-0.0.3/llama_hub/slack/requirements.txt
+-rw-r--r--   0        0        0      690 2023-05-31 00:19:23.733754 llama_hub-0.0.3/llama_hub/snscrape_twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733815 llama_hub-0.0.3/llama_hub/snscrape_twitter/__init__.py
+-rw-r--r--   0        0        0     1156 2023-05-31 00:19:23.733911 llama_hub-0.0.3/llama_hub/snscrape_twitter/base.py
+-rw-r--r--   0        0        0       56 2023-05-31 00:19:23.734041 llama_hub-0.0.3/llama_hub/snscrape_twitter/requirements.txt
+-rw-r--r--   0        0        0     1662 2023-05-31 00:19:23.734145 llama_hub-0.0.3/llama_hub/spotify/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734204 llama_hub-0.0.3/llama_hub/spotify/__init__.py
+-rw-r--r--   0        0        0     2287 2023-05-31 00:19:23.734275 llama_hub-0.0.3/llama_hub/spotify/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.734331 llama_hub-0.0.3/llama_hub/spotify/requirements.txt
+-rw-r--r--   0        0        0      846 2023-05-31 00:19:23.734458 llama_hub-0.0.3/llama_hub/stackoverflow/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734518 llama_hub-0.0.3/llama_hub/stackoverflow/__init__.py
+-rw-r--r--   0        0        0     6263 2023-05-31 00:19:23.734626 llama_hub-0.0.3/llama_hub/stackoverflow/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.734708 llama_hub-0.0.3/llama_hub/stackoverflow/requirements.txt
+-rw-r--r--   0        0        0      936 2023-05-31 00:19:23.734832 llama_hub-0.0.3/llama_hub/steamship/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.734866 llama_hub-0.0.3/llama_hub/steamship/__init__.py
+-rw-r--r--   0        0        0     3498 2023-05-31 00:19:23.734974 llama_hub-0.0.3/llama_hub/steamship/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.735057 llama_hub-0.0.3/llama_hub/steamship/requirements.txt
+-rw-r--r--   0        0        0      726 2023-05-31 00:19:23.735154 llama_hub-0.0.3/llama_hub/string_iterable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735234 llama_hub-0.0.3/llama_hub/string_iterable/__init__.py
+-rw-r--r--   0        0        0      969 2023-05-31 00:19:23.735290 llama_hub-0.0.3/llama_hub/string_iterable/base.py
+-rw-r--r--   0        0        0      676 2023-05-31 00:19:23.735435 llama_hub-0.0.3/llama_hub/trello/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735493 llama_hub-0.0.3/llama_hub/trello/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-31 00:19:23.735587 llama_hub-0.0.3/llama_hub/trello/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.735672 llama_hub-0.0.3/llama_hub/trello/requirements.txt
+-rw-r--r--   0        0        0      924 2023-05-31 00:19:23.735778 llama_hub-0.0.3/llama_hub/twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735847 llama_hub-0.0.3/llama_hub/twitter/__init__.py
+-rw-r--r--   0        0        0     1777 2023-05-31 00:19:23.735917 llama_hub-0.0.3/llama_hub/twitter/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.735976 llama_hub-0.0.3/llama_hub/twitter/requirements.txt
+-rw-r--r--   0        0        0      637 2023-05-31 00:19:23.736279 llama_hub-0.0.3/llama_hub/utils.py
+-rw-r--r--   0        0        0     1162 2023-05-31 00:19:23.736420 llama_hub-0.0.3/llama_hub/weather/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.736481 llama_hub-0.0.3/llama_hub/weather/__init__.py
+-rw-r--r--   0        0        0     2779 2023-05-31 00:19:23.736578 llama_hub-0.0.3/llama_hub/weather/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.736662 llama_hub-0.0.3/llama_hub/weather/requirements.txt
+-rw-r--r--   0        0        0     1525 2023-05-31 00:19:23.736765 llama_hub-0.0.3/llama_hub/weaviate/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.736823 llama_hub-0.0.3/llama_hub/weaviate/__init__.py
+-rw-r--r--   0        0        0     3697 2023-05-31 00:19:23.736889 llama_hub-0.0.3/llama_hub/weaviate/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.736940 llama_hub-0.0.3/llama_hub/weaviate/requirements.txt
+-rw-r--r--   0        0        0      415 2023-05-31 00:19:23.737101 llama_hub-0.0.3/llama_hub/web/async_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.737136 llama_hub-0.0.3/llama_hub/web/async_web/__init__.py
+-rw-r--r--   0        0        0     2554 2023-05-31 00:19:23.737236 llama_hub-0.0.3/llama_hub/web/async_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.737325 llama_hub-0.0.3/llama_hub/web/async_web/requirements.txt
+-rw-r--r--   0        0        0     3446 2023-05-31 00:19:23.737437 llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.737504 llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/__init__.py
+-rw-r--r--   0        0        0     6747 2023-05-31 00:19:23.737610 llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:19:23.737666 llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/requirements.txt
+-rw-r--r--   0        0        0     3672 2023-05-31 00:19:23.737782 llama_hub-0.0.3/llama_hub/web/knowledge_base/README.md
+-rw-r--r--   0        0        0        1 2023-05-31 00:19:23.737843 llama_hub-0.0.3/llama_hub/web/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     5611 2023-05-31 00:19:23.737918 llama_hub-0.0.3/llama_hub/web/knowledge_base/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.737968 llama_hub-0.0.3/llama_hub/web/knowledge_base/requirements.txt
+-rw-r--r--   0        0        0     2681 2023-05-31 00:19:23.738073 llama_hub-0.0.3/llama_hub/web/readability_web/README.md
+-rw-r--r--   0        0        0    83319 2023-05-31 00:19:23.738443 llama_hub-0.0.3/llama_hub/web/readability_web/Readability.js
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738513 llama_hub-0.0.3/llama_hub/web/readability_web/__init__.py
+-rw-r--r--   0        0        0     4531 2023-05-31 00:19:23.738613 llama_hub-0.0.3/llama_hub/web/readability_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.738660 llama_hub-0.0.3/llama_hub/web/readability_web/requirements.txt
+-rw-r--r--   0        0        0      489 2023-05-31 00:19:23.738734 llama_hub-0.0.3/llama_hub/web/rss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738780 llama_hub-0.0.3/llama_hub/web/rss/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-31 00:19:23.738829 llama_hub-0.0.3/llama_hub/web/rss/base.py
+-rw-r--r--   0        0        0     1994 2023-05-31 00:19:23.738914 llama_hub-0.0.3/llama_hub/web/simple_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738959 llama_hub-0.0.3/llama_hub/web/simple_web/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-31 00:19:23.739036 llama_hub-0.0.3/llama_hub/web/simple_web/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.739081 llama_hub-0.0.3/llama_hub/web/simple_web/requirements.txt
+-rw-r--r--   0        0        0     2009 2023-05-31 00:19:23.739158 llama_hub-0.0.3/llama_hub/web/trafilatura_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739207 llama_hub-0.0.3/llama_hub/web/trafilatura_web/__init__.py
+-rw-r--r--   0        0        0      889 2023-05-31 00:19:23.739262 llama_hub-0.0.3/llama_hub/web/trafilatura_web/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.739305 llama_hub-0.0.3/llama_hub/web/trafilatura_web/requirements.txt
+-rw-r--r--   0        0        0     1075 2023-05-31 00:19:23.739438 llama_hub-0.0.3/llama_hub/web/unstructured_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.739468 llama_hub-0.0.3/llama_hub/web/unstructured_web/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-31 00:19:23.739541 llama_hub-0.0.3/llama_hub/web/unstructured_web/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:19:23.739609 llama_hub-0.0.3/llama_hub/web/unstructured_web/requirements.txt
+-rw-r--r--   0        0        0     1315 2023-05-31 00:19:23.739686 llama_hub-0.0.3/llama_hub/whatsapp/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739729 llama_hub-0.0.3/llama_hub/whatsapp/__init__.py
+-rw-r--r--   0        0        0     1509 2023-05-31 00:19:23.739776 llama_hub-0.0.3/llama_hub/whatsapp/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739818 llama_hub-0.0.3/llama_hub/whatsapp/requirements.txt
+-rw-r--r--   0        0        0      895 2023-05-31 00:19:23.739897 llama_hub-0.0.3/llama_hub/wikipedia/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739946 llama_hub-0.0.3/llama_hub/wikipedia/__init__.py
+-rw-r--r--   0        0        0      818 2023-05-31 00:19:23.740017 llama_hub-0.0.3/llama_hub/wikipedia/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:19:23.740060 llama_hub-0.0.3/llama_hub/wikipedia/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.740135 llama_hub-0.0.3/llama_hub/wordpress/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740190 llama_hub-0.0.3/llama_hub/wordpress/__init__.py
+-rw-r--r--   0        0        0     2546 2023-05-31 00:19:23.740248 llama_hub-0.0.3/llama_hub/wordpress/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.740291 llama_hub-0.0.3/llama_hub/wordpress/requirements.txt
+-rw-r--r--   0        0        0      774 2023-05-31 00:19:23.740378 llama_hub-0.0.3/llama_hub/youtube_transcript/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740429 llama_hub-0.0.3/llama_hub/youtube_transcript/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-31 00:19:23.740509 llama_hub-0.0.3/llama_hub/youtube_transcript/base.py
+-rw-r--r--   0        0        0       29 2023-05-31 00:19:23.740552 llama_hub-0.0.3/llama_hub/youtube_transcript/requirements.txt
+-rw-r--r--   0        0        0      884 2023-05-31 00:19:23.740654 llama_hub-0.0.3/llama_hub/zendesk/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740708 llama_hub-0.0.3/llama_hub/zendesk/__init__.py
+-rw-r--r--   0        0        0     2323 2023-05-31 00:19:23.740795 llama_hub-0.0.3/llama_hub/zendesk/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.740869 llama_hub-0.0.3/llama_hub/zendesk/requirements.txt
+-rw-r--r--   0        0        0     1304 2023-05-31 00:19:23.740971 llama_hub-0.0.3/llama_hub/zulip/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.741018 llama_hub-0.0.3/llama_hub/zulip/__init__.py
+-rw-r--r--   0        0        0     2432 2023-05-31 00:19:23.741092 llama_hub-0.0.3/llama_hub/zulip/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.741155 llama_hub-0.0.3/llama_hub/zulip/requirements.txt
+-rw-r--r--   0        0        0      868 2023-06-10 07:59:48.313999 llama_hub-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 llama_hub-0.0.3/PKG-INFO
```

### Comparing `llama_hub-0.0.2/LICENSE` & `llama_hub-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/README.md` & `llama_hub-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/airtable/README.md` & `llama_hub-0.0.3/llama_hub/airtable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/airtable/base.py` & `llama_hub-0.0.3/llama_hub/airtable/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/apify/actor/README.md` & `llama_hub-0.0.3/llama_hub/apify/actor/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/apify/actor/base.py` & `llama_hub-0.0.3/llama_hub/apify/actor/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/apify/dataset/README.md` & `llama_hub-0.0.3/llama_hub/apify/dataset/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/apify/dataset/base.py` & `llama_hub-0.0.3/llama_hub/apify/dataset/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/asana/README.md` & `llama_hub-0.0.3/llama_hub/asana/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/asana/base.py` & `llama_hub-0.0.3/llama_hub/asana/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/azcognitive_search/README.md` & `llama_hub-0.0.3/llama_hub/azcognitive_search/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/azcognitive_search/base.py` & `llama_hub-0.0.3/llama_hub/azcognitive_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/azstorage_blob/README.md` & `llama_hub-0.0.3/llama_hub/azstorage_blob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/azstorage_blob/base.py` & `llama_hub-0.0.3/llama_hub/azstorage_blob/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/bilibili/README.md` & `llama_hub-0.0.3/llama_hub/bilibili/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/bilibili/base.py` & `llama_hub-0.0.3/llama_hub/bilibili/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/boarddocs/BoardDocsReader.ipynb` & `llama_hub-0.0.3/llama_hub/boarddocs/BoardDocsReader.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/boarddocs/README.md` & `llama_hub-0.0.3/llama_hub/boarddocs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/boarddocs/base.py` & `llama_hub-0.0.3/llama_hub/boarddocs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/boarddocs/crawl.ipynb` & `llama_hub-0.0.3/llama_hub/boarddocs/crawl.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/chatgpt_plugin/README.md` & `llama_hub-0.0.3/llama_hub/chatgpt_plugin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/chatgpt_plugin/base.py` & `llama_hub-0.0.3/llama_hub/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/chroma/README.md` & `llama_hub-0.0.3/llama_hub/chroma/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/chroma/base.py` & `llama_hub-0.0.3/llama_hub/chroma/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/confluence/README.md` & `llama_hub-0.0.3/llama_hub/confluence/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/confluence/base.py` & `llama_hub-0.0.3/llama_hub/confluence/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/couchdb/README.md` & `llama_hub-0.0.3/llama_hub/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/couchdb/base.py` & `llama_hub-0.0.3/llama_hub/couchdb/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/dad_jokes/README.md` & `llama_hub-0.0.3/llama_hub/dad_jokes/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/dad_jokes/base.py` & `llama_hub-0.0.3/llama_hub/dad_jokes/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/database/README.md` & `llama_hub-0.0.3/llama_hub/database/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/database/base.py` & `llama_hub-0.0.3/llama_hub/database/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/deeplake/README.md` & `llama_hub-0.0.3/llama_hub/deeplake/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/deeplake/base.py` & `llama_hub-0.0.3/llama_hub/deeplake/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/discord/README.md` & `llama_hub-0.0.3/llama_hub/discord/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/discord/base.py` & `llama_hub-0.0.3/llama_hub/discord/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/docugami/README.md` & `llama_hub-0.0.3/llama_hub/docugami/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/docugami/base.py` & `llama_hub-0.0.3/llama_hub/docugami/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/docugami/docugami.ipynb` & `llama_hub-0.0.3/llama_hub/docugami/docugami.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/elasticsearch/README.md` & `llama_hub-0.0.3/llama_hub/elasticsearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/elasticsearch/base.py` & `llama_hub-0.0.3/llama_hub/elasticsearch/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/faiss/README.md` & `llama_hub-0.0.3/llama_hub/faiss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/faiss/base.py` & `llama_hub-0.0.3/llama_hub/faiss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/feedly_rss/README.md` & `llama_hub-0.0.3/llama_hub/feedly_rss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/feedly_rss/base.py` & `llama_hub-0.0.3/llama_hub/feedly_rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/README.md` & `llama_hub-0.0.3/llama_hub/file/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/audio/README.md` & `llama_hub-0.0.3/llama_hub/file/audio/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/audio/base.py` & `llama_hub-0.0.3/llama_hub/file/audio/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/audio_gladia/README.md` & `llama_hub-0.0.3/llama_hub/file/audio_gladia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/audio_gladia/base.py` & `llama_hub-0.0.3/llama_hub/file/audio_gladia/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/base.py` & `llama_hub-0.0.3/llama_hub/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/cjk_pdf/README.md` & `llama_hub-0.0.3/llama_hub/file/cjk_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/cjk_pdf/base.py` & `llama_hub-0.0.3/llama_hub/file/cjk_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/deepdoctection/README.md` & `llama_hub-0.0.3/llama_hub/file/deepdoctection/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/deepdoctection/base.py` & `llama_hub-0.0.3/llama_hub/file/deepdoctection/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/docx/README.md` & `llama_hub-0.0.3/llama_hub/file/docx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/docx/base.py` & `llama_hub-0.0.3/llama_hub/file/docx/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/epub/README.md` & `llama_hub-0.0.3/llama_hub/file/epub/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/epub/base.py` & `llama_hub-0.0.3/llama_hub/file/epub/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/flat_pdf/README.md` & `llama_hub-0.0.3/llama_hub/file/flat_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/flat_pdf/base.py` & `llama_hub-0.0.3/llama_hub/file/flat_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/image/README.md` & `llama_hub-0.0.3/llama_hub/file/image/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/image/base.py` & `llama_hub-0.0.3/llama_hub/file/image/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/image_blip/base.py` & `llama_hub-0.0.3/llama_hub/file/image_blip/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/image_blip2/base.py` & `llama_hub-0.0.3/llama_hub/file/image_blip2/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/ipynb/base.py` & `llama_hub-0.0.3/llama_hub/file/ipynb/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/json/README.md` & `llama_hub-0.0.3/llama_hub/file/json/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/json/base.py` & `llama_hub-0.0.3/llama_hub/file/json/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/markdown/README.md` & `llama_hub-0.0.3/llama_hub/file/markdown/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/markdown/base.py` & `llama_hub-0.0.3/llama_hub/file/markdown/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/mbox/README.md` & `llama_hub-0.0.3/llama_hub/file/mbox/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/mbox/base.py` & `llama_hub-0.0.3/llama_hub/file/mbox/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/paged_csv/README.md` & `llama_hub-0.0.3/llama_hub/file/paged_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/paged_csv/base.py` & `llama_hub-0.0.3/llama_hub/file/paged_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pandas_csv/README.md` & `llama_hub-0.0.3/llama_hub/file/pandas_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pandas_csv/base.py` & `llama_hub-0.0.3/llama_hub/file/pandas_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pandas_excel/README.md` & `llama_hub-0.0.3/llama_hub/file/pandas_excel/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pandas_excel/base.py` & `llama_hub-0.0.3/llama_hub/file/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pdf/README.md` & `llama_hub-0.0.3/llama_hub/file/pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pdf/base.py` & `llama_hub-0.0.3/llama_hub/file/pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pptx/README.md` & `llama_hub-0.0.3/llama_hub/file/pptx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pptx/base.py` & `llama_hub-0.0.3/llama_hub/file/pptx/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pymu_pdf/README.md` & `llama_hub-0.0.3/llama_hub/file/pymu_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/pymu_pdf/base.py` & `llama_hub-0.0.3/llama_hub/file/pymu_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/rdf/README.md` & `llama_hub-0.0.3/llama_hub/file/rdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/rdf/base.py` & `llama_hub-0.0.3/llama_hub/file/rdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/simple_csv/README.md` & `llama_hub-0.0.3/llama_hub/file/simple_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/simple_csv/base.py` & `llama_hub-0.0.3/llama_hub/file/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/unstructured/README.md` & `llama_hub-0.0.3/llama_hub/file/unstructured/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/file/unstructured/base.py` & `llama_hub-0.0.3/llama_hub/file/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/github_repo/README.md` & `llama_hub-0.0.3/llama_hub/github_repo/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,9 +79,11 @@
     docs = loader.load_data(branch="main")
 
     with open("docs.pkl", "wb") as f:
         pickle.dump(docs, f)
 
 index = GPTVectorStoreIndex.from_documents(docs)
 
-index.query("Explain each LlamaIndex class?")
+query_engine = index.as_query_engine()
+response = query_engine.query("Explain each LlamaIndex class?")
+print(response)
 ```
```

### Comparing `llama_hub-0.0.2/llama_hub/github_repo/base.py` & `llama_hub-0.0.3/llama_hub/github_repo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/github_repo/github_client.py` & `llama_hub-0.0.3/llama_hub/github_repo/github_client.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/github_repo/utils.py` & `llama_hub-0.0.3/llama_hub/github_repo/utils.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/gmail/README.md` & `llama_hub-0.0.3/llama_hub/gmail/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/gmail/base.py` & `llama_hub-0.0.3/llama_hub/gmail/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_calendar/README.md` & `llama_hub-0.0.3/llama_hub/google_calendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_calendar/base.py` & `llama_hub-0.0.3/llama_hub/google_calendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_docs/README.md` & `llama_hub-0.0.3/llama_hub/google_docs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_docs/base.py` & `llama_hub-0.0.3/llama_hub/google_docs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_drive/README.md` & `llama_hub-0.0.3/llama_hub/google_drive/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_drive/base.py` & `llama_hub-0.0.3/llama_hub/google_drive/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_sheets/README.md` & `llama_hub-0.0.3/llama_hub/google_sheets/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/google_sheets/base.py` & `llama_hub-0.0.3/llama_hub/google_sheets/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/gpt_repo/README.md` & `llama_hub-0.0.3/llama_hub/gpt_repo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/gpt_repo/base.py` & `llama_hub-0.0.3/llama_hub/gpt_repo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/graphdb_cypher/README.md` & `llama_hub-0.0.3/llama_hub/graphdb_cypher/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/graphdb_cypher/base.py` & `llama_hub-0.0.3/llama_hub/graphdb_cypher/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/graphql/README.md` & `llama_hub-0.0.3/llama_hub/graphql/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/graphql/base.py` & `llama_hub-0.0.3/llama_hub/graphql/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/hatena_blog/README.md` & `llama_hub-0.0.3/llama_hub/hatena_blog/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/hatena_blog/base.py` & `llama_hub-0.0.3/llama_hub/hatena_blog/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/hubspot/README.md` & `llama_hub-0.0.3/llama_hub/hubspot/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/hubspot/base.py` & `llama_hub-0.0.3/llama_hub/hubspot/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/huggingface/fs/README.md` & `llama_hub-0.0.3/llama_hub/huggingface/fs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/huggingface/fs/base.py` & `llama_hub-0.0.3/llama_hub/huggingface/fs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/intercom/README.md` & `llama_hub-0.0.3/llama_hub/intercom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/intercom/base.py` & `llama_hub-0.0.3/llama_hub/intercom/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/jira/README.md` & `llama_hub-0.0.3/llama_hub/jira/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,28 @@
-# JIRA Loader
+# JIRA Reader
 
 The Jira loader returns a set of issues based on the query provided to the dataloader. The user intializes the reader with an email, API token and the URL of the server they wish to fetch issues from.
 
 ## Usage
 
 Here's an example of how to use it
 
 ```python
-from llama_index import download_loader
-import os
 
-JiraReader = download_reader('JiraReader')
+from llama_hub.jira.base import JiraReader
+
+reader = JiraReader(email=email, api_token=api_token, server_url="https://your-jira-server.com")
+documents = reader.load_data(query='project = <your-project>')
+
+```
+
+Alternately, you can also use download_loader from llama_index
+
+```python
+
+from llama_index import download_loader
+JiraReader = download_loader('JiraReader')
 
 reader = JiraReader(email=email, api_token=api_token, server_url="https://your-jira-server.com")
 documents = reader.load_data(query='project = <your-project>')
 
 ```
```

### Comparing `llama_hub-0.0.2/llama_hub/jira/base.py` & `llama_hub-0.0.3/llama_hub/jira/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/joplin/README.md` & `llama_hub-0.0.3/llama_hub/joplin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/joplin/base.py` & `llama_hub-0.0.3/llama_hub/joplin/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/jsondata/README.md` & `llama_hub-0.0.3/llama_hub/jsondata/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/jsondata/base.py` & `llama_hub-0.0.3/llama_hub/jsondata/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/kaltura/esearch/README.md` & `llama_hub-0.0.3/llama_hub/kaltura/esearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/kaltura/esearch/base.py` & `llama_hub-0.0.3/llama_hub/kaltura/esearch/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/library.json` & `llama_hub-0.0.3/llama_hub/library.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9814814814814815%*

 * *Differences: {"'FirestoreReader'": "OrderedDict([('id', 'firestore'), ('author', 'rayzhudev'), ('keywords', "*

 * *                      "['firestore', 'datastore'])])",*

 * * "'PDFMinerReader'": "OrderedDict([('id', 'file/pdf_miner'), ('author', 'thunderbug1'), "*

 * *                     "('keywords', ['pdf'])])"}*

```diff
@@ -159,14 +159,22 @@
         "author": "kychanbp",
         "id": "feedly_rss",
         "keywords": [
             "feedly",
             "rss"
         ]
     },
+    "FirestoreReader": {
+        "author": "rayzhudev",
+        "id": "firestore",
+        "keywords": [
+            "firestore",
+            "datastore"
+        ]
+    },
     "FlatPdfReader": {
         "author": "emmanuel-oliveira",
         "id": "file/flat_pdf",
         "keywords": [
             "pdf",
             "flat",
             "flattened"
@@ -439,14 +447,21 @@
         "author": "tevslin",
         "id": "outlook_localcalendar",
         "keywords": [
             "calendar",
             "outlook"
         ]
     },
+    "PDFMinerReader": {
+        "author": "thunderbug1",
+        "id": "file/pdf_miner",
+        "keywords": [
+            "pdf"
+        ]
+    },
     "PDFReader": {
         "author": "ravi03071991",
         "id": "file/pdf"
     },
     "PagedCSVReader": {
         "author": "thejessezhang",
         "id": "file/paged_csv"
```

### Comparing `llama_hub-0.0.2/llama_hub/make_com/README.md` & `llama_hub-0.0.3/llama_hub/make_com/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/make_com/base.py` & `llama_hub-0.0.3/llama_hub/make_com/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mangoapps_guides/README.md` & `llama_hub-0.0.3/llama_hub/mangoapps_guides/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mangoapps_guides/base.py` & `llama_hub-0.0.3/llama_hub/mangoapps_guides/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/maps/README.md` & `llama_hub-0.0.3/llama_hub/maps/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/maps/base.py` & `llama_hub-0.0.3/llama_hub/maps/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/memos/README.md` & `llama_hub-0.0.3/llama_hub/memos/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/memos/base.py` & `llama_hub-0.0.3/llama_hub/memos/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/metal/README.md` & `llama_hub-0.0.3/llama_hub/metal/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/metal/base.py` & `llama_hub-0.0.3/llama_hub/metal/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/milvus/README.md` & `llama_hub-0.0.3/llama_hub/milvus/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/milvus/base.py` & `llama_hub-0.0.3/llama_hub/milvus/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mondaydotcom/README.md` & `llama_hub-0.0.3/llama_hub/mondaydotcom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mondaydotcom/base.py` & `llama_hub-0.0.3/llama_hub/mondaydotcom/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mongo/README.md` & `llama_hub-0.0.3/llama_hub/mongo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/mongo/base.py` & `llama_hub-0.0.3/llama_hub/mongo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/notion/README.md` & `llama_hub-0.0.3/llama_hub/notion/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/notion/base.py` & `llama_hub-0.0.3/llama_hub/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/obsidian/README.md` & `llama_hub-0.0.3/llama_hub/obsidian/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/obsidian/base.py` & `llama_hub-0.0.3/llama_hub/obsidian/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/README.md` & `llama_hub-0.0.3/llama_hub/opendal_reader/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/azblob/README.md` & `llama_hub-0.0.3/llama_hub/opendal_reader/azblob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/azblob/base.py` & `llama_hub-0.0.3/llama_hub/opendal_reader/azblob/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/base.py` & `llama_hub-0.0.3/llama_hub/opendal_reader/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/gcs/README.md` & `llama_hub-0.0.3/llama_hub/opendal_reader/gcs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/gcs/base.py` & `llama_hub-0.0.3/llama_hub/opendal_reader/gcs/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/s3/README.md` & `llama_hub-0.0.3/llama_hub/opendal_reader/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/opendal_reader/s3/base.py` & `llama_hub-0.0.3/llama_hub/opendal_reader/s3/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/outlook_localcalendar/README.md` & `llama_hub-0.0.3/llama_hub/outlook_localcalendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/outlook_localcalendar/base.py` & `llama_hub-0.0.3/llama_hub/outlook_localcalendar/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/pandas_ai/README.md` & `llama_hub-0.0.3/llama_hub/pandas_ai/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/pandas_ai/base.py` & `llama_hub-0.0.3/llama_hub/pandas_ai/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/papers/arxiv/README.md` & `llama_hub-0.0.3/llama_hub/papers/arxiv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/papers/arxiv/base.py` & `llama_hub-0.0.3/llama_hub/papers/arxiv/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/papers/pubmed/README.md` & `llama_hub-0.0.3/llama_hub/papers/pubmed/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/papers/pubmed/base.py` & `llama_hub-0.0.3/llama_hub/papers/pubmed/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/pinecone/README.md` & `llama_hub-0.0.3/llama_hub/pinecone/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/pinecone/base.py` & `llama_hub-0.0.3/llama_hub/pinecone/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/qdrant/README.md` & `llama_hub-0.0.3/llama_hub/qdrant/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/qdrant/base.py` & `llama_hub-0.0.3/llama_hub/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/readwise/README.md` & `llama_hub-0.0.3/llama_hub/readwise/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/readwise/base.py` & `llama_hub-0.0.3/llama_hub/readwise/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/reddit/README.md` & `llama_hub-0.0.3/llama_hub/reddit/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/reddit/base.py` & `llama_hub-0.0.3/llama_hub/reddit/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/remote/README.md` & `llama_hub-0.0.3/llama_hub/remote/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/remote/base.py` & `llama_hub-0.0.3/llama_hub/remote/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/remote_depth/README.md` & `llama_hub-0.0.3/llama_hub/remote_depth/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/remote_depth/base.py` & `llama_hub-0.0.3/llama_hub/remote_depth/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/s3/README.md` & `llama_hub-0.0.3/llama_hub/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/s3/base.py` & `llama_hub-0.0.3/llama_hub/s3/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/slack/README.md` & `llama_hub-0.0.3/llama_hub/slack/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/slack/base.py` & `llama_hub-0.0.3/llama_hub/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/snscrape_twitter/README.md` & `llama_hub-0.0.3/llama_hub/snscrape_twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/snscrape_twitter/base.py` & `llama_hub-0.0.3/llama_hub/snscrape_twitter/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/spotify/README.md` & `llama_hub-0.0.3/llama_hub/spotify/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/spotify/base.py` & `llama_hub-0.0.3/llama_hub/spotify/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/stackoverflow/README.md` & `llama_hub-0.0.3/llama_hub/stackoverflow/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/stackoverflow/base.py` & `llama_hub-0.0.3/llama_hub/stackoverflow/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/steamship/README.md` & `llama_hub-0.0.3/llama_hub/steamship/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/steamship/base.py` & `llama_hub-0.0.3/llama_hub/steamship/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/string_iterable/README.md` & `llama_hub-0.0.3/llama_hub/string_iterable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/string_iterable/base.py` & `llama_hub-0.0.3/llama_hub/string_iterable/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/trello/README.md` & `llama_hub-0.0.3/llama_hub/trello/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/trello/base.py` & `llama_hub-0.0.3/llama_hub/trello/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/twitter/README.md` & `llama_hub-0.0.3/llama_hub/twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/twitter/base.py` & `llama_hub-0.0.3/llama_hub/twitter/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/utils.py` & `llama_hub-0.0.3/llama_hub/utils.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/weather/README.md` & `llama_hub-0.0.3/llama_hub/weather/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/weather/base.py` & `llama_hub-0.0.3/llama_hub/weather/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/weaviate/README.md` & `llama_hub-0.0.3/llama_hub/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/weaviate/base.py` & `llama_hub-0.0.3/llama_hub/weaviate/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/async_web/base.py` & `llama_hub-0.0.3/llama_hub/web/async_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/README.md` & `llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/beautiful_soup_web/base.py` & `llama_hub-0.0.3/llama_hub/web/beautiful_soup_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/knowledge_base/README.md` & `llama_hub-0.0.3/llama_hub/web/knowledge_base/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/knowledge_base/base.py` & `llama_hub-0.0.3/llama_hub/web/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/readability_web/README.md` & `llama_hub-0.0.3/llama_hub/web/readability_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/readability_web/Readability.js` & `llama_hub-0.0.3/llama_hub/web/readability_web/Readability.js`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/readability_web/base.py` & `llama_hub-0.0.3/llama_hub/web/readability_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/rss/base.py` & `llama_hub-0.0.3/llama_hub/web/rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/simple_web/README.md` & `llama_hub-0.0.3/llama_hub/web/simple_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/simple_web/base.py` & `llama_hub-0.0.3/llama_hub/web/simple_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/trafilatura_web/README.md` & `llama_hub-0.0.3/llama_hub/web/trafilatura_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/trafilatura_web/base.py` & `llama_hub-0.0.3/llama_hub/web/trafilatura_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/unstructured_web/README.md` & `llama_hub-0.0.3/llama_hub/web/unstructured_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/web/unstructured_web/base.py` & `llama_hub-0.0.3/llama_hub/web/unstructured_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/whatsapp/README.md` & `llama_hub-0.0.3/llama_hub/whatsapp/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/whatsapp/base.py` & `llama_hub-0.0.3/llama_hub/whatsapp/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/wikipedia/README.md` & `llama_hub-0.0.3/llama_hub/wikipedia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/wikipedia/base.py` & `llama_hub-0.0.3/llama_hub/wikipedia/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/wordpress/README.md` & `llama_hub-0.0.3/llama_hub/wordpress/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/wordpress/base.py` & `llama_hub-0.0.3/llama_hub/wordpress/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/youtube_transcript/README.md` & `llama_hub-0.0.3/llama_hub/youtube_transcript/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/youtube_transcript/base.py` & `llama_hub-0.0.3/llama_hub/youtube_transcript/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/zendesk/README.md` & `llama_hub-0.0.3/llama_hub/zendesk/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/zendesk/base.py` & `llama_hub-0.0.3/llama_hub/zendesk/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/zulip/README.md` & `llama_hub-0.0.3/llama_hub/zulip/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/llama_hub/zulip/base.py` & `llama_hub-0.0.3/llama_hub/zulip/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.2/pyproject.toml` & `llama_hub-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llama-hub"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. "
 authors = ["Jerry Liu", "Jesse Zhang"]
 # New attributes
 license = "MIT"
 readme = "README.md"
 homepage = "https://llamahub.ai"
 repository = "https://github.com/emptycrown/llama-hub"
```

### Comparing `llama_hub-0.0.2/PKG-INFO` & `llama_hub-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-hub
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. 
 Home-page: https://llamahub.ai
 License: MIT
 Keywords: llama-index,llama-hub,llama
 Author: Jerry Liu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

