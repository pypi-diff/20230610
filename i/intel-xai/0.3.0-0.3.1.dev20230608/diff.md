# Comparing `tmp/intel_xai-0.3.0-py3-none-any.whl.zip` & `tmp/intel_xai-0.3.1.dev20230608-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,65 +1,36 @@
-Zip file size: 302400 bytes, number of entries: 63
--rw-r--r--  2.0 unx     3318 b- defN 23-Mar-20 23:04 explainer/README.md
--rw-r--r--  2.0 unx      697 b- defN 23-Mar-20 23:04 explainer/version.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Mar-20 23:04 explainer/attributions/README.md
--rw-r--r--  2.0 unx      703 b- defN 23-Mar-20 23:04 explainer/attributions/__init__.py
--rw-r--r--  2.0 unx    14195 b- defN 23-Mar-20 23:04 explainer/attributions/attributions.py
--rw-r--r--  2.0 unx      876 b- defN 23-Mar-20 23:04 explainer/cam/README.md
--rw-r--r--  2.0 unx      694 b- defN 23-Mar-20 23:04 explainer/cam/__init__.py
--rw-r--r--  2.0 unx     6072 b- defN 23-Mar-20 23:04 explainer/cam/cam.py
--rw-r--r--  2.0 unx      995 b- defN 23-Mar-20 23:04 explainer/metrics/README.md
--rw-r--r--  2.0 unx      698 b- defN 23-Mar-20 23:04 explainer/metrics/__init__.py
--rw-r--r--  2.0 unx    11746 b- defN 23-Mar-20 23:04 explainer/metrics/metrics.py
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 explainer/tests/__init__.py
--rw-r--r--  2.0 unx     2772 b- defN 23-Mar-20 23:04 explainer/tests/conftest.py
--rw-r--r--  2.0 unx      672 b- defN 23-Mar-20 23:04 explainer/tests/pytest.ini
--rw-r--r--  2.0 unx     1419 b- defN 23-Mar-20 23:04 explainer/tests/test_attributions.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Mar-20 23:04 explainer/tests/test_cam.py
--rw-r--r--  2.0 unx     3196 b- defN 23-Mar-20 23:04 explainer/tests/test_metrics.py
--rw-r--r--  2.0 unx       16 b- defN 23-Mar-20 23:04 explainer/tests/test_requirements.txt
--rw-r--r--  2.0 unx     8547 b- defN 23-Mar-20 23:29 model_card_gen/README.md
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 model_card_gen/__init__.py
--rw-r--r--  2.0 unx     3423 b- defN 23-Mar-20 23:04 model_card_gen/base_model_card_field.py
--rw-r--r--  2.0 unx    20799 b- defN 23-Mar-20 23:04 model_card_gen/model_card.py
--rw-r--r--  2.0 unx    16402 b- defN 23-Mar-20 23:04 model_card_gen/model_card_gen.py
--rw-r--r--  2.0 unx     3344 b- defN 23-Mar-20 23:04 model_card_gen/validation.py
--rw-r--r--  2.0 unx      697 b- defN 23-Mar-20 23:04 model_card_gen/version.py
--rw-r--r--  2.0 unx      848 b- defN 23-Mar-20 23:04 model_card_gen/analyze/__init__.py
--rw-r--r--  2.0 unx     2764 b- defN 23-Mar-20 23:04 model_card_gen/analyze/analyzer.py
--rw-r--r--  2.0 unx     3610 b- defN 23-Mar-20 23:04 model_card_gen/analyze/analyzer_factory.py
--rw-r--r--  2.0 unx     2633 b- defN 23-Mar-20 23:04 model_card_gen/analyze/pandas_analyzer.py
--rw-r--r--  2.0 unx     3032 b- defN 23-Mar-20 23:04 model_card_gen/analyze/tf_analyzer.py
--rw-r--r--  2.0 unx     4121 b- defN 23-Mar-20 23:04 model_card_gen/analyze/torch_analyzer.py
--rw-r--r--  2.0 unx      795 b- defN 23-Mar-20 23:04 model_card_gen/datasets/__init__.py
--rw-r--r--  2.0 unx     1376 b- defN 23-Mar-20 23:04 model_card_gen/datasets/datasets.py
--rw-r--r--  2.0 unx     1092 b- defN 23-Mar-20 23:04 model_card_gen/datasets/tf_datasets.py
--rw-r--r--  2.0 unx     4180 b- defN 23-Mar-20 23:04 model_card_gen/datasets/torch_datasets.py
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 model_card_gen/docs/examples/__init__.py
--rw-r--r--  2.0 unx   510942 b- defN 23-Mar-20 23:04 model_card_gen/docs/examples/html/compas_model_card.html
--rw-r--r--  2.0 unx   520886 b- defN 23-Mar-20 23:04 model_card_gen/docs/examples/json/model_card_compas.json
--rw-r--r--  2.0 unx     4964 b- defN 23-Mar-20 23:04 model_card_gen/docs/examples/json/model_card_example.json
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 model_card_gen/graphics/__init__.py
--rw-r--r--  2.0 unx     5284 b- defN 23-Mar-20 23:04 model_card_gen/graphics/add_graphics.py
--rw-r--r--  2.0 unx    11094 b- defN 23-Mar-20 23:04 model_card_gen/graphics/plotly_graphics.py
--rw-r--r--  2.0 unx     3607 b- defN 23-Mar-20 23:04 model_card_gen/graphics/plotly_utils.py
--rw-r--r--  2.0 unx    12984 b- defN 23-Mar-20 23:04 model_card_gen/notebooks/adult-pytorch-model-card.ipynb
--rw-r--r--  2.0 unx    36039 b- defN 23-Mar-20 23:04 model_card_gen/notebooks/compas-model-card-tfx.ipynb
--rw-r--r--  2.0 unx    18662 b- defN 23-Mar-20 23:04 model_card_gen/notebooks/toxicity-tfma-model-card.ipynb
--rw-r--r--  2.0 unx    10850 b- defN 23-Mar-20 23:04 model_card_gen/schema/v0.0.1/model_card.schema.json
--rw-r--r--  2.0 unx     5965 b- defN 23-Mar-20 23:04 model_card_gen/template/html/default_template.html.jinja
--rw-r--r--  2.0 unx      581 b- defN 23-Mar-20 23:04 model_card_gen/template/html/js/plotly_js_header.html.jinja
--rw-r--r--  2.0 unx     3468 b- defN 23-Mar-20 23:04 model_card_gen/template/html/macros/default_macros.html.jinja
--rw-r--r--  2.0 unx     1574 b- defN 23-Mar-20 23:04 model_card_gen/template/html/style/default_style.html.jinja
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 model_card_gen/tests/__init__.py
--rw-r--r--  2.0 unx     1945 b- defN 23-Mar-20 23:04 model_card_gen/tests/test_end_to_end_tf.py
--rw-r--r--  2.0 unx     1947 b- defN 23-Mar-20 23:04 model_card_gen/tests/test_end_to_end_torch.py
--rw-r--r--  2.0 unx     2400 b- defN 23-Mar-20 23:04 model_card_gen/tests/test_model_card.py
--rw-r--r--  2.0 unx     3996 b- defN 23-Mar-20 23:04 model_card_gen/tests/tf_model.py
--rw-r--r--  2.0 unx     3216 b- defN 23-Mar-20 23:04 model_card_gen/tests/torch_model.py
--rw-r--r--  2.0 unx      674 b- defN 23-Mar-20 23:04 model_card_gen/utils/__init__.py
--rw-r--r--  2.0 unx      875 b- defN 23-Mar-20 23:04 model_card_gen/utils/types.py
--rw-r--r--  2.0 unx     5570 b- defN 23-Mar-21 00:59 intel_xai-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-21 00:59 intel_xai-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Mar-21 00:59 intel_xai-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5845 b- defN 23-Mar-21 00:59 intel_xai-0.3.0.dist-info/RECORD
-63 files, 1305011 bytes uncompressed, 292952 bytes compressed:  77.6%
+Zip file size: 46081 bytes, number of entries: 34
+-rw-r--r--  2.0 unx     3318 b- defN 23-Jun-09 23:26 explainer/README.md
+-rw-r--r--  2.0 unx      709 b- defN 23-Jun-09 23:26 explainer/version.py
+-rw-r--r--  2.0 unx     1057 b- defN 23-Jun-09 23:26 explainer/attributions/README.md
+-rw-r--r--  2.0 unx      703 b- defN 23-Jun-09 23:26 explainer/attributions/__init__.py
+-rw-r--r--  2.0 unx    14915 b- defN 23-Jun-09 23:26 explainer/attributions/attributions.py
+-rw-r--r--  2.0 unx     2627 b- defN 23-Jun-09 17:45 explainer/attributions/attributions_info.py
+-rw-r--r--  2.0 unx     5269 b- defN 23-Jun-09 23:25 explainer/attributions/plots.py
+-rw-r--r--  2.0 unx    14839 b- defN 23-Jun-09 16:58 explainer/attributions/pt_attributions.py
+-rw-r--r--  2.0 unx    14620 b- defN 23-Jun-09 18:02 explainer/attributions/widgets.py
+-rw-r--r--  2.0 unx      876 b- defN 23-Jun-09 23:26 explainer/cam/README.md
+-rw-r--r--  2.0 unx      694 b- defN 23-Jun-09 23:26 explainer/cam/__init__.py
+-rw-r--r--  2.0 unx     6072 b- defN 23-Jun-09 23:26 explainer/cam/cam.py
+-rw-r--r--  2.0 unx     9257 b- defN 23-Jun-09 16:58 explainer/cam/pt_cam.py
+-rw-r--r--  2.0 unx     4813 b- defN 23-Jun-09 16:58 explainer/cam/tf_cam.py
+-rw-r--r--  2.0 unx      995 b- defN 23-Jun-09 23:26 explainer/metrics/README.md
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-09 16:58 explainer/metrics/__init__.py
+-rw-r--r--  2.0 unx    11746 b- defN 23-Jun-09 23:26 explainer/metrics/metrics.py
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-09 16:58 explainer/tests/__init__.py
+-rw-r--r--  2.0 unx     2772 b- defN 23-Jun-09 23:26 explainer/tests/conftest.py
+-rw-r--r--  2.0 unx      672 b- defN 23-Jun-09 16:58 explainer/tests/pytest.ini
+-rw-r--r--  2.0 unx     2134 b- defN 23-Jun-09 23:26 explainer/tests/test_attributions.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-09 23:26 explainer/tests/test_cam.py
+-rw-r--r--  2.0 unx     3196 b- defN 23-Jun-09 23:26 explainer/tests/test_metrics.py
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-09 16:58 explainer/tests/test_requirements.txt
+-rw-r--r--  2.0 unx      768 b- defN 23-Jun-09 16:58 explainer/utils/types.py
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-09 16:58 explainer/utils/graphics/__init__.py
+-rw-r--r--  2.0 unx     2380 b- defN 23-Jun-09 16:58 explainer/utils/graphics/info.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-09 16:58 explainer/utils/model/__init__.py
+-rw-r--r--  2.0 unx      938 b- defN 23-Jun-09 16:58 explainer/utils/model/model_framework.py
+-rw-r--r--  2.0 unx    11347 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7009 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2963 b- defN 23-Jun-09 23:38 intel_xai-0.3.1.dev20230608.dist-info/RECORD
+34 files, 130219 bytes uncompressed, 41287 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -9,23 +9,41 @@
 
 Filename: explainer/attributions/__init__.py
 Comment: 
 
 Filename: explainer/attributions/attributions.py
 Comment: 
 
+Filename: explainer/attributions/attributions_info.py
+Comment: 
+
+Filename: explainer/attributions/plots.py
+Comment: 
+
+Filename: explainer/attributions/pt_attributions.py
+Comment: 
+
+Filename: explainer/attributions/widgets.py
+Comment: 
+
 Filename: explainer/cam/README.md
 Comment: 
 
 Filename: explainer/cam/__init__.py
 Comment: 
 
 Filename: explainer/cam/cam.py
 Comment: 
 
+Filename: explainer/cam/pt_cam.py
+Comment: 
+
+Filename: explainer/cam/tf_cam.py
+Comment: 
+
 Filename: explainer/metrics/README.md
 Comment: 
 
 Filename: explainer/metrics/__init__.py
 Comment: 
 
 Filename: explainer/metrics/metrics.py
@@ -48,143 +66,38 @@
 
 Filename: explainer/tests/test_metrics.py
 Comment: 
 
 Filename: explainer/tests/test_requirements.txt
 Comment: 
 
-Filename: model_card_gen/README.md
-Comment: 
-
-Filename: model_card_gen/__init__.py
-Comment: 
-
-Filename: model_card_gen/base_model_card_field.py
-Comment: 
-
-Filename: model_card_gen/model_card.py
-Comment: 
-
-Filename: model_card_gen/model_card_gen.py
-Comment: 
-
-Filename: model_card_gen/validation.py
-Comment: 
-
-Filename: model_card_gen/version.py
-Comment: 
-
-Filename: model_card_gen/analyze/__init__.py
-Comment: 
-
-Filename: model_card_gen/analyze/analyzer.py
-Comment: 
-
-Filename: model_card_gen/analyze/analyzer_factory.py
-Comment: 
-
-Filename: model_card_gen/analyze/pandas_analyzer.py
-Comment: 
-
-Filename: model_card_gen/analyze/tf_analyzer.py
-Comment: 
-
-Filename: model_card_gen/analyze/torch_analyzer.py
-Comment: 
-
-Filename: model_card_gen/datasets/__init__.py
-Comment: 
-
-Filename: model_card_gen/datasets/datasets.py
-Comment: 
-
-Filename: model_card_gen/datasets/tf_datasets.py
-Comment: 
-
-Filename: model_card_gen/datasets/torch_datasets.py
-Comment: 
-
-Filename: model_card_gen/docs/examples/__init__.py
-Comment: 
-
-Filename: model_card_gen/docs/examples/html/compas_model_card.html
-Comment: 
-
-Filename: model_card_gen/docs/examples/json/model_card_compas.json
-Comment: 
-
-Filename: model_card_gen/docs/examples/json/model_card_example.json
-Comment: 
-
-Filename: model_card_gen/graphics/__init__.py
-Comment: 
-
-Filename: model_card_gen/graphics/add_graphics.py
-Comment: 
-
-Filename: model_card_gen/graphics/plotly_graphics.py
-Comment: 
-
-Filename: model_card_gen/graphics/plotly_utils.py
-Comment: 
-
-Filename: model_card_gen/notebooks/adult-pytorch-model-card.ipynb
-Comment: 
-
-Filename: model_card_gen/notebooks/compas-model-card-tfx.ipynb
-Comment: 
-
-Filename: model_card_gen/notebooks/toxicity-tfma-model-card.ipynb
-Comment: 
-
-Filename: model_card_gen/schema/v0.0.1/model_card.schema.json
-Comment: 
-
-Filename: model_card_gen/template/html/default_template.html.jinja
-Comment: 
-
-Filename: model_card_gen/template/html/js/plotly_js_header.html.jinja
-Comment: 
-
-Filename: model_card_gen/template/html/macros/default_macros.html.jinja
-Comment: 
-
-Filename: model_card_gen/template/html/style/default_style.html.jinja
-Comment: 
-
-Filename: model_card_gen/tests/__init__.py
-Comment: 
-
-Filename: model_card_gen/tests/test_end_to_end_tf.py
-Comment: 
-
-Filename: model_card_gen/tests/test_end_to_end_torch.py
+Filename: explainer/utils/types.py
 Comment: 
 
-Filename: model_card_gen/tests/test_model_card.py
+Filename: explainer/utils/graphics/__init__.py
 Comment: 
 
-Filename: model_card_gen/tests/tf_model.py
+Filename: explainer/utils/graphics/info.py
 Comment: 
 
-Filename: model_card_gen/tests/torch_model.py
+Filename: explainer/utils/model/__init__.py
 Comment: 
 
-Filename: model_card_gen/utils/__init__.py
+Filename: explainer/utils/model/model_framework.py
 Comment: 
 
-Filename: model_card_gen/utils/types.py
+Filename: intel_xai-0.3.1.dev20230608.dist-info/LICENSE
 Comment: 
 
-Filename: intel_xai-0.3.0.dist-info/METADATA
+Filename: intel_xai-0.3.1.dev20230608.dist-info/METADATA
 Comment: 
 
-Filename: intel_xai-0.3.0.dist-info/WHEEL
+Filename: intel_xai-0.3.1.dev20230608.dist-info/WHEEL
 Comment: 
 
-Filename: intel_xai-0.3.0.dist-info/top_level.txt
+Filename: intel_xai-0.3.1.dev20230608.dist-info/top_level.txt
 Comment: 
 
-Filename: intel_xai-0.3.0.dist-info/RECORD
+Filename: intel_xai-0.3.1.dev20230608.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## explainer/version.py

```diff
@@ -14,8 +14,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-__version__ = "0.3.0"
+__version__ = "0.3.1.dev20230608"
```

## explainer/attributions/attributions.py

```diff
@@ -14,33 +14,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
+import torch
+import pandas as pd
+import numpy as np
+from typing import Union, Optional, Callable, List
+from .attributions_info import force_plot_info_panel
+from explainer.utils.graphics.info import InfoPanel
+from explainer.utils.types import TorchTensor
+from explainer.utils.model.model_framework import (is_tf_model,
+                                                   is_pt_model,
+                                                   raise_unknown_model_error)
+
+
 class FeatureAttributions:
     def __init__(self):
         import shap
         shap.initjs()
         self.shap = shap
         self.datasets = shap.datasets
         self.plots = self.shap.plots
         self.bar_plot = self.plots.bar
         self.image_plot = self.plots.image
         self.force_plot = self.shap.force_plot
         self.text_plot = self.plots.text
         self.waterfall_plot = self.shap.waterfall_plot
+        self.info_panel = {}
 
     def __call__(self, *args, **kwargs):
         pass
 
     def visualize(self, data):
         pass
 
+    def get_info(self):
+        """Display into panel in Jupyter Enviornment"""
+        if self.info_panel:
+            info = InfoPanel(**self.info_panel)
+            info.show()
+
 
 class DeepExplainer(FeatureAttributions):
     def __init__(self, model, background_images, target_images, labels):
         super().__init__()
         self.target_images = target_images
         self.explainer = self.shap.DeepExplainer(model, background_images)
         self.shap_values = self.explainer.shap_values(target_images)
@@ -96,14 +115,15 @@
 class KernelExplainer(FeatureAttributions):
     def __init__(self, model, background, targets, nsamples):
         super().__init__()
         self.bg = background
         self.targets = targets
         self.explainer = self.shap.KernelExplainer(model, self.bg)
         self.shap_values = self.explainer.shap_values(self.targets, nsamples=nsamples)
+        self.info_panel = force_plot_info_panel
 
     def visualize(self):
         return self.force_plot(self.explainer.expected_value, self.shap_values[0], self.targets)
 
 
 class PartitionExplainer(FeatureAttributions):
     def __init__(self, model, tokenizer, categories):
```

## explainer/tests/test_attributions.py

```diff
@@ -14,28 +14,51 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 ### libraries to support tests ###
-from collections import namedtuple
 import pytest
 from deepdiff import DeepDiff
 import numpy as np
-import torch, torchvision
-from torchvision import datasets, transforms
-from torch import nn, optim
-from torch.nn import functional as F
+import pandas as pd
+import scipy as sp
+import transformers
+import torch
 torch.manual_seed(0)
 ### library to be tested ###
 from explainer import attributions
+from attributions.plots import shap_waterwall_plot
+from attributions.widgets import ShapUI
 ###################################
 
 device = torch.device('cpu')
 
 def test_deep_explainer(custom_pyt_CNN):
     model, test_loader, class_names = custom_pyt_CNN 
     X_test = next(iter(test_loader))[0].to(device)
     deViz = attributions.deep_explainer(model, X_test[:2], X_test[2:4], class_names)
     assert isinstance(deViz, attributions.attributions.DeepExplainer) 
     deViz.visualize()
+
+def test_shap_waterwall_plot():
+    kwargs = dict(expected_value=.5,
+                  shap_values=np.random.normal(0, 1, 10),
+                  feature_values=np.random.rand(10),
+                  columns=list(range(10)),
+                  y_true=0)
+
+    assert shap_waterwall_plot(**kwargs)
+
+
+def test_shap_ui():
+    kwargs = dict(df=pd.DataFrame({"Feature 1": np.random.rand(10), 
+                                   "Feature 2": np.random.rand(10)}),
+                  shap_values=np.random.normal(0, 1, (10, 2)),
+                  expected_value=.5,
+                  y_true=np.random.randint(0, 2, 10),
+                  y_pred=np.random.randint(0, 2, 10))
+
+    ui = ShapUI(**kwargs)
+    ui.show()
+    assert ui.view
```

## Comparing `model_card_gen/__init__.py` & `explainer/utils/graphics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2023 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
-#
+#
```

## Comparing `model_card_gen/analyze/__init__.py` & `explainer/utils/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #
-# Copyright (c) 2022 Intel Corporation
+# Copyright (c) 2023 Intel Corporation
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,11 +14,11 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 #
 
-from .pandas_analyzer import DFAnalyzer
-from .tf_analyzer import TFAnalyzer
-from .torch_analyzer import PTAnalyzer
-from .analyzer_factory import get_analyzers, get_analysis
+from pydoc import locate
+from typing import Any
+
+TorchTensor = locate('torch.Tensor') or Any
```

## Comparing `intel_xai-0.3.0.dist-info/METADATA` & `intel_xai-0.3.1.dev20230608.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-xai
-Version: 0.3.0
+Version: 0.3.1.dev20230608
 Summary: Intel® Explainable AI Tools
 Home-page: https://github.com/IntelAI/intel-xai-tools
 Author: IntelAI
 Author-email: IntelAI@intel.com
 License: Apache 2.0
 Keywords: XAI,explainer
 Platform: any
@@ -18,107 +18,130 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.9,<3.11
 Description-Content-Type: text/markdown
-Requires-Dist: absl-py
-Requires-Dist: attrs (<22,>=19.3.0)
+License-File: LICENSE
 Requires-Dist: captum
-Requires-Dist: grad-cam
-Requires-Dist: grpcio-status (<1.49)
 Requires-Dist: intel-tensorflow (==2.11.0)
-Requires-Dist: jinja2
-Requires-Dist: joblib (>=1.2.0)
-Requires-Dist: jsonschema[format-nongpl]
-Requires-Dist: matplotlib
+Requires-Dist: ipywidgets
 Requires-Dist: numpy (<1.23.0,>=1.14.3)
 Requires-Dist: opencv-python
-Requires-Dist: pandas
-Requires-Dist: plotly
-Requires-Dist: protobuf (<3.20,>=3.9.2)
-Requires-Dist: scikit-learn
 Requires-Dist: scikit-plot
 Requires-Dist: scipy
-Requires-Dist: seaborn
-Requires-Dist: semantic-version
 Requires-Dist: shap
-Requires-Dist: tensorflow-data-validation
-Requires-Dist: tensorflow-model-analysis
 Requires-Dist: torch (==1.13.1)
 Requires-Dist: transformers
-Requires-Dist: dataclasses ; python_version < "3.7"
+Requires-Dist: plotly (==5.14.1)
+Requires-Dist: grad-cam
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: scikit-learn
+Requires-Dist: seaborn
 Provides-Extra: pytorch
 Requires-Dist: torch (==1.13.1) ; extra == 'pytorch'
 Requires-Dist: torchvision (==0.14.1) ; extra == 'pytorch'
 Provides-Extra: test
 Requires-Dist: deepdiff ; extra == 'test'
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: tensorflow-hub ; extra == 'test'
 Requires-Dist: torch (==1.13.1) ; extra == 'test'
 Requires-Dist: torchvision (==0.14.1) ; extra == 'test'
 
 # Intel® Explainable AI Tools
 
 This repository provides tools for data scientists and MLOps engineers that have requirements specific to AI model interpretability.
 
-## Features
-| Core Feature | Description | 
-|----------|-----------|
-| **Model Card Generator** |  **Allows users to create interactive HTML reports containing model performance and fairness metrics.** |
-|**Explainer** | **Allows users to run post-hoc model distillation and visualization methods to examine predictive behavior for both TensorFlow and PyTorch models via a simple Python API including the following modules:** <li> **Attributions**: visualize negative and positive attributions of tabular features, pixels, and word tokens for predictions <li> **CAM**: create heatmaps for CNN image classifications using gradient-weight class activation CAM mapping <li> **Metrics**: Gain insight into models with the measurements and visualizations needed during the machine learning workflow |
-
-## Build and Install
-Requirements:
-* Linux system (or WSL2 on Windows)
-* git
-* required python version: 3.9
-* `apt-get install build-essential python3-dev`
+## Overview
 
-### Basic Installation:
-```
-pip install intel-xai
-```
-### Advanced/Developer Installation:
-1. Clone this repo and navigate to the repo directory:
-   ```
-   git clone https://github.com/IntelAI/intel-xai-tools.git
+The Intel Explainable AI Tools are designed to help users detect and mitigate against issues of fairness and interpretability, while running best on Intel hardware.
+There are two Python* components in the repository:
 
-   cd intel-xai-tools
-   ```
-2. Create and activate a Python3.9 virtual environment using `virtualenv`:
+* [Model Card Generator](model_card_gen)
+  * Creates interactive HTML reports containing model performance and fairness metrics
+* [Explainer](explainer)
+  * Runs post-hoc model distillation and visualization methods to examine predictive behavior for both TensorFlow* and PyTorch* models via a simple Python API including the following modules:
+    * [Attributions](explainer/attributions/): Visualize negative and positive attributions of tabular features, pixels, and word tokens for predictions
+    * [CAM (Class Activation Mapping)](explainer/cam/): Create heatmaps for CNN image classifications using gradient-weight class activation CAM mapping
+    * [Metrics](explainer/metrics/): Gain insight into models with the measurements and visualizations needed during the machine learning workflow
+
+
+  * [ShapUI](explainer/attributions/widgets.py#L254): A user interface to explore and compare impact scores of model predictions for each record of a tabular data set and discover insights of a model's behavior:
+    * **Error Analysis** allows the user to filter data points based on their error type.
+    * **Impact Analysis** allows users to filter data points based on their associated SHAP impact score for top important features.
+    * **Feature Analysis** allows users to filter data points by feature values for top important features.
+
+## Get Started
+
+### Requirements
+* Linux system or WSL2 on Windows (validated on Ubuntu* 20.04/22.04 LTS)
+* Python 3.9 or 3.10
+* Install required OS packages with `apt-get install build-essential python3-dev`
+* git (only required for the "Developer Installation")
+
+### Create and activate a Python3 virtual environment
+We encourage you to use a python virtual environment (virtualenv or conda) for consistent package management.
+There are two ways to do this:
+
+a. Using `virtualenv`:
    ```
    python3.9 -m virtualenv xai_env
    source xai_env/bin/activate
    ```
 
    Or `conda`:
    ```
    conda create --name xai_env python=3.9
    conda activate xai_env
    ```
-3. Install this tool with 
+
+### Basic Installation
+```
+pip install intel-xai
+```
+### Developer Installation
+Use these instructions to install the Intel Explainable AI Tools with a clone of the
+GitHub repository. This can be done instead of the basic pip install, if you plan
+on making code changes.
+
+1. Clone this repo and navigate to the repo directory:
+   ```
+   git clone https://github.com/IntelAI/intel-xai-tools.git
+
+   cd intel-xai-tools
+   ```
+2. Install the Intel Explainable AI Tools using the following command:
    ```
    make install
    ```
 
 ## Running Notebooks
 
-Run **example notebooks** that show how to use the explainer and model card generator API in various ML domains and use cases. Notebooks may require additional dependencies listed in their associated README's.
+The following links have Jupyter* notebooks showing how to use the Explainer and Model Card Generator APIs in various ML domains and use cases:
+* [Model Card Generator Notebooks](/model_card_gen/notebooks)
+* [Explainer Notebooks](notebooks/)
+
+## Support
+
+The Intel Explainable AI Tools team tracks bugs and enhancement requests using
+[GitHub issues](https://github.com/intelai/intel-xai-tools/issues). Before submitting a
+suggestion or bug report, search the existing GitHub issues to see if your issue has already been reported.
+
+*Other names and brands may be claimed as the property of others. [Trademarks](http://www.intel.com/content/www/us/en/legal/trademarks.html)
 
 #### DISCLAIMER: ####
 These scripts are not intended for benchmarking Intel platforms. For any performance and/or benchmarking information on specific Intel platforms, visit https://www.intel.ai/blog.
-
+ 
 Intel is committed to the respect of human rights and avoiding complicity in human rights abuses, a policy reflected in the Intel Global Human Rights Principles. Accordingly, by accessing the Intel material on this platform you agree that you will not use the material in a product or application that causes or contributes to a violation of an internationally recognized human right.
-
+ 
 #### License: ####
 Intel® Explainable AI Tools is licensed under Apache License Version 2.0.
-
+ 
 #### Datasets: ####
-To the extent that any public datasets are referenced by Intel or accessed using tools or code on this site those datasets are provided by the third party indicated as the data source. Intel does not create the data, or datasets, and does not warrant their accuracy or quality. By accessing the public dataset(s) you agree to the terms associated with those datasets and that your use complies with the applicable license.
-
+To the extent that any public datasets are referenced by Intel or accessed using tools or code on this site those datasets are provided by the third party indicated as the data source. Intel does not create the data, or datasets, and does not warrant their accuracy or quality. By accessing the public dataset(s) you agree to the terms associated with those datasets and that your use complies with the applicable license. [DATASETS](DATASETS.md)
+ 
 Intel expressly disclaims the accuracy, adequacy, or completeness of any public datasets, and is not liable for any errors, omissions, or defects in the data, or for any reliance on the data.  Intel is not liable for any liability or damages relating to your use of public datasets.
-
-
```

