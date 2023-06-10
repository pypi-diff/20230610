# Comparing `tmp/rmrkl-0.0.2.tar.gz` & `tmp/rmrkl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmrkl-0.0.2.tar", last modified: Wed May  3 06:36:03 2023, max compression
+gzip compressed data, was "rmrkl-0.0.3.tar", last modified: Sat Jun 10 01:07:55 2023, max compression
```

## Comparing `rmrkl-0.0.2.tar` & `rmrkl-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-03 06:35:31.000000 rmrkl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 06:36:03.724211 rmrkl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 06:35:31.000000 rmrkl-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.720211 rmrkl-0.0.2/rmrkl/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 06:35:31.000000 rmrkl-0.0.2/rmrkl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/rmrkl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-03 06:36:03.000000 rmrkl-0.0.2/rmrkl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:36:03.724211 rmrkl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-03 06:35:31.000000 rmrkl-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:36:03.724211 rmrkl-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-03 06:35:31.000000 rmrkl-0.0.2/tests/test_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:07:55.462046 rmrkl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-10 01:07:22.000000 rmrkl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-10 01:07:55.462046 rmrkl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-10 01:07:22.000000 rmrkl-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:07:55.458046 rmrkl-0.0.3/rmrkl/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 01:07:22.000000 rmrkl-0.0.3/rmrkl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:07:55.462046 rmrkl-0.0.3/rmrkl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-10 01:07:55.000000 rmrkl-0.0.3/rmrkl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-10 01:07:55.000000 rmrkl-0.0.3/rmrkl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:07:55.000000 rmrkl-0.0.3/rmrkl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-10 01:07:55.000000 rmrkl-0.0.3/rmrkl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-10 01:07:55.000000 rmrkl-0.0.3/rmrkl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:07:55.462046 rmrkl-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-10 01:07:22.000000 rmrkl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:07:55.462046 rmrkl-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-10 01:07:22.000000 rmrkl-0.0.3/tests/test_agent.py
```

### Comparing `rmrkl-0.0.2/LICENSE` & `rmrkl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.2/PKG-INFO` & `rmrkl-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmrkl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Robust Modular Reasoning, Knowledge and Language agent that uses tools and retries on failure
 Home-page: https://github.com/whitead/robust-mrkl
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rmrkl-0.0.2/rmrkl/agent.py` & `rmrkl-0.0.3/rmrkl/agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from __future__ import annotations
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.callbacks.base import BaseCallbackManager
-from .prompts import FORMAT_INSTRUCTIONS, SUFFIX, QUESTION_PROMPT
+from .prompts import FORMAT_INSTRUCTIONS, SUFFIX, QUESTION_PROMPT, PREFIX
 from langchain.agents.agent import Agent, AgentOutputParser
 from typing import Any, Optional, Sequence
 from langchain.tools import BaseTool
 from langchain.agents.mrkl.base import ZeroShotAgent
 from langchain.prompts.chat import (
     ChatPromptTemplate,
     SystemMessagePromptTemplate,
     HumanMessagePromptTemplate,
     AIMessagePromptTemplate,
 )
+from .output_parser import ChatZeroShotOutputParser
 
 
 class ChatZeroShotAgent(ZeroShotAgent):
     """Agent for the MRKL chain."""
 
     @classmethod
     def create_prompt(
         cls,
         tools: Sequence[BaseTool],
+        prefix: str = PREFIX,
         suffix: str = SUFFIX,
         format_instructions: str = FORMAT_INSTRUCTIONS,
+        question_prompt: str = QUESTION_PROMPT,
     ) -> PromptTemplate:
         """Create prompt in the style of the zero shot agent.
 
         Args:
             tools: List of tools the agent will have access to, used to format the
                 prompt.
             prefix: String to put before the list of tools.
@@ -42,45 +45,54 @@
             [f"    {tool.name}: {tool.description}" for tool in tools]
         )
         tool_names = ", ".join([tool.name for tool in tools])
         format_instructions = format_instructions.format(
             tool_names=tool_names, tool_strings=tool_strings
         )
         human_prompt = PromptTemplate(
-            template=QUESTION_PROMPT,
+            template=question_prompt,
             input_variables=["input"],
             partial_variables={"tool_strings": tool_strings},
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=human_prompt)
         ai_message_prompt = AIMessagePromptTemplate.from_template(suffix)
         system_message_prompt = SystemMessagePromptTemplate.from_template(
-            format_instructions
+            '\n\n'.join(
+                [
+                    prefix,
+                    format_instructions
+                ]
+            )
         )
         # ignore suffix
         return ChatPromptTemplate.from_messages(
             [system_message_prompt, human_message_prompt, ai_message_prompt]
         )
 
     @classmethod
     def from_llm_and_tools(
         cls,
         llm: BaseChatModel,
         tools: Sequence[BaseTool],
         callback_manager: Optional[BaseCallbackManager] = None,
-        output_parser: Optional[AgentOutputParser] = None,
+        output_parser: Optional[AgentOutputParser] = ChatZeroShotOutputParser(),
+        prefix: str = PREFIX,
         suffix: str = SUFFIX,
         format_instructions: str = FORMAT_INSTRUCTIONS,
+        question_prompt: str = QUESTION_PROMPT,
         **kwargs: Any,
     ) -> Agent:
         """Construct an agent from an LLM and tools."""
         cls._validate_tools(tools)
         prompt = cls.create_prompt(
             tools,
+            prefix=prefix,
             suffix=suffix,
             format_instructions=format_instructions,
+            question_prompt=question_prompt,
         )
         llm_chain = LLMChain(
             llm=llm,
             prompt=prompt,
             callback_manager=callback_manager,
         )
         tool_names = [tool.name for tool in tools]
```

### Comparing `rmrkl-0.0.2/rmrkl/executor.py` & `rmrkl-0.0.3/rmrkl/executor.py`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.2/rmrkl/prompts.py` & `rmrkl-0.0.3/rmrkl/prompts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 # flake8: noqa
-FORMAT_INSTRUCTIONS = """You are an AI system that only responds
-with a single complete Thought, Action, Action Input format
+
+PREFIX = """
+You are an AI system.
+"""
+FORMAT_INSTRUCTIONS = """
+You should only respond with a single complete
+Thought, Action, Action Input format
 OR a single Final Answer format.
 
 Complete Format:
 
 Thought: (reflect on your progress and decide what to do next)
 Action: (the action name, should be one of [{tool_names}])
-Action Input: (the input string to the action) 
+Action Input: (the input string to the action)
 
 OR
 
 Final Answer: (the final answer to the original input question)
 
 """
 QUESTION_PROMPT = """
```

### Comparing `rmrkl-0.0.2/rmrkl.egg-info/PKG-INFO` & `rmrkl-0.0.3/rmrkl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmrkl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Robust Modular Reasoning, Knowledge and Language agent that uses tools and retries on failure
 Home-page: https://github.com/whitead/robust-mrkl
 Author: Andrew White
 Author-email: andrew.white@rochester.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rmrkl-0.0.2/setup.py` & `rmrkl-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `rmrkl-0.0.2/tests/test_agent.py` & `rmrkl-0.0.3/tests/test_agent.py`

 * *Files identical despite different names*

