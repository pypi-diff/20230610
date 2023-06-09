# Comparing `tmp/openlrc-0.0.3.tar.gz` & `tmp/openlrc-0.0.4.tar.gz`

## Comparing `openlrc-0.0.3.tar` & `openlrc-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/exceptions.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/logger.py
--rw-r--r--   0        0        0    10941 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/lrc.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/openlrc.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/prompter.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 openlrc-0.0.3/openlrc/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openlrc-0.0.3/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 openlrc-0.0.3/LICENSE
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 openlrc-0.0.3/README.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 openlrc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 openlrc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 openlrc-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/__init__.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/chatbot.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/exceptions.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/logger.py
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/lrc.py
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/openlrc.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/prompter.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 openlrc-0.0.4/openlrc/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openlrc-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 openlrc-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 openlrc-0.0.4/README.md
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 openlrc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 openlrc-0.0.4/PKG-INFO
```

### Comparing `openlrc-0.0.3/openlrc/lrc.py` & `openlrc-0.0.4/openlrc/lrc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import math
-import os
 import sys
-import time
 from dataclasses import dataclass
 from typing import List, Union
 
-import openai
 from langcodes import Language
 
+from openlrc.chatbot import GPTBot
 from openlrc.exceptions import SameLanguageException
 from openlrc.logger import logger
 from openlrc.prompter import BaseTranslatePrompter, format_texts
-from openlrc.utils import extend_filename, get_token_number, json2dict
+from openlrc.utils import extend_filename, json2dict
 
 
 @dataclass
 class LRCElement:
     """
     Save a LRC format element.
     """
@@ -79,96 +77,74 @@
                 )
 
                 if i != len(self.elements) - 1 and element.end != self.elements[i + 1].start:
                     print(f'[{self.format_timestamp(element.end)}]', file=f, flush=True)
 
         return file
 
-    def translate(self, chunk_size=20, source_lang=None, target_lang='zh-cn', prompter=BaseTranslatePrompter(),
+    def get_system_prompt(self, src_lang, target_lang, prompter):
+        system_prompt = str(prompter).format(
+            src_lang=Language.get(self.lang if not src_lang else src_lang).display_name('en'),
+            target_lang=Language.get(target_lang).display_name('en')
+        )
+        # Prevent translating text into Traditional Chinese
+        if target_lang == 'zh-cn':
+            system_prompt.replace(Language.get(target_lang).display_name('en'), 'Mandarin Chinese')
+
+        return system_prompt
+
+    def translate(self, prompter=BaseTranslatePrompter(), chunk_size=20, src_lang=None, target_lang='zh-cn',
                   intercept_line=None, force_translate=False):
         """
         Use GPT-3.5 to translate lyrics.
-        :param chunk_size: use smaller chunk size to avoid exceeding the token limit & output complete message.
-        :param source_lang: source language.
-        :param target_lang: target language.
-        :param prompter: translate prompter.
-        :param intercept_line: intercepted lyrics line number.
-        :return:
+        TODO: dynamically adjust the chunk size.
+        :param chunk_size: Use smaller chunk size to avoid exceeding the token limit & output complete message.
+        :param src_lang: Source language.
+        :param target_lang: Target language.
+        :param prompter: Translate prompter.
+        :param intercept_line: Intercepted lyrics line number.
+        :param force_translate: Force translation even if the source language is the same as the target language.
+        :return: The translated lrc file path.
         """
         if not force_translate and \
-                Language.get(self.lang if not source_lang else source_lang).language_name() \
+                Language.get(self.lang if not src_lang else src_lang).language_name() \
                 == Language.get(target_lang).language_name():
             raise SameLanguageException()
 
-        # Set OpenAI API key
-        openai.api_key = os.getenv("OPENAI_API_KEY")
+        # Resulted json content
+        json_content = {'total_number': 0, 'list': []}
 
-        lyrics = [element.text for element in self.elements[:intercept_line]]
+        system_prompt = self.get_system_prompt(src_lang, target_lang, prompter)
+        translate_bot = GPTBot(system_prompt=system_prompt)
 
+        lyrics = [element.text for element in self.elements[:intercept_line]]
         # Split lyrics into different chunks
         chunks = [lyrics[i:i + chunk_size] for i in range(0, len(lyrics), chunk_size)]
+        user_prompts = [format_texts(chunk) for chunk in chunks]  # Format the chunks into a single string
 
-        json_content = {'total_number': 0, 'list': []}
-
-        system_prompt = str(prompter).format(
-            source_lang=Language.get(self.lang if not source_lang else source_lang).display_name('en'),
-            target_lang=Language.get(target_lang).display_name('en')
-        )
-
-        # Prevent translating text into Traditional Chinese
-        if target_lang == 'zh-cn':
-            system_prompt.replace(Language.get(target_lang).display_name('en'), 'Mandarin Chinese')
-
-        for chunk in chunks:
-            # Format the input
-            raw_content = format_texts(chunk)
-
-            logger.info(f'Raw content: {raw_content}')
-            token_number = get_token_number(raw_content + system_prompt)
-            logger.info(f'Total token number: {token_number}')
-
-            assert token_number < 4096, 'Token number exceeds the limit.'
-
-            while 1:
-                try:
-                    response = openai.ChatCompletion.create(
-                        model="gpt-3.5-turbo",
-                        messages=[
-                            {
-                                'role': 'system',
-                                'content': system_prompt
-                            },
-                            {
-                                'role': 'user',
-                                'content': raw_content
-                            }
-                        ]
-                    )
-                    break
-                except openai.error.RateLimitError:
-                    logger.warning('Rate limit exceeded. Wait 10s before retry.')
-                    time.sleep(10)
-                except openai.error.APIConnectionError:
-                    logger.warning('API connection error. Wait 30s before retry.')
-                    time.sleep(30)
+        logger.info(f'Translating {len(user_prompts)} user_prompts of lyrics with async call.')
 
-            target_content = response.choices[0].message.content
-            logger.info(f'Target content: {target_content}')
+        # Start translate
+        responses = translate_bot.message(user_prompts)
+        for i, response in enumerate(responses):
+            content = response.choices[0].message.content
+            logger.debug(f'Target content - chunk{i}: {content}')
 
-            chunk_json_content = json2dict(target_content)
-            logger.info(f'Length of the translated chunk: {len(chunk_json_content["list"])}')
+            chunk_json_content = json2dict(content)
+            logger.debug(f'Length of the translated chunk: {len(chunk_json_content["list"])}')
 
+            chunk_size = len(chunks[i])
             # Helping OpenAI clean up their mess.
-            if len(chunk_json_content['list']) < len(chunk):
+            if len(chunk_json_content['list']) < chunk_size:
                 logger.warning('The number of translated sentences is less than that of the original list. '
                                'Add <MANUALLY-ADDED> label')
-                chunk_json_content['list'] += ['<MANUALLY-ADDED>'] * (len(chunk) - len(chunk_json_content['list']))
-            elif len(chunk_json_content['list']) > len(chunk):
+                chunk_json_content['list'] += ['<MANUALLY-ADDED>'] * (chunk_size - len(chunk_json_content['list']))
+            elif len(chunk_json_content['list']) > chunk_size:
                 logger.warning('The number of translated sentences is more than that of the original list. Truncated')
-                chunk_json_content['list'] = chunk_json_content['list'][:len(chunk)]
+                chunk_json_content['list'] = chunk_json_content['list'][:chunk_size]
 
             json_content['total_number'] += chunk_json_content['total_number']
             json_content['list'] += chunk_json_content['list']
 
         # Remove the order number at the front of each sentence
         for i, text in enumerate(json_content['list']):
             json_content['list'][i] = text[text.find('-') + 1:]
@@ -228,15 +204,15 @@
 
         for i, element in enumerate(self.lrc.elements):
             if i == 0 or element.text != new_elements[-1].text:
                 new_elements.append(element)
             else:
                 new_elements[-1].end = element.end
 
-        logger.info(f'Merge same text: {len(self.lrc.elements)} -> {len(new_elements)}')
+        logger.debug(f'Merge same text: {len(self.lrc.elements)} -> {len(new_elements)}')
 
         self.lrc.elements = new_elements
 
     def merge_short_lyrics(self, threshold=2):
         """
         Merge the short text.
         """
@@ -245,15 +221,15 @@
         for i, element, in enumerate(self.lrc.elements):
             if i == 0 or element.duration >= threshold:
                 new_elements.append(element)
             else:
                 new_elements[-1].text += ' ' + element.text
                 new_elements[-1].end = element.end
 
-        logger.info(f'Merge short text: {len(self.lrc.elements)} -> {len(new_elements)}')
+        logger.debug(f'Merge short text: {len(self.lrc.elements)} -> {len(new_elements)}')
 
         self.lrc.elements = new_elements
 
     def merge_same_words(self):
         """
         Merge the same pattern in one lyric.
         :return:
@@ -270,36 +246,37 @@
                     return text[:i]
             return None
 
         for i in range(len(elements)):
             repeat_text = get_repeat(elements[i].text)
             if repeat_text:
                 elements[i].text = repeat_text + '...(Repeat)'
-                logger.info(f'Merge same words: {repeat_text}')
+                logger.debug(f'Merge same words: {repeat_text}')
 
-        logger.info('Merge same words done.')
+        logger.debug('Merge same words done.')
 
         self.lrc.elements = elements
 
     def cut_long_lyrics(self, threshold=125, keep=20):
         elements = self.lrc.elements
 
         for i, element in enumerate(elements):
             if len(element.text) > threshold:
                 logger.warning(f'Cut long text: {element.text}\n Into: {element.text[:keep]}...')
                 elements[i].text = element.text[:keep] + f'(Cut to {keep})'
 
-        logger.info('Cut long text done.')
+        logger.debug('Cut long text done.')
 
         self.lrc.elements = elements
 
     def perform_all(self):
-        self.merge_same_lyrics()
-        self.merge_short_lyrics()
-        self.merge_same_words()
-        self.cut_long_lyrics()
+        for _ in range(2):
+            self.merge_same_lyrics()
+            self.merge_short_lyrics()
+            self.merge_same_words()
+            self.cut_long_lyrics()
 
     def save(self, output_lrc_name=None):
         optimized_name = extend_filename(self.lrc_name, '_optimized') if not output_lrc_name else output_lrc_name
         self.lrc.save_lrc(optimized_name)
         logger.info(f'Optimized LRC file saved to {optimized_name}')
         return optimized_name
```

### Comparing `openlrc-0.0.3/openlrc/prompter.py` & `openlrc-0.0.4/openlrc/prompter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 class BaseTranslatePrompter:
     def __str__(self):
-        return '''You are an advanced {source_lang} to {target_lang} translator.
+        return '''You are an advanced {src_lang} to {target_lang} translator.
 'The input format: {{"total_number": <total-number>, "list": ["1-<sentence-1>", "2-<sentence-2>", "3-<sentence-3>", ...]}}.
 'The output format: {{"total_number": <total-translated-number>, "list": ["1-<translated-sentence-1>", "2-<translated-sentence-2>", "3-<translated-sentence-3>", ..., "<total-translated-number>-<last-translated-sentence>"]}}.
 'Please remember to add an order number before each translated sentence, as the output format.
 'Return only the content inside the two curly brackets and nothing else.
 'Do not merge or eliminate any sentence.
 'Keep the number of the translated sentence in the returned list identical to that of the original list.
 'Ensure that the correspondence between the original and translated list is maintained.
+'DO NOT break the output format.
 'Utilize context to rectify any inappropriate words.
 'If a sentence is not suitable for translation, please do not translate it, but you need to complete the translation of other suitable sentences.
 'If you are not sure whether a sentence is suitable for translation, please translate it.
 'Even if encountering sentences that are not suitable for translation, please maintain the output format.'
 'Even if only one sentence is translated, please maintain the output format. Dont add any other words.
 'Use '<' and '>' to replace the double quote in the translated sentences.'''
 
 
 class LovelyPrompter(BaseTranslatePrompter):
     def __str__(self):
-        return str(super()) + 'Use lovely colloquial expressions to translate each sentence.'
+        return super().__str__() + 'Use lovely colloquial expressions to translate each sentence.'
+
+
+prompter_map = {
+    'base_trans': BaseTranslatePrompter,
+    'lovely_trans': LovelyPrompter
+}
 
 
 def format_texts(texts):
     return f'{{"total_number": {len(texts)}, "list": {list2str(texts)}}}'
 
 
 def list2str(texts):
```

### Comparing `openlrc-0.0.3/openlrc/utils.py` & `openlrc-0.0.4/openlrc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import time
 import json
-
+import time
 from os.path import splitext
-from openlrc.logger import logger
 
 import tiktoken
 
+from openlrc.logger import logger
+
 
 def json2dict(json_str):
     """ Convert json string to python dict. """
 
     try:
         result = json.loads(json_str)
         return result
@@ -39,25 +39,27 @@
 
     # The content after last found " should be "}]"
     fixed_json_str3 = fixed_json_str2[:fixed_json_str2.rfind('"') + 1] + ']}'
     try:
         result = json.loads(fixed_json_str3)
         return result
     except json.decoder.JSONDecodeError as e:
-        logger.error(f'Failed to convert into json: \n {fixed_json_str3}\n')
+        logger.error(f'Failed to convert returned content into json: \n {fixed_json_str3}\n\n')
 
         # Save the json string to file
-        with open('error.json', 'w', encoding='utf-8') as f:
+        with open('test_return.json', 'w', encoding='utf-8') as f:
             f.write(fixed_json_str3)
 
+        logger.info(f'The json file is saved to test_return.json')
+
         raise e
 
 
-def get_token_number(text):
-    encoder = tiktoken.encoding_for_model("gpt-3.5-turbo")
+def get_token_number(text, model="gpt-3.5-turbo"):
+    encoder = tiktoken.encoding_for_model(model)
 
     return len(encoder.encode(text))
 
 
 def change_ext(filename, ext):
     return f'{splitext(filename)[0]}.{ext}'
```

### Comparing `openlrc-0.0.3/LICENSE` & `openlrc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openlrc-0.0.3/README.md` & `openlrc-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,19 @@
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
     ```
+   or install directly from GitHub:
+
+    ```shell
+    pip install git+https://github.com/zh-plus/Open-Lyrics
+    ```
 
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
@@ -32,15 +37,17 @@
 
 - [ ] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 - [ ] Make translate prompt more robust.
 - [ ] Add local LLM support.
-- [ ] Multi-thead support for both whisper model and GPT request.
+- [ ] Concurrent support for both whisper model and GPT request.
+    - [ ] Whisper
+    - [x] GPT
 - [ ] Automatically fix json encoder error using GPT.
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
 - https://github.com/openai/openai-python
 - https://github.com/openai/whisper
```

### Comparing `openlrc-0.0.3/pyproject.toml` & `openlrc-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openlrc"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Hao Zheng", email = "zhenghaosustc@gmail.com" },
 ]
 description = "Transcribe and translate voice into LRC file."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     'openai',
     'faster-whisper',
     'tiktoken',
     'langcodes',
     'language-data',
-    'rich'
+    'rich',
+    'tqdm'
 ]
 keywords = [
     'openai-gpt3',
     'whisper',
     'voice transcribe',
     'lrc'
 ]
 classifiers = [
     'Programming Language :: Python :: 3',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.11',
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build]
 exclude = [
     "test*",
     "/promotion",
```

### Comparing `openlrc-0.0.3/PKG-INFO` & `openlrc-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: openlrc
-Version: 0.0.3
+Version: 0.0.4
 Summary: Transcribe and translate voice into LRC file.
 Project-URL: Homepage, https://github.com/zh-plus/Open-Lyrics
 Project-URL: Bug Tracker, https://github.com/zh-plus/Open-Lyrics/issues
 Author-email: Hao Zheng <zhenghaosustc@gmail.com>
 License-File: LICENSE
 Keywords: lrc,openai-gpt3,voice transcribe,whisper
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: faster-whisper
 Requires-Dist: langcodes
 Requires-Dist: language-data
 Requires-Dist: openai
 Requires-Dist: rich
 Requires-Dist: tiktoken
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Open-Lyrics
 
 Open-Lyrics is a open-source project to transcribe (
 using [faster-whisper](https://github.com/guillaumekln/faster-whisper)) voice file and
 translate/polish ([OpenAI-GPT](https://github.com/openai/openai-python)) the text.
@@ -38,14 +38,19 @@
 2. Add your [OpenAI API key](https://platform.openai.com/account/api-keys) to environment variable `OPENAI_API_KEY`.
 
 3. This project can be installed from PyPI:
 
     ```shell
     pip install openlrc
     ```
+   or install directly from GitHub:
+
+    ```shell
+    pip install git+https://github.com/zh-plus/Open-Lyrics
+    ```
 
 ## Usage
 
 ```python
 from openlrc import LRCer
 
 lrcer = LRCer()
@@ -56,15 +61,17 @@
 
 - [ ] Add transcribed examples.
     - [ ] Song
     - [ ] Podcast
     - [ ] Audiobook
 - [ ] Make translate prompt more robust.
 - [ ] Add local LLM support.
-- [ ] Multi-thead support for both whisper model and GPT request.
+- [ ] Concurrent support for both whisper model and GPT request.
+    - [ ] Whisper
+    - [x] GPT
 - [ ] Automatically fix json encoder error using GPT.
 
 ## Credits
 
 - https://github.com/guillaumekln/faster-whisper
 - https://github.com/openai/openai-python
 - https://github.com/openai/whisper
```

