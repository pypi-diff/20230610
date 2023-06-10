# Comparing `tmp/daffi-2.2.0.tar.gz` & `tmp/daffi-2.2.1.tar.gz`

## Comparing `daffi-2.2.0.tar` & `daffi-2.2.1.tar`

### file list

```diff
@@ -1,216 +1,217 @@
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 daffi-2.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 daffi-2.2.0/mkdocs.yml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/test_and_validate.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/test_and_validate_staging.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/__about__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/__init__.py
--rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/async_result.py
--rwxr-xr-x   0        0        0     1824 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/exceptions.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/execution_modifiers.py
--rw-r--r--   0        0        0    15016 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/globals.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/interface.py
--rw-r--r--   0        0        0    19209 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/ipc.py
--rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/method_executors.py
--rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/remote_call.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/settings.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/signals.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/store.py
--rw-r--r--   0        0        0    15214 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/__init__.py
--rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/controller.py
--rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/node.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/__init__.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/channel_store.py
--rw-r--r--   0        0        0    19283 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/controller_operations.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/freezable_queue.py
--rw-r--r--   0        0        0    19083 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/node_operations.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/streams_store.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/task_waiter.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/ttl_store.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/message.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager.proto
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager_pb2.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager_pb2_grpc.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_alias.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_base.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_callback.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_fetcher.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_local.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/__init__.py
--rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_base.py
--rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_callback.py
--rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_fetcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/colors.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/custom_types.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/debug.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/func_validation.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/logger.py
--rw-r--r--   0        0        0     6775 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/misc.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/timeparse.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 daffi-2.2.0/docker/Dockerfile
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 daffi-2.2.0/docker/main.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/async-apps.md
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/execution-modifiers.md
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/global-object.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/index.md
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/node-and-controller.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/callback.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/fetcher.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/global.md
--rw-r--r--   0        0        0   233533 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/bg.jpg
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/controller-plus-node-arch.drawio
--rw-r--r--   0        0        0    27050 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/controller-plus-node-arch.png
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/gitter.png
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo-white-sm.png
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo-white.png
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo.png
--rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/many-controllers.drawio
--rw-r--r--   0        0        0    38251 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/many-controllers.png
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/pdf-file.png
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/stand-alone-controller-arch.drawio
--rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/stand-alone-controller-arch.png
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/js/extra.js
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/aliased-methods.md
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/asynchronous-execution.md
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/basic-example.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/bidirectional-communication.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/broadcasting.md
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/callback-additional-arguments.md
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/fetchers-with-body.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/function-transfer.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/named-processes.md
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/private-methods.md
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/scheduling-tasks.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/stream-callback-to-fetcher.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/stream-fetcher-to-callback.md
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/cert.pem
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/domains.ext
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/generate_certs.sh
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/key.pem
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/root_ca.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/root_key.pem
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/sign.csr
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/docker-compose.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/colorizer/Dockerfile
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/colorizer/main.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/email_processor/Dockerfile
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/email_processor/main.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/Dockerfile
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/app.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/templates/base.html
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/templates/index.html
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/consumer.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher1.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher2.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher3.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/consumer.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher1.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher2.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher3.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/callbacks_from_class/consumer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/callbacks_from_class/publisher.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/eta/consumer.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/eta/publisher.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/kill_all/consumer.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/kill_all/publisher.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/no_return/consumer.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/no_return/publisher.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/scheduler/consumer.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/scheduler/publisher.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/stream/consumer.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/stream/publisher.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/transfer_and_call/consumer.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/transfer_and_call/publisher.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc1.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc2.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc1.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc2.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc1.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc2.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_generator/class_consumer.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_generator/class_publisher.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callbacks_from_class/consumer.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callbacks_from_class/publisher.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/class_consumer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/class_publisher.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/consumer.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/publisher.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/fetcher_generator/class_consumer.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/fetcher_generator/class_publisher.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/no_return/consumer.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/no_return/publisher.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/scheduler/consumer.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/scheduler/publisher.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/stream/consumer.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/stream/publisher.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/transfer_and_call/consumer.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/transfer_and_call/publisher.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 daffi-2.2.0/scripts/generate_coverage_summary.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 daffi-2.2.0/scripts/write_coverage_summary_report.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_many_callbacks.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_many_nodes.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_period.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_pipeline.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_stream_callback_to_fetcher.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_stream_fetcher_to_callback.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_trio.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/broadcast.jinja2
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/callback_per_node.jinja2
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/many_callbacks.jinja2
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/period1.jinja2
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/pipeline.jinja2
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/pipeline2.jinja2
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/stream.jinja2
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/stream_from_callback.jinja2
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/test_trio.jinja2
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/async_callback.jinja2
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/base.jinja2
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/callback.jinja2
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/macros.jinja2
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_async_result.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_callback_and_fecher_classes.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_callback_decorator.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_fetcher_decorator.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_freezable_queue.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_logger.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_misc.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 daffi-2.2.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 daffi-2.2.0/README.md
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daffi-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     9288 2020-02-02 00:00:00.000000 daffi-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 daffi-2.2.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 daffi-2.2.1/mkdocs.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 daffi-2.2.1/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 daffi-2.2.1/.github/workflows/test_and_validate.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 daffi-2.2.1/.github/workflows/test_and_validate_staging.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/__about__.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/__init__.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/async_result.py
+-rwxr-xr-x   0        0        0     1824 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/exceptions.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/execution_modifiers.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/globals.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/interface.py
+-rw-r--r--   0        0        0    19563 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/ipc.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/method_executors.py
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/remote_call.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/settings.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/signals.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/store.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/well_known_callbacks.py
+-rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/__init__.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/controller.py
+-rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/node.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/channel_store.py
+-rw-r--r--   0        0        0    19283 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/controller_operations.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/freezable_queue.py
+-rw-r--r--   0        0        0    19172 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/node_operations.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/streams_store.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/task_waiter.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/operations/ttl_store.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/proto/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/proto/message.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/proto/messager.proto
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/proto/messager_pb2.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/components/proto/messager_pb2_grpc.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/_alias.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/_base.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/_callback.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/_fetcher.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/decorators/_local.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/registry/__init__.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/registry/_base.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/registry/_callback.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/registry/_fetcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/colors.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/custom_types.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/debug.py
+-rw-r--r--   0        0        0     2925 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/func_validation.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/logger.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/misc.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 daffi-2.2.1/daffi/utils/timeparse.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 daffi-2.2.1/docker/Dockerfile
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 daffi-2.2.1/docker/main.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/async-apps.md
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/execution-modifiers.md
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/global-object.md
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/index.md
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/node-and-controller.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/code-reference/callback.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/code-reference/fetcher.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/code-reference/global.md
+-rw-r--r--   0        0        0   233533 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/bg.jpg
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/controller-plus-node-arch.drawio
+-rw-r--r--   0        0        0    27050 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/controller-plus-node-arch.png
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/gitter.png
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/logo-white-sm.png
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/logo-white.png
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/logo.png
+-rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/many-controllers.drawio
+-rw-r--r--   0        0        0    38251 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/many-controllers.png
+-rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/pdf-file.png
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/stand-alone-controller-arch.drawio
+-rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/images/stand-alone-controller-arch.png
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/js/extra.js
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3698 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/aliased-methods.md
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/asynchronous-execution.md
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/basic-example.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/bidirectional-communication.md
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/broadcasting.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/callback-additional-arguments.md
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/fetchers-with-body.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/function-transfer.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/lifecycle-events.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/named-processes.md
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/private-methods.md
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/scheduling-tasks.md
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/ssl-certificates.md
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/stream-callback-to-fetcher.md
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 daffi-2.2.1/docs/usage/stream-fetcher-to-callback.md
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/certs/cert.pem
+-rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/certs/generate_certs.sh
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/certs/key.pem
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/docker-compose.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/colorizer/Dockerfile
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/colorizer/main.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/email_processor/Dockerfile
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/email_processor/main.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/web/Dockerfile
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/web/app.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/web/templates/base.html
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/docker/web/templates/index.html
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/classes_based/consumer.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/classes_based/publisher1.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/classes_based/publisher2.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/classes_based/publisher3.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/decorators_based/consumer.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/decorators_based/publisher1.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/decorators_based/publisher2.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/opencv_stream/decorators_based/publisher3.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/callbacks_from_class/consumer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/callbacks_from_class/publisher.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/eta/consumer.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/eta/publisher.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/kill_all/consumer.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/kill_all/publisher.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/no_return/consumer.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/no_return/publisher.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/scheduler/consumer.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/scheduler/publisher.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/stream/consumer.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/stream/publisher.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/transfer_and_call/consumer.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/transfer_and_call/publisher.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication/class_based/proc1.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication/class_based/proc2.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc1.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc2.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_and_fetcher_decorator/consumer.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_and_fetcher_decorator/publisher.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_generator/class_consumer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callback_generator/class_publisher.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callbacks_from_class/consumer.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/callbacks_from_class/publisher.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/eta/class_consumer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/eta/class_publisher.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/eta/consumer.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/eta/publisher.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/fetcher_generator/class_consumer.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/fetcher_generator/class_publisher.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/no_return/consumer.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/no_return/publisher.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/scheduler/consumer.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/scheduler/publisher.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/stream/consumer.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/stream/publisher.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/transfer_and_call/consumer.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/transfer_and_call/publisher.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication/class_based/proc1.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication/class_based/proc2.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 daffi-2.2.1/scripts/generate_coverage_summary.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 daffi-2.2.1/scripts/write_coverage_summary_report.py
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/__init__.py
+-rwxr-xr-x   0        0        0     1990 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/conftest.py
+-rwxr-xr-x   0        0        0     1624 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/conftest.py
+-rwxr-xr-x   0        0        0     2576 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_broadcast.py
+-rwxr-xr-x   0        0        0     5618 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_many_callbacks.py
+-rwxr-xr-x   0        0        0     5243 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_many_nodes.py
+-rwxr-xr-x   0        0        0     2230 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_period.py
+-rwxr-xr-x   0        0        0     4044 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_pipeline.py
+-rwxr-xr-x   0        0        0     3934 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_stream_callback_to_fetcher.py
+-rwxr-xr-x   0        0        0     3414 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_stream_fetcher_to_callback.py
+-rwxr-xr-x   0        0        0     2110 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/test_trio.py
+-rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/broadcast.jinja2
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/callback_per_node.jinja2
+-rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/many_callbacks.jinja2
+-rwxr-xr-x   0        0        0      339 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/period1.jinja2
+-rwxr-xr-x   0        0        0      383 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/pipeline.jinja2
+-rwxr-xr-x   0        0        0      401 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/pipeline2.jinja2
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/stream.jinja2
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/stream_from_callback.jinja2
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/test_trio.jinja2
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/layout/async_callback.jinja2
+-rwxr-xr-x   0        0        0      745 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/layout/base.jinja2
+-rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/layout/callback.jinja2
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/integration/templates/layout/macros.jinja2
+-rwxr-xr-x   0        0        0     2827 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_async_result.py
+-rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_callback_and_fecher_classes.py
+-rwxr-xr-x   0        0        0     2971 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_callback_decorator.py
+-rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_fetcher_decorator.py
+-rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_freezable_queue.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_function_validation.py
+-rwxr-xr-x   0        0        0     2036 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_logger.py
+-rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_misc.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 daffi-2.2.1/tests/unit/test_multi_inheritence_prohibited.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 daffi-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 daffi-2.2.1/README.md
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daffi-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10099 2020-02-02 00:00:00.000000 daffi-2.2.1/PKG-INFO
```

### Comparing `daffi-2.2.0/CHANGELOG.rst` & `daffi-2.2.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/mkdocs.yml` & `daffi-2.2.1/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     - private methods: usage/private-methods.md
     - aliased methods: usage/aliased-methods.md
     - named processes: usage/named-processes.md
     - stream from fetcher to callback: usage/stream-fetcher-to-callback.md
     - stream from callback to fetcher: usage/stream-callback-to-fetcher.md
     - function transfer: usage/function-transfer.md
     - bidirectional communication: usage/bidirectional-communication.md
+    - SSL certificates: usage/ssl-certificates.md
+    - lifecycle events: usage/lifecycle-events.md
     - asynchronous execution: usage/asynchronous-execution.md
     - broadcasting: usage/broadcasting.md
     - task scheduling and batch delayed execution: usage/scheduling-tasks.md
   - Node and Controller: node-and-controller.md
   - Global object: global-object.md
   - Asynchronous applications: async-apps.md
   - Execution modifiers: execution-modifiers.md
```

### Comparing `daffi-2.2.0/.github/workflows/test_and_validate.yml` & `daffi-2.2.1/.github/workflows/test_and_validate.yml`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/.github/workflows/test_and_validate_staging.yml` & `daffi-2.2.1/.github/workflows/test_and_validate_staging.yml`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/async_result.py` & `daffi-2.2.1/daffi/async_result.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/exceptions.py` & `daffi-2.2.1/daffi/exceptions.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/execution_modifiers.py` & `daffi-2.2.1/daffi/execution_modifiers.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/interface.py` & `daffi-2.2.1/daffi/interface.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/ipc.py` & `daffi-2.2.1/daffi/ipc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import sys
 from itertools import chain
 from logging import Logger
+from asyncio.exceptions import CancelledError
 from inspect import iscoroutinefunction
 from threading import Thread, Event
 from concurrent.futures import ThreadPoolExecutor
 from typing import NoReturn, Dict, Union, Optional, Callable, Any, Tuple, AsyncGenerator
 
 from anyio.from_thread import start_blocking_portal
 
@@ -23,34 +24,38 @@
     search_remote_callback_in_mapping,
     resilent,
     ConditionEvent,
     async_library,
     iterable,
 )
 from daffi.utils.func_validation import pretty_callbacks
+from daffi.registry._base import BaseRegistry
+from daffi.decorators._base import Decorator
 from daffi.settings import LOCAL_CALLBACK_MAPPING, WELL_KNOWN_CALLBACKS, clear_method_type_stores
 
 
 class Ipc(Thread):
     def __init__(
         self,
+        g: "Global",
         process_name: str,
         init_controller: bool,
         init_node: bool,
         global_terminate_event: Event,
         host: Optional[str] = None,
         port: Optional[int] = None,
         unix_sock_path: Optional[os.PathLike] = None,
         ssl_certificate: Optional[os.PathLike] = None,
         ssl_key: Optional[os.PathLike] = None,
         on_node_connect: Optional[Callable[["Global", str], Any]] = None,
         on_node_disconnect: Optional[Callable[["Global", str], Any]] = None,
         logger: Logger = None,
     ):
         super().__init__()
+        self.g = g
         self.process_name = process_name
         self.init_controller = init_controller
         self.init_node = init_node
         self.global_terminate_event = global_terminate_event
         self.host = host
         self.port = port
         self.unix_sock_path = unix_sock_path
@@ -62,15 +67,16 @@
         self.async_backend = async_library()
 
         self.daemon = True
         self.global_condition_event = ConditionEvent()
         self.controller = self.node = None
         self.task_waiter = TaskWaiter(process_name)
 
-        AsyncResult._ipc = self
+        AsyncResult._ipc = BaseRegistry._ipc = self
+        BaseRegistry._g = Decorator._g = self.g
 
         if not (self.init_controller or self.init_node):
             InitializationError("At least one of 'init_controller' or 'init_node' must be True.").fire()
 
         if self.on_node_connect and iscoroutinefunction(self.on_node_connect):
             raise InitializationError("`on_node_connect` callback should not be an asynchronous function.")
         if self.on_node_disconnect and iscoroutinefunction(self.on_node_disconnect):
@@ -111,14 +117,20 @@
         return_result: Optional[bool] = True,
         func_period: Optional[Period] = None,
         broadcast: Optional[bool] = False,
         stream: Optional[bool] = False,
         receiver: Optional[str] = None,
     ):
         self._check_node()
+
+        if not self.is_running:
+            # In case IPC thread is not initialized yet and fetchers cannot be used at this moment.
+            self.logger.info("Wait IPC initialization...")
+            self.global_condition_event.wait_any_status()
+
         data = search_remote_callback_in_mapping(self.node.node_callback_mapping, func_name, exclude=self.process_name)
 
         if not data:
             # Get all callbacks without local
             available_callbacks = pretty_callbacks(
                 mapping=self.node.node_callback_mapping, exclude_proc=self.process_name, format="string"
             )
@@ -204,19 +216,20 @@
 
         # TODO add windows support
         if sys.platform == "win32":
             backend_options = {}
         else:
             backend_options = {"use_uvloop": True}
         c_future = n_future = tw_future = None
-        with resilent(RuntimeError):
+        with resilent((RuntimeError, CancelledError)):
             Controller.components.clear()
             with start_blocking_portal(backend="asyncio", backend_options=backend_options) as portal:
                 if self.init_controller:
                     self.controller = Controller(
+                        g=self.g,
                         process_name=self.process_name,
                         host=self.host,
                         port=self.port,
                         global_terminate_event=self.global_terminate_event,
                         on_node_disconnect=self.on_node_disconnect,
                         ssl_certificate=self.ssl_certificate,
                         ssl_key=self.ssl_key,
@@ -227,14 +240,15 @@
                         name=Controller.__class__.__name__,
                     )
                     self.port = getattr(self.controller, "port", None)
                     self.unix_sock_path = getattr(self.controller, "unix_sock_path", None)
 
                 if self.init_node:
                     self.node = Node(
+                        g=self.g,
                         process_name=self.process_name,
                         host=self.host,
                         port=self.port,
                         async_backend=self.async_backend,
                         global_terminate_event=self.global_terminate_event,
                         on_node_connect=self.on_node_connect,
                         ssl_certificate=self.ssl_certificate,
@@ -271,94 +285,89 @@
             self.global_condition_event.mark_fail()
 
         clear_method_type_stores()
 
     def stream(self, func_name: str, receiver: Optional[str], args: Tuple) -> NoReturn:
         from daffi.registry._fetcher import Args
 
-        if self.is_running:
-            self._check_node()
+        if len(args) != 1:
+            InitializationError(
+                "Pass exactly 1 positional argument to initialize stream."
+                f" It can be list, tuple generator or any iterable. Provided args: {args}. Provided args len: {len(args)}"
+            ).fire()
+        stream_items = args[0]
+        if not iterable(stream_items):
+            if isinstance(stream_items, AsyncGenerator):
+                InitializationError(f"Async generators are not supported yet.").fire()
+            InitializationError(
+                f"Stream support only iterable objects like lists, tuples, generators etc. "
+                f"You provided {stream_items} as argument."
+            ).fire()
 
-            if len(args) != 1:
-                InitializationError(
-                    "Pass exactly 1 positional argument to initialize stream."
-                    f" It can be list, tuple generator or any iterable. Provided args: {args}. Provided args len: {len(args)}"
-                ).fire()
-            stream_items = args[0]
-            if not iterable(stream_items):
-                if isinstance(stream_items, AsyncGenerator):
-                    InitializationError(f"Async generators are not supported yet.").fire()
-                InitializationError(
-                    f"Stream support only iterable objects like lists, tuples, generators etc. "
-                    f"You provided {stream_items} as argument."
-                ).fire()
-
-            stream_items = iter(stream_items)
-            try:
-                first_item = next(stream_items)
-            except StopIteration:
-                InitializationError("Stream is empty").fire()
+        stream_items = iter(stream_items)
+        try:
+            first_item = next(stream_items)
+        except StopIteration:
+            InitializationError("Stream is empty").fire()
 
-            data = search_remote_callback_in_mapping(
-                self.node.node_callback_mapping, func_name, exclude=self.process_name
-            )
-            _, remote_callback = data
-            if remote_callback.is_generator:
-                InitializationError(
-                    f"Stream don't work with remote callback which are generators."
-                    f" Check {remote_callback.alias} to fix this issue."
-                ).fire()
-
-            args, kwargs = Args._aggregate_args(args=first_item)
-            remote_callback.validate_provided_arguments(*args, **kwargs)
-            stream_items = chain([first_item], stream_items)
+        data = search_remote_callback_in_mapping(self.node.node_callback_mapping, func_name, exclude=self.process_name)
+        _, remote_callback = data
+        if remote_callback.is_generator:
+            InitializationError(
+                f"Stream don't work with remote callback which are generators."
+                f" Check {remote_callback.alias} to fix this issue."
+            ).fire()
 
-            msg = RpcMessage(
-                flag=MessageFlag.INIT_STREAM,
-                transmitter=self.process_name,
-                func_name=func_name,
-            )
-            # Register result in order to obtain all available receivers
-            result = self.node.send_and_register_result(msg=msg)
+        args, kwargs = Args._aggregate_args(args=first_item)
+        remote_callback.validate_provided_arguments(*args, **kwargs)
+        stream_items = chain([first_item], stream_items)
 
-            self.logger.debug("Wait available stream receivers")
-            receivers = result.get()
-            if not receivers:
-                InitializationError("Unable to find receivers for stream.").fire()
-            elif receiver and receiver not in receivers:
-                InitializationError(
-                    f"Provided receiver is not in the list of available receivers for fuction {func_name}."
-                    f" Available receivers = {receivers}"
-                ).fire()
-            elif receiver:
-                receivers = [receiver]
-
-            # Register the same result second time to track stream errors (If happened)
-            result = result._clone_and_register()
-            stream_pair_was_closed = False
-            with self.node.stream_store.request_multi_connection(
-                receivers=receivers, msg_uuid=str(msg.uuid)
-            ) as stream_pair_group:
-                for stream_item in stream_items:
-                    if stream_pair_group.closed:
-                        stream_pair_was_closed = True
-                        break
-                    # Convert stream item to args, kwargs
-                    args, kwargs = Args._aggregate_args(args=stream_item)
-                    for msg in ServiceMessage.build_stream_message(data=(args, kwargs)):
-                        stream_pair_group.send_threadsave(msg)
-            # Wait all receivers to finish stream processing.
-            self.logger.debug("Stream closed. Wait for confirmation from receivers...")
-
-            result.get()
-            if stream_pair_was_closed:
-                raise GlobalContextError(
-                    "Stream was closed unexpectedly. Seems payload is too big."
-                    " Please adjust payload size or consider using unary exec modifiers FG, BG etc."
-                )
+        msg = RpcMessage(
+            flag=MessageFlag.INIT_STREAM,
+            transmitter=self.process_name,
+            func_name=func_name,
+        )
+        # Register result in order to obtain all available receivers
+        result = self.node.send_and_register_result(msg=msg)
+
+        self.logger.debug("Wait available stream receivers")
+        receivers = result.get()
+        if not receivers:
+            InitializationError("Unable to find receivers for stream.").fire()
+        elif receiver and receiver not in receivers:
+            InitializationError(
+                f"Provided receiver is not in the list of available receivers for fuction {func_name}."
+                f" Available receivers = {receivers}"
+            ).fire()
+        elif receiver:
+            receivers = [receiver]
+
+        # Register the same result second time to track stream errors (If happened)
+        result = result._clone_and_register()
+        stream_pair_was_closed = False
+        with self.node.stream_store.request_multi_connection(
+            receivers=receivers, msg_uuid=str(msg.uuid)
+        ) as stream_pair_group:
+            for stream_item in stream_items:
+                if stream_pair_group.closed:
+                    stream_pair_was_closed = True
+                    break
+                # Convert stream item to args, kwargs
+                args, kwargs = Args._aggregate_args(args=stream_item)
+                for msg in ServiceMessage.build_stream_message(data=(args, kwargs)):
+                    stream_pair_group.send_threadsave(msg)
+        # Wait all receivers to finish stream processing.
+        self.logger.debug("Stream closed. Wait for confirmation from receivers...")
+
+        result.get()
+        if stream_pair_was_closed:
+            raise GlobalContextError(
+                "Stream was closed unexpectedly. Seems payload is too big."
+                " Please adjust payload size or consider using unary exec modifiers FG, BG etc."
+            )
 
     def update_callbacks(self) -> NoReturn:
         if self.node:
             local_mapping_without_well_known_callbacks = {
                 k: v.simplified() for k, v in LOCAL_CALLBACK_MAPPING.items() if k not in WELL_KNOWN_CALLBACKS
             }
             self.node.send_threadsave(
@@ -439,14 +448,17 @@
         if args:
             sig_num = args[0]
             sig_name = SIGNALS_TO_NAMES_DICT[sig_num]
             self.logger.warning(f"Terminated by signal {sig_name!r}")
 
         self.global_terminate_event.set()
         self.join()
+        # reset all class variables
+        AsyncResult._ipc = BaseRegistry._ipc = None
+        BaseRegistry._g = Decorator._g = None
 
     def _check_node(self) -> NoReturn:
         if not self.node:
             GlobalContextError(
                 "Support for invoking remote calls is not enabled"
                 " The node has not been initialized in the current process."
                 " Make sure you passed 'init_node' = True in Global object."
```

### Comparing `daffi-2.2.0/daffi/method_executors.py` & `daffi-2.2.1/daffi/method_executors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import time
-import logging
 from inspect import Signature
 from typing import NamedTuple, Union
 
 import daffi
 from daffi.utils.misc import Singleton
-from daffi.exceptions import GlobalContextError, InitializationError
+from daffi.exceptions import GlobalContextError
 from daffi.utils.custom_types import GlobalCallback, P, RemoteResult
 from daffi.execution_modifiers import FG, BG, BROADCAST, PERIOD
 from daffi.settings import LOCAL_FETCHER_MAPPING, LOCAL_CALLBACK_MAPPING
 
 __all__ = ["CallbackExecutor", "ClassCallbackExecutor", "FetcherExecutor", "ClassFetcherExecutor"]
 
 # ----------------------------------------------------------------------------------------------------------------------
@@ -136,50 +134,33 @@
 # ----------------------------------------------------------------------------------------------------------------------
 # Fetcher types
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 def f__call__(self, *args, **kwargs) -> RemoteResult:
     """Trigger executor with assigned execution modifier."""
-    # Get remote call by name
-    for attempt in range(5):
-        try:
-            # In case fetcher is using too early after application start.
-            # `Global` object might be not initialized at this moment.
-            g = _g()
-            break
-        except InitializationError:
-            # Keep fist attempt silent
-            if attempt > 1:
-                logging.error("Global object is not initialized. Awaiting...")
-            time.sleep(2)
-    else:
-        raise InitializationError("Global object initialization is missing!")
-
+    g = Singleton._get_self("Global")
     remote_call = getattr(g.call, self.alias)
     # Set fetcher
     remote_call._fetcher = self
     # Execute remote call
     return (remote_call & self.exec_modifier)(*args, **kwargs)
 
 
 def call(self, *args, exec_modifier: Union[FG, BG, BROADCAST, PERIOD] = FG, **kwargs):
     """Trigger executor with execution modifier provided in arguments."""
     # Get remote call by name
-    remote_call = getattr(_g().call, self.alias)
+    g = Singleton._get_self("Global")
+    remote_call = getattr(g.call, self.alias)
     # Set fetcher
     remote_call._fetcher = self
     # Execute remote call
     return (remote_call & exec_modifier)(*args, **kwargs)
 
 
-def _g() -> "Global":
-    return Singleton._get_self("Global")
-
-
 @property
 def proxy(self):
     return self.proxy_
 
 
 @proxy.setter
 def proxy(self, val):
```

### Comparing `daffi-2.2.0/daffi/remote_call.py` & `daffi-2.2.1/daffi/remote_call.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/settings.py` & `daffi-2.2.1/daffi/settings.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/store.py` & `daffi-2.2.1/daffi/store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/__init__.py` & `daffi-2.2.1/daffi/components/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from grpc import aio, ChannelConnectivity, ssl_channel_credentials, ssl_server_credentials
 from anyio.abc import TaskStatus
 from grpc.aio._call import AioRpcError
 from anyio import TASK_STATUS_IGNORED
 from tenacity import AsyncRetrying, wait_fixed, retry_if_exception_type, RetryCallState, wait_none
 
-from daffi.exceptions import StopComponentError, ControllerUnavailable, InitializationError, RemoteCallError
+from daffi.exceptions import StopComponentError, ControllerUnavailable, RemoteCallError
 from daffi.interface import ComponentI
 from daffi.components.proto import messager_pb2_grpc as grpc_messager
 from daffi.utils.misc import string_uuid
 
 
 class UnixBase(ComponentI, grpc_messager.MessagerServiceServicer):
     SOCK_FILE = ".sock"
@@ -155,34 +155,36 @@
     STOP_ACTION_ERRORS = (StopComponentError,)
 
     logger: logging.Logger = None
     components: ClassVar[Set[Callable]] = set()
 
     def __init__(
         self,
+        g: "Global",
         process_name: str,
         host: Optional[str] = None,
         port: Optional[int] = None,
         unix_sock_path: Optional[os.PathLike] = None,
         ssl_certificate: Optional[os.PathLike] = None,
         ssl_key: Optional[os.PathLike] = None,
         async_backend: Optional[str] = None,
         global_terminate_event: Optional[thEvent] = None,
         on_node_connect: Optional[Callable[["Global", str], Any]] = None,
         on_node_disconnect: Optional[Callable[["Global", str], Any]] = None,
     ):
         self._set_keyboard_interrupt_handler()
 
+        self.g = g
         self.process_name = process_name
         self.async_backend = async_backend or "asyncio"
         self.operations = None
         self.ident = string_uuid()
         self.global_terminate_event = global_terminate_event
-        self.on_node_connect = on_node_connect
-        self.on_node_disconnect = on_node_disconnect
+        self.on_node_connect_cbs = [self.on_node_connect, on_node_connect]
+        self.on_node_disconnect_cbs = [self.on_node_disconnect, on_node_disconnect]
         self._stopped = self._connected = False
         self.stop_event: bool = False
         self.stop_callbacks: List[Callable] = []
 
         self.components.add(self)
 
         if host:  # Check only host. Full host/port validation already took place before.
@@ -207,14 +209,28 @@
     async def before_connect(self) -> NoReturn:
         raise NotImplementedError
 
     async def on_stop(self) -> NoReturn:
         while not self.stop_event:
             await asyncio.sleep(0.3)
 
+    def on_node_connect(self, _, process_name: str):
+        """
+        Default on node connect event handler.
+        executed each time when connection to Controller is established
+        """
+        self.logger.info(f"Node {process_name!r} has been connected to Controller")
+
+    def on_node_disconnect(self, _, process_name: str):
+        """
+        Default on node disconnect event handler.
+        executed each time when connection to Controller is lost
+        """
+        self.logger.info(f"Node {process_name!r} has been disconnected")
+
     async def on_terminate(self):
         self.logger.info(f"{self.__class__.__name__} stopped.")
         self._stopped = True
         self.components.discard(self)
         if not self.components:
             # Cancel all existing asyncio tasks if component is the last one in termination chain. Eg if controller
             # is running along with node then controller will be in charge of cleaning.
@@ -254,54 +270,39 @@
             raise StopComponentError()
         listener = await self._base.create_listener(self)
         self._connected = True
         return listener
 
     async def execute_on_connect(self):
         """Execute `on_connect` lifecycle handler in separate thread to prevent blocking main message handler."""
-        if self.on_node_connect:
-            # Execute `on_connect` lifecycle event in case such handler exists.
-            def _on_connect_wrapper(retry=True):
-                from daffi import get_g
-
-                while True:
-                    try:
-                        g = get_g()
-                        break
-                    except InitializationError:
-                        time.sleep(0.1)
+
+        def _on_connect_wrapper():
+            # In case IPC is not ready yet.
+            self.g.ipc.global_condition_event.wait_any_status()
+            for cb in filter(None, self.on_node_connect_cbs):
                 try:
-                    self.on_node_connect(g, self.process_name)
+                    cb(self.g, self.process_name)
                 except Exception as e:
-                    if isinstance(e, RemoteCallError) and retry:
-                        # another attempt to run the callback is allowed
-                        # if the error is related to access to a remote process
-                        time.sleep(1)
-                        return _on_connect_wrapper(retry=False)
                     self.logger.error(
                         f"Exception occurred while execution `on_node_connect` handler: {e}, type: {type(e)}"
                     )
 
-            Thread(target=_on_connect_wrapper).start()
+        Thread(target=_on_connect_wrapper).start()
 
     async def execute_on_disconnect(self, process_name):
-        if self.on_node_disconnect:
-
-            def _on_disconnect_wrapper():
-                from daffi import get_g
-
-                g = get_g()
+        def _on_disconnect_wrapper():
+            for cb in filter(None, self.on_node_disconnect_cbs):
                 try:
-                    self.on_node_disconnect(g, process_name)
+                    cb(self.g, process_name)
                 except Exception as e:
                     self.logger.error(
                         f"Exception occurred while execution `on_node_disconnect` handler: {e}, type: {type(e)}"
                     )
 
-            Thread(target=_on_disconnect_wrapper).start()
+        Thread(target=_on_disconnect_wrapper).start()
 
     def after_exception(self, retry_state: RetryCallState):
         """return the result of the last call attempt"""
 
         retry_object = retry_state.retry_object
         attempt = retry_state.attempt_number
         exception = retry_state.outcome.exception()
```

### Comparing `daffi-2.2.0/daffi/components/controller.py` & `daffi-2.2.1/daffi/components/controller.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/node.py` & `daffi-2.2.1/daffi/components/node.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/scheduler.py` & `daffi-2.2.1/daffi/components/scheduler.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/channel_store.py` & `daffi-2.2.1/daffi/components/operations/channel_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/controller_operations.py` & `daffi-2.2.1/daffi/components/operations/controller_operations.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/freezable_queue.py` & `daffi-2.2.1/daffi/components/operations/freezable_queue.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/node_operations.py` & `daffi-2.2.1/daffi/components/operations/node_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
         prompting new attempts to establish a connection with the controller.
         """
         while True:
             await asyncio.sleep(5)
             time_since_last_ping = time.time() - self.last_ping_ts
             self.logger.debug(f"Time since last ping: {time_since_last_ping}")
             if time_since_last_ping > 15:
+                self.logger.error("No ping from Controller received during 15 seconds.")
                 self.on_remote_error()
                 await sg.cancel_scope.cancel()
                 sg.cancel_scope.deadline = 1
                 break
 
     def on_remote_error(self):
         err = RemoteError(
```

### Comparing `daffi-2.2.0/daffi/components/operations/streams_store.py` & `daffi-2.2.1/daffi/components/operations/streams_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/task_waiter.py` & `daffi-2.2.1/daffi/components/operations/task_waiter.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/operations/ttl_store.py` & `daffi-2.2.1/daffi/components/operations/ttl_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/proto/message.py` & `daffi-2.2.1/daffi/components/proto/message.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/proto/messager.proto` & `daffi-2.2.1/daffi/components/proto/messager.proto`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/proto/messager_pb2.py` & `daffi-2.2.1/daffi/components/proto/messager_pb2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/components/proto/messager_pb2_grpc.py` & `daffi-2.2.1/daffi/components/proto/messager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/decorators/_base.py` & `daffi-2.2.1/daffi/decorators/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from daffi.utils.custom_types import GlobalCallback, P, RemoteResult
 
 
 class Decorator(Generic[GlobalCallback]):
 
     _fn: GlobalCallback = None
     _store: dict
+    _g: "Global" = None
 
     @abstractmethod
     def __init__(self, fn: Callable[P, Any]):
         ...  # no cov
 
     __call__: GlobalCallback
     __getattr__: Union[RemoteResult, Any]
@@ -44,7 +45,11 @@
 
     @alias.setter
     def alias(self, val):
         """Assign new value for alias."""
         self._fn.alias = val
         # Take updated namedtuple instance from store
         self._fn = self._store[val]
+
+    @property
+    def g(self):
+        return self._g
```

### Comparing `daffi-2.2.0/daffi/decorators/_callback.py` & `daffi-2.2.1/daffi/decorators/_callback.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/decorators/_fetcher.py` & `daffi-2.2.1/daffi/decorators/_fetcher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/registry/_base.py` & `daffi-2.2.1/daffi/registry/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Type, Tuple, Dict, ClassVar, Callable, Optional
 
-from daffi.ipc import Ipc
 from daffi.utils import colors
 from daffi.utils.logger import get_daffi_logger
+from daffi.exceptions import InitializationError
 
 logger = get_daffi_logger("registry", colors.blue)
 
 _base_class_defined = False
 
 
 class RegistryMeta(ABCMeta):
@@ -25,25 +25,27 @@
 
                 for _cls in bases:
                     if hasattr(_cls, "__daffi_mro__"):
                         # Take `__daffi_mro__` from base class if exists.
                         daffi_mro.extend(_cls.__daffi_mro__)
 
                     if _cls in _registry_methods and _cls not in daffi_mro:
-                        daffi_mro.append(_cls)
+                        if not daffi_mro:
+                            daffi_mro.append(_cls)
+                        else:
+                            InitializationError(
+                                f"Inheritance for a class {cls_name!r} can be derived from either"
+                                f" {Fetcher} or {Callback}. Multiple inheritance is prohibited."
+                            ).fire()
 
                 if (auto_init := namespace.get("auto_init", None)) is None:
                     for base in bases:
                         if (auto_init := getattr(base, "auto_init", None)) is not None:
                             namespace.update(auto_init=auto_init)
                             break
-            if len(daffi_mro) == 2:
-                # Disable auto init forcibly if class is inherited from both `Callback` and `Fetcher`
-                auto_init = False
-                namespace.update(auto_init=auto_init)
             # Store all parent daffi classes to `__daffi_mro__` class attribute
             namespace.update(__daffi_mro__=daffi_mro)
             cls = _type = super().__new__(mcs, cls_name, bases, namespace, **kwargs)  # type: ignore
 
             if not is_registry_class:
                 if auto_init:
                     _type = _type()
@@ -64,25 +66,30 @@
     __doc__ = ""  # Null out the Representation docstring
 
     def __str__(self):
         return f"{self.__class__.__name__}<{', '.join([cl.__name__ for cl in getattr(self, '__daffi_mro__', [])])}>"
 
     __repr__ = __str__
 
-    _ipc: ClassVar[Ipc] = None
+    _ipc: ClassVar["Ipc"] = None
+    _g: ClassVar["Global"] = None
 
     def __init__(self):
         for base in self.__daffi_mro__:
             base._post_init(self)
         self.__post_init__()
 
     def __post_init__(self):
         """For additional user specific initialization"""
         pass
 
+    @property
+    def g(self):
+        return self._g
+
     @staticmethod
     @abstractmethod
     def _init_class(cls, instance_or_type):
         raise NotImplementedError()
 
     @classmethod
     @abstractmethod
```

### Comparing `daffi-2.2.0/daffi/registry/_callback.py` & `daffi-2.2.1/daffi/registry/_callback.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/registry/_fetcher.py` & `daffi-2.2.1/daffi/registry/_fetcher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/utils/colors.py` & `daffi-2.2.1/daffi/utils/colors.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/utils/debug.py` & `daffi-2.2.1/daffi/utils/debug.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/utils/func_validation.py` & `daffi-2.2.1/daffi/utils/func_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,20 +85,11 @@
         name = func.func_name
     elif hasattr(func, "__name__"):
         name = func.__name__
     elif hasattr(func, "origin_name_"):
         name = func.origin_name_
     else:
         raise InitializationError(
-            "Unable to retrieve fetcher name. If you have applied additional decorators"
+            "Unable to retrieve fetcher/callback name. If you have applied additional decorators"
             " to the decorated function consider modifying the order of the decorators."
         )
-    # Hack to detect functions not defined at the module-level
-    if hasattr(func, "func_globals") and name in func.func_globals:
-        if func.func_globals[name] is not func:
-            name = "%s-alias" % name
-    if inspect.ismethod(func):
-        # We need to add the name of the class
-        if hasattr(func, "im_class"):
-            klass = func.im_class
-            module.append(klass.__name__)
     return module, name
```

### Comparing `daffi-2.2.0/daffi/utils/logger.py` & `daffi-2.2.1/daffi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/daffi/utils/misc.py` & `daffi-2.2.1/daffi/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from uuid import uuid4
 from random import choice
 from functools import partial
 from datetime import datetime
 from queue import Queue
 from contextlib import contextmanager
 from collections.abc import Iterable
+from threading import Event
 from typing import (
     Callable,
     Any,
     NamedTuple,
     NoReturn,
     Dict,
     DefaultDict,
@@ -75,29 +76,34 @@
 
 class ConditionEvent:
     """Register Event objects and wait for release when any of them is set"""
 
     def __init__(self):
         self._cond_q = Queue(maxsize=1)
         self._is_success = False
+        self._done_event = Event()
 
     @property
     def success(self) -> bool:
         return self._is_success
 
     def mark_success(self) -> NoReturn:
         self._cond_q.put(True)
 
     def mark_fail(self) -> NoReturn:
         self._cond_q.put(False)
 
     def wait(self) -> bool:
         self._is_success = self._cond_q.get()
+        self._done_event.set()
         return self._is_success
 
+    def wait_any_status(self):
+        self._done_event.wait()
+
 
 class Singleton(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls.__name__ not in cls._instances:
             cls._instances[cls.__name__] = super(Singleton, cls).__call__(*args, **kwargs)
```

### Comparing `daffi-2.2.0/daffi/utils/timeparse.py` & `daffi-2.2.1/daffi/utils/timeparse.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/async-apps.md` & `daffi-2.2.1/docs/async-apps.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/execution-modifiers.md` & `daffi-2.2.1/docs/execution-modifiers.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/global-object.md` & `daffi-2.2.1/docs/global-object.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/index.md` & `daffi-2.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,36 +17,47 @@
 [![Downloads](https://static.pepy.tech/badge/daffi/month)](https://pepy.tech/project/daffi)
 
 Daffi facilitates remote computing and enables remote procedure calls between multiple endpoints.
 It supports many-to-many relationships between endpoints, allowing for seamless communication between distributed systems.
 The library abstracts the complexities of remote computing and provides a user-friendly interface for initiating and managing remote procedure calls.
 It also offers various features such as fault tolerance, load balancing, streaming and security, to ensure reliable and secure communication between endpoints.
 
+Daffi comprises three primary classes:
+
+- *Global* - Initialization entrypoint. Once *Global* object is initialized application can respond on remote requests and trigger remote callbacks itself.
+- *Callback* - Represents a collection of methods encapsulated in a class inherited from *Callback* or a standalone function decorated with the *callback* decorator. These functions/methods can be triggered from another process.
+- *Fetcher* - Represents a collection of methods encapsulated in a class inherited from *Fetcher* or a standalone function decorated with the *fetcher* decorator. These functions/methods serve as triggers for the corresponding callbacks defined in another process.
+
+## Documentation
+
+View full documentation at: [https://600apples.github.io/dafi/](https://600apples.github.io/dafi/)
+
 
 ## Basic example
 
 You need to create two files `shopping_service.py` and `shopper.py`
 
 `shopping_service.py` - represents a set of remote callbacks that can be triggered by a client application.
 
-`shopper.py` - represents shopping_service client
+`shopper.py` - represents shopping_service client (fetcher)
 
 #### Class based approach
 
 
 `shopping_service.py`:
 ```python
 import logging
 from daffi import Global
 from daffi.registry import Callback
 
 logging.basicConfig(level=logging.INFO)
 
 
 class ShoppingService(Callback):
+    auto_init = True # class is automatically initialized, eliminating the need to manually create an object.
 
     def __post_init__(self):
         self.shopping_list = []
 
     def get_items(self):
         """Return all items that are currently present in shopping list"""
         return self.shopping_list
```

### Comparing `daffi-2.2.0/docs/node-and-controller.md` & `daffi-2.2.1/docs/node-and-controller.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/bg.jpg` & `daffi-2.2.1/docs/images/bg.jpg`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/controller-plus-node-arch.drawio` & `daffi-2.2.1/docs/images/controller-plus-node-arch.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/controller-plus-node-arch.png` & `daffi-2.2.1/docs/images/controller-plus-node-arch.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/gitter.png` & `daffi-2.2.1/docs/images/gitter.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/logo-white-sm.png` & `daffi-2.2.1/docs/images/logo-white-sm.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/logo-white.png` & `daffi-2.2.1/docs/images/logo-white.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/logo.png` & `daffi-2.2.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/many-controllers.drawio` & `daffi-2.2.1/docs/images/many-controllers.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/many-controllers.png` & `daffi-2.2.1/docs/images/many-controllers.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/pdf-file.png` & `daffi-2.2.1/docs/images/pdf-file.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/stand-alone-controller-arch.drawio` & `daffi-2.2.1/docs/images/stand-alone-controller-arch.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/images/stand-alone-controller-arch.png` & `daffi-2.2.1/docs/images/stand-alone-controller-arch.png`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/js/extra.js` & `daffi-2.2.1/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/stylesheets/extra.css` & `daffi-2.2.1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/usage/aliased-methods.md` & `daffi-2.2.1/docs/usage/aliased-methods.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class CalculatorService(Callback):
+        auto_init = True
     
         def calculate_sum(self, num1, num2):
             return num1 + num2
     
     
     if __name__ == '__main__':
         Global(init_controller=True, host="localhost", port=8888).join()
```

### Comparing `daffi-2.2.0/docs/usage/asynchronous-execution.md` & `daffi-2.2.1/docs/usage/asynchronous-execution.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class CalculatorService(Callback):
+        auto_init = True
     
         def calculate_fibonacci(self, n):
             # Check if n is 0
             # then it will return 0
             if n == 0:
                 return 0
```

### Comparing `daffi-2.2.0/docs/usage/basic-example.md` & `daffi-2.2.1/docs/usage/basic-example.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class CalculatorService(Callback):
+        auto_init = True
     
         def calculate_sum(self, *numbers):
             return sum(numbers)
     
     
     if __name__ == '__main__':
         Global(init_controller=True, host="localhost", port=8888).join()
```

### Comparing `daffi-2.2.0/docs/usage/bidirectional-communication.md` & `daffi-2.2.1/docs/usage/bidirectional-communication.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 logging.basicConfig(level=logging.INFO)
 
 PROCESS_NAME = "shopping service"
 
 
 class ShoppingService(Callback):
+    auto_init = True
 
     def __post_init__(self):
         self.shop_items = ["orange", "bread", "cheese"]
 
     def get_shop_items(self):
         return self.shop_items
 
@@ -50,14 +51,15 @@
 
 logging.basicConfig(level=logging.INFO)
 
 PROCESS_NAME = "calculator service"
 
 
 class CalculatorService(Callback):
+    auto_init = True
 
     def calculate_sum(self, *numbers):
         return sum(numbers)
 
 
 class ShoppingClient(Fetcher):
```

### Comparing `daffi-2.2.0/docs/usage/broadcasting.md` & `daffi-2.2.1/docs/usage/broadcasting.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class BurgerMenu(Callback):
+        auto_init = True
     
         def get_menu(self):
             return ["The IceBurg", "The Grill Thrill", "Burger Mania", "Chicha Burger"]
     
     
     if __name__ == '__main__':
         Global(init_controller=True, host="localhost", port=8888, process_name="burger menu").join()
```

### Comparing `daffi-2.2.0/docs/usage/callback-additional-arguments.md` & `daffi-2.2.1/docs/usage/callback-additional-arguments.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 The Callback class allows users to include extra initialization arguments.
-By default, any subclass of Callback is automatically initialized without any additional input.
-To turn off this default behavior, users can set the `auto_init` flag to False.
+For this reason you need to set `auto_init` flag to False (or omit it as it is default behavior).
 
 In this scenario, it is the user's responsibility to explicitly create an instance of the class.
 
 
 `calculator_service.py` content:
 ```python
 import logging
 from daffi import Global
 from daffi.registry import Callback
 
 logging.basicConfig(level=logging.INFO)
 
 
 class CalculatorService(Callback):
-
     auto_init = False
 
     def __init__(self, multiplier):
         super().__init__()
         self.multiplier = multiplier
 
     def calculate_sum(self, num1, num2):
```

### Comparing `daffi-2.2.0/docs/usage/fetchers-with-body.md` & `daffi-2.2.1/docs/usage/fetchers-with-body.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class CalculatorService(Callback):
+        auto_init = True
     
         def calculate_sum(self, num1, num2):
             return num1 + num2
     
         def calculate_difference(self, num1, num2):
             return num1 - num2
```

### Comparing `daffi-2.2.0/docs/usage/function-transfer.md` & `daffi-2.2.1/docs/usage/function-transfer.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/usage/named-processes.md` & `daffi-2.2.1/docs/usage/named-processes.md`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/docs/usage/private-methods.md` & `daffi-2.2.1/docs/usage/private-methods.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from daffi.registry import Callback
 from daffi.decorators import local
 
 logging.basicConfig(level=logging.INFO)
 
 
 class CalculatorService(Callback):
+    auto_init = True
 
     def calculate_sum(self, num1, num2):
         return self.get_sum(num1, num2)
 
     @local
     def get_sum(self, num1, num2):
         return num1 + num2
```

### Comparing `daffi-2.2.0/docs/usage/scheduling-tasks.md` & `daffi-2.2.1/docs/usage/scheduling-tasks.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class Scheduler(Callback):
+        auto_init = True
     
         def long_running_task1(self):
             print("Start long running task 1")
             for i in range(1, 3):
                 print(f"Processing item {i}...")
                 time.sleep(1)
             print("Task 1 complete.")
```

### Comparing `daffi-2.2.0/docs/usage/stream-callback-to-fetcher.md` & `daffi-2.2.1/docs/usage/stream-callback-to-fetcher.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class StreamerService(Callback):
+        auto_init = True
     
         def generate_stream(self, end):
             for i in range(end):
                 yield i
     
     
     if __name__ == '__main__':
```

### Comparing `daffi-2.2.0/docs/usage/stream-fetcher-to-callback.md` & `daffi-2.2.1/docs/usage/stream-fetcher-to-callback.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from daffi import Global
     from daffi.registry import Callback
     
     logging.basicConfig(level=logging.INFO)
     
     
     class StreamerService(Callback):
+        auto_init = True
     
         def __post_init__(self):
             self.items = []
     
         def stream_to_service(self, item, process_name):
             self.items.append(item)
             print(f"Received item: {item} from process: {process_name}")
```

### Comparing `daffi-2.2.0/examples/docker/colorizer/main.py` & `daffi-2.2.1/examples/docker/colorizer/main.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/docker/email_processor/main.py` & `daffi-2.2.1/examples/docker/email_processor/main.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/docker/web/app.py` & `daffi-2.2.1/examples/docker/web/app.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/docker/web/templates/base.html` & `daffi-2.2.1/examples/docker/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/docker/web/templates/index.html` & `daffi-2.2.1/examples/docker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/classes_based/consumer.py` & `daffi-2.2.1/examples/opencv_stream/classes_based/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/classes_based/publisher1.py` & `daffi-2.2.1/examples/opencv_stream/classes_based/publisher1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/classes_based/publisher2.py` & `daffi-2.2.1/examples/opencv_stream/classes_based/publisher2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/classes_based/publisher3.py` & `daffi-2.2.1/examples/opencv_stream/classes_based/publisher3.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/decorators_based/consumer.py` & `daffi-2.2.1/examples/opencv_stream/decorators_based/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher1.py` & `daffi-2.2.1/examples/opencv_stream/decorators_based/publisher1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher2.py` & `daffi-2.2.1/examples/opencv_stream/decorators_based/publisher2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher3.py` & `daffi-2.2.1/examples/opencv_stream/decorators_based/publisher3.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/callbacks_from_class/consumer.py` & `daffi-2.2.1/examples/tcp/callbacks_from_class/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/callbacks_from_class/publisher.py` & `daffi-2.2.1/examples/tcp/callbacks_from_class/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/eta/consumer.py` & `daffi-2.2.1/examples/tcp/eta/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/eta/publisher.py` & `daffi-2.2.1/examples/tcp/eta/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/no_return/consumer.py` & `daffi-2.2.1/examples/tcp/no_return/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/no_return/publisher.py` & `daffi-2.2.1/examples/tcp/no_return/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/scheduler/consumer.py` & `daffi-2.2.1/examples/tcp/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/scheduler/publisher.py` & `daffi-2.2.1/examples/tcp/scheduler/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/stream/consumer.py` & `daffi-2.2.1/examples/tcp/stream/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/stream/publisher.py` & `daffi-2.2.1/examples/tcp/stream/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/transfer_and_call/consumer.py` & `daffi-2.2.1/examples/tcp/transfer_and_call/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication/class_based/proc1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "White Rabbit"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
     def greeting1(self, arg1, arg2):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
 
     def greeting2(self):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
+class Greetings(Fetcher):
+    def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    def greeting2(self):
+        __body_unknown__()
+
+
 def main():
     gret = Greetings()
     remote_proc = "Brown Fox"
     g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from trio import run, sleep
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Brown Fox"
+PROC_NAME = "Trio Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
-    def greeting1(self, arg1, arg2):
-        return (
-            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
-        )
+@callback
+@fetcher
+async def greeting1(arg1, arg2):
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
 
-    def greeting2(self):
-        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
+@callback
+@fetcher
+async def greeting2():
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
-def main():
-    gret = Greetings()
-    remote_proc = "White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
+
+async def main():
+    remote_proc = "Trio White Rabbit"
+    g = Global(process_name=PROC_NAME)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = gret.greeting1("foo", "bar")
+            res = await greeting1("foo", "bar")
             print(res)
-            time.sleep(2)
-            res = gret.greeting2()
+            await sleep(2)
+            res = await greeting2()
             print(res)
-            time.sleep(2)
+            await sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    main()
+    run(main)
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
+import asyncio
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "White Rabbit"
+PROC_NAME = "Async White Rabbit"
 
 
 @callback
 @fetcher
-def greeting1(arg1, arg2):
+async def greeting1(arg1, arg2):
     return (
         f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
     )
 
 
 @callback
 @fetcher
-def greeting2():
+async def greeting2():
     return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
-def main():
-    remote_proc = "Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
+async def main():
+    remote_proc = "Async Brown Fox"
+    g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = greeting1("foo", "bar")
+            res = await greeting1("foo", "bar")
             print(res)
             time.sleep(2)
-            res = greeting2()
+            res = await greeting2()
             print(res)
             time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    main()
+    asyncio.run(main())
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from pathlib import Path
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Brown Fox"
+ROOT = Path(__file__).parents[3]
+SSL_CERT = ROOT / "certs" / "cert.pem"
+SSL_KEY = ROOT / "certs" / "key.pem"
 
 
 @callback
 @fetcher
 def greeting1(arg1, arg2):
     return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
 
@@ -18,15 +23,15 @@
 @fetcher
 def greeting2():
     return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
 def main():
     remote_proc = "White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication/class_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import time
 import logging
-import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Async White Rabbit"
+PROC_NAME = "Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
-    async def greeting1(self, arg1, arg2):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+class GreetingsCallback(Callback):
+    auto_init = True
 
-    async def greeting2(self):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+    def greeting1(self, arg1, arg2):
+        return (
+            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+        )
 
+    def greeting2(self):
+        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
-async def main():
+
+class Greetings(Fetcher):
+    def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    def greeting2(self):
+        __body_unknown__()
+
+
+def main():
     gret = Greetings()
-    remote_proc = "Async Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
+    remote_proc = "White Rabbit"
+    g = Global(process_name=PROC_NAME)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await gret.greeting1("foo", "bar")
+            res = gret.greeting1("foo", "bar")
             print(res)
             time.sleep(2)
-            res = await gret.greeting2()
+            res = gret.greeting2()
             print(res)
             time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    main()
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import time
 import logging
 import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Async Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
     async def greeting1(self, arg1, arg2):
         return (
             f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
         )
 
     async def greeting2(self):
         return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
+class Greetings(Fetcher):
+    async def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    async def greeting2(self):
+        __body_unknown__()
+
+
 async def main():
     gret = Greetings()
     remote_proc = "Async White Rabbit"
     g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication/decorators_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 import time
 import logging
-import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
-
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Async White Rabbit"
+PROC_NAME = "Brown Fox"
 
 
 @callback
 @fetcher
-async def greeting1(arg1, arg2):
-    return (
-        f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
-    )
+def greeting1(arg1, arg2):
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
 
 
 @callback
 @fetcher
-async def greeting2():
-    return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+def greeting2():
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
-async def main():
-    remote_proc = "Async Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
+def main():
+    remote_proc = "White Rabbit"
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await greeting1("foo", "bar")
+            res = greeting1("foo", "bar")
             print(res)
             time.sleep(2)
-            res = await greeting2()
+            res = greeting2()
             print(res)
             time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    main()
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import asyncio
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Async Brown Fox"
 
 
@@ -19,15 +20,15 @@
 @fetcher
 async def greeting2():
     return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
 async def main():
     remote_proc = "Async White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
+    g = Global(process_name=PROC_NAME)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 import time
 import logging
 from daffi import Global
 from pathlib import Path
 from daffi.exceptions import RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "White Rabbit"
+PROC_NAME = "Brown Fox"
 ROOT = Path(__file__).parents[3]
 SSL_CERT = ROOT / "certs" / "cert.pem"
 SSL_KEY = ROOT / "certs" / "key.pem"
 
 
+class GreetingsCallback(Callback):
+    auto_init = True
 
-class Greetings(Callback, Fetcher):
     def greeting1(self, arg1, arg2):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+        return (
+            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+        )
 
     def greeting2(self):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+
+
+class Greetings(Fetcher):
+    def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    def greeting2(self):
+        __body_unknown__()
 
 
 def main():
     gret = Greetings()
-    remote_proc = "Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
+    remote_proc = "White Rabbit"
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = gret.greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 import time
 import logging
 from daffi import Global
 from pathlib import Path
 from daffi.exceptions import RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Brown Fox"
+PROC_NAME = "White Rabbit"
 ROOT = Path(__file__).parents[3]
 SSL_CERT = ROOT / "certs" / "cert.pem"
 SSL_KEY = ROOT / "certs" / "key.pem"
 
-class Greetings(Callback, Fetcher):
+
+class GreetingsCallback(Callback):
+    auto_init = True
+
+    def greeting1(self, arg1, arg2):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+
+    def greeting2(self):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+
+
+class Greetings(Fetcher):
     def greeting1(self, arg1, arg2):
-        return (
-            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
-        )
+        __body_unknown__(arg1, arg2)
 
     def greeting2(self):
-        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+        __body_unknown__()
 
 
 def main():
     gret = Greetings()
-    remote_proc = "White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
+    remote_proc = "Brown Fox"
+    g = Global(
+        process_name=PROC_NAME,
+        init_controller=True,
+        host="localhost",
+        port=8888,
+        ssl_certificate=SSL_CERT,
+        ssl_key=SSL_KEY,
+    )
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = gret.greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc1.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,22 @@
 @fetcher
 def greeting2():
     return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
 def main():
     remote_proc = "Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
+    g = Global(
+        process_name=PROC_NAME,
+        init_controller=True,
+        host="localhost",
+        port=8888,
+        ssl_certificate=SSL_CERT,
+        ssl_key=SSL_KEY,
+    )
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-import time
 import logging
-from daffi import Global
-from pathlib import Path
-from daffi.exceptions import RemoteStoppedUnexpectedly
+from trio import run, sleep
+from daffi import Global, RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Brown Fox"
-ROOT = Path(__file__).parents[3]
-SSL_CERT = ROOT / "certs" / "cert.pem"
-SSL_KEY = ROOT / "certs" / "key.pem"
+PROC_NAME = "Trio Brown Fox"
 
 
 @callback
 @fetcher
-def greeting1(arg1, arg2):
+async def greeting1(arg1, arg2):
     return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
 
 
 @callback
 @fetcher
-def greeting2():
+async def greeting2():
     return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
-def main():
-    remote_proc = "White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888, ssl_certificate=SSL_CERT, ssl_key=SSL_KEY)
+async def main():
+    remote_proc = "Trio White Rabbit"
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = greeting1("foo", "bar")
+            res = await greeting1("foo", "bar")
             print(res)
-            time.sleep(2)
-            res = greeting2()
+            await sleep(2)
+            res = await greeting2()
             print(res)
-            time.sleep(2)
+            await sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    main()
+    run(main)
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import logging
 from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio White Rabbit"
+PROC_NAME = "Trio Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
+    async def greeting1(self, arg1, arg2):
+        return (
+            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+        )
+
+    async def greeting2(self):
+        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+
+
+class Greetings(Fetcher):
     async def greeting1(self, arg1, arg2):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+        __body_unknown__(arg1, arg2)
 
     async def greeting2(self):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+        __body_unknown__()
 
 
 async def main():
     gret = Greetings()
-    remote_proc = "Trio Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
+    remote_proc = "Trio White Rabbit"
+    g = Global(process_name=PROC_NAME)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await gret.greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,50 @@
+import time
+import asyncio
 import logging
-from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio Brown Fox"
+PROC_NAME = "Async Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
-    async def greeting1(self, arg1, arg2):
-        return (
-            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
-        )
+@callback
+@fetcher
+async def greeting1(arg1, arg2):
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
 
-    async def greeting2(self):
-        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+
+@callback
+@fetcher
+async def greeting2():
+    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
 async def main():
-    gret = Greetings()
-    remote_proc = "Trio White Rabbit"
+    remote_proc = "Async White Rabbit"
     g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await gret.greeting1("foo", "bar")
+            res = await greeting1("foo", "bar")
             print(res)
-            await sleep(2)
-            res = await gret.greeting2()
+            time.sleep(2)
+            res = await greeting2()
             print(res)
-            await sleep(2)
+            time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    run(main)
+    asyncio.run(main())
```

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import logging
 from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
+
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio Brown Fox"
+PROC_NAME = "Trio White Rabbit"
 
 
 @callback
 @fetcher
 async def greeting1(arg1, arg2):
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+    return (
+        f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+    )
 
 
 @callback
 @fetcher
 async def greeting2():
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+    return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
 async def main():
-    remote_proc = "Trio White Rabbit"
-    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
+    remote_proc = "Trio Brown Fox"
+    g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py` & `daffi-2.2.1/examples/unix_socket/callback_and_fetcher_decorator/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py` & `daffi-2.2.1/examples/unix_socket/callback_and_fetcher_decorator/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py` & `daffi-2.2.1/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py` & `daffi-2.2.1/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callback_generator/class_consumer.py` & `daffi-2.2.1/examples/unix_socket/callback_generator/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callback_generator/class_publisher.py` & `daffi-2.2.1/examples/unix_socket/callback_generator/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callbacks_from_class/consumer.py` & `daffi-2.2.1/examples/unix_socket/callbacks_from_class/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/callbacks_from_class/publisher.py` & `daffi-2.2.1/examples/unix_socket/callbacks_from_class/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/eta/class_consumer.py` & `daffi-2.2.1/examples/unix_socket/eta/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/eta/class_publisher.py` & `daffi-2.2.1/examples/unix_socket/eta/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/eta/consumer.py` & `daffi-2.2.1/examples/unix_socket/eta/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/eta/publisher.py` & `daffi-2.2.1/examples/unix_socket/eta/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/fetcher_generator/class_consumer.py` & `daffi-2.2.1/examples/unix_socket/fetcher_generator/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/fetcher_generator/class_publisher.py` & `daffi-2.2.1/examples/unix_socket/fetcher_generator/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/no_return/consumer.py` & `daffi-2.2.1/examples/unix_socket/no_return/consumer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Consumer is the process that consumes available remote functions.
 """
 
 import time
 import logging
-from daffi import Global, GlobalContextError, BG
+from daffi import Global, BG
 from daffi.decorators import fetcher
+from daffi.exceptions import GlobalContextError
 
 logging.basicConfig(level=logging.INFO)
 
 
 @fetcher(BG(return_result=False))
 def some_func():
     pass
```

### Comparing `daffi-2.2.0/examples/unix_socket/no_return/publisher.py` & `daffi-2.2.1/examples/unix_socket/no_return/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/scheduler/consumer.py` & `daffi-2.2.1/examples/unix_socket/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/scheduler/publisher.py` & `daffi-2.2.1/examples/unix_socket/scheduler/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/stream/consumer.py` & `daffi-2.2.1/examples/unix_socket/stream/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/stream/publisher.py` & `daffi-2.2.1/examples/unix_socket/stream/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/transfer_and_call/consumer.py` & `daffi-2.2.1/examples/unix_socket/transfer_and_call/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication/class_based/proc2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "White Rabbit"
+PROC_NAME = "Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
+    def greeting1(self, arg1, arg2):
+        return (
+            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+        )
+
+    def greeting2(self):
+        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+
+
+class Greetings(Fetcher):
     def greeting1(self, arg1, arg2):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+        __body_unknown__(arg1, arg2)
 
     def greeting2(self):
-        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+        __body_unknown__()
 
 
 def main():
     gret = Greetings()
-    remote_proc = "Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True)
+    remote_proc = "White Rabbit"
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = gret.greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,56 @@
-import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from trio import run, sleep
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Brown Fox"
+PROC_NAME = "Trio White Rabbit"
 
 
-class Greetings(Callback, Fetcher):
-    def greeting1(self, arg1, arg2):
-        return (
-            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
-        )
+class GreetingsCallback(Callback):
+    auto_init = True
 
-    def greeting2(self):
-        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+    async def greeting1(self, arg1, arg2):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
 
+    async def greeting2(self):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
-def main():
+
+class Greetings(Fetcher):
+    async def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    async def greeting2(self):
+        __body_unknown__()
+
+
+async def main():
     gret = Greetings()
-    remote_proc = "White Rabbit"
-    g = Global(process_name=PROC_NAME)
+    remote_proc = "Trio Brown Fox"
+    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = gret.greeting1("foo", "bar")
+            res = await gret.greeting1("foo", "bar")
             print(res)
-            time.sleep(2)
-            res = gret.greeting2()
+            await sleep(2)
+            res = await gret.greeting2()
             print(res)
-            time.sleep(2)
+            await sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    main()
+    run(main)
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication/decorators_based/proc1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "White Rabbit"
 
@@ -21,15 +22,15 @@
 @fetcher
 def greeting2():
     return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
 def main():
     remote_proc = "Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True)
+    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Brown Fox"
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import time
 import logging
 import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Async White Rabbit"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
     async def greeting1(self, arg1, arg2):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
 
     async def greeting2(self):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
+class Greetings(Fetcher):
+    async def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    async def greeting2(self):
+        __body_unknown__()
+
+
 async def main():
     gret = Greetings()
     remote_proc = "Async Brown Fox"
     g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import time
 import logging
 import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Async Brown Fox"
+PROC_NAME = "Async White Rabbit"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
+    async def greeting1(self, arg1, arg2):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
+
+    async def greeting2(self):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+
+
+class Greetings(Fetcher):
     async def greeting1(self, arg1, arg2):
-        return (
-            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
-        )
+        __body_unknown__(arg1, arg2)
 
     async def greeting2(self):
-        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+        __body_unknown__()
 
 
 async def main():
     gret = Greetings()
-    remote_proc = "Async White Rabbit"
-    g = Global(process_name=PROC_NAME)
+    remote_proc = "Async Brown Fox"
+    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await gret.greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import logging
 import asyncio
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Async White Rabbit"
 
@@ -22,15 +23,15 @@
 @fetcher
 async def greeting2():
     return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
 async def main():
     remote_proc = "Async Brown Fox"
-    g = Global(process_name=PROC_NAME, init_controller=True)
+    g = Global(process_name=PROC_NAME, init_controller=True, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await greeting1("foo", "bar")
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,56 @@
-import time
-import asyncio
 import logging
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.decorators import callback, fetcher
+from trio import run, sleep
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Async Brown Fox"
+PROC_NAME = "Trio White Rabbit"
 
 
-@callback
-@fetcher
-async def greeting1(arg1, arg2):
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+class GreetingsCallback(Callback):
+    auto_init = True
 
+    async def greeting1(self, arg1, arg2):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
 
-@callback
-@fetcher
-async def greeting2():
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+    async def greeting2(self):
+        return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
+
+
+class Greetings(Fetcher):
+    async def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    async def greeting2(self):
+        __body_unknown__()
 
 
 async def main():
-    remote_proc = "Async White Rabbit"
-    g = Global(process_name=PROC_NAME)
+    gret = Greetings()
+    remote_proc = "Trio Brown Fox"
+    g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await greeting1("foo", "bar")
+            res = await gret.greeting1("foo", "bar")
             print(res)
-            time.sleep(2)
-            res = await greeting2()
+            await sleep(2)
+            res = await gret.greeting2()
             print(res)
-            time.sleep(2)
+            await sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    asyncio.run(main())
+    run(main)
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication/class_based/proc1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,56 @@
+import time
 import logging
-from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio White Rabbit"
+PROC_NAME = "White Rabbit"
 
 
-class Greetings(Callback, Fetcher):
-    async def greeting1(self, arg1, arg2):
+class GreetingsCallback(Callback):
+    auto_init = True
+
+    def greeting1(self, arg1, arg2):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
 
-    async def greeting2(self):
+    def greeting2(self):
         return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
-async def main():
+class Greetings(Fetcher):
+    def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    def greeting2(self):
+        __body_unknown__()
+
+
+def main():
     gret = Greetings()
-    remote_proc = "Trio Brown Fox"
+    remote_proc = "Brown Fox"
     g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await gret.greeting1("foo", "bar")
+            res = gret.greeting1("foo", "bar")
             print(res)
-            await sleep(2)
-            res = await gret.greeting2()
+            time.sleep(2)
+            res = gret.greeting2()
             print(res)
-            await sleep(2)
+            time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    run(main)
+    main()
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,59 @@
+import time
 import logging
-from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.registry import Callback, Fetcher
+import asyncio
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio Brown Fox"
+PROC_NAME = "Async Brown Fox"
 
 
-class Greetings(Callback, Fetcher):
+class GreetingsCallback(Callback):
+    auto_init = True
+
     async def greeting1(self, arg1, arg2):
         return (
             f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
         )
 
     async def greeting2(self):
         return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
 
 
+class Greetings(Fetcher):
+    async def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    async def greeting2(self):
+        __body_unknown__()
+
+
 async def main():
     gret = Greetings()
-    remote_proc = "Trio White Rabbit"
+    remote_proc = "Async White Rabbit"
     g = Global(process_name=PROC_NAME)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
             res = await gret.greeting1("foo", "bar")
             print(res)
-            await sleep(2)
+            time.sleep(2)
             res = await gret.greeting2()
             print(res)
-            await sleep(2)
+            time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    run(main)
+    asyncio.run(main())
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py` & `daffi-2.2.1/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,52 @@
+import time
 import logging
-from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
 from daffi.decorators import callback, fetcher
 
 
 logging.basicConfig(level=logging.INFO)
 
-PROC_NAME = "Trio White Rabbit"
+PROC_NAME = "White Rabbit"
 
 
 @callback
 @fetcher
-async def greeting1(arg1, arg2):
+def greeting1(arg1, arg2):
     return (
         f"Greeting from {PROC_NAME!r} process. You called function greeting1 with arguments: arg1={arg1}, arg2={arg2}"
     )
 
 
 @callback
 @fetcher
-async def greeting2():
+def greeting2():
     return f"Greeting from {PROC_NAME!r} process. You called function greeting2"
 
 
-async def main():
-    remote_proc = "Trio Brown Fox"
+def main():
+    remote_proc = "Brown Fox"
     g = Global(process_name=PROC_NAME, init_controller=True)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await greeting1("foo", "bar")
+            res = greeting1("foo", "bar")
             print(res)
-            await sleep(2)
-            res = await greeting2()
+            time.sleep(2)
+            res = greeting2()
             print(res)
-            await sleep(2)
+            time.sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
 
     g.stop()
 
 
 if __name__ == "__main__":
-    run(main)
+    main()
```

### Comparing `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py` & `daffi-2.2.1/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 import logging
 from trio import run, sleep
-from daffi import Global, RemoteStoppedUnexpectedly
-from daffi.decorators import callback, fetcher
+from daffi import Global
+from daffi.exceptions import RemoteStoppedUnexpectedly
+from daffi.registry import Callback, Fetcher, __body_unknown__
 
 logging.basicConfig(level=logging.INFO)
 
 PROC_NAME = "Trio Brown Fox"
 
 
-@callback
-@fetcher
-async def greeting1(arg1, arg2):
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+class GreetingsCallback(Callback):
+    auto_init = True
 
+    def greeting1(self, arg1, arg2):
+        return (
+            f"Cheers from {PROC_NAME!r} process. You called function cheers1 with arguments: arg1={arg1}, arg2={arg2}"
+        )
 
-@callback
-@fetcher
-async def greeting2():
-    return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+    def greeting2(self):
+        return f"Cheers from {PROC_NAME!r} process. You called function cheers2"
+
+
+class Greetings(Fetcher):
+    def greeting1(self, arg1, arg2):
+        __body_unknown__(arg1, arg2)
+
+    def greeting2(self):
+        __body_unknown__()
 
 
 async def main():
+    gret = Greetings()
     remote_proc = "Trio White Rabbit"
-    g = Global(process_name=PROC_NAME)
+    g = Global(process_name=PROC_NAME, host="localhost", port=8888)
 
     print(f"wait for {remote_proc} process to be started...")
     g.wait_process(remote_proc)
 
     for _ in range(10):
         try:
-            res = await greeting1("foo", "bar")
+            res = await gret.greeting1("foo", "bar")
             print(res)
             await sleep(2)
-            res = await greeting2()
+            res = await gret.greeting2()
             print(res)
             await sleep(2)
         except RemoteStoppedUnexpectedly as e:
             # We need to handle GlobalContextError in order one process exit earlier.
             # It means remote callbacks becomes unavailable.
             print(e)
             break
```

### Comparing `daffi-2.2.0/scripts/generate_coverage_summary.py` & `daffi-2.2.1/scripts/generate_coverage_summary.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/scripts/write_coverage_summary_report.py` & `daffi-2.2.1/scripts/write_coverage_summary_report.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/conftest.py` & `daffi-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/integration/conftest.py` & `daffi-2.2.1/tests/integration/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
+import asyncio
 from pathlib import Path
 import socketserver
 
 from daffi import Global
 from jinja2 import FileSystemLoader, Environment
 
-
 THIS = Path(__file__)
 
 templateLoader = FileSystemLoader(searchpath=THIS.parent / "templates")
 templateEnv = Environment(loader=templateLoader)
 
 
 @pytest.fixture
@@ -48,11 +48,23 @@
     finally:
         if gl:
             gl.stop()
 
 
 @pytest.fixture
 def free_port() -> int:
-
     with socketserver.TCPServer(("localhost", 0), None) as s:
         free_port = s.server_address[1]
         return free_port
+
+
+@pytest.fixture
+def stop_components():
+    async def stop_process(prop):
+        prop.terminate()
+        prop.wait()
+
+    async def dec(remotes, g):
+        await asyncio.gather(*(stop_process(prop=p) for p in remotes))
+        g.stop()
+
+    yield dec
```

### Comparing `daffi-2.2.0/tests/integration/test_broadcast.py` & `daffi-2.2.1/tests/integration/test_trio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,74 @@
 import pytest
 import sys
-from daffi import BROADCAST
-from daffi.decorators import __body_unknown__, fetcher
+from daffi import FG, BG
+from daffi.exceptions import GlobalContextError
+from daffi.decorators import fetcher, __body_unknown__
 from subprocess import Popen
 
 
-expected = {
-    "node-1": "node-1.broadcast_test",
-    "node-4": "node-4.broadcast_test",
-    "node-3": "node-3.broadcast_test",
-    "node-5": "node-5.broadcast_test",
-    "node-6": "node-6.broadcast_test",
-    "node-7": "node-7.broadcast_test",
-    "node-8": "node-8.broadcast_test",
-    "node-2": "node-2.broadcast_test",
-    "node-9": "node-9.broadcast_test",
-}
-
-
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_callback_per_node_unix(remote_callbacks_path, g):
-    @fetcher(BROADCAST(return_result=True, timeout=10))
-    def broadcast_callback(value: str):
-        __body_unknown__(value)
-
+async def test_callback_per_node_unix(remote_callbacks_path, g, stop_components):
     g = g()
-    start_range = 1
-    end_range = 10
-    range_ = list(range(start_range, end_range))
+
+    @fetcher(FG(timeout="7s"))
+    async def test_callback():
+        __body_unknown__()
 
     executable_files = [
         remote_callbacks_path(
-            filename=f"{i}.py",
-            template_name="broadcast.jinja2",
-            process_name=f"node-{i}",
+            template_name="test_trio.jinja2",
+            process_name=f"test-node",
         )
-        for i in range_
     ]
-
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
-    for i in range_:
-        g.wait_process(f"node-{i}")
 
-    result = broadcast_callback(value="broadcast_test")
-    assert result == expected
+    g.wait_process(f"test-node")
 
-    g.stop(True)
-    [p.terminate() for p in remotes]
+    try:
+        res = await test_callback()
+        assert res == "Ok"
+
+        res = await test_callback.call(exec_modifier=BG(eta=2))
+        res = await res.get_async()
+        assert res == "Ok"
+
+        res = await test_callback.call(exec_modifier=FG(timeout="7s"))
+        assert res == "Ok"
+
+        res = await test_callback.call(exec_modifier=BG(eta=2))
+        res = await res.get_async()
+        assert res == "Ok"
+    finally:
+        await stop_components(remotes, g)
 
 
-async def test_callback_per_node_tcp(remote_callbacks_path, g):
-    @fetcher(BROADCAST(return_result=True, timeout=10))
-    def broadcast_callback(value: str):
-        __body_unknown__(value)
+@pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
+async def test_callback_per_node_unix_wrong_body_args(remote_callbacks_path, g, stop_components):
+    g = g()
 
-    g = g(host="localhost")
-    start_range = 1
-    end_range = 10
-    range_ = list(range(start_range, end_range))
+    @fetcher(FG(timeout="7s"))
+    async def test_callback(a, b):
+        return a, b
 
     executable_files = [
         remote_callbacks_path(
-            filename=f"{i}.py",
-            template_name="broadcast.jinja2",
-            process_name=f"node-{i}",
-            host="localhost",
-            port=g.port,
+            template_name="test_trio.jinja2",
+            process_name=f"test-node",
         )
-        for i in range_
     ]
-
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
-    for i in range_:
-        g.wait_process(f"node-{i}")
 
-    result = broadcast_callback(value="broadcast_test")
-    assert result == expected
-    g.stop(True)
-    [p.terminate() for p in remotes]
+    g.wait_process(f"test-node")
+
+    try:
+        with pytest.raises(GlobalContextError):
+            await test_callback(a="foo", b="bar")
+
+        with pytest.raises(GlobalContextError):
+            await test_callback.call(a="foo", b="bar", exec_modifier=BG(eta=2))
+    finally:
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_many_callbacks.py` & `daffi-2.2.1/tests/integration/test_many_callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from datetime import datetime
 from random import choices, choice
 from subprocess import Popen
 
 import pytest
 from daffi import FG, BG, PERIOD
 
-
 timings = []
 remote_type = "callback_func_", "async_callback_func_"
 
 
 async def call_remote(g, _range, exec_type):
     random_args = [1, 2, 134566, "12345", "867", ("a", "b", "c"), {"foo": "bar"}, object]
 
@@ -36,15 +35,14 @@
 
             assert func_args == res[0]
             assert {} == res[1]
             timings.append(time.time() - start)
 
 
 async def call_remote_no_return(g, num, exec_type, path):
-
     for i in range(5):
         func_args = dict(path=str(path), text=str(i))
         start = datetime.utcnow().timestamp()
         future = getattr(g.call, remote_type[bool(i % 2)] + str(num))(**func_args)
 
         if exec_type == PERIOD:
             future & PERIOD(at_time=start + 2)
@@ -52,15 +50,15 @@
         elif exec_type == BG:
             future & BG(return_result=False)
             await asyncio.sleep(3)
 
 
 @pytest.mark.parametrize("exec_type", [BG, FG])
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_many_callbacks_unix(remote_callbacks_path, exec_type, g):
+async def test_many_callbacks_unix(remote_callbacks_path, exec_type, g, stop_components):
     timings.clear()
     g = g()
     process_name = "test_node"
     start_range = 1
     end_range = 500
     range_ = list(range(start_range, end_range))
     executable_file = remote_callbacks_path(
@@ -72,21 +70,20 @@
         g.wait_process(process_name)
         await asyncio.gather(*[call_remote(g, range_, exec_type) for _ in range(500)])
 
         max_time = max(timings)
         assert max_time < 1
 
     finally:
-        g.stop(True)
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [PERIOD, BG])
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_many_callbacks_unix_no_return(remote_callbacks_path, exec_type, g):
+async def test_many_callbacks_unix_no_return(remote_callbacks_path, exec_type, g, stop_components):
     timings.clear()
     g = g()
     process_name = "test_node"
     start_range = 1
     end_range = 251
     executable_file = remote_callbacks_path(
         template_name="many_callbacks.jinja2",
@@ -112,20 +109,19 @@
             assert set(file.read_text()) == set("01234")
     except AssertionError:
         raise
     except Exception as e:
         print(f"Exeption while execution : {type(e)}, {e}")
 
     finally:
-        g.stop(True)
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [BG, FG])
-async def test_many_callbacks_tcp(remote_callbacks_path, exec_type, g):
+async def test_many_callbacks_tcp(remote_callbacks_path, exec_type, g, stop_components):
     timings.clear()
     g = g(host="localhost")
     process_name = "test_node"
     start_range = 1
     end_range = 500
     range_ = list(range(start_range, end_range))
     executable_file = remote_callbacks_path(
@@ -139,20 +135,19 @@
     try:
         remotes = [Popen([sys.executable, executable_file])]
         g.wait_process(process_name)
         await asyncio.gather(*[call_remote(g, range_, exec_type) for _ in range(500)])
         max_time = max(timings)
         assert max_time < 1
     finally:
-        g.stop(True)
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [PERIOD, BG])
-async def test_many_callbacks_tcp_no_return(remote_callbacks_path, exec_type, g):
+async def test_many_callbacks_tcp_no_return(remote_callbacks_path, exec_type, g, stop_components):
     timings.clear()
     g = g(host="0.0.0.0")
     process_name = "test_node"
     start_range = 1
     end_range = 251
     executable_file = remote_callbacks_path(
         template_name="many_callbacks.jinja2",
@@ -175,9 +170,8 @@
         g.ipc._wait_all_bg_tasks()
 
         all_files = list(path.iterdir())
         assert len(all_files) == 250
         for file in all_files:
             assert set(file.read_text()) == set("01234")
     finally:
-        g.stop(True)
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_many_nodes.py` & `daffi-2.2.1/tests/integration/test_many_nodes.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from daffi.decorators import fetcher, __body_unknown__
 
 
 async def call_remote(g, _range, exec_type):
     for _ in range(5):
         node_num = choice(_range)
         callback_name = f"get_process_name{node_num}"
-        expected_process_name = f"node-{node_num}"
+        expected_process_name = f"mn-node-{node_num}"
         future = getattr(g.call, callback_name)()
 
         if exec_type == FG:
             res = future & FG(timeout=60)
         elif exec_type == BG:
             future = future & BG(timeout=60)
             res = future.get()
@@ -27,49 +27,49 @@
     @fetcher(BROADCAST(return_result=True, timeout=60))
     async def get_process_name1(path):
         __body_unknown__(path)
 
     for i in range(5):
         res = await get_process_name1(path=path / str(i))
         assert set(res) == {
-            "node-1",
-            "node-4",
-            "node-3",
-            "node-6",
-            "node-7",
-            "node-5",
-            "node-8",
-            "node-2",
-            "node-9",
+            "mn-node-1",
+            "mn-node-4",
+            "mn-node-3",
+            "mn-node-6",
+            "mn-node-7",
+            "mn-node-5",
+            "mn-node-8",
+            "mn-node-2",
+            "mn-node-9",
         }
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
 async def test_callback_per_node_unix(remote_callbacks_path, exec_type, g):
     g = g()
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
-            filename=f"{i}.py", callback_index=i, template_name="callback_per_node.jinja2", process_name=f"node-{i}"
+            filename=f"{i}.py", callback_index=i, template_name="callback_per_node.jinja2", process_name=f"mn-node-{i}"
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"mn-node-{i}")
 
     await asyncio.gather(*[call_remote(g, range_, exec_type) for _ in range(500)])
-    g.stop(True)
+    g.stop()
     [p.terminate() for p in remotes]
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
 async def test_callback_per_node_tcp(remote_callbacks_path, exec_type, g):
     g = g(host="localhost")
     start_range = 1
@@ -77,103 +77,103 @@
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             callback_index=i,
             template_name="callback_per_node.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"mn-node-{i}",
             host="localhost",
             port=g.port,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"mn-node-{i}")
 
     await asyncio.gather(*[call_remote(g, range_, exec_type) for _ in range(500)])
-    g.stop(True)
+    g.stop()
     [p.terminate() for p in remotes]
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_callback_per_node_broadcast_unix(remote_callbacks_path, g):
+async def test_callback_per_node_broadcast_unix(remote_callbacks_path, g, stop_components):
     g = g()
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
-            filename=f"{i}.py", callback_index=1, template_name="callback_per_node.jinja2", process_name=f"node-{i}"
+            filename=f"{i}.py", callback_index=1, template_name="callback_per_node.jinja2", process_name=f"mn-node-{i}"
         )
         for i in range_
     ]
 
     path = executable_files[0].parent / "test_data"
     path.mkdir()
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"mn-node-{i}")
 
-    await asyncio.gather(*[call_remote_broadcast(path=path) for _ in range(500)])
+    try:
+        await asyncio.gather(*[call_remote_broadcast(path=path) for _ in range(500)])
 
-    all_files = list(path.iterdir())
-    assert len(all_files) == 5
+        all_files = list(path.iterdir())
+        assert len(all_files) == 5
 
-    all_processes = [f"node-{i}" for i in range_]
-    for file in all_files:
-        file_text = file.read_text()
-        for proc_name in all_processes:
-            assert proc_name in file_text
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+        all_processes = [f"mn-node-{i}" for i in range_]
+        for file in all_files:
+            file_text = file.read_text()
+            for proc_name in all_processes:
+                assert proc_name in file_text
+    finally:
+        await stop_components(remotes, g)
 
 
-async def test_callback_per_node_broadcast_tcp(remote_callbacks_path, g):
+async def test_callback_per_node_broadcast_tcp(remote_callbacks_path, g, stop_components):
     g = g(host="localhost")
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             callback_index=1,
             template_name="callback_per_node.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"mn-node-{i}",
             host="localhost",
             port=g.port,
         )
         for i in range_
     ]
 
     path = executable_files[0].parent / "test_data"
     path.mkdir()
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"mn-node-{i}")
 
-    await asyncio.gather(*[call_remote_broadcast(path=path) for _ in range(500)])
+    try:
+        await asyncio.gather(*[call_remote_broadcast(path=path) for _ in range(500)])
 
-    all_files = list(path.iterdir())
-    assert len(all_files) == 5
+        all_files = list(path.iterdir())
+        assert len(all_files) == 5
 
-    all_processes = [f"node-{i}" for i in range_]
-    for file in all_files:
-        file_text = file.read_text()
-        for proc_name in all_processes:
-            assert proc_name in file_text
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+        all_processes = [f"mn-node-{i}" for i in range_]
+        for file in all_files:
+            file_text = file.read_text()
+            for proc_name in all_processes:
+                assert proc_name in file_text
+    finally:
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_period.py` & `daffi-2.2.1/tests/integration/test_period.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import pytest
 import sys
 from datetime import datetime
-from daffi import PERIOD, GlobalContextError, RemoteCallError
+from daffi import PERIOD
+from daffi.exceptions import GlobalContextError, RemoteCallError
 from subprocess import Popen
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_callback_per_node_unix(remote_callbacks_path, g):
+async def test_callback_per_node_unix(remote_callbacks_path, g, stop_components):
     g = g()
     now = datetime.utcnow().timestamp()
 
     executable_files = [
         remote_callbacks_path(
             template_name="period1.jinja2",
             process_name=f"test-node",
@@ -19,34 +20,35 @@
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
 
     g.wait_process(f"test-node")
 
-    with pytest.raises(GlobalContextError) as ex_context:
-        g.call.cb1() & PERIOD(interval="10s")
+    try:
+        with pytest.raises(GlobalContextError) as ex_context:
+            g.call.cb1() & PERIOD(interval="10s")
+
+        assert "[ test_callback, func1, func2 ]" in str(ex_context)
+
+        task1 = g.call.test_callback() & PERIOD(interval="20s")
+        registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
+        assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task1.uuid}]
+        task1.cancel()
+        registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
+        assert registered_tasks == []
+
+        # Cancel by id
+        task2 = g.call.test_callback() & PERIOD(interval="20s")
+        registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
+        assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task2.uuid}]
+        assert g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=task1.uuid) is False
+        with pytest.raises(RemoteCallError):
+            g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=1234567890)
+        registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
+        assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task2.uuid}]
+        g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=task2.uuid)
+        registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
+        assert registered_tasks == []
 
-    assert "[ test_callback, func1, func2 ]" in str(ex_context)
-
-    task1 = g.call.test_callback() & PERIOD(interval="20s")
-    registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
-    assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task1.uuid}]
-    task1.cancel()
-    registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
-    assert registered_tasks == []
-
-    # Cancel by id
-    task2 = g.call.test_callback() & PERIOD(interval="20s")
-    registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
-    assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task2.uuid}]
-    assert g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=task1.uuid) is False
-    with pytest.raises(RemoteCallError):
-        g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=1234567890)
-    registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
-    assert registered_tasks == [{"condition": "period", "func_name": "test_callback", "uuid": task2.uuid}]
-    g.cancel_scheduled_task_by_uuid(remote_process="test-node", uuid=task2.uuid)
-    registered_tasks = g.get_scheduled_tasks(remote_process="test-node")
-    assert registered_tasks == []
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+    finally:
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_pipeline.py` & `daffi-2.2.1/tests/integration/test_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,141 +2,138 @@
 import sys
 from daffi import FG, BG
 from subprocess import Popen
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_callback_per_node_unix(remote_callbacks_path, exec_type, g):
+async def test_callback_per_node_unix(remote_callbacks_path, exec_type, g, stop_components):
     g = g()
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             cb_name=f"cb{i}",
             next_cb_name=f"cb{i + 1}",
             last=len(range_) == i,
             template_name="pipeline.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"pl-node-{i}",
             exec_type=exec_type.__name__,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
-
-    value = g.call.cb1() & FG
-    assert value == "My secret value"
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+        g.wait_process(f"pl-node-{i}")
+    try:
+        value = g.call.cb1() & FG
+        assert value == "My secret value"
+    finally:
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
-async def test_callback_per_node_tcp(remote_callbacks_path, exec_type, g):
+async def test_callback_per_node_tcp(remote_callbacks_path, exec_type, g, stop_components):
     g = g(host="localhost")
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             cb_name=f"cb{i}",
             next_cb_name=f"cb{i + 1}",
             last=len(range_) == i,
             template_name="pipeline.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"pl-node-{i}",
             exec_type=exec_type.__name__,
             host="localhost",
             port=g.port,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"pl-node-{i}")
 
-    value = g.call.cb1() & FG
-    assert value == "My secret value"
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+    try:
+        value = g.call.cb1() & FG
+        assert value == "My secret value"
+    finally:
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_callback_per_node_unix_async(remote_callbacks_path, exec_type, g):
+async def test_callback_per_node_unix_async(remote_callbacks_path, exec_type, g, stop_components):
     g = g()
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             cb_name=f"cb{i}",
             next_cb_name=f"cb{i + 1}",
             last=len(range_) == i,
             template_name="pipeline2.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"pl-node-{i}",
             exec_type=exec_type.__name__,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
-
-    value = g.call.cb1() & FG
-    assert value == "My secret value"
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+        g.wait_process(f"pl-node-{i}")
+    try:
+        value = g.call.cb1() & FG
+        assert value == "My secret value"
+    finally:
+        await stop_components(remotes, g)
 
 
 @pytest.mark.parametrize("exec_type", [FG, BG])
-async def test_callback_per_node_tcp_async(remote_callbacks_path, exec_type, g):
+async def test_callback_per_node_tcp_async(remote_callbacks_path, exec_type, g, stop_components):
     g = g(host="localhost")
     start_range = 1
     end_range = 10
     range_ = list(range(start_range, end_range))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             cb_name=f"cb{i}",
             next_cb_name=f"cb{i + 1}",
             last=len(range_) == i,
             template_name="pipeline2.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"pl-node-{i}",
             exec_type=exec_type.__name__,
             host="localhost",
             port=g.port,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
-
-    value = g.call.cb1() & FG
-    assert value == "My secret value"
-
-    g.stop(True)
-    [p.terminate() for p in remotes]
+        g.wait_process(f"pl-node-{i}")
+    try:
+        value = g.call.cb1() & FG
+        assert value == "My secret value"
+    finally:
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_stream_callback_to_fetcher.py` & `daffi-2.2.1/tests/integration/test_stream_callback_to_fetcher.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from daffi.decorators import alias
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_stream_callback_to_fetcher_per_node_unix(remote_callbacks_path, g):
+async def test_stream_callback_to_fetcher_per_node_unix(remote_callbacks_path, g, stop_components):
     g = g()
     start_range = 1
     end_range = 6
     range_ = list(range(start_range, end_range))
 
     class StreamReceiver(Fetcher):
         def process_stream(self, end: int):
@@ -30,33 +30,15 @@
             return Args(end=end)
 
         @alias("process_class_stream")
         def process_class_stream_with_alias(self, end: int):
             end = end * 2
             return Args(end=end)
 
-    class StreamReceiverWithCallback(Fetcher, Callback):
-        def process_stream(self, end: int):
-            return end
-
-        def process_class_stream(self, end: int):
-            return end
-
-        @alias("process_stream")
-        def process_stream_with_alias(self, end: int):
-            end = end * 2
-            return Args(end=end)
-
-        @alias("process_class_stream")
-        def process_class_stream_with_alias(self, end: int):
-            end = end * 2
-            return Args(end=end)
-
     stream_receiver = StreamReceiver()
-    stream_with_callback_receiver = StreamReceiverWithCallback()
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             template_name="stream_from_callback.jinja2",
             process_name=f"node-{i}",
         )
@@ -67,51 +49,32 @@
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
         g.wait_process(f"node-{i}")
 
     try:
         res = stream_receiver.process_stream(1000)
-
-        assert set(res) == set(range(1000))
+        assert set(res.get()) == set(range(1000))
 
         # Execute with different exec modifier
         res = stream_receiver.process_class_stream.call(exec_modifier=BG(timeout=10, eta=2), end=2000)
-        assert set(res) == set(range(2000))
+        assert set(res.get()) == set(range(2000))
 
         res = stream_receiver.process_stream_with_alias(1000)
-        assert set(res) == set(range(2000))
+        assert set(res.get()) == set(range(2000))
 
         # Execute with different exec modifier
         res = stream_receiver.process_class_stream_with_alias.call(exec_modifier=BG(timeout=10, eta=2), end=2000)
-        assert set(res) == set(range(4000))
-
-        # Test Fetcher and Callback parents. Fetcher method must be proxy in this case
-        res = stream_with_callback_receiver.process_stream(1000)
-
-        assert set(res) == set(range(1000))
-
-        # Execute with different exec modifier
-        res = stream_with_callback_receiver.process_class_stream.call(exec_modifier=BG(timeout=10, eta=2), end=2000)
-        assert set(res) == set(range(2000))
-
-        res = stream_with_callback_receiver.process_stream_with_alias(1000)
-        assert set(res) == set(range(1000))
-
-        # Execute with different exec modifier
-        res = stream_with_callback_receiver.process_class_stream_with_alias.call(
-            exec_modifier=BG(timeout=10, eta=2), end=2000
-        )
-        assert set(res) == set(range(2000))
+        assert set(res.get()) == set(range(4000))
 
     finally:
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
-async def test_stream_callback_to_fetcher_per_node_tcp(remote_callbacks_path, g):
+async def test_stream_callback_to_fetcher_per_node_tcp(remote_callbacks_path, g, stop_components):
     g = g(host="localhost")
     start_range = 1
     end_range = 6
     range_ = list(range(start_range, end_range))
 
     class StreamReceiver(Fetcher):
         def process_stream(self, end: int):
@@ -145,22 +108,22 @@
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
         g.wait_process(f"node-{i}")
 
     try:
         res = stream_receiver.process_stream(1000)
-        assert set(res) == set(range(1000))
+        assert set(res.get()) == set(range(1000))
 
         # Execute with different exec modifier
         res = stream_receiver.process_class_stream.call(exec_modifier=BG(timeout=10, eta=2), end=2000)
-        assert set(res) == set(range(2000))
+        assert set(res.get()) == set(range(2000))
 
         res = stream_receiver.process_stream_with_alias(1000)
-        assert set(res) == set(range(1000))
+        assert set(res.get()) == set(range(1000))
 
         # Execute with different exec modifier
         res = stream_receiver.process_class_stream_with_alias.call(exec_modifier=BG(timeout=10, eta=2), end=2000)
-        assert set(res) == set(range(2000))
+        assert set(res.get()) == set(range(2000))
 
     finally:
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/test_stream_fetcher_to_callback.py` & `daffi-2.2.1/tests/integration/test_stream_fetcher_to_callback.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from daffi.decorators import fetcher, __body_unknown__
 from subprocess import Popen
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_stream_per_node_unix(remote_callbacks_path, g):
+async def test_stream_per_node_unix(remote_callbacks_path, g, stop_components):
     g = g()
     start_range = 1
     end_range = 6
     range_ = list(range(start_range, end_range))
     stream_values = list(range(int(1e3)))
 
     @fetcher
@@ -21,109 +21,104 @@
         for i in stream_values:
             yield i
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             template_name="stream.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"stream1-node-{i}",
             cb_name=i,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"stream1-node-{i}")
 
     try:
         process_stream()
         for i in range_:
             processed_arr = getattr(g.call, f"stream_result_{i}")() & FG(timeout=10)
             assert set(stream_values) == set(processed_arr)
-        g.stop(True)
-
     finally:
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
 @pytest.mark.skipif(sys.platform == "win32", reason="Unix sockets dont work on windows")
-async def test_stream_per_node_unix_using_remote_decorator(remote_callbacks_path, g):
+async def test_stream_per_node_unix_using_remote_decorator(remote_callbacks_path, g, stop_components):
     @fetcher
     def process_stream(stream):
         yield from iter(stream)
 
     g = g()
     start_range = 1
     end_range = 6
     range_ = list(range(start_range, end_range))
     stream_values = list(range(int(1e3)))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             template_name="stream.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"stream2-node-{i}",
             cb_name=i,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"stream2-node-{i}")
 
     try:
         process_stream(stream_values)
 
         for i in range_:
             processed_arr = getattr(g.call, f"stream_result_{i}")() & FG(timeout=10)
             assert set(stream_values) == set(processed_arr)
-
-        g.stop(True)
     finally:
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
 
 
-async def test_stream_per_node_tcp(remote_callbacks_path, g):
+async def test_stream_per_node_tcp(remote_callbacks_path, g, stop_components):
     @fetcher
     def process_stream(stream):
         yield from iter(stream)
 
     g = g(host="localhost")
     start_range = 1
     end_range = 6
     range_ = list(range(start_range, end_range))
     stream_values = list(range(int(1e3)))
 
     executable_files = [
         remote_callbacks_path(
             filename=f"{i}.py",
             template_name="stream.jinja2",
-            process_name=f"node-{i}",
+            process_name=f"stream3-node-{i}",
             cb_name=i,
             host="localhost",
             port=g.port,
         )
         for i in range_
     ]
 
     remotes = []
     for exc in executable_files:
         remotes.append(Popen([sys.executable, exc]))
     for i in range_:
-        g.wait_process(f"node-{i}")
+        g.wait_process(f"stream3-node-{i}")
 
     try:
         process_stream(stream_values)
 
         for i in range_:
             processed_arr = getattr(g.call, f"stream_result_{i}")() & FG(timeout=10)
             assert set(stream_values) == set(processed_arr)
 
-        g.stop(True)
     finally:
-        [p.terminate() for p in remotes]
+        await stop_components(remotes, g)
```

### Comparing `daffi-2.2.0/tests/integration/templates/test_trio.jinja2` & `daffi-2.2.1/tests/integration/templates/test_trio.jinja2`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/integration/templates/layout/base.jinja2` & `daffi-2.2.1/tests/integration/templates/layout/base.jinja2`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/unit/test_async_result.py` & `daffi-2.2.1/tests/unit/test_async_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,22 +46,25 @@
         asyncio.create_task(set_result(1, 12345, "test"))
         res = await ares.get_async(5)
         assert res == "test"
         # second time the same result
         assert ares.get() == "test"
 
     async def test_get_result_type(self):
-        res = get_result_type(False, False)
+        res, allow_compute = get_result_type(False, False)
         assert isinstance(res, type(AsyncResult))
+        assert allow_compute is True
 
-        res = get_result_type(False, True)
+        res, allow_compute = get_result_type(False, True)
         assert isinstance(res, type(SchedulerTask))
+        assert allow_compute is False
 
-        res = get_result_type(True, True)
+        res, allow_compute = get_result_type(True, True)
         assert isinstance(res, type(IterableAsyncResult))
+        assert allow_compute is False
 
 
 class TestScheduledTaskSuite:
     async def test_get_result(self):
         ares = SchedulerTask(msg=msg)._register()
         asyncio.create_task(set_result(1, 12345, "test"))
         res = await to_thread.run_sync(ares.get)
```

### Comparing `daffi-2.2.0/tests/unit/test_callback_decorator.py` & `daffi-2.2.1/tests/unit/test_callback_decorator.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/unit/test_fetcher_decorator.py` & `daffi-2.2.1/tests/unit/test_fetcher_decorator.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/unit/test_freezable_queue.py` & `daffi-2.2.1/tests/unit/test_freezable_queue.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/tests/unit/test_logger.py` & `daffi-2.2.1/tests/unit/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,42 +23,42 @@
         return self.msg
 
 
 class TestConsoleWarningFormatter:
     @pytest.mark.parametrize(
         "record, expected_result",
         [
-            (MockLevelRecord(logging.ERROR, "error"), f"{colors.red('error')}"),
+            (MockLevelRecord(logging.ERROR, "error"), f"{colors.red('error')}:"),
             (
                 MockLevelRecord(logging.WARNING, "warning"),
-                f"{colors.yellow('warning')}",
+                f"{colors.yellow('warning')}:",
             ),
-            (MockLevelRecord(logging.INFO, "info"), "info"),
+            (MockLevelRecord(logging.INFO, "info"), f"{colors.green('info')}:"),
         ],
     )
     async def test_get_level_message(self, record, expected_result):
         # Preparation
         formatter = ColoredFormatter()
 
         # Execution
         result = formatter.get_level_message(record)
 
         # Assertion
-        assert result == expected_result
+        assert result.strip() == expected_result
 
     @pytest.mark.parametrize(
         "record, expected_result",
         [
             (
                 MockLevelRecord(logging.ERROR, "error", "error"),
-                f"{colors.red('error')} error",
+                f"{colors.red('error')}:   error",
             ),
             (
                 MockLevelRecord(logging.WARNING, "warning", b"warning"),
-                f"{colors.yellow('warning')} warning",
+                f"{colors.yellow('warning')}: warning",
             ),
         ],
     )
     async def test_format(self, record, expected_result):
         # Preparation
         formatter = ColoredFormatter()
```

### Comparing `daffi-2.2.0/tests/unit/test_misc.py` & `daffi-2.2.1/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/.gitignore` & `daffi-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/LICENSE.txt` & `daffi-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/README.md` & `daffi-2.2.1/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -17,261 +17,268 @@
 [![Downloads](https://static.pepy.tech/badge/daffi/month)](https://pepy.tech/project/daffi)
 
 Daffi facilitates remote computing and enables remote procedure calls between multiple endpoints.
 It supports many-to-many relationships between endpoints, allowing for seamless communication between distributed systems.
 The library abstracts the complexities of remote computing and provides a user-friendly interface for initiating and managing remote procedure calls.
 It also offers various features such as fault tolerance, load balancing, streaming and security, to ensure reliable and secure communication between endpoints.
 
-## Documentation
-
-View full documentation at: [https://600apples.github.io/dafi/](https://600apples.github.io/dafi/)
+Daffi comprises three primary classes:
 
+- *Global* - Initialization entrypoint. Once *Global* object is initialized application can respond on remote requests and trigger remote callbacks itself.
+- *Callback* - Represents a collection of methods encapsulated in a class inherited from *Callback* or a standalone function decorated with the *callback* decorator. These functions/methods can be triggered from another process.
+- *Fetcher* - Represents a collection of methods encapsulated in a class inherited from *Fetcher* or a standalone function decorated with the *fetcher* decorator. These functions/methods serve as triggers for the corresponding callbacks defined in another process.
 
 ## Basic example
 
 You need to create two files `shopping_service.py` and `shopper.py`
 
 `shopping_service.py` - represents a set of remote callbacks that can be triggered by a client application.
 
-`shopper.py` - represents shopping_service client
-
-#### Class based approach
-
-
-`shopping_service.py`:
-```python
-import logging
-from daffi import Global
-from daffi.registry import Callback
-
-logging.basicConfig(level=logging.INFO)
+`shopper.py` - represents shopping_service client (fetcher)
 
 
-class ShoppingService(Callback):
+=== "class based approach"
 
-    def __post_init__(self):
-        self.shopping_list = []
-
-    def get_items(self):
+    `shopping_service.py`:
+    ```python
+    import logging
+    from daffi import Global
+    from daffi.registry import Callback
+    
+    logging.basicConfig(level=logging.INFO)
+    
+    
+    class ShoppingService(Callback):
+        auto_init = True # class is automatically initialized, eliminating the need to manually create an object.
+    
+        def __post_init__(self):
+            self.shopping_list = []
+    
+        def get_items(self):
+            """Return all items that are currently present in shopping list"""
+            return self.shopping_list
+    
+        def add_item(self, item):
+            """Add new item to shopping list"""
+            self.shopping_list.append(item)
+    
+        def clear_items(self):
+            """Clear shopping list"""
+            self.shopping_list.clear()
+    
+    
+    if __name__ == '__main__':
+        Global(init_controller=True, host="localhost", port=8888).join()
+    ```
+    (This script is complete, it should run "as is")
+    
+    
+    `shopper.py`:
+    ```python
+    import logging
+    from daffi import Global
+    from daffi.decorators import alias
+    from daffi.registry import Fetcher
+    
+    logging.basicConfig(level=logging.INFO)
+    
+    
+    class Shopper(Fetcher):
+        """
+        Note: Functions without a body are treated as proxies for remote callbacks.
+        All arguments provided to this function will be sent to the remote service as-is.
+        """
+    
+        def get_items(self):
+            """Return all items that are currently present in shopping list."""
+            pass
+    
+        def add_item(self, item):
+            """Add new item to shopping list."""
+            pass
+    
+        def clear_items(self):
+            """Clear shopping list"""
+            pass
+    
+        @alias("add_item")
+        def add_many_items(self, *items):
+            """
+            Alias for `add_item` callback.
+            This function shows streaming capabilities for transferring data from one service to another.
+            """
+            for item in items:
+                yield item
+    
+    
+    if __name__ == '__main__':
+        g = Global(host="localhost", port=8888)
+    
+        shopper = Shopper()
+        items = shopper.get_items()
+        print(items)
+    
+        shopper.add_item("orange")
+        items = shopper.get_items()
+        print(items)
+    
+        shopper.add_many_items("bread", "cheese")
+        items = shopper.get_items()
+        print(items)
+    
+        shopper.clear_items()
+        items = shopper.get_items()
+        print(items)
+    
+        g.stop()
+    ```
+    (This script is complete, it should run "as is")
+    
+    To check the full example, you need to execute two scripts in separate terminals
+    
+    ```bash
+    python3 shopping_service.py
+    
+    ...
+    INFO 2023-03-27 19:49:45 | controller[0x91adb83e] | Controller has been started successfully. Process identificator: '0x91adb83e'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    INFO 2023-03-27 19:49:45 | node[0x91adb83e] | Node has been started successfully. Process identificator: '0x91adb83e'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    ```
+    
+    ```bash
+    python3 shopper.py
+    
+    ...
+    INFO 2023-03-27 19:53:15 | node[0xd7e5d488] | Node has been started successfully. Process identificator: '0xd7e5d488'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    []
+    ['orange']
+    ['orange', 'bread', 'cheese']
+    []
+    INFO 2023-03-27 19:53:15 | node[0xd7e5d488] | Node stopped.
+    ```
+
+=== "decorator based approach"
+    
+      `shopping_service.py`:
+    ```python
+    import logging
+    from daffi import Global
+    from daffi.decorators import callback
+    
+    logging.basicConfig(level=logging.INFO)
+    
+    shopping_list = []
+    
+    
+    @callback
+    def get_items():
         """Return all items that are currently present in shopping list"""
-        return self.shopping_list
-
-    def add_item(self, item):
+        return shopping_list
+    
+    
+    @callback
+    def add_item(item):
         """Add new item to shopping list"""
-        self.shopping_list.append(item)
-
-    def clear_items(self):
+        shopping_list.append(item)
+    
+    
+    @callback
+    def clear_items():
         """Clear shopping list"""
-        self.shopping_list.clear()
-
-
-if __name__ == '__main__':
-    Global(init_controller=True, host="localhost", port=8888).join()
-```
-(This script is complete, it should run "as is")
-
-
-`shopper.py`:
-```python
-import logging
-from daffi import Global
-from daffi.decorators import alias
-from daffi.registry import Fetcher
-
-logging.basicConfig(level=logging.INFO)
-
-
-class Shopper(Fetcher):
+        shopping_list.clear()
+    
+    
+    if __name__ == '__main__':
+        Global(init_controller=True, host="localhost", port=8888).join()
+    ```
+    (This script is complete, it should run "as is")
+    
+    
+    `shopper.py`:
+    ```python
     """
     Note: Functions without a body are treated as proxies for remote callbacks.
-    All arguments provided to this function will be sent to the remote service as-is.
+        All arguments provided to this function will be sent to the remote service as-is.
     """
-
-    def get_items(self):
+    import logging
+    from daffi import Global
+    from daffi.decorators import alias, fetcher
+    
+    logging.basicConfig(level=logging.INFO)
+    
+    
+    @fetcher
+    def get_items():
         """Return all items that are currently present in shopping list."""
         pass
-
-    def add_item(self, item):
+    
+    
+    @fetcher
+    def add_item(item):
         """Add new item to shopping list."""
         pass
-
-    def clear_items(self):
-        """Clear shopping list"""
+    
+    
+    @fetcher
+    def clear_items():
+        """Add new item to shopping list."""
         pass
-
+    
+    
     @alias("add_item")
-    def add_many_items(self, *items):
+    @fetcher
+    def add_many_items(*items):
         """
         Alias for `add_item` callback.
         This function shows streaming capabilities for transferring data from one service to another.
         """
         for item in items:
             yield item
-
-
-if __name__ == '__main__':
-    g = Global(host="localhost", port=8888)
-
-    shopper = Shopper()
-    items = shopper.get_items()
-    print(items)
-
-    shopper.add_item("orange")
-    items = shopper.get_items()
-    print(items)
-
-    shopper.add_many_items("bread", "cheese")
-    items = shopper.get_items()
-    print(items)
-
-    shopper.clear_items()
-    items = shopper.get_items()
-    print(items)
-
-    g.stop()
-```
-(This script is complete, it should run "as is")
-
-To check the full example, you need to execute two scripts in separate terminals
-
-```bash
-python3 shopping_service.py
-
-...
-INFO 2023-03-27 19:49:45 | controller[0x91adb83e] | Controller has been started successfully. Process identificator: '0x91adb83e'. Connection info: tcp: [ host '[::]', port: 8888 ]
-INFO 2023-03-27 19:49:45 | node[0x91adb83e] | Node has been started successfully. Process identificator: '0x91adb83e'. Connection info: tcp: [ host '[::]', port: 8888 ]
-```
-
-```bash
-python3 shopper.py
-
-...
-INFO 2023-03-27 19:53:15 | node[0xd7e5d488] | Node has been started successfully. Process identificator: '0xd7e5d488'. Connection info: tcp: [ host '[::]', port: 8888 ]
-[]
-['orange']
-['orange', 'bread', 'cheese']
-[]
-INFO 2023-03-27 19:53:15 | node[0xd7e5d488] | Node stopped.
-```
-
-### Decorators base approach
-
-`shopping_service.py`:
-```python
-import logging
-from daffi import Global
-from daffi.decorators import callback
-
-logging.basicConfig(level=logging.INFO)
-
-shopping_list = []
-
-
-@callback
-def get_items():
-    """Return all items that are currently present in shopping list"""
-    return shopping_list
-
-
-@callback
-def add_item(item):
-    """Add new item to shopping list"""
-    shopping_list.append(item)
-
-
-@callback
-def clear_items():
-    """Clear shopping list"""
-    shopping_list.clear()
-
-
-if __name__ == '__main__':
-    Global(init_controller=True, host="localhost", port=8888).join()
-```
-(This script is complete, it should run "as is")
-
-
-`shopper.py`:
-```python
-"""
-Note: Functions without a body are treated as proxies for remote callbacks.
-    All arguments provided to this function will be sent to the remote service as-is.
-"""
-import logging
-from daffi import Global
-from daffi.decorators import alias, fetcher
-
-logging.basicConfig(level=logging.INFO)
-
-
-@fetcher
-def get_items():
-    """Return all items that are currently present in shopping list."""
-    pass
-
-
-@fetcher
-def add_item(item):
-    """Add new item to shopping list."""
-    pass
-
-
-@fetcher
-def clear_items():
-    """Add new item to shopping list."""
-    pass
-
-
-@alias("add_item")
-@fetcher
-def add_many_items(*items):
-    """
-    Alias for `add_item` callback.
-    This function shows streaming capabilities for transferring data from one service to another.
-    """
-    for item in items:
-        yield item
-
-
-if __name__ == '__main__':
-    g = Global(host="localhost", port=8888)
-
-    items = get_items()
-    print(items)
-
-    add_item("orange")
-    items = get_items()
-    print(items)
-
-    add_many_items("bread", "cheese")
-    items = get_items()
-    print(items)
-
-    clear_items()
-    items = get_items()
-    print(items)
-
-    g.stop()
-```
-(This script is complete, it should run "as is")
-
-To check the full example, you need to execute two scripts in separate terminals
-
-```bash
-python3 shopping_service.py
-
-...
-INFO 2023-03-27 20:31:27 | controller[0xbac16ef4] | Controller has been started successfully. Process identificator: '0xbac16ef4'. Connection info: tcp: [ host '[::]', port: 8888 ]
-INFO 2023-03-27 20:31:27 | node[0xbac16ef4] | Node has been started successfully. Process identificator: '0xbac16ef4'. Connection info: tcp: [ host '[::]', port: 8888 ]
-```
-
-```bash
-python3 shopper.py
-
-...
-INFO 2023-03-27 20:31:43 | node[0xb9e10444] | Node has been started successfully. Process identificator: '0xb9e10444'. Connection info: tcp: [ host '[::]', port: 8888 ]
-[]
-['orange']
-['orange', 'bread', 'cheese']
-[]
-INFO 2023-03-27 20:31:44 | node[0xb9e10444] | Node stopped.
-```
+    
+    
+    if __name__ == '__main__':
+        g = Global(host="localhost", port=8888)
+    
+        items = get_items()
+        print(items)
+    
+        add_item("orange")
+        items = get_items()
+        print(items)
+    
+        add_many_items("bread", "cheese")
+        items = get_items()
+        print(items)
+    
+        clear_items()
+        items = get_items()
+        print(items)
+    
+        g.stop()
+    ```
+    (This script is complete, it should run "as is")
+    
+    To check the full example, you need to execute two scripts in separate terminals
+    
+    ```bash
+    python3 shopping_service.py
+    
+    ...
+    INFO 2023-03-27 20:31:27 | controller[0xbac16ef4] | Controller has been started successfully. Process identificator: '0xbac16ef4'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    INFO 2023-03-27 20:31:27 | node[0xbac16ef4] | Node has been started successfully. Process identificator: '0xbac16ef4'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    ```
+    
+    ```bash
+    python3 shopper.py
+    
+    ...
+    INFO 2023-03-27 20:31:43 | node[0xb9e10444] | Node has been started successfully. Process identificator: '0xb9e10444'. Connection info: tcp: [ host '[::]', port: 8888 ]
+    []
+    ['orange']
+    ['orange', 'bread', 'cheese']
+    []
+    INFO 2023-03-27 20:31:44 | node[0xb9e10444] | Node stopped.
+    ```
+
+
+!!! note 
+    To use UNIX socket instead of TCP for communication, you should remove the `host` and `port` parameters from 
+    the initialization of the Global object, and optionally include the `unix_sock_path` parameter.
```

### Comparing `daffi-2.2.0/pyproject.toml` & `daffi-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `daffi-2.2.0/PKG-INFO` & `daffi-2.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffi
-Version: 2.2.0
+Version: 2.2.1
 Summary: Daffi is fast, simple and lightweight library for inter process communication
 Project-URL: Documentation, https://600apples.github.io/dafi/
 Project-URL: Source, https://github.com/600apples/dafi
 Author-email: Volodymyr Boiko <600apples@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: async,distributed,grpc,job,python,queue,rpc,stream,task
@@ -59,40 +59,47 @@
 [![Downloads](https://static.pepy.tech/badge/daffi/month)](https://pepy.tech/project/daffi)
 
 Daffi facilitates remote computing and enables remote procedure calls between multiple endpoints.
 It supports many-to-many relationships between endpoints, allowing for seamless communication between distributed systems.
 The library abstracts the complexities of remote computing and provides a user-friendly interface for initiating and managing remote procedure calls.
 It also offers various features such as fault tolerance, load balancing, streaming and security, to ensure reliable and secure communication between endpoints.
 
+Daffi comprises three primary classes:
+
+- *Global* - Initialization entrypoint. Once *Global* object is initialized application can respond on remote requests and trigger remote callbacks itself.
+- *Callback* - Represents a collection of methods encapsulated in a class inherited from *Callback* or a standalone function decorated with the *callback* decorator. These functions/methods can be triggered from another process.
+- *Fetcher* - Represents a collection of methods encapsulated in a class inherited from *Fetcher* or a standalone function decorated with the *fetcher* decorator. These functions/methods serve as triggers for the corresponding callbacks defined in another process.
+
 ## Documentation
 
 View full documentation at: [https://600apples.github.io/dafi/](https://600apples.github.io/dafi/)
 
 
 ## Basic example
 
 You need to create two files `shopping_service.py` and `shopper.py`
 
 `shopping_service.py` - represents a set of remote callbacks that can be triggered by a client application.
 
-`shopper.py` - represents shopping_service client
+`shopper.py` - represents shopping_service client (fetcher)
 
 #### Class based approach
 
 
 `shopping_service.py`:
 ```python
 import logging
 from daffi import Global
 from daffi.registry import Callback
 
 logging.basicConfig(level=logging.INFO)
 
 
 class ShoppingService(Callback):
+    auto_init = True # class is automatically initialized, eliminating the need to manually create an object.
 
     def __post_init__(self):
         self.shopping_list = []
 
     def get_items(self):
         """Return all items that are currently present in shopping list"""
         return self.shopping_list
```

