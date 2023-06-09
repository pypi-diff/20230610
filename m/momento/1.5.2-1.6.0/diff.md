# Comparing `tmp/momento-1.5.2.tar.gz` & `tmp/momento-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.5.2.tar", max compression
+gzip compressed data, was "momento-1.6.0.tar", max compression
```

## Comparing `momento-1.5.2.tar` & `momento-1.6.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2023-06-05 16:42:27.604468 momento-1.5.2/LICENSE
--rw-r--r--   0        0        0     4142 2023-06-05 16:42:27.604468 momento-1.5.2/README.md
--rw-r--r--   0        0        0     3805 2023-06-05 16:42:51.981947 momento-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      619 2023-06-05 16:42:27.604468 momento-1.5.2/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43756 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/cache_client.py
--rw-r--r--   0        0        0    44407 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      406 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4735 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0      531 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/_utilities/_momento_version.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5794 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    47746 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3206 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5700 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    47366 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2436 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6841 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0      849 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/flush.py
--rw-r--r--   0        0        0     2275 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-06-05 16:42:27.608468 momento-1.5.2/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1046 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/increment.py
--rw-r--r--   0        0        0      944 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-06-05 16:42:27.612468 momento-1.5.2/src/momento/typing.py
--rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 momento-1.5.2/setup.py
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 momento-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 22:36:27.728766 momento-1.6.0/LICENSE
+-rw-r--r--   0        0        0     4142 2023-06-09 22:36:27.728766 momento-1.6.0/README.md
+-rw-r--r--   0        0        0     3805 2023-06-09 22:36:50.288958 momento-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43798 2023-06-09 22:36:27.728766 momento-1.6.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44449 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4735 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0      531 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/_utilities/_momento_version.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     5794 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    47789 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3206 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     5700 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    47409 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2436 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6841 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2275 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-06-09 22:36:27.732766 momento-1.6.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1087 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/increment_score.py
+-rw-r--r--   0        0        0      944 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-06-09 22:36:27.736766 momento-1.6.0/src/momento/typing.py
+-rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 momento-1.6.0/setup.py
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 momento-1.6.0/PKG-INFO
```

### Comparing `momento-1.5.2/LICENSE` & `momento-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/README.md` & `momento-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/pyproject.toml` & `momento-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.5.2"
+version = "1.6.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
```

### Comparing `momento-1.5.2/src/momento/__init__.py` & `momento-1.6.0/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/auth/credential_provider.py` & `momento-1.6.0/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.6.0/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/cache_client.py` & `momento-1.6.0/src/momento/cache_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     CacheSortedSetGetScore,
     CacheSortedSetGetScoreResponse,
 )
 from momento.responses.data.sorted_set.get_scores import (
     CacheSortedSetGetScores,
     CacheSortedSetGetScoresResponse,
 )
-from momento.responses.data.sorted_set.increment import CacheSortedSetIncrementResponse
+from momento.responses.data.sorted_set.increment_score import (
+    CacheSortedSetIncrementScoreResponse,
+)
 from momento.responses.data.sorted_set.put_element import (
     CacheSortedSetPutElement,
     CacheSortedSetPutElementResponse,
 )
 from momento.responses.data.sorted_set.put_elements import (
     CacheSortedSetPutElements,
     CacheSortedSetPutElementsResponse,
@@ -1014,38 +1016,38 @@
             values (Iterable[str | bytes]): The values of the elements to remove from the sorted set.
 
         Returns:
             CacheSortedSetRemoveElementsResponse: result of the remove elements operation.
         """
         return self._data_client.sorted_set_remove_elements(cache_name, sorted_set_name, values)
 
-    def sorted_set_increment(
+    def sorted_set_increment_score(
         self,
         cache_name: str,
         sorted_set_name: str,
         value: str | bytes,
         score: float = 1.0,
         *,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
-    ) -> CacheSortedSetIncrementResponse:
+    ) -> CacheSortedSetIncrementScoreResponse:
         """Increments the score for the given sorted set and value.
 
         If the value doesn't exist in the sorted set, it will be added and its score set to the given score.
 
         Args:
             cache_name (str): Name of the cache to perform the lookup in.
             sorted_set_name (str): The sorted set to look up.
             value (str | bytes): The value in the sorted set to look up.
             score (float): The quantity to add to the score. May be positive, negative, or zero. Defaults to 1.0.
             ttl: (CollectionTtl, optional): How to treat the sorted set's TTL.
                 Defaults to `CollectionTtl.from_cache_ttl()`
 
         Returns:
-            CacheSortedSetIncrementResponse: the status and associated score for each value.
+            CacheSortedSetIncrementScoreResponse: the status and associated score for each value.
         """
-        return self._data_client.sorted_set_increment(cache_name, sorted_set_name, value, score, ttl)
+        return self._data_client.sorted_set_increment_score(cache_name, sorted_set_name, value, score, ttl)
 
     @property
     def _data_client(self) -> _ScsDataClient:
         client = self._data_clients[self._next_client_index]
         self._next_client_index = (self._next_client_index + 1) % len(self._data_clients)
         return client
```

### Comparing `momento-1.5.2/src/momento/cache_client_async.py` & `momento-1.6.0/src/momento/cache_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     CacheSortedSetGetScore,
     CacheSortedSetGetScoreResponse,
 )
 from momento.responses.data.sorted_set.get_scores import (
     CacheSortedSetGetScores,
     CacheSortedSetGetScoresResponse,
 )
-from momento.responses.data.sorted_set.increment import CacheSortedSetIncrementResponse
+from momento.responses.data.sorted_set.increment_score import (
+    CacheSortedSetIncrementScoreResponse,
+)
 from momento.responses.data.sorted_set.put_element import (
     CacheSortedSetPutElement,
     CacheSortedSetPutElementResponse,
 )
 from momento.responses.data.sorted_set.put_elements import (
     CacheSortedSetPutElements,
     CacheSortedSetPutElementsResponse,
@@ -1021,38 +1023,38 @@
             values (Iterable[str | bytes]): The values of the elements to remove from the sorted set.
 
         Returns:
             CacheSortedSetRemoveElementsResponse: result of the remove elements operation.
         """
         return await self._data_client.sorted_set_remove_elements(cache_name, sorted_set_name, values)
 
-    async def sorted_set_increment(
+    async def sorted_set_increment_score(
         self,
         cache_name: str,
         sorted_set_name: str,
         value: str | bytes,
         score: float = 1.0,
         *,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
-    ) -> CacheSortedSetIncrementResponse:
+    ) -> CacheSortedSetIncrementScoreResponse:
         """Increments the score for the given sorted set and value.
 
         If the value doesn't exist in the sorted set, it will be added and its score set to the given score.
 
         Args:
             cache_name (str): Name of the cache to perform the lookup in.
             sorted_set_name (str): The sorted set to look up.
             value (str | bytes): The value in the sorted set to look up.
             score (float): The quantity to add to the score. May be positive, negative, or zero. Defaults to 1.0.
             ttl: (CollectionTtl, optional): How to treat the sorted set's TTL.
                 Defaults to `CollectionTtl.from_cache_ttl()`
 
         Returns:
-            CacheSortedSetIncrementResponse: the status and associated score for each value.
+            CacheSortedSetIncrementScoreResponse: the status and associated score for each value.
         """
-        return await self._data_client.sorted_set_increment(cache_name, sorted_set_name, value, score, ttl)
+        return await self._data_client.sorted_set_increment_score(cache_name, sorted_set_name, value, score, ttl)
 
     @property
     def _data_client(self) -> _ScsDataClient:
         client = self._data_clients[self._next_client_index]
         self._next_client_index = (self._next_client_index + 1) % len(self._data_clients)
         return client
```

### Comparing `momento-1.5.2/src/momento/config/configuration.py` & `momento-1.6.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/config/configurations.py` & `momento-1.6.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/config/transport/transport_strategy.py` & `momento-1.6.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/errors/__init__.py` & `momento-1.6.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/errors/error_converter.py` & `momento-1.6.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/errors/error_details.py` & `momento-1.6.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/errors/exceptions.py` & `momento-1.6.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/_utilities/_data_validation.py` & `momento-1.6.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/_utilities/_momento_version.py` & `momento-1.6.0/src/momento/internal/_utilities/_momento_version.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.6.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.6.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/aio/_scs_control_client.py` & `momento-1.6.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/aio/_scs_data_client.py` & `momento-1.6.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     CacheSortedSetGetScore,
     CacheSortedSetGetScoreResponse,
 )
 from momento.responses.data.sorted_set.get_scores import (
     CacheSortedSetGetScores,
     CacheSortedSetGetScoresResponse,
 )
-from momento.responses.data.sorted_set.increment import (
-    CacheSortedSetIncrement,
-    CacheSortedSetIncrementResponse,
+from momento.responses.data.sorted_set.increment_score import (
+    CacheSortedSetIncrementScore,
+    CacheSortedSetIncrementScoreResponse,
 )
 from momento.responses.data.sorted_set.put_elements import (
     CacheSortedSetPutElements,
     CacheSortedSetPutElementsResponse,
 )
 from momento.responses.data.sorted_set.remove_elements import (
     CacheSortedSetRemoveElements,
@@ -1040,22 +1040,22 @@
             self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_remove_elements", e)
             return CacheSortedSetRemoveElements.Error(convert_error(e))
 
-    async def sorted_set_increment(
+    async def sorted_set_increment_score(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         score: TSortedSetScore,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
-    ) -> CacheSortedSetIncrementResponse:
+    ) -> CacheSortedSetIncrementScoreResponse:
         try:
             self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
             _validate_sorted_set_score(score)
 
             request = cache_pb._SortedSetIncrementRequest(
@@ -1068,18 +1068,18 @@
             response = await self._build_stub().SortedSetIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
 
-            return CacheSortedSetIncrement.Success(response.score)
+            return CacheSortedSetIncrementScore.Success(response.score)
         except Exception as e:
-            self._log_request_error("sorted_set_increment", e)
-            return CacheSortedSetIncrement.Error(convert_error(e))
+            self._log_request_error("sorted_set_increment_score", e)
+            return CacheSortedSetIncrementScore.Error(convert_error(e))
 
     def _log_received_response(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Received a {request_type} response for {request_args}")
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
```

### Comparing `momento-1.5.2/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.6.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.6.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.6.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.6.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.6.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     CacheSortedSetGetScore,
     CacheSortedSetGetScoreResponse,
 )
 from momento.responses.data.sorted_set.get_scores import (
     CacheSortedSetGetScores,
     CacheSortedSetGetScoresResponse,
 )
-from momento.responses.data.sorted_set.increment import (
-    CacheSortedSetIncrement,
-    CacheSortedSetIncrementResponse,
+from momento.responses.data.sorted_set.increment_score import (
+    CacheSortedSetIncrementScore,
+    CacheSortedSetIncrementScoreResponse,
 )
 from momento.responses.data.sorted_set.put_elements import (
     CacheSortedSetPutElements,
     CacheSortedSetPutElementsResponse,
 )
 from momento.responses.data.sorted_set.remove_elements import (
     CacheSortedSetRemoveElements,
@@ -1038,22 +1038,22 @@
             self._log_received_response("SortedSetRemoveElements", {"sorted_set_name": str(request.set_name)})
 
             return CacheSortedSetRemoveElements.Success()
         except Exception as e:
             self._log_request_error("sorted_set_remove_elements", e)
             return CacheSortedSetRemoveElements.Error(convert_error(e))
 
-    def sorted_set_increment(
+    def sorted_set_increment_score(
         self,
         cache_name: TCacheName,
         sorted_set_name: TSortedSetName,
         value: TSortedSetValue,
         score: TSortedSetScore,
         ttl: CollectionTtl = CollectionTtl.from_cache_ttl(),
-    ) -> CacheSortedSetIncrementResponse:
+    ) -> CacheSortedSetIncrementScoreResponse:
         try:
             self._log_issuing_request("SortedSetIncrement", {"sorted_set_name": str(sorted_set_name)})
             _validate_cache_name(cache_name)
             _validate_sorted_set_name(sorted_set_name)
             _validate_sorted_set_score(score)
 
             request = cache_pb._SortedSetIncrementRequest(
@@ -1066,18 +1066,18 @@
             response = self._build_stub().SortedSetIncrement(
                 request,
                 metadata=make_metadata(cache_name),
                 timeout=self._default_deadline_seconds,
             )
             self._log_received_response("SortedSetIncrement", {"sorted_set_name": str(request.set_name)})
 
-            return CacheSortedSetIncrement.Success(response.score)
+            return CacheSortedSetIncrementScore.Success(response.score)
         except Exception as e:
-            self._log_request_error("sorted_set_increment", e)
-            return CacheSortedSetIncrement.Error(convert_error(e))
+            self._log_request_error("sorted_set_increment_score", e)
+            return CacheSortedSetIncrementScore.Error(convert_error(e))
 
     def _log_received_response(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Received a {request_type} response for {request_args}")
 
     def _log_issuing_request(self, request_type: str, request_args: dict[str, str]) -> None:
         self._logger.log(logs.TRACE, f"Issuing a {request_type} request with {request_args}")
```

### Comparing `momento-1.5.2/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.6.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/logs.py` & `momento-1.6.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/requests/collection_ttl.py` & `momento-1.6.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/__init__.py` & `momento-1.6.0/src/momento/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/cache/create.py` & `momento-1.6.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/cache/delete.py` & `momento-1.6.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/cache/flush.py` & `momento-1.6.0/src/momento/responses/control/cache/flush.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/cache/list.py` & `momento-1.6.0/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/signing_key/create.py` & `momento-1.6.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/signing_key/list.py` & `momento-1.6.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/control/signing_key/revoke.py` & `momento-1.6.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/fetch.py` & `momento-1.6.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/get_field.py` & `momento-1.6.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.6.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/increment.py` & `momento-1.6.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.6.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.6.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/set_field.py` & `momento-1.6.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.6.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/concatenate_back.py` & `momento-1.6.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/concatenate_front.py` & `momento-1.6.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/fetch.py` & `momento-1.6.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/length.py` & `momento-1.6.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/pop_back.py` & `momento-1.6.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/pop_front.py` & `momento-1.6.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/push_back.py` & `momento-1.6.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/push_front.py` & `momento-1.6.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/list/remove_value.py` & `momento-1.6.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/scalar/delete.py` & `momento-1.6.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/scalar/get.py` & `momento-1.6.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/scalar/increment.py` & `momento-1.6.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/scalar/set.py` & `momento-1.6.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.6.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/set/add_element.py` & `momento-1.6.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/set/add_elements.py` & `momento-1.6.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/set/fetch.py` & `momento-1.6.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/set/remove_element.py` & `momento-1.6.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/set/remove_elements.py` & `momento-1.6.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/increment.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/increment_score.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from abc import ABC
 from dataclasses import dataclass
 
 from ...mixins import ErrorResponseMixin
 from ...response import CacheResponse
 
 
-class CacheSortedSetIncrementResponse(CacheResponse):
-    """Parent response type for a cache `sorted_set_increment` request.
+class CacheSortedSetIncrementScoreResponse(CacheResponse):
+    """Parent response type for a cache `sorted_set_increment_score` request.
 
     Its subtypes are:
-    - `CacheSortedSetIncrement.Success`
-    - `CacheSortedSetIncrement.Error`
+    - `CacheSortedSetIncrementScore.Success`
+    - `CacheSortedSetIncrementScore.Error`
 
     See `CacheClient` for how to work with responses.
     """
 
 
-class CacheSortedSetIncrement(ABC):
-    """Groups all `CacheSortedSetIncrementResponse` derived types under a common namespace."""
+class CacheSortedSetIncrementScore(ABC):
+    """Groups all `CacheSortedSetIncrementScoreResponse` derived types under a common namespace."""
 
     @dataclass
-    class Success(CacheSortedSetIncrementResponse):
+    class Success(CacheSortedSetIncrementScoreResponse):
         """Indicates the request was successful."""
 
         score: float
         """The score of the element post-increment."""
 
-    class Error(CacheSortedSetIncrementResponse, ErrorResponseMixin):
+    class Error(CacheSortedSetIncrementScoreResponse, ErrorResponseMixin):
         """Contains information about an error returned from a request.
 
         This includes:
         - `error_code`: `MomentoErrorCode` value for the error.
         - `message`: a detailed error message.
         """
```

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.6.0/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/mixins.py` & `momento-1.6.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/responses/response.py` & `momento-1.6.0/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/retry/default_eligibility_strategy.py` & `momento-1.6.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.6.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/src/momento/typing.py` & `momento-1.6.0/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.5.2/setup.py` & `momento-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'pyjwt>=2.4.0,<3.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4']}
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.5.2',
+    'version': '1.6.0',
     'description': 'SDK for Momento',
     'long_description': '<head>\n  <meta name="Momento Python Client Library Documentation" content="Python client software development kit for Momento Cache">\n</head>\n<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n\n# Momento Python Client Library\n\nMomento Cache is a fast, simple, pay-as-you-go caching solution without any of the operational overhead\nrequired by traditional caching solutions.  This repo contains the source code for the Momento Python client library.\n\n* Website: [https://www.gomomento.com/](https://www.gomomento.com/)\n* Momento Documentation: [https://docs.momentohq.com/](https://docs.momentohq.com/)\n* Getting Started: [https://docs.momentohq.com/getting-started](https://docs.momentohq.com/getting-started)\n* Python SDK Documentation: [https://docs.momentohq.com/develop/sdks/python](https://docs.momentohq.com/develop/sdks/python)\n* Discuss: [Momento Discord](https://discord.gg/3HkAKjUZGq)\n\n## Packages\n\nThe Momento Python SDK package is available on pypi: [momento](https://pypi.org/project/momento/).\n\n## Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache, ListCaches\n\ncache_client = CacheClient(\n    Configurations.Laptop.v1(),\n    CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n    timedelta(seconds=60)\n)\n\ncreate_cache_response = cache_client.create_cache("cache")\nset_response = cache_client.set("cache", "my-key", "my-value")\nget_response = cache_client.get(_CACHE_NAME, _KEY)\nmatch get_response:\n    case CacheGet.Hit() as hit:\n        print(f"Got value: {hit.value_string}")\n    case _:\n        print(f"Response was not a hit: {get_response}")\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\ncache_client = CacheClient(\n    configuration=Configurations.Laptop.v1(),\n    credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n    default_ttl=timedelta(seconds=60)\n)\ncache_client.create_cache("cache")\ncache_client.set("cache", "myKey", "myValue")\nget_response = cache_client.get("cache", "myKey")\nif isinstance(get_response, CacheGet.Hit):\n    print(f"Got value: {get_response.value_string}")\n\n```\n\n## Getting Started and Documentation\n\nDocumentation is available on the [Momento Docs website](https://docs.momentohq.com).\n\n## Examples\n\nWorking example projects, with all required build configuration files, are available for both Python 3.10 and up\nand Python versions before 3.10:\n\n* [Python 3.10+ examples](./examples/py310)\n* [Pre-3.10 Python examples](./examples/prepy310)\n\n## Developing\n\nIf you are interested in contributing to the SDK, please see the [CONTRIBUTING](./CONTRIBUTING.md) docs.\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
```

### Comparing `momento-1.5.2/PKG-INFO` & `momento-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.5.2
+Version: 1.6.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<4.0
```

