# Comparing `tmp/aioqui-2.1.0.tar.gz` & `tmp/aioqui-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqui-2.1.0.tar", last modified: Sat Jun 10 15:41:02 2023, max compression
+gzip compressed data, was "aioqui-2.1.1.tar", last modified: Sat Jun 10 15:50:55 2023, max compression
```

## Comparing `aioqui-2.1.0.tar` & `aioqui-2.1.1.tar`

### file list

```diff
@@ -1,376 +1,376 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.398235 aioqui-2.1.0/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2680 2023-06-10 15:41:02.397234 aioqui-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.1.0/README.md
--rw-rw-rw-   0        0        0     1538 2023-06-10 15:40:36.000000 aioqui-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 15:41:02.398235 aioqui-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.109234 aioqui-2.1.0/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.1.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.110235 aioqui-2.1.0/src/aioqui/
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.103249 aioqui-2.1.0/src/aioqui/.assets/
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.350238 aioqui-2.1.0/src/aioqui/.assets/icons/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.1.0/src/aioqui/.assets/icons/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.0/src/aioqui/.assets/icons/zoom-out.svg
--rw-rw-rw-   0        0        0      181 2023-06-09 15:58:57.000000 aioqui-2.1.0/src/aioqui/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-06-09 00:29:28.000000 aioqui-2.1.0/src/aioqui/asynq.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.352238 aioqui-2.1.0/src/aioqui/context/
--rw-rw-rw-   0        0        0       71 2023-06-10 12:25:08.000000 aioqui-2.1.0/src/aioqui/context/__init__.py
--rw-rw-rw-   0        0        0      501 2023-06-08 23:59:03.000000 aioqui-2.1.0/src/aioqui/context/context_api.py
--rw-rw-rw-   0        0        0     9972 2023-06-10 15:34:57.000000 aioqui-2.1.0/src/aioqui/context/context_obj.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.357237 aioqui-2.1.0/src/aioqui/misc/
--rw-rw-rw-   0        0        0      123 2023-06-10 12:26:25.000000 aioqui-2.1.0/src/aioqui/misc/__init__.py
--rw-rw-rw-   0        0        0     3527 2023-06-09 22:36:04.000000 aioqui-2.1.0/src/aioqui/misc/aiorequest.py
--rw-rw-rw-   0        0        0      975 2023-05-26 19:00:03.000000 aioqui-2.1.0/src/aioqui/misc/animation.py
--rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.1.0/src/aioqui/misc/conthrq.py
--rw-rw-rw-   0        0        0     1387 2023-06-10 12:25:08.000000 aioqui-2.1.0/src/aioqui/misc/fileops.py
--rw-rw-rw-   0        0        0     2156 2023-06-10 12:25:08.000000 aioqui-2.1.0/src/aioqui/misc/qss_parser.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.361234 aioqui-2.1.0/src/aioqui/types/
--rw-rw-rw-   0        0        0       93 2023-05-16 21:16:03.000000 aioqui-2.1.0/src/aioqui/types/__init__.py
--rw-rw-rw-   0        0        0      278 2023-06-10 12:25:08.000000 aioqui-2.1.0/src/aioqui/types/common.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.368235 aioqui-2.1.0/src/aioqui/types/enums/
--rw-rw-rw-   0        0        0      294 2023-05-16 17:41:17.000000 aioqui-2.1.0/src/aioqui/types/enums/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.1.0/src/aioqui/types/enums/alignment.py
--rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.1.0/src/aioqui/types/enums/echo_mode.py
--rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.1.0/src/aioqui/types/enums/elide_mode.py
--rw-rw-rw-   0        0        0      283 2023-05-16 17:57:41.000000 aioqui-2.1.0/src/aioqui/types/enums/logic_button.py
--rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.1.0/src/aioqui/types/enums/orientation.py
--rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.1.0/src/aioqui/types/enums/scroll_policy.py
--rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.1.0/src/aioqui/types/enums/size_policy.py
--rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.1.0/src/aioqui/types/enums/window_hint.py
--rw-rw-rw-   0        0        0     3595 2023-05-26 18:03:40.000000 aioqui-2.1.0/src/aioqui/types/icon.py
--rw-rw-rw-   0        0        0      331 2023-05-15 15:26:00.000000 aioqui-2.1.0/src/aioqui/types/size.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.381235 aioqui-2.1.0/src/aioqui/widgets/
--rw-rw-rw-   0        0        0      675 2023-06-09 23:49:23.000000 aioqui-2.1.0/src/aioqui/widgets/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.387235 aioqui-2.1.0/src/aioqui/widgets/custom/
--rw-rw-rw-   0        0        0      220 2023-06-09 00:40:35.000000 aioqui-2.1.0/src/aioqui/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     2230 2023-06-09 00:40:35.000000 aioqui-2.1.0/src/aioqui/widgets/custom/duration_label.py
--rw-rw-rw-   0        0        0     2484 2023-06-09 23:31:11.000000 aioqui-2.1.0/src/aioqui/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     3176 2023-06-10 00:04:27.000000 aioqui-2.1.0/src/aioqui/widgets/custom/popup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.392235 aioqui-2.1.0/src/aioqui/widgets/custom/qss/
--rw-rw-rw-   0        0        0      201 2023-06-09 23:42:41.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-16 20:25:11.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/colors.py
--rw-rw-rw-   0        0        0     1491 2023-05-16 20:59:19.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/date_time.py
--rw-rw-rw-   0        0        0      306 2023-05-16 21:06:26.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/image_button.py
--rw-rw-rw-   0        0        0      829 2023-05-16 21:12:30.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/popup.py
--rw-rw-rw-   0        0        0       24 2023-05-16 20:13:39.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/scrollbar.py
--rw-rw-rw-   0        0        0      436 2023-05-16 20:17:25.000000 aioqui-2.1.0/src/aioqui/widgets/custom/qss/searchbar.py
--rw-rw-rw-   0        0        0     1013 2023-06-09 16:22:55.000000 aioqui-2.1.0/src/aioqui/widgets/custom/searchbar.py
--rw-rw-rw-   0        0        0     1736 2023-05-26 19:00:03.000000 aioqui-2.1.0/src/aioqui/widgets/custom/state_button.py
--rw-rw-rw-   0        0        0     1445 2023-06-09 16:49:05.000000 aioqui-2.1.0/src/aioqui/widgets/custom/total_button.py
--rw-rw-rw-   0        0        0      963 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/date_time.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.396235 aioqui-2.1.0/src/aioqui/widgets/extensions/
--rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.1.0/src/aioqui/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0      746 2023-05-16 21:18:22.000000 aioqui-2.1.0/src/aioqui/widgets/extensions/input_ext.py
--rw-rw-rw-   0        0        0     1762 2023-06-10 15:34:21.000000 aioqui-2.1.0/src/aioqui/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      710 2023-05-16 21:18:22.000000 aioqui-2.1.0/src/aioqui/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1932 2023-06-10 12:16:32.000000 aioqui-2.1.0/src/aioqui/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      668 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/frame.py
--rw-rw-rw-   0        0        0     2314 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/input.py
--rw-rw-rw-   0        0        0     1348 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/label.py
--rw-rw-rw-   0        0        0     1328 2023-05-16 21:18:22.000000 aioqui-2.1.0/src/aioqui/widgets/layout.py
--rw-rw-rw-   0        0        0      375 2023-06-09 23:20:54.000000 aioqui-2.1.0/src/aioqui/widgets/panel.py
--rw-rw-rw-   0        0        0     1721 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1185 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/selector.py
--rw-rw-rw-   0        0        0      842 2023-05-16 21:16:52.000000 aioqui-2.1.0/src/aioqui/widgets/slider.py
--rw-rw-rw-   0        0        0      358 2023-06-10 00:17:15.000000 aioqui-2.1.0/src/aioqui/widgets/spacer.py
--rw-rw-rw-   0        0        0     1583 2023-06-10 15:26:55.000000 aioqui-2.1.0/src/aioqui/widgets/splitter.py
--rw-rw-rw-   0        0        0     1140 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.1.0/src/aioqui/widgets/statusbar.py
--rw-rw-rw-   0        0        0      595 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/widget.py
--rw-rw-rw-   0        0        0      594 2023-06-10 15:25:30.000000 aioqui-2.1.0/src/aioqui/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-06-10 15:41:02.115235 aioqui-2.1.0/src/aioqui.egg-info/
--rw-rw-rw-   0        0        0     2680 2023-06-10 15:41:02.000000 aioqui-2.1.0/src/aioqui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13439 2023-06-10 15:41:02.000000 aioqui-2.1.0/src/aioqui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 15:41:02.000000 aioqui-2.1.0/src/aioqui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-10 15:41:02.000000 aioqui-2.1.0/src/aioqui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-10 15:41:02.000000 aioqui-2.1.0/src/aioqui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.524554 aioqui-2.1.1/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2680 2023-06-10 15:50:55.523554 aioqui-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.1.1/README.md
+-rw-rw-rw-   0        0        0     1538 2023-06-10 15:50:36.000000 aioqui-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-10 15:50:55.524554 aioqui-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.235706 aioqui-2.1.1/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.1.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.240705 aioqui-2.1.1/src/aioqui/
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.229706 aioqui-2.1.1/src/aioqui/.assets/
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.477554 aioqui-2.1.1/src/aioqui/.assets/icons/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.1.1/src/aioqui/.assets/icons/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.1.1/src/aioqui/.assets/icons/zoom-out.svg
+-rw-rw-rw-   0        0        0      181 2023-06-09 15:58:57.000000 aioqui-2.1.1/src/aioqui/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-06-09 00:29:28.000000 aioqui-2.1.1/src/aioqui/asynq.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.479552 aioqui-2.1.1/src/aioqui/context/
+-rw-rw-rw-   0        0        0       71 2023-06-10 12:25:08.000000 aioqui-2.1.1/src/aioqui/context/__init__.py
+-rw-rw-rw-   0        0        0      501 2023-06-08 23:59:03.000000 aioqui-2.1.1/src/aioqui/context/context_api.py
+-rw-rw-rw-   0        0        0     9972 2023-06-10 15:34:57.000000 aioqui-2.1.1/src/aioqui/context/context_obj.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.484554 aioqui-2.1.1/src/aioqui/misc/
+-rw-rw-rw-   0        0        0      123 2023-06-10 12:26:25.000000 aioqui-2.1.1/src/aioqui/misc/__init__.py
+-rw-rw-rw-   0        0        0     3527 2023-06-09 22:36:04.000000 aioqui-2.1.1/src/aioqui/misc/aiorequest.py
+-rw-rw-rw-   0        0        0      975 2023-05-26 19:00:03.000000 aioqui-2.1.1/src/aioqui/misc/animation.py
+-rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.1.1/src/aioqui/misc/conthrq.py
+-rw-rw-rw-   0        0        0     1387 2023-06-10 12:25:08.000000 aioqui-2.1.1/src/aioqui/misc/fileops.py
+-rw-rw-rw-   0        0        0     2156 2023-06-10 12:25:08.000000 aioqui-2.1.1/src/aioqui/misc/qss_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.487553 aioqui-2.1.1/src/aioqui/types/
+-rw-rw-rw-   0        0        0       93 2023-05-16 21:16:03.000000 aioqui-2.1.1/src/aioqui/types/__init__.py
+-rw-rw-rw-   0        0        0      278 2023-06-10 12:25:08.000000 aioqui-2.1.1/src/aioqui/types/common.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.494553 aioqui-2.1.1/src/aioqui/types/enums/
+-rw-rw-rw-   0        0        0      294 2023-05-16 17:41:17.000000 aioqui-2.1.1/src/aioqui/types/enums/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.1.1/src/aioqui/types/enums/alignment.py
+-rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.1.1/src/aioqui/types/enums/echo_mode.py
+-rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.1.1/src/aioqui/types/enums/elide_mode.py
+-rw-rw-rw-   0        0        0      283 2023-05-16 17:57:41.000000 aioqui-2.1.1/src/aioqui/types/enums/logic_button.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.1.1/src/aioqui/types/enums/orientation.py
+-rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.1.1/src/aioqui/types/enums/scroll_policy.py
+-rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.1.1/src/aioqui/types/enums/size_policy.py
+-rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.1.1/src/aioqui/types/enums/window_hint.py
+-rw-rw-rw-   0        0        0     3595 2023-05-26 18:03:40.000000 aioqui-2.1.1/src/aioqui/types/icon.py
+-rw-rw-rw-   0        0        0      331 2023-05-15 15:26:00.000000 aioqui-2.1.1/src/aioqui/types/size.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.507554 aioqui-2.1.1/src/aioqui/widgets/
+-rw-rw-rw-   0        0        0      675 2023-06-09 23:49:23.000000 aioqui-2.1.1/src/aioqui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.513554 aioqui-2.1.1/src/aioqui/widgets/custom/
+-rw-rw-rw-   0        0        0      220 2023-06-09 00:40:35.000000 aioqui-2.1.1/src/aioqui/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     2230 2023-06-09 00:40:35.000000 aioqui-2.1.1/src/aioqui/widgets/custom/duration_label.py
+-rw-rw-rw-   0        0        0     2484 2023-06-09 23:31:11.000000 aioqui-2.1.1/src/aioqui/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     3176 2023-06-10 00:04:27.000000 aioqui-2.1.1/src/aioqui/widgets/custom/popup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.518554 aioqui-2.1.1/src/aioqui/widgets/custom/qss/
+-rw-rw-rw-   0        0        0      201 2023-06-09 23:42:41.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-16 20:25:11.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/colors.py
+-rw-rw-rw-   0        0        0     1491 2023-05-16 20:59:19.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/date_time.py
+-rw-rw-rw-   0        0        0      306 2023-05-16 21:06:26.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/image_button.py
+-rw-rw-rw-   0        0        0      829 2023-05-16 21:12:30.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/popup.py
+-rw-rw-rw-   0        0        0       24 2023-05-16 20:13:39.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/scrollbar.py
+-rw-rw-rw-   0        0        0      436 2023-05-16 20:17:25.000000 aioqui-2.1.1/src/aioqui/widgets/custom/qss/searchbar.py
+-rw-rw-rw-   0        0        0     1013 2023-06-09 16:22:55.000000 aioqui-2.1.1/src/aioqui/widgets/custom/searchbar.py
+-rw-rw-rw-   0        0        0     1736 2023-05-26 19:00:03.000000 aioqui-2.1.1/src/aioqui/widgets/custom/state_button.py
+-rw-rw-rw-   0        0        0     1445 2023-06-09 16:49:05.000000 aioqui-2.1.1/src/aioqui/widgets/custom/total_button.py
+-rw-rw-rw-   0        0        0      963 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/date_time.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.522553 aioqui-2.1.1/src/aioqui/widgets/extensions/
+-rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.1.1/src/aioqui/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-05-16 21:18:22.000000 aioqui-2.1.1/src/aioqui/widgets/extensions/input_ext.py
+-rw-rw-rw-   0        0        0     1995 2023-06-10 15:50:13.000000 aioqui-2.1.1/src/aioqui/widgets/extensions/layout_ext.py
+-rw-rw-rw-   0        0        0      710 2023-05-16 21:18:22.000000 aioqui-2.1.1/src/aioqui/widgets/extensions/side_menu_ext.py
+-rw-rw-rw-   0        0        0     1932 2023-06-10 12:16:32.000000 aioqui-2.1.1/src/aioqui/widgets/extensions/splitter_widget_ext.py
+-rw-rw-rw-   0        0        0      668 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/frame.py
+-rw-rw-rw-   0        0        0     2314 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/input.py
+-rw-rw-rw-   0        0        0     1348 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/label.py
+-rw-rw-rw-   0        0        0     1328 2023-05-16 21:18:22.000000 aioqui-2.1.1/src/aioqui/widgets/layout.py
+-rw-rw-rw-   0        0        0      375 2023-06-09 23:20:54.000000 aioqui-2.1.1/src/aioqui/widgets/panel.py
+-rw-rw-rw-   0        0        0     1721 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1185 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/selector.py
+-rw-rw-rw-   0        0        0      842 2023-05-16 21:16:52.000000 aioqui-2.1.1/src/aioqui/widgets/slider.py
+-rw-rw-rw-   0        0        0      358 2023-06-10 00:17:15.000000 aioqui-2.1.1/src/aioqui/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1583 2023-06-10 15:26:55.000000 aioqui-2.1.1/src/aioqui/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1140 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.1.1/src/aioqui/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/widget.py
+-rw-rw-rw-   0        0        0      594 2023-06-10 15:25:30.000000 aioqui-2.1.1/src/aioqui/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-06-10 15:50:55.245705 aioqui-2.1.1/src/aioqui.egg-info/
+-rw-rw-rw-   0        0        0     2680 2023-06-10 15:50:55.000000 aioqui-2.1.1/src/aioqui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13439 2023-06-10 15:50:55.000000 aioqui-2.1.1/src/aioqui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 15:50:55.000000 aioqui-2.1.1/src/aioqui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-10 15:50:55.000000 aioqui-2.1.1/src/aioqui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-10 15:50:55.000000 aioqui-2.1.1/src/aioqui.egg-info/top_level.txt
```

### Comparing `aioqui-2.1.0/LICENSE.txt` & `aioqui-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/PKG-INFO` & `aioqui-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.1.0
+Version: 2.1.1
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `aioqui-2.1.0/pyproject.toml` & `aioqui-2.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioqui"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "Asynchronous GUI framework based on PySide6"
```

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/aperture.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/cloud-drizzle.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/cloud-snow.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/codesandbox.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/cpu.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/figma.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/figma.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/film.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/film.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/github.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/life-buoy.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/loader.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/package.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/package.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-call.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-forwarded.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-incoming.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-missed.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-off.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone-outgoing.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/phone.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/settings.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/slack.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/sliders.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/sun.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/sunrise.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/sunset.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/wifi-off.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/.assets/icons/youtube.svg` & `aioqui-2.1.1/src/aioqui/.assets/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/asynq.py` & `aioqui-2.1.1/src/aioqui/asynq.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/context/context_obj.py` & `aioqui-2.1.1/src/aioqui/context/context_obj.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/misc/aiorequest.py` & `aioqui-2.1.1/src/aioqui/misc/aiorequest.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/misc/animation.py` & `aioqui-2.1.1/src/aioqui/misc/animation.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/misc/conthrq.py` & `aioqui-2.1.1/src/aioqui/misc/conthrq.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/misc/fileops.py` & `aioqui-2.1.1/src/aioqui/misc/fileops.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/misc/qss_parser.py` & `aioqui-2.1.1/src/aioqui/misc/qss_parser.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/types/enums/alignment.py` & `aioqui-2.1.1/src/aioqui/types/enums/alignment.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/types/icon.py` & `aioqui-2.1.1/src/aioqui/types/icon.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/__init__.py` & `aioqui-2.1.1/src/aioqui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/duration_label.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/duration_label.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/image_button.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/image_button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/popup.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/popup.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/qss/colors.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/qss/colors.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/qss/date_time.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/qss/date_time.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/qss/popup.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/qss/popup.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/searchbar.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/searchbar.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/state_button.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/state_button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/custom/total_button.py` & `aioqui-2.1.1/src/aioqui/widgets/custom/total_button.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/date_time.py` & `aioqui-2.1.1/src/aioqui/widgets/date_time.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/extensions/input_ext.py` & `aioqui-2.1.1/src/aioqui/widgets/extensions/input_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/extensions/layout_ext.py` & `aioqui-2.1.1/src/aioqui/widgets/extensions/layout_ext.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 from ...types import Alignment
 
 
 class LayoutExt(Alignment):
     async def init(
             self, *,
+            margins: tuple[int, int, int, int] = (0, 0, 0, 0), spacing: int = 0,  # do not remove, since default
             items: Sequence[QObject] = (),
             **kwargs
     ) -> 'LayoutExt':
+        self.setContentMargins(*margins)
+        self.setSpacing(spacing)
+        # add items according to the rule
         i = 0
         while i < len(items):
             if i + 1 < len(items) and isinstance(items[i + 1], (Qt.AlignmentFlag, Qt.Alignment)):
                 self.add(items[i], items[i + 1])
                 i += 1
             else:
                 self.add(items[i])
```

### Comparing `aioqui-2.1.0/src/aioqui/widgets/extensions/side_menu_ext.py` & `aioqui-2.1.1/src/aioqui/widgets/extensions/side_menu_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/extensions/splitter_widget_ext.py` & `aioqui-2.1.1/src/aioqui/widgets/extensions/splitter_widget_ext.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/frame.py` & `aioqui-2.1.1/src/aioqui/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/input.py` & `aioqui-2.1.1/src/aioqui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/label.py` & `aioqui-2.1.1/src/aioqui/widgets/label.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/layout.py` & `aioqui-2.1.1/src/aioqui/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/scroll_area.py` & `aioqui-2.1.1/src/aioqui/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/selector.py` & `aioqui-2.1.1/src/aioqui/widgets/selector.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/slider.py` & `aioqui-2.1.1/src/aioqui/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/splitter.py` & `aioqui-2.1.1/src/aioqui/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/stacked_widget.py` & `aioqui-2.1.1/src/aioqui/widgets/stacked_widget.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/widget.py` & `aioqui-2.1.1/src/aioqui/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui/widgets/window.py` & `aioqui-2.1.1/src/aioqui/widgets/window.py`

 * *Files identical despite different names*

### Comparing `aioqui-2.1.0/src/aioqui.egg-info/PKG-INFO` & `aioqui-2.1.1/src/aioqui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 2.1.0
+Version: 2.1.1
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `aioqui-2.1.0/src/aioqui.egg-info/SOURCES.txt` & `aioqui-2.1.1/src/aioqui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

