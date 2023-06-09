# Comparing `tmp/custom_diffusion-0.0.6.tar.gz` & `tmp/custom_diffusion-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.0.6.tar", last modified: Fri Jun  9 22:05:30 2023, max compression
+gzip compressed data, was "custom_diffusion-0.0.7.tar", last modified: Fri Jun  9 22:30:32 2023, max compression
```

## Comparing `custom_diffusion-0.0.6.tar` & `custom_diffusion-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.170365 custom_diffusion-0.0.6/
--rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:05:30.170365 custom_diffusion-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.130354 custom_diffusion-0.0.6/custom_diffusion/
--rw-rw-rw-   0        0        0       22 2023-06-09 22:05:01.000000 custom_diffusion-0.0.6/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0      921 2023-06-09 21:56:06.000000 custom_diffusion-0.0.6/custom_diffusion/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.161360 custom_diffusion-0.0.6/custom_diffusion/pipelines/
--rw-rw-rw-   0        0        0        0 2023-06-09 22:04:46.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/__init__.py
--rw-rw-rw-   0        0        0     6684 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-rw-rw-   0        0        0     8952 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.168363 custom_diffusion-0.0.6/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1338 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0     1273 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3517 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 22:05:30.155358 custom_diffusion-0.0.6/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     1354 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-06-09 22:05:30.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-09 22:05:29.000000 custom_diffusion-0.0.6/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      105 2023-06-09 22:05:09.000000 custom_diffusion-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-09 22:05:30.172364 custom_diffusion-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.674478 custom_diffusion-0.0.7/
+-rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1354 2023-06-09 22:30:32.674478 custom_diffusion-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.636227 custom_diffusion-0.0.7/custom_diffusion/
+-rw-rw-rw-   0        0        0       22 2023-06-09 22:30:25.000000 custom_diffusion-0.0.7/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0      859 2023-06-09 22:29:27.000000 custom_diffusion-0.0.7/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.665478 custom_diffusion-0.0.7/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-09 22:04:46.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     6684 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py
+-rw-rw-rw-   0        0        0     6759 2023-06-09 22:29:37.000000 custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     8952 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.672478 custom_diffusion-0.0.7/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2242 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1338 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0     1268 2023-06-09 22:29:52.000000 custom_diffusion-0.0.7/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3517 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 22:30:32.660231 custom_diffusion-0.0.7/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     1354 2023-06-09 22:30:31.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-09 22:30:32.000000 custom_diffusion-0.0.7/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-06-09 22:23:40.000000 custom_diffusion-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-09 22:30:32.681480 custom_diffusion-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.0.7/setup.py
```

### Comparing `custom_diffusion-0.0.6/LICENSE` & `custom_diffusion-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/PKG-INFO` & `custom_diffusion-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom_diffusion
-Version: 0.0.6
+Version: 0.0.7
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `custom_diffusion-0.0.6/custom_diffusion/demo.py` & `custom_diffusion-0.0.7/custom_diffusion/demo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from custom_diffusion.pipelines.controlnet_pipeline import StableDiffusionControlNetGenerator
-
-
 def main():
     generator = StableDiffusionControlNetGenerator()
 
 
     generated_image = generator.generate_image(
         stable_model_path="runwayml/stable-diffusion-v1-5",
         controlnet_model_path="lllyasviel/sd-controlnet-scribble",
         scheduler_name="DDIM",
-        image_path="test.png",
+        image_path="data/1.png",
         prompts="anime girl",
         negative_prompt="bad",
         height=512,
         width=512,
         guess_mode=False,
         num_images_per_prompt=1,
         num_inference_steps=10,
         guidance_scale=7.0,
         controlnet_conditioning_scale=1.0,
         generator_seed=0,
         preprocess_type="Canny",
         resize_type="center_crop_and_resize",
+        crop_size=512,
     )
 
     # Save or display your generated image
     # For example, save it as a file
     return generated_image
 
 
 if __name__ == "__main__":
-    main()
+    output = main()
```

### Comparing `custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py` & `custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_inpaint_pipeline.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/custom_diffusion/pipelines/controlnet_pipeline.py` & `custom_diffusion-0.0.7/custom_diffusion/pipelines/controlnet_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from diffusers import ControlNetModel, StableDiffusionControlNetPipeline
 
 from custom_diffusion.preprocces import preprocces_dicts
 from custom_diffusion.utils.data_utils import center_crop_and_resize
 from custom_diffusion.utils.scheduler_utils import get_scheduler
 
 
+from typing import List, Optional
+
+import torch
+from diffusers import ControlNetModel, StableDiffusionControlNetPipeline
+
+
 class StableDiffusionControlNetGenerator:
     """
     A class to handle image generation using stable diffusion and control net models.
     """
 
     def __init__(self):
         self.controlnet = None
@@ -81,15 +87,15 @@
         crop_size (int): The size of the crop.
         height (int): The height of the image to generate.
         width (int): The width of the image to generate.
 
         Returns:
         Image: The resized and loaded PIL Image.
         """
-        image = image.open(image_path)
+        image = Image.open(image_path)
 
         if resize_type == "center_crop_and_resize":
             image = center_crop_and_resize(image, crop_size=crop_size, height=height, width=width)
 
         elif resize_type == "resize":
             image = image.resize((height, width))
 
@@ -120,14 +126,15 @@
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
         guidance_scale: int = 7.0,
         controlnet_conditioning_scale: int = 1.0,
         generator_seed: int = 0,
         preprocess_type: str = "Canny",
         resize_type: str = "center_crop_and_resize",
+        crop_size: int = 512
     ):
         """
         This function generates an image based on the given parameters.
 
         Args:
         stable_model_path (str): Path to the stable model.
         controlnet_model_path (str): Path to the controlnet model.
@@ -145,16 +152,16 @@
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
 
         Returns:
         output: The generated image.
         """
         read_image = self.load_and_resize_image(
-            image_path=image_path, resize_type=resize_type, height=height, width=width
-        )
+            image_path=image_path, resize_type=resize_type, height=height, width=width, crop_size=crop_size)
+        
 
         control_image = preprocces_dicts[preprocess_type](read_image)
 
         pipe = self.load_model(
             stable_model_path=stable_model_path,
             controlnet_model_path=controlnet_model_path,
             scheduler_name=scheduler_name,
@@ -163,15 +170,15 @@
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompts,
             height=height,
             width=width,
             guess_mode=guess_mode,
-            control_image=control_image,
+            image=control_image,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             controlnet_conditioning_scale=float(controlnet_conditioning_scale),
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.0.6/custom_diffusion/preprocces.py` & `custom_diffusion-0.0.7/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.0.7/custom_diffusion/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.0.7/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.0.7/custom_diffusion/utils/scheduler_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     "UniPCMultistep": UniPCMultistepScheduler,
 }
 
 
 def get_scheduler(pipe, scheduler_name):
     if scheduler_name in SCHEDULER_MAPPING:
         SchedulerClass = SCHEDULER_MAPPING[scheduler_name]
-        pipe.scheduler = SchedulerClass.from_config(pipe.scheduler_name.config)
+        pipe.scheduler = SchedulerClass.from_config(pipe.scheduler.config)
     else:
         raise ValueError(f"Invalid scheduler name {scheduler_name}")
 
     return pipe
```

### Comparing `custom_diffusion-0.0.6/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.0.7/custom_diffusion/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.0.7/custom_diffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-diffusion
-Version: 0.0.6
+Version: 0.0.7
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `custom_diffusion-0.0.6/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.0.7/custom_diffusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.0.6/setup.py` & `custom_diffusion-0.0.7/setup.py`

 * *Files identical despite different names*

