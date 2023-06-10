# Comparing `tmp/span_marker-1.0.1.tar.gz` & `tmp/span_marker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.0.1.tar", last modified: Mon May  1 15:03:11 2023, max compression
+gzip compressed data, was "span_marker-1.1.0.tar", last modified: Sat Jun 10 13:24:05 2023, max compression
```

## Comparing `span_marker-1.0.1.tar` & `span_marker-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:11.597072 span_marker-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-01 14:49:51.000000 span_marker-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7461 2023-05-01 15:03:11.597072 span_marker-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6884 2023-05-01 14:49:51.000000 span_marker-1.0.1/README.md
--rw-rw-rw-   0        0        0     2436 2023-05-01 14:49:51.000000 span_marker-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-01 15:03:11.597072 span_marker-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:11.590072 span_marker-1.0.1/span_marker/
--rw-rw-rw-   0        0        0      446 2023-05-01 15:01:57.000000 span_marker-1.0.1/span_marker/__init__.py
--rw-rw-rw-   0        0        0     6368 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6154 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     4684 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2488 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/model_card.py
--rw-rw-rw-   0        0        0    26535 2023-05-01 15:01:42.000000 span_marker-1.0.1/span_marker/modeling.py
--rw-rw-rw-   0        0        0     1798 2023-05-01 14:56:04.000000 span_marker-1.0.1/span_marker/output.py
--rw-rw-rw-   0        0        0    12478 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    11257 2023-05-01 14:49:51.000000 span_marker-1.0.1/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:11.594072 span_marker-1.0.1/span_marker.egg-info/
--rw-rw-rw-   0        0        0     7461 2023-05-01 15:03:11.000000 span_marker-1.0.1/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-05-01 15:03:11.000000 span_marker-1.0.1/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:03:11.000000 span_marker-1.0.1/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      244 2023-05-01 15:03:11.000000 span_marker-1.0.1/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-01 15:03:11.000000 span_marker-1.0.1/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 15:03:11.596071 span_marker-1.0.1/tests/
--rw-rw-rw-   0        0        0      961 2023-05-01 14:49:51.000000 span_marker-1.0.1/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-05-01 14:49:51.000000 span_marker-1.0.1/tests/test_model_card.py
--rw-rw-rw-   0        0        0     4708 2023-05-01 14:49:51.000000 span_marker-1.0.1/tests/test_modeling.py
--rw-rw-rw-   0        0        0     8518 2023-05-01 14:49:51.000000 span_marker-1.0.1/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.389672 span_marker-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7875 2023-06-10 13:24:05.389672 span_marker-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7298 2023-06-01 10:38:31.000000 span_marker-1.1.0/README.md
+-rw-rw-rw-   0        0        0     2455 2023-06-10 13:15:43.000000 span_marker-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 13:24:05.389672 span_marker-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.377657 span_marker-1.1.0/span_marker/
+-rw-rw-rw-   0        0        0      446 2023-06-10 13:15:59.000000 span_marker-1.1.0/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7018 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5066 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.1.0/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2471 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    30144 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/output.py
+-rw-rw-rw-   0        0        0    11885 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    19774 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.382163 span_marker-1.1.0/span_marker.egg-info/
+-rw-rw-rw-   0        0        0     7875 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.388668 span_marker-1.1.0/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.1.0/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     7875 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     8733 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_trainer.py
```

### Comparing `span_marker-1.0.1/LICENSE` & `span_marker-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.0.1/PKG-INFO` & `span_marker-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span_marker
-Version: 1.0.1
+Version: 1.1.0
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -95,12 +95,22 @@
 ## Pretrained Models
 
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, very competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 
+## Context
+<h1 align="center">
+    <a href="https://github.com/argilla-io/argilla">
+    <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
+    </a>
+</h1>
+
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
+Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

### Comparing `span_marker-1.0.1/README.md` & `span_marker-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -79,12 +79,22 @@
 ## Pretrained Models
 
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, very competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 
+## Context
+<h1 align="center">
+    <a href="https://github.com/argilla-io/argilla">
+    <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
+    </a>
+</h1>
+
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
+Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

### Comparing `span_marker-1.0.1/pyproject.toml` & `span_marker-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     {name = "Tom Aarsen"}
 ]
 maintainers = [
     {name = "Tom Aarsen"}
 ]
 dependencies = [
     "torch",
+    "accelerate",
     "transformers>=4.19.0", # required for EvalPrediction.inputs
     "datasets>=2.0.0",
     "packaging>=20.0",
     "evaluate",
     "seqeval",
     "jinja2",
     "huggingface_hub"
```

### Comparing `span_marker-1.0.1/span_marker/configuration.py` & `span_marker-1.1.0/span_marker/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,20 @@
             truncation. If None, the tokenizer its `model_max_length` is used, and if that value is
             not defined, it becomes 512 instead. Defaults to None.
         marker_max_length (`int`): The maximum length for each of the span markers. A value of 128
             means that each training and inferencing sample contains a maximum of 128 start markers
             and 128 end markers, for a total of 256 markers per sample. Defaults to 128.
         entity_max_length (`int`): The maximum length of an entity span in terms of words.
             Defaults to 8.
+        max_prev_context (`Optional[int]`): The maximum number of previous sentences to include as
+            context. If `None`, the maximum amount that fits in `model_max_length` is chosen.
+            Defaults to `None`.
+        max_next_context (`Optional[int]`): The maximum number of next sentences to include as
+            context. If `None`, the maximum amount that fits in `model_max_length` is chosen.
+            Defaults to `None`.
 
     Example::
 
         # These configuration settings are provided via kwargs to `SpanMarkerModel.from_pretrained`:
         model = SpanMarkerModel.from_pretrained(
             "bert-base-cased",
             labels=labels,
@@ -40,21 +46,25 @@
 
     def __init__(
         self,
         encoder_config: Optional[Dict[str, Any]] = None,
         model_max_length: Optional[int] = None,
         marker_max_length: int = 128,
         entity_max_length: int = 8,
+        max_prev_context: Optional[int] = None,
+        max_next_context: Optional[int] = None,
         **kwargs,
     ) -> None:
         self.encoder = encoder_config
         self.model_max_length = model_max_length
         self.model_max_length_default = 512
         self.marker_max_length = marker_max_length
         self.entity_max_length = entity_max_length
+        self.max_prev_context = max_prev_context
+        self.max_next_context = max_next_context
         self.span_marker_version = kwargs.pop("span_marker_version", None)
         super().__init__(**kwargs)
 
         # label2id and id2label are automatically set by super().__init__, but we want to rely on
         # the encoder configs instead if we can, so we delete them under two conditions
         # 1. if they're the default ({0: "LABEL_0", 1: "LABEL_1"})
         # 2. if they're identical to the encoder label2id
```

### Comparing `span_marker-1.0.1/span_marker/data_collator.py` & `span_marker-1.1.0/span_marker/data_collator.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 
         Returns:
             Dict[str, torch.Tensor]: Batch dictionary ready to be fed into :meth:`~span_marker.modeling.SpanMarkerModel.forward`.
         """
         total_size = self.tokenizer.model_max_length + 2 * self.marker_max_length
         batch = defaultdict(list)
         num_words = []
+        document_ids = []
+        sentence_ids = []
         start_marker_indices = []
         num_marker_pairs = []
         for sample in features:
             input_ids = sample["input_ids"]
             num_spans = sample["num_spans"]
             num_tokens = len(input_ids)
 
@@ -70,21 +72,23 @@
                 input_ids.to(torch.int)
             input_ids = F.pad(input_ids, (0, total_size - len(input_ids)), value=self.tokenizer.pad_token_id)
             input_ids[start_marker_idx : start_marker_idx + num_spans] = self.tokenizer.start_marker_id
             input_ids[end_marker_idx : end_marker_idx + num_spans] = self.tokenizer.end_marker_id
             batch["input_ids"].append(input_ids)
 
             # Prepare position IDs
-            position_ids = torch.arange(num_tokens, dtype=torch.int)
-            position_ids = F.pad(position_ids, (0, total_size - len(position_ids)), value=0)
-            position_ids[start_marker_idx : start_marker_idx + num_spans] = torch.tensor(sample["start_position_ids"])
-            position_ids[end_marker_idx : end_marker_idx + num_spans] = torch.tensor(sample["end_position_ids"])
+            position_ids = torch.arange(num_tokens, dtype=torch.int) + 2
+            position_ids = F.pad(position_ids, (0, total_size - len(position_ids)), value=1)
+            position_ids[start_marker_idx : start_marker_idx + num_spans] = (
+                torch.tensor(sample["start_position_ids"]) + 2
+            )
+            position_ids[end_marker_idx : end_marker_idx + num_spans] = torch.tensor(sample["end_position_ids"]) + 2
             # Increase the position_ids by 2, inspired by PL-Marker. The intuition is that these position IDs
             # better match the circumstances under which the underlying encoders are trained.
-            batch["position_ids"].append(position_ids + 2)
+            batch["position_ids"].append(position_ids)
 
             # Prepare attention mask matrix
             attention_mask = torch.zeros((total_size, total_size), dtype=torch.bool)
             # text tokens self-attention
             attention_mask[:num_tokens, :num_tokens] = 1
             # let markers attend text tokens
             attention_mask[start_marker_idx : start_marker_idx + num_spans, :num_tokens] = 1
@@ -98,22 +102,29 @@
             attention_mask[end_index_list, end_index_list] = 1
             batch["attention_mask"].append(attention_mask)
 
             # Add start of the markers, so the model knows where the input IDs end and where the markers start
             start_marker_indices.append(start_marker_idx)
             num_marker_pairs.append(end_marker_idx - start_marker_idx)
 
+            if "num_words" in sample:
+                num_words.append(sample["num_words"])
+            if "document_id" in sample:
+                document_ids.append(sample["document_id"])
+            if "sentence_id" in sample:
+                sentence_ids.append(sample["sentence_id"])
             if "labels" in sample:
                 labels = torch.tensor(sample["labels"])
                 labels = F.pad(labels, (0, (total_size // 2) - len(labels)), value=-100)
                 batch["labels"].append(labels)
 
-            if "num_words" in sample:
-                num_words.append(sample["num_words"])
-
         batch = {key: torch.stack(value) for key, value in batch.items()}
         # Used for evaluation, does not need to be padded/stacked
         if num_words:
             batch["num_words"] = torch.tensor(num_words)
+        if document_ids:
+            batch["document_ids"] = torch.tensor(document_ids)
+        if sentence_ids:
+            batch["sentence_ids"] = torch.tensor(sentence_ids)
         batch["start_marker_indices"] = torch.tensor(start_marker_indices)
         batch["num_marker_pairs"] = torch.tensor(num_marker_pairs)
         return batch
```

### Comparing `span_marker-1.0.1/span_marker/evaluation.py` & `span_marker-1.1.0/span_marker/evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,53 +23,59 @@
     Returns:
         Dict[str, float]: Dictionary with ``"overall_precision"``, ``"overall_recall"``, ``"overall_f1"``
             and ``"overall_accuracy"`` keys.
     """
     inputs = eval_prediction.inputs
     gold_labels = eval_prediction.label_ids
     logits = eval_prediction.predictions[0]
-    num_words = eval_prediction.predictions[-1]
+    num_words = eval_prediction.predictions[2]
+    has_document_context = len(eval_prediction.predictions) == 5
+    if has_document_context:
+        document_ids = eval_prediction.predictions[3]
+        sentence_ids = eval_prediction.predictions[4]
 
     # Compute probabilities via softmax and extract 'winning' scores/labels
     probs = torch.tensor(logits, dtype=torch.float32).softmax(dim=-1)
     scores, pred_labels = probs.max(-1)
 
     # Collect all samples in one dict. We do this because some samples are spread between multiple inputs
-    sample_dict = {}
+    sample_list = []
     for sample_idx in range(inputs.shape[0]):
         tokens = inputs[sample_idx]
         text = tokenizer.decode(tokens, skip_special_tokens=True)
-        token_hash = hash(text)
-        if token_hash not in sample_dict:
-            spans = list(tokenizer.get_all_valid_spans(num_words[sample_idx], tokenizer.config.entity_max_length))
+        token_hash = hash(text) if not has_document_context else (document_ids[sample_idx], sentence_ids[sample_idx])
+        if not sample_list or sample_list[-1]["hash"] != token_hash:
             mask = gold_labels[sample_idx] != -100
-            sample_dict[token_hash] = {
-                "text": text,
-                "spans": spans,
-                "gold_labels": gold_labels[sample_idx][mask].tolist(),
-                "pred_labels": pred_labels[sample_idx][mask].tolist(),
-                "scores": scores[sample_idx].tolist(),
-                "num_words": num_words[sample_idx],
-            }
+            sample_list.append(
+                {
+                    "text": text,
+                    "gold_labels": gold_labels[sample_idx][mask].tolist(),
+                    "pred_labels": pred_labels[sample_idx][mask].tolist(),
+                    "scores": scores[sample_idx].tolist(),
+                    "num_words": num_words[sample_idx],
+                    "hash": token_hash,
+                }
+            )
         else:
             mask = gold_labels[sample_idx] != -100
-            sample_dict[token_hash]["gold_labels"] += gold_labels[sample_idx][mask].tolist()
-            sample_dict[token_hash]["pred_labels"] += pred_labels[sample_idx][mask].tolist()
-            sample_dict[token_hash]["scores"] += scores[sample_idx].tolist()
+            sample_list[-1]["gold_labels"] += gold_labels[sample_idx][mask].tolist()
+            sample_list[-1]["pred_labels"] += pred_labels[sample_idx][mask].tolist()
+            sample_list[-1]["scores"] += scores[sample_idx].tolist()
 
     outside_id = tokenizer.config.outside_id
     id2label = tokenizer.config.id2label
     # seqeval works wonders for NER evaluation
     seqeval = evaluate.load("seqeval")
-    for sample in sample_dict.values():
-        spans = sample["spans"]
+    for sample in sample_list:
         scores = sample["scores"]
         num_words = sample["num_words"]
+        spans = list(tokenizer.get_all_valid_spans(num_words, tokenizer.config.entity_max_length))
         gold_labels = sample["gold_labels"]
         pred_labels = sample["pred_labels"]
+        assert len(gold_labels) == len(pred_labels) and len(spans) == len(pred_labels)
 
         # Construct IOB2 format for gold labels, useful for seqeval
         gold_labels_per_tokens = ["O"] * num_words
         for span, gold_label in zip(spans, gold_labels):
             if gold_label != outside_id:
                 gold_labels_per_tokens[span[0]] = "B-" + id2label[gold_label]
                 gold_labels_per_tokens[span[0] + 1 : span[1]] = ["I-" + id2label[gold_label]] * (span[1] - span[0] - 1)
```

### Comparing `span_marker-1.0.1/span_marker/label_normalizer.py` & `span_marker-1.1.0/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.0.1/span_marker/model_card.py` & `span_marker-1.1.0/span_marker/model_card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import tempfile
 from pathlib import Path
 from typing import Union
 
 import jinja2
 from huggingface_hub import model_info
 from huggingface_hub.utils import RepositoryNotFoundError
```

### Comparing `span_marker-1.0.1/span_marker/modeling.py` & `span_marker-1.1.0/span_marker/modeling.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import os
 import re
 import warnings
 from typing import Callable, Dict, List, Optional, Type, TypeVar, Union
 
 import torch
 import torch.nn.functional as F
+from datasets import Dataset
 from packaging.version import Version, parse
 from torch import device, nn
+from tqdm.autonotebook import trange
 from transformers import AutoConfig, AutoModel, PretrainedConfig, PreTrainedModel
 from typing_extensions import Self
 
 from span_marker import __version__ as span_marker_version
 from span_marker.configuration import SpanMarkerConfig
 from span_marker.data_collator import SpanMarkerDataCollator
-from span_marker.model_card import MODEL_CARD_TEMPLATE, generate_model_card
+from span_marker.model_card import generate_model_card
 from span_marker.output import SpanMarkerOutput
 from span_marker.tokenizer import SpanMarkerTokenizer
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound="SpanMarkerModel")
 
@@ -114,14 +116,16 @@
         input_ids: torch.Tensor,
         attention_mask: torch.Tensor,
         position_ids: torch.Tensor,
         start_marker_indices: torch.Tensor,
         num_marker_pairs: torch.Tensor,
         labels: Optional[torch.Tensor] = None,
         num_words: Optional[torch.Tensor] = None,
+        document_ids: Optional[torch.Tensor] = None,
+        sentence_ids: Optional[torch.Tensor] = None,
     ) -> SpanMarkerOutput:
         """Forward call of the SpanMarkerModel.
 
         Args:
             input_ids (~torch.Tensor): Input IDs including start/end markers.
             attention_mask (~torch.Tensor): Attention mask matrix including one-directional attention for markers.
             position_ids (~torch.Tensor): Position IDs including start/end markers.
@@ -149,24 +153,25 @@
         # Get the indices where the end markers start
         end_marker_indices = start_marker_indices + num_marker_pairs
 
         # The start marker embeddings concatenated with the end marker embeddings.
         # This is kind of breaking the cardinal rule of GPU-based ML, as this is processing
         # the batch iteratively per sample, but every sample produces a different shape matrix
         # and this is the most convenient way to recombine them into a matrix.
-        embeddings = [
-            torch.cat(
-                (
-                    last_hidden_state[i, start_marker_indices[i] : end_marker_indices[i]],
-                    last_hidden_state[i, end_marker_indices[i] : end_marker_indices[i] + num_marker_pairs[i]],
-                ),
-                dim=-1,
+        embeddings = []
+        for i in range(batch_size):
+            embeddings.append(
+                torch.cat(
+                    (
+                        last_hidden_state[i, start_marker_indices[i] : end_marker_indices[i]],
+                        last_hidden_state[i, end_marker_indices[i] : end_marker_indices[i] + num_marker_pairs[i]],
+                    ),
+                    dim=-1,
+                )
             )
-            for i in range(batch_size)
-        ]
         padded_embeddings = [
             F.pad(embedding, (0, 0, 0, sequence_length // 2 - len(embedding))) for embedding in embeddings
         ]
         feature_vector = torch.stack(padded_embeddings)
 
         # NOTE: This was wrong in the older tests
         feature_vector = self.dropout(feature_vector)
@@ -177,14 +182,16 @@
 
         return SpanMarkerOutput(
             loss=loss if labels is not None else None,
             logits=logits,
             *outputs[2:],
             num_marker_pairs=num_marker_pairs,
             num_words=num_words,
+            document_ids=document_ids,
+            sentence_ids=sentence_ids,
         )
 
     @classmethod
     def from_pretrained(
         cls: Type[T],
         pretrained_model_name_or_path: Union[str, os.PathLike],
         *model_args,
@@ -229,15 +236,16 @@
                 for inference via :meth:`SpanMarkerModel.predict`.
         """
         # If loading a SpanMarkerConfig, then we don't want to override id2label and label2id
         # Create an encoder or SpanMarker config
         config: PretrainedConfig = AutoConfig.from_pretrained(pretrained_model_name_or_path, *model_args, **kwargs)
 
         # if 'pretrained_model_name_or_path' refers to a SpanMarkerModel instance, initialize it directly
-        if isinstance(config, cls.config_class):
+        loading_span_marker = isinstance(config, cls.config_class)
+        if loading_span_marker:
             model_span_marker_version = config.get("span_marker_version") or "0.1.0"
             if parse(model_span_marker_version) < Version("1.0.0.dev"):
                 logger.warning(
                     f"Loading a model trained using SpanMarker v{model_span_marker_version},"
                     f" while SpanMarker v{span_marker_version} is installed. Due to large changes"
                     " introduced in v1.0.0, this is not recommended. Either retrain your model for"
                     f" v{span_marker_version}, or install `span_marker < 1.0.0`."
@@ -274,15 +282,14 @@
         # Pass the tokenizer directly to the model for convenience, this way the user doesn't have to
         # make it themselves.
         tokenizer = SpanMarkerTokenizer.from_pretrained(
             config.encoder.get("_name_or_path", pretrained_model_name_or_path), config=config, **kwargs
         )
         model.set_tokenizer(tokenizer)
         model.resize_token_embeddings(len(tokenizer))
-
         return model
 
     @classmethod
     def _load_encoder_with_kwargs(
         cls, pretrained_model_name_or_path: str, config: PretrainedConfig, *model_args, **kwargs
     ) -> PreTrainedModel:
         """Load an underlying encoder using keyword arguments, even if those kwargs are not (all) supported.
@@ -311,15 +318,15 @@
                     return SpanMarkerModel._load_encoder_with_kwargs(
                         pretrained_model_name_or_path, config, *model_args, **kwargs
                     )
             # Otherwise, just raise the exception
             raise exc
 
     def predict(
-        self, inputs: Union[str, List[str], List[List[str]]], allow_overlapping: bool = False
+        self, inputs: Union[str, List[str], List[List[str]], Dataset], batch_size: int = 4
     ) -> Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
         """Predict named entities from input texts.
 
         Example::
 
             >>> model = SpanMarkerModel.from_pretrained(...)
             >>> model.predict("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
@@ -330,23 +337,23 @@
             >>> model.predict(['Caesar', 'led', 'the', 'Roman', 'armies', 'in', 'the', 'Gallic', 'Wars', 'before', 'defeating', 'his', 'political', 'rival', 'Pompey', 'in', 'a', 'civil', 'war'])
             [{'span': ['Caesar'], 'label': 'person-politician', 'score': 0.683479905128479, 'word_start_index': 0, 'word_end_index': 1},
              {'span': ['Roman'], 'label': 'location-GPE', 'score': 0.7114525437355042, 'word_start_index': 3, 'word_end_index': 4},
              {'span': ['Gallic', 'Wars'], 'label': 'event-attack/battle/war/militaryconflict', 'score': 0.9015670418739319, 'word_start_index': 7, 'word_end_index': 9},
              {'span': ['Pompey'], 'label': 'person-politician', 'score': 0.9601260423660278, 'word_start_index': 14, 'word_end_index': 15}]
 
         Args:
-            inputs (Union[str, List[str], List[List[str]]]): Input sentences from which to extract entities.
+            inputs (Union[str, List[str], List[List[str]], Dataset]): Input sentences from which to extract entities.
                 Valid datastructures are:
 
                 * str: a string sentence.
                 * List[str]: a pre-tokenized string sentence, i.e. a list of words.
                 * List[str]: a list of multiple string sentences.
                 * List[List[str]]: a list of multiple pre-tokenized string sentences, i.e. a list with lists of words.
-            allow_overlapping (bool, optional): Whether to allow entity spans to overlap. The model does not
-                have good support for this, so False is recommended. Defaults to False.
+                * Dataset: A 🤗 :class:`~datasets.Dataset` with a ``tokens`` column and optionally ``document_id`` and ``sentence_id`` columns.
+                    If the optional columns are provided, they will be used to provide document-level context.
 
         Returns:
             Union[List[Dict[str, Union[str, int, float]]], List[List[Dict[str, Union[str, int, float]]]]]:
                 If the input is a single sentence, then we output a list of dictionaries. Each dictionary
                 represents one predicted entity, and contains the following keys:
 
                 * ``label``: The predicted entity label.
@@ -355,104 +362,169 @@
                 * ``word_start_index`` & ``word_end_index``: The word indices for the start/end of the entity,
                   if the input is pre-tokenized.
                 * ``char_start_index`` & ``char_end_index``: The character indices for the start/end of the entity,
                   if the input is a string.
 
                 If the input is multiple sentences, then we return a list containing multiple of the aforementioned lists.
         """
+        from span_marker.trainer import Trainer
+
         if torch.cuda.is_available() and self.device == torch.device("cpu"):
             warnings.warn(
                 "SpanMarker model predictions are being computed on the CPU while CUDA is available."
                 " Moving the model to CUDA using `model.cuda()` before performing predictions is heavily"
                 " recommended to significantly boost prediction speeds.",
                 UserWarning,
                 stacklevel=2,
             )
 
+        # Disable dropout, etc.
+        self.eval()
+
         if not inputs:
             return []
 
         # Check if inputs is a string, i.e. a string sentence, or
         # if it is a list of strings without spaces, i.e. if it's 1 tokenized sentence
         if isinstance(inputs, str) or (
             isinstance(inputs, list) and all(isinstance(element, str) and " " not in element for element in inputs)
         ):
-            return self._predict_one(inputs, allow_overlapping=allow_overlapping)
+            # return self._predict_one(inputs, allow_overlapping=allow_overlapping)
+            dataset = Dataset.from_dict({"tokens": [inputs]})
 
         # Otherwise, we likely have a list of strings, i.e. a list of string sentences,
         # or a list of lists of strings, i.e. a list of tokenized sentences
         # if isinstance(inputs, list) and all(isinstance(element, str) and " " not in element for element in inputs):
-        return [self._predict_one(sentence) for sentence in inputs]
+        # return [self._predict_one(sentence) for sentence in inputs]
+        elif isinstance(inputs, list):
+            dataset = Dataset.from_dict({"tokens": inputs})
 
-    def _predict_one(
-        self, sentence: Union[str, List[str]], allow_overlapping: bool = False
-    ) -> List[Dict[str, Union[str, int, float]]]:
-        # Tokenization, i.e. computing spans, adding span markers to position_ids
-        tokenized = self.tokenizer(sentence, return_num_words=True, return_batch_encoding=True)
-        num_words = tokenized.pop("num_words")[0]
-        batch_encoding = tokenized.pop("batch_encoding")
-        # Converting into a common batch format like the data collator wants
-        tokenized = [
-            {key: value[idx] for key, value in tokenized.items()} for idx in range(len(tokenized["input_ids"]))
+        elif isinstance(inputs, Dataset):
+            dataset = inputs
+
+        else:
+            raise ValueError(
+                "`SpanMarkerModel.predict` could not recognize your input. It accepts the following:\n"
+                "* str: a string sentence.\n"
+                "* List[str]: a pre-tokenized string sentence, i.e. a list of words.\n"
+                "* List[str]: a list of multiple string sentences.\n"
+                "* List[List[str]]: a list of multiple pre-tokenized string sentences, i.e. a list with lists of words.\n"
+                "* Dataset: A 🤗 Dataset with `tokens` column and optionally `document_id` and `sentence_id` columns.\n"
+                "    If the optional columns are provided, they will be used to provide document-level context."
+            )
+
+        dataset = dataset.remove_columns(set(dataset.column_names) - {"tokens", "document_id", "sentence_id"})
+        num_inputs = len(dataset)
+        dataset: Dataset = dataset.add_column("id", range(num_inputs))
+        results = [
+            {
+                "tokens": tokens,
+                "scores": [],
+                "labels": [],
+                "num_words": None,
+            }
+            for tokens in dataset["tokens"]
         ]
-        # Expanding the small tokenized output into full-scale input_ids, position_ids and attention_mask matrices.
-        collated = self.data_collator(tokenized)
-        # Moving the inputs to the right device
-        inputs = {key: value.to(self.device) for key, value in collated.items()}
-
-        output = self(**inputs)
-        # use `num_marker_pairs` to remove all padding
-        logits = torch.cat(
-            [logits[:num_marker_pairs] for logits, num_marker_pairs in zip(output.logits, output.num_marker_pairs)]
+
+        # Tokenize & add start/end markers
+        tokenizer_dict = self.tokenizer(
+            {"tokens": dataset["tokens"]}, return_num_words=True, return_batch_encoding=True
         )
-        # Computing probabilities based on the logits
-        probs = logits.softmax(-1)
-        # Get the labels and the correponding probability scores
-        scores, labels = probs.max(-1)
-        scores = scores.tolist()
-        labels = labels.tolist()
-        # Get all of the valid spans to match with the score and labels
-        spans = list(self.tokenizer.get_all_valid_spans(num_words, self.config.entity_max_length))
+        batch_encoding = tokenizer_dict.pop("batch_encoding")
+        for key, value in tokenizer_dict.items():
+            dataset = dataset.add_column(key, value)
+        # Add context if possible
+        if {"document_id", "sentence_id"} <= set(dataset.column_names):
+            # Add column to be able to revert sorting later
+            dataset = dataset.add_column("__sort_id", range(len(dataset)))
+            # Sorting by doc ID and then sentence ID is required for add_context
+            dataset = dataset.sort(column_names=["document_id", "sentence_id"])
+            dataset = Trainer.add_context(
+                dataset,
+                self.tokenizer.model_max_length,
+                max_prev_context=self.config.max_prev_context,
+                max_next_context=self.config.max_next_context,
+            )
+            dataset = dataset.sort(column_names=["__sort_id"])
+            dataset = dataset.remove_columns("__sort_id")
+
+        dataset = dataset.map(
+            lambda sample: Trainer.spread_sample(
+                self.tokenizer.model_max_length, self.config.marker_max_length, sample
+            ),
+            batched=True,
+            batch_size=1,
+            desc="Spreading data between multiple samples",
+        )
+        for batch_start_idx in trange(0, len(dataset), batch_size):
+            batch = dataset.select(range(batch_start_idx, min(len(dataset), batch_start_idx + batch_size)))
+            # Expanding the small tokenized output into full-scale input_ids, position_ids and attention_mask matrices.
+            batch = self.data_collator(batch)
+            # Moving the inputs to the right device
+            batch = {key: value.to(self.device) for key, value in batch.items()}
+            with torch.no_grad():
+                output = self(**batch)
+            # Computing probabilities based on the logits
+            probs = output.logits.softmax(-1)
+            # Get the labels and the correponding probability scores
+            scores, labels = probs.max(-1)
+            # TODO: Iterate over output.num_marker_pairs instead with enumerate
+            for iter_idx in range(output.num_marker_pairs.size(0)):
+                input_id = dataset["id"][batch_start_idx + iter_idx]
+                num_marker_pairs = output.num_marker_pairs[iter_idx]
+                results[input_id]["scores"].extend(scores[iter_idx, :num_marker_pairs].tolist())
+                results[input_id]["labels"].extend(labels[iter_idx, :num_marker_pairs].tolist())
+                results[input_id]["num_words"] = output.num_words[iter_idx]
 
-        output = []
+        all_entities = []
         id2label = self.config.id2label
-        # If we don't allow overlapping, then we keep track of a boolean for each word, indicating if it has been
-        # selected already by a previous, higher score entity span
-        if not allow_overlapping:
+        for sample_idx, sample in enumerate(results):
+            scores = sample["scores"]
+            labels = sample["labels"]
+            num_words = sample["num_words"]
+            sentence = sample["tokens"]
+            # Get all of the valid spans to match with the score and labels
+            spans = list(self.tokenizer.get_all_valid_spans(num_words, self.config.entity_max_length))
+
             word_selected = [False] * num_words
-        for (word_start_index, word_end_index), score, label_id in sorted(
-            zip(spans, scores, labels), key=lambda tup: tup[1], reverse=True
-        ):
-            if label_id != self.config.outside_id and (
-                allow_overlapping or not any(word_selected[word_start_index:word_end_index])
+            sentence_entities = []
+            assert len(spans) == len(scores) and len(spans) == len(labels)
+            for (word_start_index, word_end_index), score, label_id in sorted(
+                zip(spans, scores, labels), key=lambda tup: tup[1], reverse=True
             ):
-                char_start_index = batch_encoding.word_to_chars(0, word_start_index).start
-                char_end_index = batch_encoding.word_to_chars(0, word_end_index - 1).end
-                output.append(
-                    {
+                if label_id != self.config.outside_id and not any(word_selected[word_start_index:word_end_index]):
+                    char_start_index = batch_encoding.word_to_chars(sample_idx, word_start_index).start
+                    char_end_index = batch_encoding.word_to_chars(sample_idx, word_end_index - 1).end
+                    entity = {
                         "span": sentence[char_start_index:char_end_index]
                         if isinstance(sentence, str)
                         else sentence[word_start_index:word_end_index],
                         "label": id2label[label_id],
                         "score": score,
                     }
-                )
-                if isinstance(sentence, str):
-                    output[-1]["char_start_index"] = char_start_index
-                    output[-1]["char_end_index"] = char_end_index
-                else:
-                    output[-1]["word_start_index"] = word_start_index
-                    output[-1]["word_end_index"] = word_end_index
+                    if isinstance(sentence, str):
+                        entity["char_start_index"] = char_start_index
+                        entity["char_end_index"] = char_end_index
+                    else:
+                        entity["word_start_index"] = word_start_index
+                        entity["word_end_index"] = word_end_index
+                    sentence_entities.append(entity)
 
-                if not allow_overlapping:
                     word_selected[word_start_index:word_end_index] = [True] * (word_end_index - word_start_index)
-        return sorted(
-            output,
-            key=lambda entity: entity["char_start_index"] if isinstance(sentence, str) else entity["word_start_index"],
-        )
+            all_entities.append(
+                sorted(
+                    sentence_entities,
+                    key=lambda entity: entity["char_start_index"]
+                    if isinstance(sentence, str)
+                    else entity["word_start_index"],
+                )
+            )
+        if len(all_entities) == 1:
+            return all_entities[0]
+        return all_entities
 
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         is_main_process: bool = True,
         state_dict: Optional[dict] = None,
         save_function: Callable = torch.save,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `span_marker-1.0.1/span_marker/output.py` & `span_marker-1.1.0/span_marker/output.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,11 +26,17 @@
             sequence_length)``. Returned when ``config.output_attentions=True``.
 
             Attentions weights after the attention softmax, used to compute the weighted average in the self-attention
             heads.
         num_words (Optional[~torch.Tensor]):
             A vector with shape ``(batch_size,)`` that tracks how many words were in the input of each sample in the batch.
             Required for evaluation purposes.
+        document_ids (Optional[~torch.Tensor]):
+            A vector with shape ``(batch_size,)`` that tracks the document the input text belongs to.
+        sentence_ids (Optional[~torch.Tensor]):
+            A vector with shape ``(batch_size,)`` that tracks the sentence in the document that the input text belongs to.
     """
 
     num_marker_pairs: Optional[torch.Tensor] = None
     num_words: Optional[torch.Tensor] = None
+    document_ids: Optional[torch.Tensor] = None
+    sentence_ids: Optional[torch.Tensor] = None
```

### Comparing `span_marker-1.0.1/span_marker/tokenizer.py` & `span_marker-1.1.0/span_marker/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import itertools
 import logging
 import os
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
+import numpy as np
 from transformers import AutoTokenizer, PreTrainedTokenizer
 
 from span_marker.configuration import SpanMarkerConfig
 
 logger = logging.getLogger(__name__)
 
 
@@ -171,41 +171,41 @@
     def __getattribute__(self, key: str) -> Any:
         try:
             return super().__getattribute__(key)
         except AttributeError:
             return super().__getattribute__("tokenizer").__getattribute__(key)
 
     def __call__(
-        self, inputs, labels=None, return_num_words: bool = False, return_batch_encoding=False, **kwargs
+        self, batch: Dict[str, List[Any]], return_num_words: bool = False, return_batch_encoding=False, **kwargs
     ) -> Dict[str, List]:
+        tokens = batch["tokens"]
+        labels = batch.get("ner_tags", None)
         # TODO: Increase robustness of this
         is_split_into_words = True
-        if isinstance(inputs, str) or (inputs and " " in inputs[0]):
+        if isinstance(tokens, str) or (tokens and " " in tokens[0]):
             is_split_into_words = False
 
         batch_encoding = self.tokenizer(
-            inputs,
+            tokens,
             **kwargs,
             is_split_into_words=is_split_into_words,
             padding="max_length",
             truncation=True,
             max_length=self.model_max_length,
             return_tensors="pt",
         )
 
         all_input_ids = []
         all_num_spans = []
         all_start_position_ids = []
         all_end_position_ids = []
         all_labels = []
         all_num_words = []
-
         for sample_idx, input_ids in enumerate(batch_encoding["input_ids"]):
-            word_ids = itertools.takewhile(lambda word_id: word_id is not None, batch_encoding.word_ids(sample_idx)[1:])
-            num_words = max(word_ids) + 1
+            num_words = int(np.nanmax(np.array(batch_encoding.word_ids(sample_idx), dtype=float))) + 1
             if self.tokenizer.pad_token_id in input_ids:
                 num_tokens = list(input_ids).index(self.tokenizer.pad_token_id)
             else:
                 num_tokens = len(input_ids)
             if labels:
                 span_to_label = {(start_idx, end_idx): label for label, start_idx, end_idx in labels[sample_idx]}
                 if self.entity_tracker.enabled:
@@ -221,42 +221,33 @@
                 # entity was ignored, and we may want to track it for a useful warning
                 if self.entity_tracker.enabled:
                     for start, end in span_to_label.keys():
                         self.entity_tracker.missed(end - start)
             else:
                 spans = list(self.get_all_valid_spans(num_words, self.config.entity_max_length))
 
-            # Compute the total number of start and end marker pairs we can include in this sample
-            num_marker_pairs = (self.model_max_length + 2 * self.config.marker_max_length - num_tokens) // 2
+            start_position_ids, end_position_ids = [], []
+            for start_word_i, end_word_i in spans:
+                start_token_span = batch_encoding.word_to_tokens(sample_idx, word_index=start_word_i)
+                # The if ... else 0 exists because of words like '\u2063'
+                start_position_ids.append(start_token_span.start if start_token_span else 0)
+
+                end_token_span = batch_encoding.word_to_tokens(sample_idx, word_index=end_word_i - 1)
+                end_position_ids.append(end_token_span.end - 1 if end_token_span else 0)
+
+            all_input_ids.append(input_ids[:num_tokens].tolist())
+            all_num_spans.append(len(spans))
+            all_start_position_ids.append(start_position_ids)
+            all_end_position_ids.append(end_position_ids)
 
-            for group_start_idx in range(0, len(spans), num_marker_pairs):
-                group_end_idx = group_start_idx + num_marker_pairs
-                group_spans = spans[group_start_idx:group_end_idx]
-                group_num_spans = len(group_spans)
-
-                start_position_ids, end_position_ids = [], []
-                for start_word_i, end_word_i in group_spans:
-                    start_token_span = batch_encoding.word_to_tokens(sample_idx, word_index=start_word_i)
-                    # The if ... else 0 exists because of words like '\u2063'
-                    start_position_ids.append(start_token_span.start if start_token_span else 0)
-
-                    end_token_span = batch_encoding.word_to_tokens(sample_idx, word_index=end_word_i - 1)
-                    end_position_ids.append(end_token_span.end - 1 if end_token_span else 0)
-
-                all_input_ids.append(input_ids[:num_tokens])
-                all_num_spans.append(group_num_spans)
-                all_start_position_ids.append(start_position_ids)
-                all_end_position_ids.append(end_position_ids)
-
-                if labels:
-                    group_labels = span_labels[group_start_idx:group_end_idx]
-                    all_labels.append(group_labels)
+            if labels:
+                all_labels.append(span_labels)
 
-                if return_num_words:
-                    all_num_words.append(num_words)
+            if return_num_words:
+                all_num_words.append(num_words)
 
         output = {
             "input_ids": all_input_ids,
             "num_spans": all_num_spans,
             "start_position_ids": all_start_position_ids,
             "end_position_ids": all_end_position_ids,
         }
```

### Comparing `span_marker-1.0.1/span_marker.egg-info/PKG-INFO` & `span_marker-1.1.0/span_marker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 1.0.1
+Version: 1.1.0
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -95,12 +95,22 @@
 ## Pretrained Models
 
 * [`tomaarsen/span-marker-bert-base-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-bert-base-fewnerd-fine-super) is a model that I have trained in 2 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd). It reached a 0.7053 Test F1, competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup) using `bert-base`. My training script resembles the one that you can see above.
   * Try the model out online using this [🤗 Space](https://tomaarsen-span-marker-bert-base-fewnerd-fine-super.hf.space/).
 
 * [`tomaarsen/span-marker-roberta-large-fewnerd-fine-super`](https://huggingface.co/tomaarsen/span-marker-roberta-large-fewnerd-fine-super) was trained in 6 hours on the finegrained, supervised [Few-NERD dataset](https://huggingface.co/datasets/DFKI-SLT/few-nerd) using `roberta-large`. It reached a 0.7103 Test F1, very competitive in the all-time [Few-NERD leaderboard](https://paperswithcode.com/sota/named-entity-recognition-on-few-nerd-sup).
 
+## Context
+<h1 align="center">
+    <a href="https://github.com/argilla-io/argilla">
+    <img src="https://github.com/dvsrepo/imgs/raw/main/rg.svg" alt="Argilla" width="150">
+    </a>
+</h1>
+
+I have developed this library as a part of my thesis work at [Argilla](https://github.com/argilla-io/argilla).
+Feel free to ⭐ star or watch the SpanMarker repository to get notified when my thesis is published.
+
 ## Changelog
 See [CHANGELOG.md](CHANGELOG.md) for news on all SpanMarker versions.
 
 ## License
 See [LICENSE](LICENSE.md) for the current license.
```

### Comparing `span_marker-1.0.1/span_marker.egg-info/SOURCES.txt` & `span_marker-1.1.0/span_marker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `span_marker-1.0.1/tests/test_model_card.py` & `span_marker-1.1.0/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.0.1/tests/test_modeling.py` & `span_marker-1.1.0/tests/test_modeling.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from typing import Dict, List, Optional, Union
 
 import pytest
 import torch
+from datasets import Dataset
 
 from span_marker.configuration import SpanMarkerConfig
 from span_marker.modeling import SpanMarkerModel
 from span_marker.tokenizer import SpanMarkerTokenizer
 from tests.constants import CONLL_LABELS, FEWNERD_COARSE_LABELS, TINY_BERT
 from tests.helpers import compare_entities
 
@@ -21,15 +22,15 @@
         ("tomaarsen/span-marker-bert-tiny-conll03", None),
         ("tomaarsen/span-marker-bert-tiny-fewnerd-coarse-super", FEWNERD_COARSE_LABELS),
         ("tomaarsen/span-marker-bert-tiny-fewnerd-coarse-super", None),
     ],
 )
 def test_from_pretrained(model_name: str, labels: Optional[List[str]]) -> None:
     def load() -> SpanMarkerModel:
-        return SpanMarkerModel.from_pretrained(model_name, labels=labels)
+        return SpanMarkerModel.from_pretrained(model_name, labels=labels).try_cuda()
 
     # If labels have to be provided
     if model_name == TINY_BERT and labels is None:
         with pytest.raises(
             ValueError, match=re.escape("Please provide a `labels` list to `SpanMarkerModel.from_pretrained()`")
         ):
             model = load()
@@ -75,25 +76,100 @@
     ],
 )
 def test_correct_predictions(
     finetuned_conll_span_marker_model: SpanMarkerModel,
     inputs: Union[str, List[str]],
     gold_entities: List[Dict[str, Union[str, int]]],
 ) -> None:
-    model = finetuned_conll_span_marker_model
+    model = finetuned_conll_span_marker_model.try_cuda()
 
     # Single sentence
     pred_entities = model.predict(inputs)
     compare_entities(pred_entities, gold_entities)
 
     # Multiple sentences
     pred_entity_list = model.predict([inputs] * 3)
     for pred_entities in pred_entity_list:
         compare_entities(pred_entities, gold_entities)
 
+    # As a Dataset
+    pred_entities = model.predict(Dataset.from_dict({"tokens": [inputs]}))
+    compare_entities(pred_entities, gold_entities)
+
+
+@pytest.mark.parametrize(
+    ("inputs", "gold_entity_list"),
+    [
+        (
+            Dataset.from_dict(
+                {
+                    "tokens": [
+                        "I'm living in the Netherlands, but I work in Spain.",
+                        "My name is Tom and this is a test.",
+                        "I hope it can detect Paris here.",
+                        "And nothing in this sentence.",
+                    ],
+                    "document_id": [0, 0, 0, 0],
+                    "sentence_id": [0, 1, 2, 3],
+                }
+            ),
+            [
+                [
+                    {"span": "Netherlands", "label": "LOC", "char_start_index": 18, "char_end_index": 29},
+                    {"span": "Spain", "label": "LOC", "char_start_index": 45, "char_end_index": 50},
+                ],
+                [{"span": "Tom", "label": "PER", "char_start_index": 11, "char_end_index": 14}],
+                [{"span": "Paris", "label": "LOC", "char_start_index": 21, "char_end_index": 26}],
+                [],
+            ],
+        ),
+        (
+            Dataset.from_dict(
+                {
+                    "tokens": [
+                        "I'm living in the Netherlands, but I work in Spain.",
+                        "My name is Tom and this is a test.",
+                        "I hope it can detect Paris here.",
+                        "And nothing in this sentence.",
+                    ],
+                    "document_id": [0, 1, 0, 0],
+                    "sentence_id": [0, 0, 2, 1],
+                }
+            ),
+            [
+                [
+                    {"span": "Netherlands", "label": "LOC", "char_start_index": 18, "char_end_index": 29},
+                    {"span": "Spain", "label": "LOC", "char_start_index": 45, "char_end_index": 50},
+                ],
+                [{"span": "Tom", "label": "PER", "char_start_index": 11, "char_end_index": 14}],
+                [{"span": "Paris", "label": "LOC", "char_start_index": 21, "char_end_index": 26}],
+                [],
+            ],
+        ),
+    ],
+)
+def test_correct_predictions_with_document_level_context(
+    finetuned_conll_span_marker_model: SpanMarkerModel,
+    inputs: Union[str, List[str]],
+    gold_entity_list: List[Dict[str, Union[str, int]]],
+) -> None:
+    model = finetuned_conll_span_marker_model.try_cuda()
+
+    pred_entity_list = model.predict(inputs)
+    for pred_entities, gold_entities in zip(pred_entity_list, gold_entity_list):
+        compare_entities(pred_entities, gold_entities)
+
+
+def test_incorrect_predict_inputs(finetuned_conll_span_marker_model: SpanMarkerModel):
+    model = finetuned_conll_span_marker_model.try_cuda()
+    with pytest.raises(ValueError, match="could not recognize your input"):
+        model.predict(12)
+    with pytest.raises(ValueError, match="could not recognize your input"):
+        model.predict(True)
+
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         # Reasonable kwargs that will be used by SpanMarkerConfig
         {
             "model_max_length": 256,
```

### Comparing `span_marker-1.0.1/tests/test_trainer.py` & `span_marker-1.1.0/tests/test_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,33 @@
         "eval_steps_per_second",
         "epoch",
     }
 
     # Try saving and loading the model
     model_path = tmp_path / model_fixture / dataset_fixture
     model.save_pretrained(model_path)
-    loaded_model = model.from_pretrained(model_path)
+    loaded_model = model.from_pretrained(model_path).try_cuda()
     output = loaded_model.predict(
         "This might just output confusing things like M.C. Escher, but it should at least not crash in Germany."
     )
     assert isinstance(output, list)
 
 
+@pytest.mark.parametrize(
+    "dataset_fixture",
+    [
+        "conll_dataset_dict",
+        "document_context_conll_dataset_dict",
+    ],
+)
 def test_trainer_model_init(
-    finetuned_conll_span_marker_model: SpanMarkerModel, conll_dataset_dict: DatasetDict
+    finetuned_conll_span_marker_model: SpanMarkerModel, dataset_fixture: str, request: pytest.FixtureRequest
 ) -> None:
     model = finetuned_conll_span_marker_model
-    dataset = conll_dataset_dict
+    dataset: DatasetDict = request.getfixturevalue(dataset_fixture)
 
     def model_init() -> SpanMarkerModel:
         return model
 
     trainer = Trainer(
         model_init=model_init, args=DEFAULT_ARGS, train_dataset=dataset["train"], eval_dataset=dataset["test"]
     )
```

