# Comparing `tmp/photobooth_app-0.1.0b4.tar.gz` & `tmp/photobooth_app-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth_app-0.1.0b4.tar", max compression
+gzip compressed data, was "photobooth_app-0.1.0b5.tar", max compression
```

## Comparing `photobooth_app-0.1.0b4.tar` & `photobooth_app-0.1.0b5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1084 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/LICENSE.md
--rw-r--r--   0        0        0     6552 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/README.md
--rw-r--r--   0        0        0       33 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/application.py
--rw-r--r--   0        0        0     1427 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/containers.py
--rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      463 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0    11560 2023-06-09 05:57:53.633929 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2023-06-09 05:57:53.637930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2023-06-09 05:57:53.637930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2023-06-09 05:57:53.641930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2023-06-09 05:57:53.645930 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2023-06-09 05:57:53.661931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0    43739 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0     2618 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10517 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16264 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7597 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0      506 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3207 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2022 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0       36 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     6010 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0     1934 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0    10102 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4068 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/services/wledservice.py
--rw-r--r--   0        0        0       93 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2023-06-09 05:57:53.669931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2023-06-09 05:57:53.673931 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2023-06-09 05:57:53.677932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2023-06-09 05:57:53.681932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0      131 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0     3794 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      144 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    64483 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/favicon.ico-todo
--rw-r--r--   0        0        0    20436 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2023-06-09 05:57:53.685932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     5336 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0      905 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/index.html
--rw-r--r--   0        0        0     9915 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1217 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3034 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/645.2ddc3ded.js
--rw-r--r--   0        0        0     5660 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/692.cf3b55d3.js
--rw-r--r--   0        0        0     3924 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0     1581 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/770.b7df615e.js
--rw-r--r--   0        0        0      778 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0    12590 2023-06-09 05:57:53.689932 photobooth_app-0.1.0b4/photobooth/web_spa/js/app.ed0492eb.js
--rw-r--r--   0        0        0  1417500 2023-06-09 05:57:53.697933 photobooth_app-0.1.0b4/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0     3959 2023-06-09 05:57:53.697933 photobooth_app-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0     8041 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/LICENSE.md
+-rw-r--r--   0        0        0     3305 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/README.md
+-rw-r--r--   0        0        0       33 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/__init__.py
+-rw-r--r--   0        0        0     3726 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/__main__.py
+-rw-r--r--   0        0        0    17065 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1135 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      463 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0    11560 2023-06-10 11:33:48.004122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2023-06-10 11:33:48.008122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2023-06-10 11:33:48.012122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2023-06-10 11:33:48.016122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2023-06-10 11:33:48.020122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2023-06-10 11:33:48.036122 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0    43739 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0     2618 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    10517 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16264 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7597 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0      506 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3207 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2022 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0       36 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     6010 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0     1934 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0    10102 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8753 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4068 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5647 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0       93 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2023-06-10 11:33:48.048123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2023-06-10 11:33:48.052122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2023-06-10 11:33:48.052122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2023-06-10 11:33:48.056122 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2023-06-10 11:33:48.060123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2023-06-10 11:33:48.064123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0      131 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0     3794 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      144 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/31.363e41a9.css
+-rw-r--r--   0        0        0       88 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/706.42cb67d0.css
+-rw-r--r--   0        0        0      163 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/71.0be6c807.css
+-rw-r--r--   0        0        0      359 2023-06-10 11:33:48.068123 photobooth_app-0.1.0b5/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    64483 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/favicon.ico-todo
+-rw-r--r--   0        0        0    20436 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     5336 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0      905 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0     9915 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/31.51d7e662.js
+-rw-r--r--   0        0        0     2918 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1217 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3034 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/645.2ddc3ded.js
+-rw-r--r--   0        0        0     5660 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/692.cf3b55d3.js
+-rw-r--r--   0        0        0     3924 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9305 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/706.f32434a0.js
+-rw-r--r--   0        0        0     5357 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/71.3aaf5d7d.js
+-rw-r--r--   0        0        0     1581 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/770.b7df615e.js
+-rw-r--r--   0        0        0      778 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0    12590 2023-06-10 11:33:48.072123 photobooth_app-0.1.0b5/photobooth/web_spa/js/app.ed0492eb.js
+-rw-r--r--   0        0        0  1417500 2023-06-10 11:33:48.084123 photobooth_app-0.1.0b5/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0     3970 2023-06-10 11:33:48.084123 photobooth_app-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0     4878 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b5/PKG-INFO
```

### Comparing `photobooth_app-0.1.0b4/LICENSE.md` & `photobooth_app-0.1.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/__main__.py` & `photobooth_app-0.1.0b5/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/appconfig.py` & `photobooth_app-0.1.0b5/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/application.py` & `photobooth_app-0.1.0b5/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/containers.py` & `photobooth_app-0.1.0b5/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0b5/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/config.py` & `photobooth_app-0.1.0b5/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/home.py` & `photobooth_app-0.1.0b5/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/log.py` & `photobooth_app-0.1.0b5/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0b5/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0b5/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/processing.py` & `photobooth_app-0.1.0b5/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/sse.py` & `photobooth_app-0.1.0b5/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/routers/system.py` & `photobooth_app-0.1.0b5/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0b5/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0b5/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0b5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0b5/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/containers.py` & `photobooth_app-0.1.0b5/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/informationservice.py` & `photobooth_app-0.1.0b5/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0b5/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0b5/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0b5/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0b5/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0b5/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0b5/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/processingservice.py` & `photobooth_app-0.1.0b5/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/systemservice.py` & `photobooth_app-0.1.0b5/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/services/wledservice.py` & `photobooth_app-0.1.0b5/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0b5/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0b5/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0b5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0b5/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0b5/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/favicon.ico-todo` & `photobooth_app-0.1.0b5/photobooth/web_spa/favicon.ico-todo`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0b5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0b5/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/index.html` & `photobooth_app-0.1.0b5/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/31.51d7e662.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/645.2ddc3ded.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/645.2ddc3ded.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/692.cf3b55d3.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/692.cf3b55d3.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/706.f32434a0.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/71.3aaf5d7d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/770.b7df615e.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/770.b7df615e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/app.ed0492eb.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/app.ed0492eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0b5/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b4/pyproject.toml` & `photobooth_app-0.1.0b5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3062 3422 0d0a 6465 7363 7269  0.1.0b4"..descri
+00000050: 302e 312e 3062 3522 0d0a 6465 7363 7269  0.1.0b5"..descri
 00000060: 7074 696f 6e20 3d20 2250 686f 746f 626f  ption = "Photobo
 00000070: 6f74 6820 6170 7020 7772 6974 7465 6e20  oth app written 
 00000080: 696e 2050 7974 686f 6e20 7375 7070 6f72  in Python suppor
 00000090: 7469 6e67 2044 534c 522c 2070 6963 616d  ting DSLR, picam
 000000a0: 6572 6132 2c20 7765 6263 616d 6572 6173  era2, webcameras
 000000b0: 220d 0a61 7574 686f 7273 203d 205b 7b20  "..authors = [{ 
 000000c0: 6e61 6d65 203d 2022 4d69 6368 6165 6c20  name = "Michael 
@@ -68,15 +68,15 @@
 00000430: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
 00000440: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
 00000450: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
 00000460: 6373 220d 0a0d 0a0d 0a5b 746f 6f6c 2e70  cs"......[tool.p
 00000470: 6f65 7472 795d 0d0a 6e61 6d65 203d 2022  oetry]..name = "
 00000480: 7068 6f74 6f62 6f6f 7468 2d61 7070 220d  photobooth-app".
 00000490: 0a76 6572 7369 6f6e 203d 2022 302e 312e  .version = "0.1.
-000004a0: 3062 3422 0d0a 6465 7363 7269 7074 696f  0b4"..descriptio
+000004a0: 3062 3522 0d0a 6465 7363 7269 7074 696f  0b5"..descriptio
 000004b0: 6e20 3d20 2250 686f 746f 626f 6f74 6820  n = "Photobooth 
 000004c0: 6170 7020 7772 6974 7465 6e20 696e 2050  app written in P
 000004d0: 7974 686f 6e20 7375 7070 6f72 7469 6e67  ython supporting
 000004e0: 2044 534c 522c 2070 6963 616d 6572 6132   DSLR, picamera2
 000004f0: 2c20 7765 6263 616d 6572 6173 220d 0a61  , webcameras"..a
 00000500: 7574 686f 7273 203d 205b 224d 6963 6861  uthors = ["Micha
 00000510: 656c 2047 203c 6d65 406d 6772 6c2e 6465  el G <me@mgrl.de
@@ -206,43 +206,44 @@
 00000cd0: 6c64 6e74 2d70 6172 7365 3a20 6874 7470  ldnt-parse: http
 00000ce0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
 00000cf0: 6564 6261 742f 636f 7665 7261 6765 7079  edbat/coveragepy
 00000d00: 2f69 7373 7565 732f 3133 3932 0d0a 6469  /issues/1392..di
 00000d10: 7361 626c 655f 7761 726e 696e 6773 203d  sable_warnings =
 00000d20: 205b 2263 6f75 6c64 6e74 2d70 6172 7365   ["couldnt-parse
 00000d30: 225d 0d0a 6f6d 6974 203d 205b 0d0a 2020  "]..omit = [..  
-00000d40: 2020 2269 6e73 7461 6c6c 2e70 7922 2c0d    "install.py",.
-00000d50: 0a20 2020 2022 7465 7374 5f2a 2e70 7922  .    "test_*.py"
-00000d60: 2c0d 0a20 2020 2022 2e2f 7465 7374 732f  ,..    "./tests/
-00000d70: 2a22 0d0a 2020 2020 5d0d 0a70 6172 616c  *"..    ]..paral
-00000d80: 6c65 6c20 3d20 7472 7565 0d0a 636f 6e63  lel = true..conc
-00000d90: 7572 7265 6e63 7920 3d20 5b22 7468 7265  urrency = ["thre
-00000da0: 6164 222c 226d 756c 7469 7072 6f63 6573  ad","multiproces
-00000db0: 7369 6e67 225d 0d0a 0d0a 5b74 6f6f 6c2e  sing"]....[tool.
-00000dc0: 626c 6163 6b5d 0d0a 6c69 6e65 2d6c 656e  black]..line-len
-00000dd0: 6774 6820 3d20 3132 300d 0a0d 0a5b 746f  gth = 120....[to
-00000de0: 6f6c 2e72 7566 665d 0d0a 6c69 6e65 2d6c  ol.ruff]..line-l
-00000df0: 656e 6774 6820 3d20 3132 300d 0a73 656c  ength = 120..sel
-00000e00: 6563 7420 3d20 5b0d 0a20 2022 4522 2c20  ect = [..  "E", 
-00000e10: 2020 2320 7079 636f 6465 7374 796c 650d    # pycodestyle.
-00000e20: 0a20 2022 5722 2c20 2020 2320 7079 636f  .  "W",   # pyco
-00000e30: 6465 7374 796c 650d 0a20 2022 4622 2c20  destyle..  "F", 
-00000e40: 2020 2320 7079 666c 616b 6573 0d0a 2020    # pyflakes..  
-00000e50: 2242 222c 2020 2023 2062 7567 6265 6172  "B",   # bugbear
-00000e60: 0d0a 2020 2255 5022 2c20 2023 2070 7975  ..  "UP",  # pyu
-00000e70: 7067 7261 6465 0d0a 2020 2249 222c 2020  pgrade..  "I",  
-00000e80: 2023 2069 736f 7274 0d0a 2020 2322 4422   # isort..  #"D"
-00000e90: 2c20 2020 2320 7079 646f 6373 7479 6c65  ,   # pydocstyle
-00000ea0: 2020 2023 2061 6464 206c 6174 6572 0d0a     # add later..
-00000eb0: 5d0d 0a69 676e 6f72 6520 3d20 5b0d 0a20  ]..ignore = [.. 
-00000ec0: 2022 4230 3038 2220 2375 7365 6420 666f   "B008" #used fo
-00000ed0: 7220 4449 2069 6e6a 6563 7469 6f6e 0d0a  r DI injection..
-00000ee0: 2020 5d0d 0a65 7874 656e 642d 6578 636c    ]..extend-excl
-00000ef0: 7564 6520 3d20 5b22 7665 6e64 6f72 225d  ude = ["vendor"]
-00000f00: 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666 2e70  ....[tool.ruff.p
-00000f10: 6572 2d66 696c 652d 6967 6e6f 7265 735d  er-file-ignores]
-00000f20: 0d0a 2270 686f 746f 626f 6f74 682f 6170  .."photobooth/ap
-00000f30: 7063 6f6e 6669 672e 7079 2220 3d20 5b22  pconfig.py" = ["
-00000f40: 4535 3031 225d 0d0a 0d0a 5b74 6f6f 6c2e  E501"]....[tool.
-00000f50: 7275 6666 2e70 7964 6f63 7374 796c 655d  ruff.pydocstyle]
-00000f60: 0d0a 636f 6e76 656e 7469 6f6e 203d 2022  ..convention = "
-00000f70: 676f 6f67 6c65 22                        google"
+00000d40: 2020 2274 6573 745f 2a2e 7079 222c 0d0a    "test_*.py",..
+00000d50: 2020 2020 222e 2f74 6573 7473 2f2a 222c      "./tests/*",
+00000d60: 0d0a 2020 2020 222e 2f70 686f 746f 626f  ..    "./photobo
+00000d70: 6f74 682f 7665 6e64 6f72 2f2a 220d 0a20  oth/vendor/*".. 
+00000d80: 2020 205d 0d0a 7061 7261 6c6c 656c 203d     ]..parallel =
+00000d90: 2074 7275 650d 0a63 6f6e 6375 7272 656e   true..concurren
+00000da0: 6379 203d 205b 2274 6872 6561 6422 2c22  cy = ["thread","
+00000db0: 6d75 6c74 6970 726f 6365 7373 696e 6722  multiprocessing"
+00000dc0: 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61 636b  ]....[tool.black
+00000dd0: 5d0d 0a6c 696e 652d 6c65 6e67 7468 203d  ]..line-length =
+00000de0: 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e 7275   120....[tool.ru
+00000df0: 6666 5d0d 0a6c 696e 652d 6c65 6e67 7468  ff]..line-length
+00000e00: 203d 2031 3230 0d0a 7365 6c65 6374 203d   = 120..select =
+00000e10: 205b 0d0a 2020 2245 222c 2020 2023 2070   [..  "E",   # p
+00000e20: 7963 6f64 6573 7479 6c65 0d0a 2020 2257  ycodestyle..  "W
+00000e30: 222c 2020 2023 2070 7963 6f64 6573 7479  ",   # pycodesty
+00000e40: 6c65 0d0a 2020 2246 222c 2020 2023 2070  le..  "F",   # p
+00000e50: 7966 6c61 6b65 730d 0a20 2022 4222 2c20  yflakes..  "B", 
+00000e60: 2020 2320 6275 6762 6561 720d 0a20 2022    # bugbear..  "
+00000e70: 5550 222c 2020 2320 7079 7570 6772 6164  UP",  # pyupgrad
+00000e80: 650d 0a20 2022 4922 2c20 2020 2320 6973  e..  "I",   # is
+00000e90: 6f72 740d 0a20 2023 2244 222c 2020 2023  ort..  #"D",   #
+00000ea0: 2070 7964 6f63 7374 796c 6520 2020 2320   pydocstyle   # 
+00000eb0: 6164 6420 6c61 7465 720d 0a5d 0d0a 6967  add later..]..ig
+00000ec0: 6e6f 7265 203d 205b 0d0a 2020 2242 3030  nore = [..  "B00
+00000ed0: 3822 2023 7573 6564 2066 6f72 2044 4920  8" #used for DI 
+00000ee0: 696e 6a65 6374 696f 6e0d 0a20 205d 0d0a  injection..  ]..
+00000ef0: 6578 7465 6e64 2d65 7863 6c75 6465 203d  extend-exclude =
+00000f00: 205b 2276 656e 646f 7222 5d0d 0a0d 0a5b   ["vendor"]....[
+00000f10: 746f 6f6c 2e72 7566 662e 7065 722d 6669  tool.ruff.per-fi
+00000f20: 6c65 2d69 676e 6f72 6573 5d0d 0a22 7068  le-ignores].."ph
+00000f30: 6f74 6f62 6f6f 7468 2f61 7070 636f 6e66  otobooth/appconf
+00000f40: 6967 2e70 7922 203d 205b 2245 3530 3122  ig.py" = ["E501"
+00000f50: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+00000f60: 7079 646f 6373 7479 6c65 5d0d 0a63 6f6e  pydocstyle]..con
+00000f70: 7665 6e74 696f 6e20 3d20 2267 6f6f 676c  vention = "googl
+00000f80: 6522                                     e"
```

