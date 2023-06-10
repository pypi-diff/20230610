# Comparing `tmp/nodezator-1.3.8.tar.gz` & `tmp/nodezator-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodezator-1.3.8.tar", last modified: Thu Dec 22 20:14:40 2022, max compression
+gzip compressed data, was "nodezator-1.3.9.tar", last modified: Thu Dec 22 20:54:41 2022, max compression
```

## Comparing `nodezator-1.3.8.tar` & `nodezator-1.3.9.tar`

### file list

```diff
@@ -1,629 +1,629 @@
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.978862 nodezator-1.3.8/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       21 2022-08-24 19:38:58.000000 nodezator-1.3.8/MANIFEST.in
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7806 2022-12-22 20:14:40.978862 nodezator-1.3.8/PKG-INFO
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6137 2022-09-08 21:07:31.000000 nodezator-1.3.8/README.md
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.890863 nodezator-1.3.8/nodezator/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       22 2022-12-22 20:08:20.000000 nodezator-1.3.8/nodezator/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2271 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/__main__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/alphamask/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/alphamask/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12491 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/alphamask/basicop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6319 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/alphamask/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10565 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/alphamask/masksop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6253 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/alphamask/utils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2038 2022-12-22 20:08:20.000000 nodezator-1.3.8/nodezator/appinfo.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8632 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/audioplayer.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/classes2d/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/classes2d/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9925 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/classes2d/collections.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3441 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/classes2d/single.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1317 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/classes2d/surfaceswitcher.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/colorsman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5993 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/color2d.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1018 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/colors.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/colorsman/editor/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/editor/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11667 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/colorsman/editor/loopop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4250 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/colorsman/editor/panel/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/editor/panel/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15271 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/panel/colorsop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       85 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/colorsman/editor/panel/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2448 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/colorsman/editor/panel/data.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16592 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/colorsman/editor/panel/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11464 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetop.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.894863 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14118 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/button.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      521 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3991 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/entry.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4550 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/label.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3623 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/scale.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/colorsman/picker/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/picker/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      102 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/colorsman/picker/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7416 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/picker/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15610 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/colorsman/picker/op.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/colorsman/viewer/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/viewer/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13198 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/viewer/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/colorsman/viewer/modes/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15939 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/colorlist.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8948 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11563 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/particles.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5375 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/waves.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1800 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/config.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/data/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3144 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/app_icon.png
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/data/app_themes/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11480 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/app_themes/emeralds_on_coal.pyl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.878863 nodezator-1.3.8/nodezator/data/aww/
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.898863 nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7832 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/general-controls.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      556 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/index.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2746 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/text-editor-default-behavior.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4310 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/text-editor-vim-like-behavior.htsl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.902863 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1553 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-color-coded-annotations.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11197 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-intfloat-words.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13337 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-configurations.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3824 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-presets.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11441 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-basic-way-define-widgets.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4837 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-color-coding-inputs-outputs.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    25368 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-complex-viewer-nodes.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7863 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-viewer-nodes.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13781 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-your-first-node.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7261 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-distributing-nodes.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10066 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-full-syntax-more-widgets.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7197 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-loading-nodes.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12797 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-more-ways-define-nodes.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8632 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-nodes-variable-parameters-custom-outputs.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7102 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-other-objects.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8501 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-preview-widgets.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12981 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-widget-presets-more-widgets.htsl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.910863 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5079 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11553 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5116 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5980 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img03.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5786 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img04.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5982 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img05.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4987 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img06_and_07.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9102 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img08.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10244 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10264 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7708 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3389 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img03.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3283 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img04.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6001 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img05.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4730 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-viewer-nodes_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5147 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6403 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6553 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9158 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9199 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5699 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6688 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7942 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img03.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18748 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16216 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12547 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21575 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img03.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    45056 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img04.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7141 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img05.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21107 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img06.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6095 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9153 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_0.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15559 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_1.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7801 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12137 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_0.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    52214 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_1.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18691 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_0.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    56790 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_1.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20459 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_0.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    31971 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_1.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11141 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img00.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13894 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img01.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6427 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img02.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7317 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img03.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10589 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img04.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10838 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img05.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8254 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/index.htsl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.910863 nodezator-1.3.8/nodezator/data/aww/nodezator.pysite/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      845 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/nodezator.pysite/about.htsl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2397 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/aww/nodezator.pysite/license.htsl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.918863 nodezator-1.3.8/nodezator/data/fonts/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4696 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/OFL_license_for_all_other_fonts.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7048 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/cc0_license_for_nodezator_icons.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)  1956592 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/enc_sans_sexp_bold_mplus_1p_2000em_med.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)  1810280 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/fira_mono_bold_mplus_1m_med.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22000 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/nodezator_icons.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   557380 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/noto_sans_bold.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   403724 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/noto_sans_italic.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   353368 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/noto_sans_mono_medium.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   556216 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/fonts/noto_sans_regular.ttf
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20578 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/glossary.rst
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.918863 nodezator-1.3.8/nodezator/data/images/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      256 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/README.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19148 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/colors_editor_scale_images.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4480 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/discord_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11684 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/github_mark.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1364 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/indie_python_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1041 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/kennedy_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1207 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/mask_wave.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8085 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/patreon_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1969 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/pygame_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1054 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/python_filemanager_icon.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1260 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/python_menu_icon.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1248 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/python_splashscreen_icon.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24666 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/splash_nodezator_robot.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5510 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/twitter_logo.png
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1408 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/images/unlicense_logo.png
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.878863 nodezator-1.3.8/nodezator/data/locale/
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.918863 nodezator-1.3.8/nodezator/data/locale/en_us/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2618 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/locale/en_us/dialogs_map.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        4 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/locale/en_us/status_messages_map.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6918 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/data/locale/en_us/translations_map.pyl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/data/locale/pt_br/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4030 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/locale/pt_br/dialogs_map.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        4 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/locale/pt_br/status_messages_map.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1818 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/locale/pt_br/translations_map.pyl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.878863 nodezator-1.3.8/nodezator/data/syntax_themes/
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/data/syntax_themes/comment/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      225 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/comment/fresh_eucalyptus_dark.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      224 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/comment/pale_green.pyl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/data/syntax_themes/python/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1174 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/python/ice_with_candy.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1174 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/python/sprinkled_dark.pyl
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/data/syntax_themes/user_log/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      387 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/user_log/message_temperature.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      384 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/data/syntax_themes/user_log/message_temperature_dark.pyl
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17837 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/dialog.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/editing/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14096 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/categorycolors.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11812 2022-09-23 14:16:35.000000 nodezator-1.3.8/nodezator/editing/data.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/editing/export/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/export/__init__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/editing/export/form/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/export/form/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20189 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/export/form/image.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14577 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/export/form/python.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16297 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/export/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5883 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/gridlogic.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3287 2022-09-23 14:16:35.000000 nodezator-1.3.8/nodezator/editing/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.922863 nodezator-1.3.8/nodezator/editing/nodepacksforms/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-23 14:16:35.000000 nodezator-1.3.8/nodezator/editing/nodepacksforms/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16357 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/nodepacksforms/renaming.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26077 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/nodepacksforms/selection.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16146 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objinsert.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/editing/objpopups/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/objpopups/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3390 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objpopups/callablenode.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3329 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objpopups/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4991 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objpopups/operatornode.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2490 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objpopups/proxynode.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2042 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/objpopups/textblock.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10506 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/reposition.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12270 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/selection.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/editing/socketpopups/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/socketpopups/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1672 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/socketpopups/input.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      749 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/socketpopups/output.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      707 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/editing/socketpopups/proxy.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/editing/widgetpicker/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/widgetpicker/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16086 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/widgetpicker/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    50492 2022-10-22 19:59:07.000000 nodezator-1.3.8/nodezator/editing/widgetpicker/subforms.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/editing/widgetpopups/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/editing/widgetpopups/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2025 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/editing/widgetpopups/creation.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/fileman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fileman/__init__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.926863 nodezator-1.3.8/nodezator/fileman/bookmarkpanel/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fileman/bookmarkpanel/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14909 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/bookmarkpanel/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      696 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/bookmarkpanel/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      619 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/constants.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.930863 nodezator-1.3.8/nodezator/fileman/dirpanel/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12740 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/extraop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5667 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/loadop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15697 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7326 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/mouseop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11856 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/newpathform.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2182 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/dirpanel/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14205 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/fileman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12623 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/fileman/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9180 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/pathobj.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2402 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fileman/surfs.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.930863 nodezator-1.3.8/nodezator/fontsman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fontsman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6528 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/cache.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      854 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      532 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/exception.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.930863 nodezator-1.3.8/nodezator/fontsman/preview/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fontsman/preview/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3526 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/preview/cache.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2147 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/preview/render.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.930863 nodezator-1.3.8/nodezator/fontsman/viewer/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/fontsman/viewer/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5236 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/fontsman/viewer/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1016 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/fontsman/viewer/render.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.934863 nodezator-1.3.8/nodezator/graphman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/__init__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.934863 nodezator-1.3.8/nodezator/graphman/builtinnode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/builtinnode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13470 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/builtinnode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      554 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/builtinnode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4122 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/builtinnode/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.934863 nodezator-1.3.8/nodezator/graphman/callablenode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1421 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18691 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/execution.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18190 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5242 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12859 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/callablenode/preproc.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.934863 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19349 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12497 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/segment.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7124 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/unpacking.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    23782 2022-10-04 15:21:24.000000 nodezator-1.3.8/nodezator/graphman/callablenode/subparam/widget.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7236 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1201 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.934863 nodezator-1.3.8/nodezator/graphman/callablenode/vizop/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizop/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5598 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizop/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10129 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizop/reposition.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.938863 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/__init__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.938863 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12013 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/creation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7144 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17009 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5854 2022-09-15 21:35:55.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/param.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14966 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/varparam.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.938863 nodezator-1.3.8/nodezator/graphman/capsulenode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/capsulenode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11117 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/capsulenode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      554 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/capsulenode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4376 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/capsulenode/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3130 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/editlogic.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10301 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/exception.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15462 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/execution.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7706 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5921 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/nodepacksissues.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.938863 nodezator-1.3.8/nodezator/graphman/operatornode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/operatornode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3959 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6289 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/execution.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6009 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2655 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5785 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4513 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/vizop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4459 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/operatornode/vizprep.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4622 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/presets.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/proxynode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/proxynode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      469 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5278 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2170 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3712 2022-11-03 14:48:11.000000 nodezator-1.3.8/nodezator/graphman/proxynode/segment.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2865 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1060 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/titleupdate.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      777 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/proxynode/vizop/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/proxynode/vizop/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4574 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/vizop/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1065 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/vizop/reposition.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8707 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/vizprep.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5220 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/proxynode/widget.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    29139 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/pythonrepr.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19244 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/graphman/scriptloading.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/socket/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/socket/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      570 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socket/base.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6039 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/graphman/socket/input.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4007 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socket/output.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1619 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socket/placeholder.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3918 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socket/proxy.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5186 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socket/surfs.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/socketparenthood/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5525 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/action.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2539 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/draw.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1638 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6034 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17705 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/support.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8426 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/socketparenthood/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/stlibnode/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/stlibnode/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10264 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/stlibnode/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      563 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/stlibnode/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4275 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/stlibnode/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.942863 nodezator-1.3.8/nodezator/graphman/textblock/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/textblock/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1046 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/textblock/check.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      265 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/textblock/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3335 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/textblock/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4138 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/textblock/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3533 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/textblock/surf.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11027 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/graphman/validation/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-09-05 21:27:33.000000 nodezator-1.3.8/nodezator/graphman/validation/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2798 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/validation/fixtures.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2686 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/validation/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5479 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/graphman/validation/tests.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/graphman/widget/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/graphman/widget/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2162 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/widget/export.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17777 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/graphman/widget/utils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5177 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/hideswitch.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/htsl/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/htsl/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6267 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/htsl/codeblock.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2815 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/htsl/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24519 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/htsl/creation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1055 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/htsl/image.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13719 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/htsl/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4455 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/htsl/prep.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/imagesman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/imagesman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5991 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/imagesman/cache.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5601 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/imagesman/render.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/imagesman/viewer/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/imagesman/viewer/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3799 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/imagesman/viewer/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7510 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/imagesman/viewer/fullop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4635 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/imagesman/viewer/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6063 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/imagesman/viewer/normalop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2080 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/knownpacks.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.946863 nodezator-1.3.8/nodezator/logman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/logman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7899 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/logman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1641 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/logman/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.950863 nodezator-1.3.8/nodezator/loopman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/loopman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1283 2022-12-22 20:08:20.000000 nodezator-1.3.8/nodezator/loopman/exception.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2115 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/loopman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5938 2022-12-22 19:20:13.000000 nodezator-1.3.8/nodezator/mainloop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3119 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/memoryman.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.950863 nodezator-1.3.8/nodezator/menu/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/menu/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21371 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/menu/behaviour.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5014 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/command.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6995 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/common.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14960 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/hover.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10847 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/iconfactory.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19975 2022-12-22 16:23:55.000000 nodezator-1.3.8/nodezator/menu/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    25187 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/scroll.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.950863 nodezator-1.3.8/nodezator/menu/submenu/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/menu/submenu/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20284 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/submenu/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19837 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/submenu/scroll.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1826 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/submenu/utils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7955 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/menu/surffactory.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.950863 nodezator-1.3.8/nodezator/our3rdlibs/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/our3rdlibs/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3975 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/our3rdlibs/behaviour.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6245 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/our3rdlibs/button.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2762 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/our3rdlibs/debug.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.950863 nodezator-1.3.8/nodezator/our3rdlibs/grid/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/our3rdlibs/grid/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9639 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/grid/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3155 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/grid/oop.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.954862 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6489 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/list.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15718 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      130 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/set.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1537 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/surfs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      369 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/keyconst.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5849 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/our3rdlibs/scale.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.954862 nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14848 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16631 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/modes.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4668 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/our3rdlibs/userlogger.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.954862 nodezator-1.3.8/nodezator/ourstdlibs/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/ourstdlibs/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17477 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/behaviour.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.954862 nodezator-1.3.8/nodezator/ourstdlibs/collections/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/__init__.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.954862 nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16768 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26710 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/tests.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1830 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/general.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      872 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/collections/nestedfromdict.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.958862 nodezator-1.3.8/nodezator/ourstdlibs/color/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      785 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5750 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/conversion.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7428 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/creation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16775 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/custom.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26080 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/largemaps.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1128 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/property.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8885 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/color/utils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1965 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/debug.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2911 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/dictutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11337 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/exceptionutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      852 2022-10-04 14:37:14.000000 nodezator-1.3.8/nodezator/ourstdlibs/importutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5734 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/iterutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8738 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/mathutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2550 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/meta.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9205 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/ourstdlibs/path.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6927 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/profileutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1040 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/pyl.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1916 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/stringutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5013 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/timeutils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5173 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/ourstdlibs/treeutils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.958862 nodezator-1.3.8/nodezator/pointsman2d/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/pointsman2d/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      288 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/pointsman2d/create.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1685 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/pointsman2d/shape.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      465 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/pointsman2d/transform.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1672 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/pygameconstants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2350 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/recentfile.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.958862 nodezator-1.3.8/nodezator/rectsman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-09-05 21:27:33.000000 nodezator-1.3.8/nodezator/rectsman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1789 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/cluster.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1525 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/constants.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.962862 nodezator-1.3.8/nodezator/rectsman/doctests/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-08-24 19:38:58.000000 nodezator-1.3.8/nodezator/rectsman/doctests/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4028 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/doctests/fixtures.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16742 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test01_intro.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10879 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test02_01_operations.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14691 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test02_02_operations.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13141 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test02_03_operations.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11629 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test03_01_specialmethods.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12102 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test03_02_specialmethods.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17978 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test04_01_other.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20310 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test04_02_other.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3589 2022-09-09 18:44:59.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test04_03_other.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6374 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/doctests/test05_align.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12120 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9677 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/singlepos.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11624 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/sizepos.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9048 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/spatial.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4336 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/special.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      498 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/rectsman/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.962862 nodezator-1.3.8/nodezator/splashscreen/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/splashscreen/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4439 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/splashscreen/animsetup.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      967 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/splashscreen/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16129 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/splashscreen/factoryfuncs.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15358 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/splashscreen/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8278 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/splashscreen/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9277 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/surfdef.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.962862 nodezator-1.3.8/nodezator/surfsman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/surfsman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1775 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/surfsman/cache.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15422 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/surfsman/draw.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10053 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/surfsman/icon.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6001 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/surfsman/render.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.962862 nodezator-1.3.8/nodezator/syntaxman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/syntaxman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      608 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/exception.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.962862 nodezator-1.3.8/nodezator/syntaxman/syntaxes/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9668 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/comment.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13140 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2117 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/namemap.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11562 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/utils.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6524 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/syntaxes/userlog.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6669 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/syntaxman/utils.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/textman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10561 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/cache.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/textman/editor/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/editor/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2025 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/constants.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/textman/editor/cursor/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9413 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/textman/editor/cursor/modes/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/modes/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19679 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/modes/insert.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9147 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/modes/normal.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12778 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/navigation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11165 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11762 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/cursor/syntaxhigh.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6756 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/editor/line.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18726 2022-10-22 21:00:36.000000 nodezator-1.3.8/nodezator/textman/editor/main.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.966863 nodezator-1.3.8/nodezator/textman/entryedition/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/entryedition/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12763 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/entryedition/cursor.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4100 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/entryedition/line.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.970862 nodezator-1.3.8/nodezator/textman/label/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/label/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1845 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/label/autolabel.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11522 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/label/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13390 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/render.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6140 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/text.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.970862 nodezator-1.3.8/nodezator/textman/viewer/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/textman/viewer/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1100 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/viewer/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7725 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/viewer/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13402 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/textman/viewer/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14587 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/textman/viewer/prep.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1969 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/translation.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.970862 nodezator-1.3.8/nodezator/userprefsman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/userprefsman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12746 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/userprefsman/editionform.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2818 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/userprefsman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1033 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/userprefsman/validation.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.970862 nodezator-1.3.8/nodezator/videopreview/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/videopreview/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6601 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/videopreview/cache.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      975 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/videopreview/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5807 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/videopreview/previewer.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2492 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/videopreview/render.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.970862 nodezator-1.3.8/nodezator/widget/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/widget/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7892 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/checkbutton.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22100 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/colorbutton.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6803 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/defaultholder.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.974862 nodezator-1.3.8/nodezator/widget/intfloatentry/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/widget/intfloatentry/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19886 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/intfloatentry/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17692 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/intfloatentry/modes.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9181 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/intfloatentry/numeval.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18300 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/intfloatentry/op.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22522 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/literaldisplay.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17715 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/literalentry.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.974862 nodezator-1.3.8/nodezator/widget/optionmenu/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/widget/optionmenu/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10672 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/optionmenu/creation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19862 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/optionmenu/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15939 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/optionmenu/op.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.974862 nodezator-1.3.8/nodezator/widget/optiontray/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/widget/optiontray/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6688 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/optiontray/creation.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16540 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/optiontray/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6398 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/optiontray/op.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.974862 nodezator-1.3.8/nodezator/widget/pathpreview/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/widget/pathpreview/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1841 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/audio.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14962 2022-12-17 14:28:27.000000 nodezator-1.3.8/nodezator/widget/pathpreview/base.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6232 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/constants.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8390 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/font.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9316 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/image.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      785 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/path.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20620 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/text.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8728 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/pathpreview/video.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12094 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/widget/sortingbutton.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24025 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/stringentry.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    30951 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/widget/textdisplay.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.974862 nodezator-1.3.8/nodezator/winman/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/winman/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22666 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/fileop.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2727 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/label.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17001 2022-12-22 16:19:30.000000 nodezator-1.3.8/nodezator/winman/main.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21031 2022-12-22 16:23:00.000000 nodezator-1.3.8/nodezator/winman/menu.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.978862 nodezator-1.3.8/nodezator/winman/states/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.8/nodezator/winman/states/__init__.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2835 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/boxselection.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17622 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/loadedfile.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4312 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/movingobject.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2726 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/nofile.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3621 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/segmentdef.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1789 2022-12-22 20:10:40.000000 nodezator-1.3.8/nodezator/winman/states/segmentsev.py
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1622 2022-09-10 14:45:30.000000 nodezator-1.3.8/nodezator/winman/switch.py
-drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:14:40.890863 nodezator-1.3.8/nodezator.egg-info/
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7806 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/PKG-INFO
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22780 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/SOURCES.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        1 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/dependency_links.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       73 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/entry_points.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       13 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/requires.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       10 2022-12-22 20:14:40.000000 nodezator-1.3.8/nodezator.egg-info/top_level.txt
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       94 2022-08-24 19:38:58.000000 nodezator-1.3.8/pyproject.toml
--rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1709 2022-12-22 20:14:40.978862 nodezator-1.3.8/setup.cfg
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.349899 nodezator-1.3.9/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       21 2022-08-24 19:38:58.000000 nodezator-1.3.9/MANIFEST.in
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7806 2022-12-22 20:54:41.349899 nodezator-1.3.9/PKG-INFO
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6137 2022-09-08 21:07:31.000000 nodezator-1.3.9/README.md
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       22 2022-12-22 20:52:58.000000 nodezator-1.3.9/nodezator/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2271 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/__main__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator/alphamask/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/alphamask/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12491 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/alphamask/basicop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6319 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/alphamask/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10565 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/alphamask/masksop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6253 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/alphamask/utils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2038 2022-12-22 20:52:58.000000 nodezator-1.3.9/nodezator/appinfo.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8632 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/audioplayer.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator/classes2d/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/classes2d/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9925 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/classes2d/collections.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3441 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/classes2d/single.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1317 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/classes2d/surfaceswitcher.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator/colorsman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5993 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/color2d.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1018 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/colors.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator/colorsman/editor/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/editor/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11667 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/colorsman/editor/loopop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4250 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/editor/panel/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/editor/panel/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15271 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/panel/colorsop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       85 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/colorsman/editor/panel/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2448 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/colorsman/editor/panel/data.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16592 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/colorsman/editor/panel/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11464 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetop.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14118 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/button.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      521 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3991 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/entry.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4550 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/label.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3623 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/scale.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/picker/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/picker/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      102 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/colorsman/picker/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7416 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/picker/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15610 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/colorsman/picker/op.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/viewer/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/viewer/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13198 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/viewer/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/viewer/modes/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15939 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/colorlist.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8948 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11563 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/particles.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5375 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/waves.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1800 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/config.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/data/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3144 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/app_icon.png
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.257898 nodezator-1.3.9/nodezator/data/app_themes/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11480 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/app_themes/emeralds_on_coal.pyl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.241898 nodezator-1.3.9/nodezator/data/aww/
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.261899 nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7832 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/general-controls.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      556 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/index.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2746 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/text-editor-default-behavior.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4310 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/text-editor-vim-like-behavior.htsl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.265899 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1553 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-color-coded-annotations.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11197 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-intfloat-words.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13337 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-configurations.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3824 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-presets.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11441 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-basic-way-define-widgets.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4837 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-color-coding-inputs-outputs.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    25368 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-complex-viewer-nodes.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7863 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-viewer-nodes.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13781 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-your-first-node.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7261 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-distributing-nodes.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10066 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-full-syntax-more-widgets.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7197 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-loading-nodes.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12797 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-more-ways-define-nodes.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8632 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-nodes-variable-parameters-custom-outputs.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7102 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-other-objects.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8501 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-preview-widgets.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12981 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-widget-presets-more-widgets.htsl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.277898 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5079 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11553 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5116 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5980 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img03.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5786 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img04.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5982 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img05.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4987 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img06_and_07.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9102 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img08.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10244 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10264 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7708 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3389 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img03.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3283 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img04.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6001 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img05.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4730 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-viewer-nodes_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5147 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6403 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6553 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9158 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9199 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5699 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6688 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7942 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img03.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18748 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16216 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12547 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21575 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img03.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    45056 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img04.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7141 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img05.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21107 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img06.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6095 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9153 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_0.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15559 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_1.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7801 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12137 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_0.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    52214 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_1.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18691 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_0.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    56790 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_1.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20459 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_0.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    31971 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_1.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11141 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img00.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13894 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img01.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6427 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img02.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7317 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img03.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10589 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img04.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10838 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img05.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8254 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/index.htsl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.277898 nodezator-1.3.9/nodezator/data/aww/nodezator.pysite/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      845 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/nodezator.pysite/about.htsl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2397 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/aww/nodezator.pysite/license.htsl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.285899 nodezator-1.3.9/nodezator/data/fonts/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4696 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/OFL_license_for_all_other_fonts.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7048 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/cc0_license_for_nodezator_icons.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)  1956592 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/enc_sans_sexp_bold_mplus_1p_2000em_med.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)  1810280 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/fira_mono_bold_mplus_1m_med.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22000 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/nodezator_icons.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   557380 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/noto_sans_bold.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   403724 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/noto_sans_italic.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   353368 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/noto_sans_mono_medium.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)   556216 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/fonts/noto_sans_regular.ttf
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20578 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/glossary.rst
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.289898 nodezator-1.3.9/nodezator/data/images/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      256 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/README.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19148 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/colors_editor_scale_images.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4480 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/discord_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11684 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/github_mark.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1364 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/indie_python_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1041 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/kennedy_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1207 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/mask_wave.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8085 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/patreon_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1969 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/pygame_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1054 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/python_filemanager_icon.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1260 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/python_menu_icon.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1248 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/python_splashscreen_icon.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24666 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/splash_nodezator_robot.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5510 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/twitter_logo.png
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1408 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/images/unlicense_logo.png
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.241898 nodezator-1.3.9/nodezator/data/locale/
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.289898 nodezator-1.3.9/nodezator/data/locale/en_us/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2618 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/locale/en_us/dialogs_map.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        4 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/locale/en_us/status_messages_map.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6918 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/data/locale/en_us/translations_map.pyl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.289898 nodezator-1.3.9/nodezator/data/locale/pt_br/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4030 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/locale/pt_br/dialogs_map.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        4 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/locale/pt_br/status_messages_map.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1818 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/locale/pt_br/translations_map.pyl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.241898 nodezator-1.3.9/nodezator/data/syntax_themes/
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.289898 nodezator-1.3.9/nodezator/data/syntax_themes/comment/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      225 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/comment/fresh_eucalyptus_dark.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      224 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/comment/pale_green.pyl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/data/syntax_themes/python/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1174 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/python/ice_with_candy.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1174 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/python/sprinkled_dark.pyl
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/data/syntax_themes/user_log/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      387 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/user_log/message_temperature.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      384 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/data/syntax_themes/user_log/message_temperature_dark.pyl
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17837 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/dialog.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/editing/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14096 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/categorycolors.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11812 2022-09-23 14:16:35.000000 nodezator-1.3.9/nodezator/editing/data.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/editing/export/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/export/__init__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/editing/export/form/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/export/form/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20189 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/export/form/image.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14577 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/export/form/python.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16297 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/export/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5883 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/gridlogic.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3287 2022-09-23 14:16:35.000000 nodezator-1.3.9/nodezator/editing/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.293898 nodezator-1.3.9/nodezator/editing/nodepacksforms/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-23 14:16:35.000000 nodezator-1.3.9/nodezator/editing/nodepacksforms/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16357 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/nodepacksforms/renaming.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26077 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/nodepacksforms/selection.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16146 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objinsert.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/editing/objpopups/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/objpopups/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3390 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objpopups/callablenode.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3329 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objpopups/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4991 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objpopups/operatornode.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2490 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objpopups/proxynode.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2042 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/objpopups/textblock.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10506 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/reposition.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12270 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/selection.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/editing/socketpopups/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/socketpopups/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1672 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/socketpopups/input.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      749 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/socketpopups/output.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      707 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/editing/socketpopups/proxy.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/editing/widgetpicker/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/widgetpicker/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16086 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/widgetpicker/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    50492 2022-10-22 19:59:07.000000 nodezator-1.3.9/nodezator/editing/widgetpicker/subforms.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/editing/widgetpopups/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/editing/widgetpopups/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2025 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/editing/widgetpopups/creation.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/fileman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fileman/__init__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.297899 nodezator-1.3.9/nodezator/fileman/bookmarkpanel/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fileman/bookmarkpanel/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14909 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/bookmarkpanel/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      696 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/bookmarkpanel/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      619 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/constants.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/fileman/dirpanel/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12740 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/extraop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5667 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/loadop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15697 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7326 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/mouseop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11856 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/newpathform.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2182 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/dirpanel/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14205 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/fileman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12623 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/fileman/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9180 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/pathobj.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2402 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fileman/surfs.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/fontsman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fontsman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6528 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/cache.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      854 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      532 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/exception.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/fontsman/preview/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fontsman/preview/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3526 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/preview/cache.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2147 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/preview/render.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/fontsman/viewer/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/fontsman/viewer/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5236 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/fontsman/viewer/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1016 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/fontsman/viewer/render.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/graphman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/__init__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.301899 nodezator-1.3.9/nodezator/graphman/builtinnode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/builtinnode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13470 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/builtinnode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      554 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/builtinnode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4122 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/builtinnode/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/callablenode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1421 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18691 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/execution.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18190 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5242 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12859 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/callablenode/preproc.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19349 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12497 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/segment.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7124 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/unpacking.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    23782 2022-10-04 15:21:24.000000 nodezator-1.3.9/nodezator/graphman/callablenode/subparam/widget.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7236 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1201 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/callablenode/vizop/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizop/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5598 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizop/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10129 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizop/reposition.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/__init__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12013 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/creation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7144 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17009 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5854 2022-09-15 21:35:55.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/param.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14966 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/varparam.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.305899 nodezator-1.3.9/nodezator/graphman/capsulenode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/capsulenode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11117 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/capsulenode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      554 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/capsulenode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4376 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/capsulenode/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3130 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/editlogic.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10301 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/exception.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15462 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/execution.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7706 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5921 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/nodepacksissues.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.309898 nodezator-1.3.9/nodezator/graphman/operatornode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/operatornode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3959 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6289 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/execution.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6009 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2655 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5785 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4513 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/vizop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4459 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/operatornode/vizprep.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4622 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/presets.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.309898 nodezator-1.3.9/nodezator/graphman/proxynode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/proxynode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      469 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5278 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2170 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3712 2022-11-03 14:48:11.000000 nodezator-1.3.9/nodezator/graphman/proxynode/segment.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2865 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1060 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/titleupdate.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      777 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.309898 nodezator-1.3.9/nodezator/graphman/proxynode/vizop/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/proxynode/vizop/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4574 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/vizop/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1065 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/vizop/reposition.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8707 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/vizprep.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5220 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/proxynode/widget.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    29139 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/pythonrepr.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19244 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/graphman/scriptloading.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.309898 nodezator-1.3.9/nodezator/graphman/socket/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/socket/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      570 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socket/base.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6039 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/graphman/socket/input.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4007 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socket/output.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1619 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socket/placeholder.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3918 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socket/proxy.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5186 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socket/surfs.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.313899 nodezator-1.3.9/nodezator/graphman/socketparenthood/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5525 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/action.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2539 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/draw.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1638 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6034 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17705 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/support.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8426 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/socketparenthood/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.313899 nodezator-1.3.9/nodezator/graphman/stlibnode/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/stlibnode/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10264 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/stlibnode/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      563 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/stlibnode/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4275 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/stlibnode/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.313899 nodezator-1.3.9/nodezator/graphman/textblock/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/textblock/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1046 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/textblock/check.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      265 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/textblock/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3335 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/textblock/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4138 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/textblock/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3533 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/textblock/surf.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11027 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.313899 nodezator-1.3.9/nodezator/graphman/validation/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-09-05 21:27:33.000000 nodezator-1.3.9/nodezator/graphman/validation/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2798 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/validation/fixtures.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2686 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/validation/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5479 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/graphman/validation/tests.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/graphman/widget/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/graphman/widget/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2162 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/widget/export.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17777 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/graphman/widget/utils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5177 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/hideswitch.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/htsl/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/htsl/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6267 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/htsl/codeblock.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2815 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/htsl/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24519 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/htsl/creation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1055 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/htsl/image.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13719 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/htsl/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4455 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/htsl/prep.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/imagesman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/imagesman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5991 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/imagesman/cache.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5601 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/imagesman/render.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/imagesman/viewer/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/imagesman/viewer/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3799 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/imagesman/viewer/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7510 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/imagesman/viewer/fullop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4635 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/imagesman/viewer/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6063 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/imagesman/viewer/normalop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2080 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/knownpacks.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/logman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/logman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7899 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/logman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1641 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/logman/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.317899 nodezator-1.3.9/nodezator/loopman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/loopman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1283 2022-12-22 20:08:20.000000 nodezator-1.3.9/nodezator/loopman/exception.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2115 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/loopman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5938 2022-12-22 19:20:13.000000 nodezator-1.3.9/nodezator/mainloop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3119 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/memoryman.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.321899 nodezator-1.3.9/nodezator/menu/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/menu/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21371 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/menu/behaviour.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5014 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/command.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6995 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/common.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14960 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/hover.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10847 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/iconfactory.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19975 2022-12-22 16:23:55.000000 nodezator-1.3.9/nodezator/menu/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    25187 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/scroll.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.321899 nodezator-1.3.9/nodezator/menu/submenu/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/menu/submenu/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20284 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/submenu/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19837 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/submenu/scroll.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1826 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/submenu/utils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7955 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/menu/surffactory.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.321899 nodezator-1.3.9/nodezator/our3rdlibs/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/our3rdlibs/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3975 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/our3rdlibs/behaviour.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6245 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/our3rdlibs/button.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2762 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/our3rdlibs/debug.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.321899 nodezator-1.3.9/nodezator/our3rdlibs/grid/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/our3rdlibs/grid/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9639 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/grid/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3155 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/grid/oop.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.321899 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6489 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/list.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15718 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      130 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/set.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1537 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/surfs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      369 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/keyconst.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5849 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/our3rdlibs/scale.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.325899 nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14848 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16631 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/modes.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4668 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/our3rdlibs/userlogger.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.325899 nodezator-1.3.9/nodezator/ourstdlibs/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/ourstdlibs/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17477 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/behaviour.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.325899 nodezator-1.3.9/nodezator/ourstdlibs/collections/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/__init__.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.329898 nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16768 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26710 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/tests.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1830 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/general.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      872 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/collections/nestedfromdict.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.329898 nodezator-1.3.9/nodezator/ourstdlibs/color/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      785 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5750 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/conversion.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7428 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/creation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16775 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/custom.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    26080 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/largemaps.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1128 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/property.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8885 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/color/utils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1965 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/debug.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2911 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/dictutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11337 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/exceptionutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      852 2022-10-04 14:37:14.000000 nodezator-1.3.9/nodezator/ourstdlibs/importutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5734 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/iterutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8738 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/mathutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2550 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/meta.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9205 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/ourstdlibs/path.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6927 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/profileutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1040 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/pyl.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1916 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/stringutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5013 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/timeutils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5173 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/ourstdlibs/treeutils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.329898 nodezator-1.3.9/nodezator/pointsman2d/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/pointsman2d/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      288 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/pointsman2d/create.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1685 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/pointsman2d/shape.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      465 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/pointsman2d/transform.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1672 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/pygameconstants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2350 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/recentfile.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.329898 nodezator-1.3.9/nodezator/rectsman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-09-05 21:27:33.000000 nodezator-1.3.9/nodezator/rectsman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1789 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/cluster.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1525 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/constants.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.333899 nodezator-1.3.9/nodezator/rectsman/doctests/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      326 2022-08-24 19:38:58.000000 nodezator-1.3.9/nodezator/rectsman/doctests/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4028 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/doctests/fixtures.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16742 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test01_intro.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10879 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test02_01_operations.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14691 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test02_02_operations.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13141 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test02_03_operations.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11629 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test03_01_specialmethods.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12102 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test03_02_specialmethods.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17978 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test04_01_other.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20310 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test04_02_other.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3589 2022-09-09 18:44:59.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test04_03_other.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6374 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/doctests/test05_align.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12120 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9677 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/singlepos.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11624 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/sizepos.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9048 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/spatial.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4336 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/special.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      498 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/rectsman/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.333899 nodezator-1.3.9/nodezator/splashscreen/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/splashscreen/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4439 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/splashscreen/animsetup.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      967 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/splashscreen/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16129 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/splashscreen/factoryfuncs.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15358 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/splashscreen/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8278 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/splashscreen/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9277 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/surfdef.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.333899 nodezator-1.3.9/nodezator/surfsman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/surfsman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1775 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/surfsman/cache.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15422 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/surfsman/draw.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10053 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/surfsman/icon.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6001 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/surfsman/render.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.333899 nodezator-1.3.9/nodezator/syntaxman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/syntaxman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      608 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/exception.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/syntaxman/syntaxes/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9668 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/comment.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13140 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2117 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/namemap.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11562 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/utils.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6524 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/syntaxes/userlog.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6669 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/syntaxman/utils.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/textman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10561 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/cache.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/textman/editor/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/editor/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2025 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/constants.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/textman/editor/cursor/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9413 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/textman/editor/cursor/modes/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/modes/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19679 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/modes/insert.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9147 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/modes/normal.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12778 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/navigation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11165 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11762 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/cursor/syntaxhigh.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6756 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/editor/line.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18726 2022-10-22 21:00:36.000000 nodezator-1.3.9/nodezator/textman/editor/main.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.337899 nodezator-1.3.9/nodezator/textman/entryedition/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/entryedition/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12763 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/entryedition/cursor.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4100 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/entryedition/line.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.341899 nodezator-1.3.9/nodezator/textman/label/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/label/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1845 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/label/autolabel.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    11522 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/label/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13390 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/render.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6140 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/text.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.341899 nodezator-1.3.9/nodezator/textman/viewer/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/textman/viewer/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1100 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/viewer/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7725 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/viewer/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    13402 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/textman/viewer/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14587 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/textman/viewer/prep.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1969 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/translation.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.341899 nodezator-1.3.9/nodezator/userprefsman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/userprefsman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12746 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/userprefsman/editionform.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2818 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/userprefsman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1033 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/userprefsman/validation.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.341899 nodezator-1.3.9/nodezator/videopreview/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/videopreview/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6601 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/videopreview/cache.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      975 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/videopreview/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     5807 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/videopreview/previewer.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2492 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/videopreview/render.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.341899 nodezator-1.3.9/nodezator/widget/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/widget/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7892 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/checkbutton.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22100 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/colorbutton.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6803 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/defaultholder.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.345898 nodezator-1.3.9/nodezator/widget/intfloatentry/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/widget/intfloatentry/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19886 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/intfloatentry/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17692 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/intfloatentry/modes.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9181 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/intfloatentry/numeval.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    18300 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/intfloatentry/op.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22522 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/literaldisplay.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17715 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/literalentry.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.345898 nodezator-1.3.9/nodezator/widget/optionmenu/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/widget/optionmenu/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    10672 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/optionmenu/creation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    19862 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/optionmenu/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    15939 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/optionmenu/op.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.345898 nodezator-1.3.9/nodezator/widget/optiontray/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/widget/optiontray/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6688 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/optiontray/creation.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    16540 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/optiontray/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6398 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/optiontray/op.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.345898 nodezator-1.3.9/nodezator/widget/pathpreview/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/widget/pathpreview/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1841 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/audio.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    14962 2022-12-17 14:28:27.000000 nodezator-1.3.9/nodezator/widget/pathpreview/base.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     6232 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/constants.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8390 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/font.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     9316 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/image.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)      785 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/path.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    20620 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/text.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     8728 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/pathpreview/video.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    12094 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/widget/sortingbutton.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    24025 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/stringentry.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    30951 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/widget/textdisplay.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.345898 nodezator-1.3.9/nodezator/winman/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/winman/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    23077 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/fileop.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2727 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/label.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17001 2022-12-22 16:19:30.000000 nodezator-1.3.9/nodezator/winman/main.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    21031 2022-12-22 16:23:00.000000 nodezator-1.3.9/nodezator/winman/menu.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.349899 nodezator-1.3.9/nodezator/winman/states/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        0 2022-09-06 14:02:32.000000 nodezator-1.3.9/nodezator/winman/states/__init__.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2835 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/boxselection.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    17622 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/loadedfile.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     4312 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/movingobject.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     2726 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/nofile.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     3621 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/segmentdef.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1789 2022-12-22 20:53:31.000000 nodezator-1.3.9/nodezator/winman/states/segmentsev.py
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1622 2022-09-10 14:45:30.000000 nodezator-1.3.9/nodezator/winman/switch.py
+drwxrwxr-x   0 kennedy   (1000) kennedy   (1000)        0 2022-12-22 20:54:41.253898 nodezator-1.3.9/nodezator.egg-info/
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     7806 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/PKG-INFO
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)    22780 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/SOURCES.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)        1 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/dependency_links.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       73 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/entry_points.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       13 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/requires.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       10 2022-12-22 20:54:41.000000 nodezator-1.3.9/nodezator.egg-info/top_level.txt
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)       94 2022-08-24 19:38:58.000000 nodezator-1.3.9/pyproject.toml
+-rw-rw-r--   0 kennedy   (1000) kennedy   (1000)     1709 2022-12-22 20:54:41.349899 nodezator-1.3.9/setup.cfg
```

### Comparing `nodezator-1.3.8/PKG-INFO` & `nodezator-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodezator
-Version: 1.3.8
+Version: 1.3.9
 Summary: A multi-purpose visual node editor for the Python programming language
 Home-page: https://nodezator.com
 Author: Kennedy Richard
 Author-email: kennedy@kennedyrichard.com
 License: Unlicense
 Project-URL: Source code, https://github.com/IndiePython/nodezator
 Project-URL: Forum, https://github.com/IndiePython/nodezator/discussions
```

### Comparing `nodezator-1.3.8/README.md` & `nodezator-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/__main__.py` & `nodezator-1.3.9/nodezator/__main__.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/alphamask/basicop.py` & `nodezator-1.3.9/nodezator/alphamask/basicop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/alphamask/main.py` & `nodezator-1.3.9/nodezator/alphamask/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/alphamask/masksop.py` & `nodezator-1.3.9/nodezator/alphamask/masksop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/alphamask/utils.py` & `nodezator-1.3.9/nodezator/alphamask/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/appinfo.py` & `nodezator-1.3.9/nodezator/appinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ###                       be used in production, though;
 ###
 ### 'stable' : can be used in production; bugs,
 ###            if existent, are considered tolerable;
 
 AppVersion = namedtuple("AppVersion", "major minor micro release_level")
 
-APP_VERSION = AppVersion(1, 3, 8, "release_candidate")
+APP_VERSION = AppVersion(1, 3, 9, "release_candidate")
 
 
 ### titles for the application
 
 TITLE = "Nodezator"
 
 ## used to name directories related to the app, like
```

### Comparing `nodezator-1.3.8/nodezator/audioplayer.py` & `nodezator-1.3.9/nodezator/audioplayer.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/classes2d/collections.py` & `nodezator-1.3.9/nodezator/classes2d/collections.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/classes2d/single.py` & `nodezator-1.3.9/nodezator/classes2d/single.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/classes2d/surfaceswitcher.py` & `nodezator-1.3.9/nodezator/classes2d/surfaceswitcher.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/color2d.py` & `nodezator-1.3.9/nodezator/colorsman/color2d.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/colors.py` & `nodezator-1.3.9/nodezator/colorsman/colors.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/loopop.py` & `nodezator-1.3.9/nodezator/colorsman/editor/loopop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/main.py` & `nodezator-1.3.9/nodezator/colorsman/editor/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/panel/colorsop.py` & `nodezator-1.3.9/nodezator/colorsman/editor/panel/colorsop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/panel/data.py` & `nodezator-1.3.9/nodezator/colorsman/editor/panel/data.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/panel/main.py` & `nodezator-1.3.9/nodezator/colorsman/editor/panel/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetop.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/button.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/button.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/constants.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/entry.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/entry.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/label.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/label.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/editor/widgetsetup/scale.py` & `nodezator-1.3.9/nodezator/colorsman/editor/widgetsetup/scale.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/picker/main.py` & `nodezator-1.3.9/nodezator/colorsman/picker/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/picker/op.py` & `nodezator-1.3.9/nodezator/colorsman/picker/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/viewer/main.py` & `nodezator-1.3.9/nodezator/colorsman/viewer/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/viewer/modes/colorlist.py` & `nodezator-1.3.9/nodezator/colorsman/viewer/modes/colorlist.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/main.py` & `nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/particles.py` & `nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/particles.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/colorsman/viewer/modes/patterns/waves.py` & `nodezator-1.3.9/nodezator/colorsman/viewer/modes/patterns/waves.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/config.py` & `nodezator-1.3.9/nodezator/config.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/app_icon.png` & `nodezator-1.3.9/nodezator/data/app_icon.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/app_themes/emeralds_on_coal.pyl` & `nodezator-1.3.9/nodezator/data/app_themes/emeralds_on_coal.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/general-controls.htsl` & `nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/general-controls.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/index.htsl` & `nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/index.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/text-editor-default-behavior.htsl` & `nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/text-editor-default-behavior.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/help.nodezator.pysite/text-editor-vim-like-behavior.htsl` & `nodezator-1.3.9/nodezator/data/aww/help.nodezator.pysite/text-editor-vim-like-behavior.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-color-coded-annotations.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-color-coded-annotations.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-intfloat-words.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-intfloat-words.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-configurations.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-configurations.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-presets.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/appendix-widget-presets.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-basic-way-define-widgets.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-basic-way-define-widgets.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-color-coding-inputs-outputs.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-color-coding-inputs-outputs.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-complex-viewer-nodes.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-complex-viewer-nodes.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-viewer-nodes.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-viewer-nodes.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-defining-your-first-node.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-defining-your-first-node.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-distributing-nodes.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-distributing-nodes.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-full-syntax-more-widgets.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-full-syntax-more-widgets.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-loading-nodes.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-loading-nodes.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-more-ways-define-nodes.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-more-ways-define-nodes.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-nodes-variable-parameters-custom-outputs.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-nodes-variable-parameters-custom-outputs.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-other-objects.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-other-objects.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-preview-widgets.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-preview-widgets.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/ch-widget-presets-more-widgets.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/ch-widget-presets-more-widgets.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img03.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img03.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img04.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img04.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img05.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img05.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img06_and_07.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img06_and_07.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img08.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-basic-way-define-widgets_img08.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img03.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img03.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img04.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img04.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img05.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-color-coding_img05.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-viewer-nodes_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-viewer-nodes_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-defining-your-first_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-full-syntax_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img03.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-nodes-variable-parameters_img03.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img03.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img03.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img04.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img04.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img05.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img05.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img06.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-other-objects_img06.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_0.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_0.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_1.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img01_1.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_0.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_0.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_1.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img03_1.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_0.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_0.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_1.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img04_1.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_0.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_0.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_1.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-preview-widgets_img05_1.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img00.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img00.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img01.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img01.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img02.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img02.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img03.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img03.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img04.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img04.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img05.png` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/images/ch-widget-presets_img05.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/manual.nodezator.pysite/index.htsl` & `nodezator-1.3.9/nodezator/data/aww/manual.nodezator.pysite/index.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/nodezator.pysite/about.htsl` & `nodezator-1.3.9/nodezator/data/aww/nodezator.pysite/about.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/aww/nodezator.pysite/license.htsl` & `nodezator-1.3.9/nodezator/data/aww/nodezator.pysite/license.htsl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/OFL_license_for_all_other_fonts.txt` & `nodezator-1.3.9/nodezator/data/fonts/OFL_license_for_all_other_fonts.txt`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/cc0_license_for_nodezator_icons.txt` & `nodezator-1.3.9/nodezator/data/fonts/cc0_license_for_nodezator_icons.txt`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/enc_sans_sexp_bold_mplus_1p_2000em_med.ttf` & `nodezator-1.3.9/nodezator/data/fonts/enc_sans_sexp_bold_mplus_1p_2000em_med.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/fira_mono_bold_mplus_1m_med.ttf` & `nodezator-1.3.9/nodezator/data/fonts/fira_mono_bold_mplus_1m_med.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/nodezator_icons.ttf` & `nodezator-1.3.9/nodezator/data/fonts/nodezator_icons.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/noto_sans_bold.ttf` & `nodezator-1.3.9/nodezator/data/fonts/noto_sans_bold.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/noto_sans_italic.ttf` & `nodezator-1.3.9/nodezator/data/fonts/noto_sans_italic.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/noto_sans_mono_medium.ttf` & `nodezator-1.3.9/nodezator/data/fonts/noto_sans_mono_medium.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/fonts/noto_sans_regular.ttf` & `nodezator-1.3.9/nodezator/data/fonts/noto_sans_regular.ttf`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/glossary.rst` & `nodezator-1.3.9/nodezator/data/glossary.rst`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/colors_editor_scale_images.png` & `nodezator-1.3.9/nodezator/data/images/colors_editor_scale_images.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/discord_logo.png` & `nodezator-1.3.9/nodezator/data/images/discord_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/github_mark.png` & `nodezator-1.3.9/nodezator/data/images/github_mark.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/indie_python_logo.png` & `nodezator-1.3.9/nodezator/data/images/indie_python_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/kennedy_logo.png` & `nodezator-1.3.9/nodezator/data/images/kennedy_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/mask_wave.png` & `nodezator-1.3.9/nodezator/data/images/mask_wave.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/patreon_logo.png` & `nodezator-1.3.9/nodezator/data/images/patreon_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/pygame_logo.png` & `nodezator-1.3.9/nodezator/data/images/pygame_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/python_filemanager_icon.png` & `nodezator-1.3.9/nodezator/data/images/python_filemanager_icon.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/python_menu_icon.png` & `nodezator-1.3.9/nodezator/data/images/python_menu_icon.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/python_splashscreen_icon.png` & `nodezator-1.3.9/nodezator/data/images/python_splashscreen_icon.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/splash_nodezator_robot.png` & `nodezator-1.3.9/nodezator/data/images/splash_nodezator_robot.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/twitter_logo.png` & `nodezator-1.3.9/nodezator/data/images/twitter_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/images/unlicense_logo.png` & `nodezator-1.3.9/nodezator/data/images/unlicense_logo.png`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/locale/en_us/dialogs_map.pyl` & `nodezator-1.3.9/nodezator/data/locale/en_us/dialogs_map.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/locale/en_us/translations_map.pyl` & `nodezator-1.3.9/nodezator/data/locale/en_us/translations_map.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/locale/pt_br/dialogs_map.pyl` & `nodezator-1.3.9/nodezator/data/locale/pt_br/dialogs_map.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/locale/pt_br/translations_map.pyl` & `nodezator-1.3.9/nodezator/data/locale/pt_br/translations_map.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/syntax_themes/python/ice_with_candy.pyl` & `nodezator-1.3.9/nodezator/data/syntax_themes/python/ice_with_candy.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/data/syntax_themes/python/sprinkled_dark.pyl` & `nodezator-1.3.9/nodezator/data/syntax_themes/python/sprinkled_dark.pyl`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/dialog.py` & `nodezator-1.3.9/nodezator/dialog.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/categorycolors.py` & `nodezator-1.3.9/nodezator/editing/categorycolors.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/data.py` & `nodezator-1.3.9/nodezator/editing/data.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/export/form/image.py` & `nodezator-1.3.9/nodezator/editing/export/form/image.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/export/form/python.py` & `nodezator-1.3.9/nodezator/editing/export/form/python.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/export/main.py` & `nodezator-1.3.9/nodezator/editing/export/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/gridlogic.py` & `nodezator-1.3.9/nodezator/editing/gridlogic.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/main.py` & `nodezator-1.3.9/nodezator/editing/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/nodepacksforms/renaming.py` & `nodezator-1.3.9/nodezator/editing/nodepacksforms/renaming.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/nodepacksforms/selection.py` & `nodezator-1.3.9/nodezator/editing/nodepacksforms/selection.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objinsert.py` & `nodezator-1.3.9/nodezator/editing/objinsert.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objpopups/callablenode.py` & `nodezator-1.3.9/nodezator/editing/objpopups/callablenode.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objpopups/constants.py` & `nodezator-1.3.9/nodezator/editing/objpopups/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objpopups/operatornode.py` & `nodezator-1.3.9/nodezator/editing/objpopups/operatornode.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objpopups/proxynode.py` & `nodezator-1.3.9/nodezator/editing/objpopups/proxynode.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/objpopups/textblock.py` & `nodezator-1.3.9/nodezator/editing/objpopups/textblock.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/reposition.py` & `nodezator-1.3.9/nodezator/editing/reposition.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/selection.py` & `nodezator-1.3.9/nodezator/editing/selection.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/socketpopups/input.py` & `nodezator-1.3.9/nodezator/editing/socketpopups/input.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/socketpopups/output.py` & `nodezator-1.3.9/nodezator/editing/socketpopups/output.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/socketpopups/proxy.py` & `nodezator-1.3.9/nodezator/editing/socketpopups/proxy.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/widgetpicker/main.py` & `nodezator-1.3.9/nodezator/editing/widgetpicker/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/widgetpicker/subforms.py` & `nodezator-1.3.9/nodezator/editing/widgetpicker/subforms.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/editing/widgetpopups/creation.py` & `nodezator-1.3.9/nodezator/editing/widgetpopups/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/bookmarkpanel/main.py` & `nodezator-1.3.9/nodezator/fileman/bookmarkpanel/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/bookmarkpanel/surfs.py` & `nodezator-1.3.9/nodezator/fileman/bookmarkpanel/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/constants.py` & `nodezator-1.3.9/nodezator/fileman/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/extraop.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/extraop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/loadop.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/loadop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/main.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/mouseop.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/mouseop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/newpathform.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/newpathform.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/dirpanel/surfs.py` & `nodezator-1.3.9/nodezator/fileman/dirpanel/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/main.py` & `nodezator-1.3.9/nodezator/fileman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/op.py` & `nodezator-1.3.9/nodezator/fileman/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/pathobj.py` & `nodezator-1.3.9/nodezator/fileman/pathobj.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fileman/surfs.py` & `nodezator-1.3.9/nodezator/fileman/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/cache.py` & `nodezator-1.3.9/nodezator/fontsman/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/constants.py` & `nodezator-1.3.9/nodezator/fontsman/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/exception.py` & `nodezator-1.3.9/nodezator/fontsman/exception.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/preview/cache.py` & `nodezator-1.3.9/nodezator/fontsman/preview/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/preview/render.py` & `nodezator-1.3.9/nodezator/fontsman/preview/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/viewer/main.py` & `nodezator-1.3.9/nodezator/fontsman/viewer/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/fontsman/viewer/render.py` & `nodezator-1.3.9/nodezator/fontsman/viewer/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/builtinnode/constants.py` & `nodezator-1.3.9/nodezator/graphman/builtinnode/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/builtinnode/export.py` & `nodezator-1.3.9/nodezator/graphman/builtinnode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/builtinnode/main.py` & `nodezator-1.3.9/nodezator/graphman/builtinnode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/constants.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/execution.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/execution.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/export.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/main.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/preproc.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/preproc.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/subparam/main.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/subparam/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/subparam/segment.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/subparam/segment.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/subparam/unpacking.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/subparam/unpacking.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/subparam/widget.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/subparam/widget.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/surfs.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/utils.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizop/main.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizop/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizop/reposition.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizop/reposition.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/creation.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/bodysetup/main.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/bodysetup/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/main.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/param.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/param.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/callablenode/vizprep/varparam.py` & `nodezator-1.3.9/nodezator/graphman/callablenode/vizprep/varparam.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/capsulenode/constants.py` & `nodezator-1.3.9/nodezator/graphman/capsulenode/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/capsulenode/export.py` & `nodezator-1.3.9/nodezator/graphman/capsulenode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/capsulenode/main.py` & `nodezator-1.3.9/nodezator/graphman/capsulenode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/editlogic.py` & `nodezator-1.3.9/nodezator/graphman/editlogic.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/exception.py` & `nodezator-1.3.9/nodezator/graphman/exception.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/execution.py` & `nodezator-1.3.9/nodezator/graphman/execution.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/main.py` & `nodezator-1.3.9/nodezator/graphman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/nodepacksissues.py` & `nodezator-1.3.9/nodezator/graphman/nodepacksissues.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/constants.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/execution.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/execution.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/export.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/main.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/surfs.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/vizop.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/vizop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/operatornode/vizprep.py` & `nodezator-1.3.9/nodezator/graphman/operatornode/vizprep.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/presets.py` & `nodezator-1.3.9/nodezator/graphman/presets.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/export.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/main.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/segment.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/segment.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/surfs.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/titleupdate.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/titleupdate.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/utils.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/vizop/main.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/vizop/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/vizop/reposition.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/vizop/reposition.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/vizprep.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/vizprep.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/proxynode/widget.py` & `nodezator-1.3.9/nodezator/graphman/proxynode/widget.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/pythonrepr.py` & `nodezator-1.3.9/nodezator/graphman/pythonrepr.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/scriptloading.py` & `nodezator-1.3.9/nodezator/graphman/scriptloading.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/base.py` & `nodezator-1.3.9/nodezator/graphman/socket/base.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/input.py` & `nodezator-1.3.9/nodezator/graphman/socket/input.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/output.py` & `nodezator-1.3.9/nodezator/graphman/socket/output.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/placeholder.py` & `nodezator-1.3.9/nodezator/graphman/socket/placeholder.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/proxy.py` & `nodezator-1.3.9/nodezator/graphman/socket/proxy.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socket/surfs.py` & `nodezator-1.3.9/nodezator/graphman/socket/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/action.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/action.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/draw.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/draw.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/export.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/main.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/support.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/support.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/socketparenthood/utils.py` & `nodezator-1.3.9/nodezator/graphman/socketparenthood/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/stlibnode/constants.py` & `nodezator-1.3.9/nodezator/graphman/stlibnode/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/stlibnode/export.py` & `nodezator-1.3.9/nodezator/graphman/stlibnode/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/stlibnode/main.py` & `nodezator-1.3.9/nodezator/graphman/stlibnode/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/textblock/check.py` & `nodezator-1.3.9/nodezator/graphman/textblock/check.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/textblock/export.py` & `nodezator-1.3.9/nodezator/graphman/textblock/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/textblock/main.py` & `nodezator-1.3.9/nodezator/graphman/textblock/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/textblock/surf.py` & `nodezator-1.3.9/nodezator/graphman/textblock/surf.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/utils.py` & `nodezator-1.3.9/nodezator/graphman/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/validation/fixtures.py` & `nodezator-1.3.9/nodezator/graphman/validation/fixtures.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/validation/main.py` & `nodezator-1.3.9/nodezator/graphman/validation/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/validation/tests.py` & `nodezator-1.3.9/nodezator/graphman/validation/tests.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/widget/export.py` & `nodezator-1.3.9/nodezator/graphman/widget/export.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/graphman/widget/utils.py` & `nodezator-1.3.9/nodezator/graphman/widget/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/hideswitch.py` & `nodezator-1.3.9/nodezator/hideswitch.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/codeblock.py` & `nodezator-1.3.9/nodezator/htsl/codeblock.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/constants.py` & `nodezator-1.3.9/nodezator/htsl/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/creation.py` & `nodezator-1.3.9/nodezator/htsl/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/image.py` & `nodezator-1.3.9/nodezator/htsl/image.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/main.py` & `nodezator-1.3.9/nodezator/htsl/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/htsl/prep.py` & `nodezator-1.3.9/nodezator/htsl/prep.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/cache.py` & `nodezator-1.3.9/nodezator/imagesman/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/render.py` & `nodezator-1.3.9/nodezator/imagesman/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/viewer/constants.py` & `nodezator-1.3.9/nodezator/imagesman/viewer/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/viewer/fullop.py` & `nodezator-1.3.9/nodezator/imagesman/viewer/fullop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/viewer/main.py` & `nodezator-1.3.9/nodezator/imagesman/viewer/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/imagesman/viewer/normalop.py` & `nodezator-1.3.9/nodezator/imagesman/viewer/normalop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/knownpacks.py` & `nodezator-1.3.9/nodezator/knownpacks.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/logman/main.py` & `nodezator-1.3.9/nodezator/logman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/logman/utils.py` & `nodezator-1.3.9/nodezator/logman/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/loopman/exception.py` & `nodezator-1.3.9/nodezator/loopman/exception.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/loopman/main.py` & `nodezator-1.3.9/nodezator/loopman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/mainloop.py` & `nodezator-1.3.9/nodezator/mainloop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/memoryman.py` & `nodezator-1.3.9/nodezator/memoryman.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/behaviour.py` & `nodezator-1.3.9/nodezator/menu/behaviour.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/command.py` & `nodezator-1.3.9/nodezator/menu/command.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/common.py` & `nodezator-1.3.9/nodezator/menu/common.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/hover.py` & `nodezator-1.3.9/nodezator/menu/hover.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/iconfactory.py` & `nodezator-1.3.9/nodezator/menu/iconfactory.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/main.py` & `nodezator-1.3.9/nodezator/menu/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/scroll.py` & `nodezator-1.3.9/nodezator/menu/scroll.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/submenu/main.py` & `nodezator-1.3.9/nodezator/menu/submenu/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/submenu/scroll.py` & `nodezator-1.3.9/nodezator/menu/submenu/scroll.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/submenu/utils.py` & `nodezator-1.3.9/nodezator/menu/submenu/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/menu/surffactory.py` & `nodezator-1.3.9/nodezator/menu/surffactory.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/behaviour.py` & `nodezator-1.3.9/nodezator/our3rdlibs/behaviour.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/button.py` & `nodezator-1.3.9/nodezator/our3rdlibs/button.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/debug.py` & `nodezator-1.3.9/nodezator/our3rdlibs/debug.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/grid/main.py` & `nodezator-1.3.9/nodezator/our3rdlibs/grid/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/grid/oop.py` & `nodezator-1.3.9/nodezator/our3rdlibs/grid/oop.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/list.py` & `nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/list.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/op.py` & `nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/iterablewidget/surfs.py` & `nodezator-1.3.9/nodezator/our3rdlibs/iterablewidget/surfs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/scale.py` & `nodezator-1.3.9/nodezator/our3rdlibs/scale.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/main.py` & `nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/sortingeditor/modes.py` & `nodezator-1.3.9/nodezator/our3rdlibs/sortingeditor/modes.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/our3rdlibs/userlogger.py` & `nodezator-1.3.9/nodezator/our3rdlibs/userlogger.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/behaviour.py` & `nodezator-1.3.9/nodezator/ourstdlibs/behaviour.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/main.py` & `nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/collections/fldict/tests.py` & `nodezator-1.3.9/nodezator/ourstdlibs/collections/fldict/tests.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/collections/general.py` & `nodezator-1.3.9/nodezator/ourstdlibs/collections/general.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/collections/nestedfromdict.py` & `nodezator-1.3.9/nodezator/ourstdlibs/collections/nestedfromdict.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/constants.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/conversion.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/conversion.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/creation.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/custom.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/custom.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/largemaps.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/largemaps.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/property.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/property.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/color/utils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/color/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/debug.py` & `nodezator-1.3.9/nodezator/ourstdlibs/debug.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/dictutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/dictutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/exceptionutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/exceptionutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/importutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/importutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/iterutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/iterutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/mathutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/mathutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/meta.py` & `nodezator-1.3.9/nodezator/ourstdlibs/meta.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/path.py` & `nodezator-1.3.9/nodezator/ourstdlibs/path.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/profileutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/profileutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/pyl.py` & `nodezator-1.3.9/nodezator/ourstdlibs/pyl.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/stringutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/stringutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/timeutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/timeutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/ourstdlibs/treeutils.py` & `nodezator-1.3.9/nodezator/ourstdlibs/treeutils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/pointsman2d/shape.py` & `nodezator-1.3.9/nodezator/pointsman2d/shape.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/pygameconstants.py` & `nodezator-1.3.9/nodezator/pygameconstants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/recentfile.py` & `nodezator-1.3.9/nodezator/recentfile.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/cluster.py` & `nodezator-1.3.9/nodezator/rectsman/cluster.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/constants.py` & `nodezator-1.3.9/nodezator/rectsman/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/fixtures.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test01_intro.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test01_intro.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test02_01_operations.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test02_01_operations.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test02_02_operations.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test02_02_operations.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test02_03_operations.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test02_03_operations.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test03_01_specialmethods.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test03_01_specialmethods.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test03_02_specialmethods.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test03_02_specialmethods.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test04_01_other.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test04_01_other.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test04_02_other.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test04_02_other.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test04_03_other.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test04_03_other.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/doctests/test05_align.py` & `nodezator-1.3.9/nodezator/rectsman/doctests/test05_align.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/main.py` & `nodezator-1.3.9/nodezator/rectsman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/singlepos.py` & `nodezator-1.3.9/nodezator/rectsman/singlepos.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/sizepos.py` & `nodezator-1.3.9/nodezator/rectsman/sizepos.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/spatial.py` & `nodezator-1.3.9/nodezator/rectsman/spatial.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/rectsman/special.py` & `nodezator-1.3.9/nodezator/rectsman/special.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/splashscreen/animsetup.py` & `nodezator-1.3.9/nodezator/splashscreen/animsetup.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/splashscreen/constants.py` & `nodezator-1.3.9/nodezator/splashscreen/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/splashscreen/factoryfuncs.py` & `nodezator-1.3.9/nodezator/splashscreen/factoryfuncs.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/splashscreen/main.py` & `nodezator-1.3.9/nodezator/splashscreen/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/splashscreen/op.py` & `nodezator-1.3.9/nodezator/splashscreen/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/surfdef.py` & `nodezator-1.3.9/nodezator/surfdef.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/surfsman/cache.py` & `nodezator-1.3.9/nodezator/surfsman/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/surfsman/draw.py` & `nodezator-1.3.9/nodezator/surfsman/draw.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/surfsman/icon.py` & `nodezator-1.3.9/nodezator/surfsman/icon.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/surfsman/render.py` & `nodezator-1.3.9/nodezator/surfsman/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/exception.py` & `nodezator-1.3.9/nodezator/syntaxman/exception.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/syntaxes/comment.py` & `nodezator-1.3.9/nodezator/syntaxman/syntaxes/comment.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/main.py` & `nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/namemap.py` & `nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/namemap.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/syntaxes/python/utils.py` & `nodezator-1.3.9/nodezator/syntaxman/syntaxes/python/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/syntaxes/userlog.py` & `nodezator-1.3.9/nodezator/syntaxman/syntaxes/userlog.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/syntaxman/utils.py` & `nodezator-1.3.9/nodezator/syntaxman/utils.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/cache.py` & `nodezator-1.3.9/nodezator/textman/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/constants.py` & `nodezator-1.3.9/nodezator/textman/editor/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/main.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/modes/insert.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/modes/insert.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/modes/normal.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/modes/normal.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/navigation.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/navigation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/op.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/cursor/syntaxhigh.py` & `nodezator-1.3.9/nodezator/textman/editor/cursor/syntaxhigh.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/line.py` & `nodezator-1.3.9/nodezator/textman/editor/line.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/editor/main.py` & `nodezator-1.3.9/nodezator/textman/editor/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/entryedition/cursor.py` & `nodezator-1.3.9/nodezator/textman/entryedition/cursor.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/entryedition/line.py` & `nodezator-1.3.9/nodezator/textman/entryedition/line.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/label/autolabel.py` & `nodezator-1.3.9/nodezator/textman/label/autolabel.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/label/main.py` & `nodezator-1.3.9/nodezator/textman/label/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/render.py` & `nodezator-1.3.9/nodezator/textman/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/text.py` & `nodezator-1.3.9/nodezator/textman/text.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/viewer/constants.py` & `nodezator-1.3.9/nodezator/textman/viewer/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/viewer/main.py` & `nodezator-1.3.9/nodezator/textman/viewer/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/viewer/op.py` & `nodezator-1.3.9/nodezator/textman/viewer/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/textman/viewer/prep.py` & `nodezator-1.3.9/nodezator/textman/viewer/prep.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/translation.py` & `nodezator-1.3.9/nodezator/translation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/userprefsman/editionform.py` & `nodezator-1.3.9/nodezator/userprefsman/editionform.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/userprefsman/main.py` & `nodezator-1.3.9/nodezator/userprefsman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/userprefsman/validation.py` & `nodezator-1.3.9/nodezator/userprefsman/validation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/videopreview/cache.py` & `nodezator-1.3.9/nodezator/videopreview/cache.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/videopreview/constants.py` & `nodezator-1.3.9/nodezator/videopreview/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/videopreview/previewer.py` & `nodezator-1.3.9/nodezator/videopreview/previewer.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/videopreview/render.py` & `nodezator-1.3.9/nodezator/videopreview/render.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/checkbutton.py` & `nodezator-1.3.9/nodezator/widget/checkbutton.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/colorbutton.py` & `nodezator-1.3.9/nodezator/widget/colorbutton.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/defaultholder.py` & `nodezator-1.3.9/nodezator/widget/defaultholder.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/intfloatentry/main.py` & `nodezator-1.3.9/nodezator/widget/intfloatentry/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/intfloatentry/modes.py` & `nodezator-1.3.9/nodezator/widget/intfloatentry/modes.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/intfloatentry/numeval.py` & `nodezator-1.3.9/nodezator/widget/intfloatentry/numeval.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/intfloatentry/op.py` & `nodezator-1.3.9/nodezator/widget/intfloatentry/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/literaldisplay.py` & `nodezator-1.3.9/nodezator/widget/literaldisplay.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/literalentry.py` & `nodezator-1.3.9/nodezator/widget/literalentry.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optionmenu/creation.py` & `nodezator-1.3.9/nodezator/widget/optionmenu/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optionmenu/main.py` & `nodezator-1.3.9/nodezator/widget/optionmenu/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optionmenu/op.py` & `nodezator-1.3.9/nodezator/widget/optionmenu/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optiontray/creation.py` & `nodezator-1.3.9/nodezator/widget/optiontray/creation.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optiontray/main.py` & `nodezator-1.3.9/nodezator/widget/optiontray/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/optiontray/op.py` & `nodezator-1.3.9/nodezator/widget/optiontray/op.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/audio.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/audio.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/base.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/base.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/constants.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/constants.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/font.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/font.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/image.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/image.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/path.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/path.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/text.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/text.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/pathpreview/video.py` & `nodezator-1.3.9/nodezator/widget/pathpreview/video.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/sortingbutton.py` & `nodezator-1.3.9/nodezator/widget/sortingbutton.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/stringentry.py` & `nodezator-1.3.9/nodezator/widget/stringentry.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/widget/textdisplay.py` & `nodezator-1.3.9/nodezator/widget/textdisplay.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/fileop.py` & `nodezator-1.3.9/nodezator/winman/fileop.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,20 +126,35 @@
                     ### make it appear as if there are no
                     ### unsaved changes; this will cause the
                     ### current changes to be ignored and
                     ### thereby lost when the newly created
                     ### file is opened
                     indicate_saved()
 
+                    ### delete swap path contents
+                    APP_REFS.swap_path.unlink()
+
                 elif answer == "save_first":
                     self.save()
 
                 else:
                     return
 
+        ### if there are not and there's a file loaded, it means it
+        ### is a regular file, so delete its swap file
+
+        else:
+
+            try:
+                APP_REFS.source_path
+            except AttributeError:
+                pass
+            else:
+                APP_REFS.swap_path.unlink()
+
         ### generate new temporary filepath
         filepath = APP_REFS.temp_filepaths_man.get_new_temp_filepath()
 
         ### save file
         save_pyl({}, filepath)
 
         ### finally, load (open) the file
```

### Comparing `nodezator-1.3.8/nodezator/winman/label.py` & `nodezator-1.3.9/nodezator/winman/label.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/main.py` & `nodezator-1.3.9/nodezator/winman/main.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/menu.py` & `nodezator-1.3.9/nodezator/winman/menu.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/boxselection.py` & `nodezator-1.3.9/nodezator/winman/states/boxselection.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/loadedfile.py` & `nodezator-1.3.9/nodezator/winman/states/loadedfile.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/movingobject.py` & `nodezator-1.3.9/nodezator/winman/states/movingobject.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/nofile.py` & `nodezator-1.3.9/nodezator/winman/states/nofile.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/segmentdef.py` & `nodezator-1.3.9/nodezator/winman/states/segmentdef.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/states/segmentsev.py` & `nodezator-1.3.9/nodezator/winman/states/segmentsev.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator/winman/switch.py` & `nodezator-1.3.9/nodezator/winman/switch.py`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/nodezator.egg-info/PKG-INFO` & `nodezator-1.3.9/nodezator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodezator
-Version: 1.3.8
+Version: 1.3.9
 Summary: A multi-purpose visual node editor for the Python programming language
 Home-page: https://nodezator.com
 Author: Kennedy Richard
 Author-email: kennedy@kennedyrichard.com
 License: Unlicense
 Project-URL: Source code, https://github.com/IndiePython/nodezator
 Project-URL: Forum, https://github.com/IndiePython/nodezator/discussions
```

### Comparing `nodezator-1.3.8/nodezator.egg-info/SOURCES.txt` & `nodezator-1.3.9/nodezator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodezator-1.3.8/setup.cfg` & `nodezator-1.3.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nodezator
-version = 1.3.8
+version = 1.3.9
 author = Kennedy Richard
 author_email = kennedy@kennedyrichard.com
 description = A multi-purpose visual node editor for the Python programming language
 keywords = gui, desktop, application, pygame, graph, graphs, nodes, node, editor
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Unlicense
```

