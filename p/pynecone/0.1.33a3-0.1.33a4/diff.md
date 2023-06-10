# Comparing `tmp/pynecone-0.1.33a3.tar.gz` & `tmp/pynecone-0.1.33a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.33a3.tar", max compression
+gzip compressed data, was "pynecone-0.1.33a4.tar", max compression
```

## Comparing `pynecone-0.1.33a3.tar` & `pynecone-0.1.33a4.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a3/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a3/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a3/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a3/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a3/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a3/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a3/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a3/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-09 19:48:33.040538 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a3/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a3/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a3/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a3/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a3/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a3/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a3/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a3/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a3/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     8450 2023-06-09 19:48:33.040820 pynecone-0.1.33a3/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a3/pynecone/__init__.py
--rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a3/pynecone/admin.py
--rw-r--r--   0        0        0    21426 2023-06-09 19:48:39.955078 pynecone-0.1.33a3/pynecone/app.py
--rw-r--r--   0        0        0     2548 2023-06-07 19:04:43.443201 pynecone-0.1.33a3/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a3/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6689 2023-06-09 19:48:33.041803 pynecone-0.1.33a3/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2642 2023-06-09 19:48:33.042227 pynecone-0.1.33a3/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7767 2023-06-09 19:48:39.955794 pynecone-0.1.33a3/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a3/pynecone/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-09 19:48:39.957002 pynecone-0.1.33a3/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a3/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a3/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a3/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a3/pynecone/components/base/head.py
--rw-r--r--   0        0        0      933 2023-06-09 19:48:39.957851 pynecone-0.1.33a3/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1412 2023-06-07 19:04:43.443671 pynecone-0.1.33a3/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a3/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a3/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a3/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a3/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a3/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a3/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a3/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a3/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a3/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a3/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a3/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a3/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3517 2023-06-09 19:48:39.958158 pynecone-0.1.33a3/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a3/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a3/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a3/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a3/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a3/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a3/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a3/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a3/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a3/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a3/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a3/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a3/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a3/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a3/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a3/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a3/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a3/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a3/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a3/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-06-09 18:42:18.512736 pynecone-0.1.33a3/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a3/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a3/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a3/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a3/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a3/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a3/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a3/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a3/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1573 2023-06-09 19:48:39.959122 pynecone-0.1.33a3/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1532 2023-06-09 19:48:39.959281 pynecone-0.1.33a3/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a3/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a3/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a3/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a3/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a3/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a3/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      766 2023-06-09 19:48:39.959611 pynecone-0.1.33a3/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a3/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a3/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a3/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a3/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a3/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a3/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a3/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a3/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a3/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a3/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a3/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a3/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a3/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a3/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a3/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a3/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a3/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a3/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a3/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a3/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a3/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a3/pynecone/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a3/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a3/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1844 2023-06-09 19:48:39.960619 pynecone-0.1.33a3/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a3/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a3/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a3/pynecone/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a3/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a3/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a3/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a3/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a3/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a3/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a3/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a3/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a3/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a3/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a3/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-06-09 19:48:33.042551 pynecone-0.1.33a3/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a3/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a3/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a3/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a3/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a3/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a3/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a3/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     6960 2023-06-09 19:48:39.960810 pynecone-0.1.33a3/pynecone/config.py
--rw-r--r--   0        0        0    10219 2023-06-09 19:48:33.049660 pynecone-0.1.33a3/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a3/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a3/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a3/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a3/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a3/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a3/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a3/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a3/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a3/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a3/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a3/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a3/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2388 2023-06-09 19:48:39.961091 pynecone-0.1.33a3/pynecone/model.py
--rw-r--r--   0        0        0     8575 2023-06-07 19:04:43.444311 pynecone-0.1.33a3/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a3/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a3/pynecone/route.py
--rw-r--r--   0        0        0    30945 2023-06-09 19:48:33.050053 pynecone-0.1.33a3/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a3/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a3/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7394 2023-06-09 19:48:33.050640 pynecone-0.1.33a3/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a3/pynecone/utils/console.py
--rw-r--r--   0        0        0     5317 2023-06-07 19:04:43.444774 pynecone-0.1.33a3/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-09 19:48:33.051324 pynecone-0.1.33a3/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a3/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a3/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10873 2023-06-09 19:48:39.961277 pynecone-0.1.33a3/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a3/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-06-09 19:48:33.052076 pynecone-0.1.33a3/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a3/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a3/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-06-09 19:48:33.052425 pynecone-0.1.33a3/pynecone/vars.py
--rw-r--r--   0        0        0     1874 2023-06-09 19:48:53.289852 pynecone-0.1.33a3/pyproject.toml
--rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a4/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a4/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a4/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a4/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a4/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a4/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a4/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a4/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-09 19:48:33.040538 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a4/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a4/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a4/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a4/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a4/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a4/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a4/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a4/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a4/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8450 2023-06-09 19:48:33.040820 pynecone-0.1.33a4/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a4/pynecone/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a4/pynecone/admin.py
+-rw-r--r--   0        0        0    21426 2023-06-09 19:48:39.955078 pynecone-0.1.33a4/pynecone/app.py
+-rw-r--r--   0        0        0     2548 2023-06-07 19:04:43.443201 pynecone-0.1.33a4/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a4/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6689 2023-06-09 19:48:33.041803 pynecone-0.1.33a4/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2642 2023-06-09 19:48:33.042227 pynecone-0.1.33a4/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7767 2023-06-09 19:48:39.955794 pynecone-0.1.33a4/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a4/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-09 19:48:39.957002 pynecone-0.1.33a4/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a4/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a4/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a4/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a4/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      933 2023-06-09 19:48:39.957851 pynecone-0.1.33a4/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1412 2023-06-07 19:04:43.443671 pynecone-0.1.33a4/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a4/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a4/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a4/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a4/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a4/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a4/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a4/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a4/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a4/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a4/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a4/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a4/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3517 2023-06-09 19:48:39.958158 pynecone-0.1.33a4/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a4/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a4/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a4/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a4/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a4/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a4/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a4/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a4/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a4/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a4/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a4/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a4/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a4/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a4/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a4/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a4/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a4/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a4/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a4/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-06-09 18:42:18.512736 pynecone-0.1.33a4/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a4/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a4/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a4/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a4/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a4/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a4/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a4/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a4/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1573 2023-06-09 19:48:39.959122 pynecone-0.1.33a4/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1532 2023-06-09 19:48:39.959281 pynecone-0.1.33a4/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a4/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a4/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a4/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a4/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a4/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a4/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      766 2023-06-09 19:48:39.959611 pynecone-0.1.33a4/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a4/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a4/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a4/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a4/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a4/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a4/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a4/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a4/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a4/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a4/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a4/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a4/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a4/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a4/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a4/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a4/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a4/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a4/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a4/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a4/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a4/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a4/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a4/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a4/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1616 2023-06-10 01:56:25.822303 pynecone-0.1.33a4/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a4/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a4/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a4/pynecone/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a4/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a4/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a4/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a4/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a4/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a4/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a4/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a4/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a4/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a4/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a4/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-06-09 19:48:33.042551 pynecone-0.1.33a4/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a4/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a4/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a4/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a4/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a4/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a4/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a4/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     6960 2023-06-09 19:48:39.960810 pynecone-0.1.33a4/pynecone/config.py
+-rw-r--r--   0        0        0    10219 2023-06-09 19:48:33.049660 pynecone-0.1.33a4/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a4/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a4/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a4/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a4/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a4/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a4/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a4/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a4/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a4/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a4/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a4/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a4/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2388 2023-06-09 19:48:39.961091 pynecone-0.1.33a4/pynecone/model.py
+-rw-r--r--   0        0        0     8575 2023-06-07 19:04:43.444311 pynecone-0.1.33a4/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a4/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a4/pynecone/route.py
+-rw-r--r--   0        0        0    30945 2023-06-09 19:48:33.050053 pynecone-0.1.33a4/pynecone/state.py
+-rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a4/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a4/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7394 2023-06-09 19:48:33.050640 pynecone-0.1.33a4/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a4/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5317 2023-06-07 19:04:43.444774 pynecone-0.1.33a4/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-09 19:48:33.051324 pynecone-0.1.33a4/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a4/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a4/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10873 2023-06-09 19:48:39.961277 pynecone-0.1.33a4/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a4/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-06-09 19:48:33.052076 pynecone-0.1.33a4/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a4/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a4/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-06-09 19:48:33.052425 pynecone-0.1.33a4/pynecone/vars.py
+-rw-r--r--   0        0        0     1874 2023-06-10 01:56:28.309131 pynecone-0.1.33a4/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a4/PKG-INFO
```

### Comparing `pynecone-0.1.33a3/LICENSE` & `pynecone-0.1.33a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/README.md` & `pynecone-0.1.33a4/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.33a4/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.33a4/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.33a4/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.33a4/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/web/package.json` & `pynecone-0.1.33a4/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.33a4/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.33a4/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.33a4/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/__init__.py` & `pynecone-0.1.33a4/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/app.py` & `pynecone-0.1.33a4/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/base.py` & `pynecone-0.1.33a4/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/compiler/compiler.py` & `pynecone-0.1.33a4/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/compiler/templates.py` & `pynecone-0.1.33a4/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/compiler/utils.py` & `pynecone-0.1.33a4/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/__init__.py` & `pynecone-0.1.33a4/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/base/bare.py` & `pynecone-0.1.33a4/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/base/document.py` & `pynecone-0.1.33a4/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/base/link.py` & `pynecone-0.1.33a4/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/base/meta.py` & `pynecone-0.1.33a4/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/component.py` & `pynecone-0.1.33a4/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/code.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/list.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/table.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.33a4/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.33a4/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.33a4/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/disclosure/transition.py` & `pynecone-0.1.33a4/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/feedback/alert.py` & `pynecone-0.1.33a4/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.33a4/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/feedback/progress.py` & `pynecone-0.1.33a4/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.33a4/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/feedback/spinner.py` & `pynecone-0.1.33a4/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/__init__.py` & `pynecone-0.1.33a4/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/button.py` & `pynecone-0.1.33a4/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/checkbox.py` & `pynecone-0.1.33a4/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.33a4/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/editable.py` & `pynecone-0.1.33a4/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/form.py` & `pynecone-0.1.33a4/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.33a4/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/input.py` & `pynecone-0.1.33a4/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/multiselect.py` & `pynecone-0.1.33a4/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/numberinput.py` & `pynecone-0.1.33a4/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/pininput.py` & `pynecone-0.1.33a4/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/radio.py` & `pynecone-0.1.33a4/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.33a4/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/select.py` & `pynecone-0.1.33a4/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/slider.py` & `pynecone-0.1.33a4/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/switch.py` & `pynecone-0.1.33a4/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/textarea.py` & `pynecone-0.1.33a4/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/forms/upload.py` & `pynecone-0.1.33a4/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/graphing/plotly.py` & `pynecone-0.1.33a4/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/graphing/victory.py` & `pynecone-0.1.33a4/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/__init__.py` & `pynecone-0.1.33a4/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/box.py` & `pynecone-0.1.33a4/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/card.py` & `pynecone-0.1.33a4/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/cond.py` & `pynecone-0.1.33a4/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/flex.py` & `pynecone-0.1.33a4/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/foreach.py` & `pynecone-0.1.33a4/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/grid.py` & `pynecone-0.1.33a4/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/html.py` & `pynecone-0.1.33a4/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/responsive.py` & `pynecone-0.1.33a4/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/stack.py` & `pynecone-0.1.33a4/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/layout/wrap.py` & `pynecone-0.1.33a4/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/libs/react_player.py` & `pynecone-0.1.33a4/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/media/avatar.py` & `pynecone-0.1.33a4/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/media/icon.py` & `pynecone-0.1.33a4/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/media/image.py` & `pynecone-0.1.33a4/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.33a4/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/navigation/link.py` & `pynecone-0.1.33a4/pynecone/components/navigation/link.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,34 +29,29 @@
     # If true, the link will open in new tab.
     is_external: Var[bool]
 
     def _get_imports(self) -> imports.ImportDict:
         return {**super()._get_imports(), **NextLink.create()._get_imports()}
 
     @classmethod
-    def create(
-        cls, *children, href: Optional[Var] = None, rel: Optional[Var] = None, **props
-    ) -> Component:
+    def create(cls, *children, href: Optional[Var] = None, **props) -> Component:
         """Create a Link component.
 
         Args:
             *children: The children of the component.
-            href (Var): The href attribute of the link. Defaults to None.
-            rel (Var): The rel attribute of the link. Defaults to None.
+            href: The href attribute of the link.
             **props: The props of the component.
 
         Raises:
             ValueError: in case of missing children
-            ValueError: in case of missing href
 
         Returns:
             Component: The link component
         """
         if href and not len(children):
             raise ValueError("Link without a child will not display")
         elif href is None and len(children):
-            raise ValueError("Link without 'href' props will not work.")
-        else:
-            props.update({"href": href})
-        if rel:
-            props.update({"rel": rel})
+            # Don't use a NextLink if there is no href.
+            props["as_"] = "Link"
+        if href:
+            props["href"] = href
         return super().create(*children, **props)
```

### Comparing `pynecone-0.1.33a3/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.33a4/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/navigation/stepper.py` & `pynecone-0.1.33a4/pynecone/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/__init__.py` & `pynecone-0.1.33a4/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.33a4/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/banner.py` & `pynecone-0.1.33a4/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/drawer.py` & `pynecone-0.1.33a4/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/menu.py` & `pynecone-0.1.33a4/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/modal.py` & `pynecone-0.1.33a4/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/popover.py` & `pynecone-0.1.33a4/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.33a4/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.33a4/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/tags/tag.py` & `pynecone-0.1.33a4/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/tags/tagless.py` & `pynecone-0.1.33a4/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/typography/highlight.py` & `pynecone-0.1.33a4/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/components/typography/markdown.py` & `pynecone-0.1.33a4/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/config.py` & `pynecone-0.1.33a4/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/constants.py` & `pynecone-0.1.33a4/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/constants/html.py` & `pynecone-0.1.33a4/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/constants/pynecone.py` & `pynecone-0.1.33a4/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/constants/react.py` & `pynecone-0.1.33a4/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/element.py` & `pynecone-0.1.33a4/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/elements/__init__.py` & `pynecone-0.1.33a4/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/el/precompile.py` & `pynecone-0.1.33a4/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/event.py` & `pynecone-0.1.33a4/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.33a4/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/middleware/middleware.py` & `pynecone-0.1.33a4/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/model.py` & `pynecone-0.1.33a4/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/pc.py` & `pynecone-0.1.33a4/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/route.py` & `pynecone-0.1.33a4/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/state.py` & `pynecone-0.1.33a4/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/style.py` & `pynecone-0.1.33a4/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/build.py` & `pynecone-0.1.33a4/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/console.py` & `pynecone-0.1.33a4/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/exec.py` & `pynecone-0.1.33a4/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/format.py` & `pynecone-0.1.33a4/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/imports.py` & `pynecone-0.1.33a4/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/path_ops.py` & `pynecone-0.1.33a4/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/prerequisites.py` & `pynecone-0.1.33a4/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/processes.py` & `pynecone-0.1.33a4/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/telemetry.py` & `pynecone-0.1.33a4/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/types.py` & `pynecone-0.1.33a4/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/utils/watch.py` & `pynecone-0.1.33a4/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pynecone/vars.py` & `pynecone-0.1.33a4/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a3/pyproject.toml` & `pynecone-0.1.33a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.33a3"
+version = "0.1.33a4"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.33a3/PKG-INFO` & `pynecone-0.1.33a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.33a3
+Version: 0.1.33a4
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

