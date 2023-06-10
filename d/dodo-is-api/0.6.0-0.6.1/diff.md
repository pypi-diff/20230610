# Comparing `tmp/dodo_is_api-0.6.0.tar.gz` & `tmp/dodo_is_api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.6.0.tar", max compression
+gzip compressed data, was "dodo_is_api-0.6.1.tar", max compression
```

## Comparing `dodo_is_api-0.6.0.tar` & `dodo_is_api-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.6.0/LICENSE
--rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.6.0/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.6.0/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0     4078 2023-05-10 05:30:00.804758 dodo_is_api-0.6.0/dodo_is_api/connection/asynchronous.py
--rw-r--r--   0        0        0     1291 2023-05-10 05:26:32.091787 dodo_is_api-0.6.0/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.6.0/dodo_is_api/connection/http_clients.py
--rw-r--r--   0        0        0     7300 2023-05-10 05:26:32.092054 dodo_is_api-0.6.0/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.6.0/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0     7200 2023-05-10 05:26:32.092333 dodo_is_api-0.6.0/dodo_is_api/mappers.py
--rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.6.0/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0     2798 2023-05-10 05:26:32.092595 dodo_is_api-0.6.0/dodo_is_api/models/dodo_is_api.py
--rw-r--r--   0        0        0     1685 2023-05-10 05:26:32.092836 dodo_is_api-0.6.0/dodo_is_api/models/raw.py
--rw-r--r--   0        0        0      539 2023-05-10 05:31:21.339757 dodo_is_api-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dodo_is_api-0.6.0/setup.py
--rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 dodo_is_api-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.6.1/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-10 05:26:32.091241 dodo_is_api-0.6.1/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0     3607 2023-06-10 06:32:02.342004 dodo_is_api-0.6.1/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     1291 2023-05-10 05:26:32.091787 dodo_is_api-0.6.1/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.6.1/dodo_is_api/connection/http_clients.py
+-rw-r--r--   0        0        0     8913 2023-06-10 06:30:13.600381 dodo_is_api-0.6.1/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.6.1/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0      583 2023-06-10 06:25:28.732549 dodo_is_api-0.6.1/dodo_is_api/logger.py
+-rw-r--r--   0        0        0     8145 2023-06-10 06:09:51.664171 dodo_is_api-0.6.1/dodo_is_api/mappers.py
+-rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.6.1/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0     3110 2023-06-10 06:07:19.624806 dodo_is_api-0.6.1/dodo_is_api/models/dodo_is_api.py
+-rw-r--r--   0        0        0     1938 2023-06-10 05:51:51.801439 dodo_is_api-0.6.1/dodo_is_api/models/raw.py
+-rw-r--r--   0        0        0      561 2023-06-10 06:44:45.178633 dodo_is_api-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4440 1970-01-01 00:00:00.000000 dodo_is_api-0.6.1/setup.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 dodo_is_api-0.6.1/PKG-INFO
```

### Comparing `dodo_is_api-0.6.0/LICENSE` & `dodo_is_api-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.0/README.md` & `dodo_is_api-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.0/dodo_is_api/connection/asynchronous.py` & `dodo_is_api-0.6.1/dodo_is_api/connection/asynchronous.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,29 @@
 import datetime
 from collections.abc import Iterable, AsyncGenerator
 from uuid import UUID
 
 import httpx
+from structlog.contextvars import bound_contextvars
 
 from .base import concatenate_uuids, raise_for_status
+from ..logger import logger
 from ..models import raw as raw_models
+from ..models.dodo_is_api import SalesChannel
 
 __all__ = ('AsyncDodoISAPIConnection',)
 
 
 class AsyncDodoISAPIConnection:
 
     __slots__ = ('__http_client',)
 
     def __init__(self, *, http_client: httpx.AsyncClient):
         self.__http_client = http_client
 
-    async def iter_late_delivery_vouchers(
-            self,
-            *,
-            from_date: datetime.datetime,
-            to_date: datetime.datetime,
-            units: Iterable[UUID],
-            skip: int = 0,
-            take: int = 1000,
-    ) -> AsyncGenerator[list[dict], None]:
-        url = '/delivery/vouchers'
-        request_query_params = {
-            'from': from_date.strftime('%Y-%m-%dT%H:%M:%S'),
-            'to': to_date.strftime('%Y-%m-%dT%H:%M:%S'),
-            'units': concatenate_uuids(units),
-            'skip': skip,
-            'take': take,
-        }
-
-        while True:
-            response = await self.__http_client.get(
-                url=url,
-                params=request_query_params,
-            )
-            raise_for_status(response)
-
-            response_data = response.json()
-            yield response_data['vouchers']
-            if response_data['isEndOfListReached']:
-                break
-            request_query_params['skip'] += take
-
-    async def get_delivery_statistics(
-            self,
-            *,
-            from_date: datetime.datetime,
-            to_date: datetime.datetime,
-            units: Iterable[UUID],
-    ) -> list[raw_models.UnitDeliveryStatisticsTypedDict]:
-        """
-        References:
-            Documentation: https://dodo-brands.stoplight.io/docs/dodo-is/2845c1de4776d-dostavka-statistika.
-
-        Keyword Args:
-            from_date: start of period in ISO 8601 format.
-            to_date: end of period in ISO 8601 format.
-            units: collection of unit's UUIDs.
-
-        Returns:
-            List of unit's delivery statistics.
-        """
-        url = '/delivery/statistics/'
-        request_query_params = {
-            'from': from_date.strftime('%Y-%m-%dT%H:%M:%S'),
-            'to': to_date.strftime('%Y-%m-%dT%H:%M:%S'),
-            'units': concatenate_uuids(units),
-        }
-        response = await self.__http_client.get(
-            url=url,
-            params=request_query_params,
-        )
-        raise_for_status(response)
-
-        response_data: dict = response.json()
-        return response_data['unitsStatistics']
-
     async def iter_courier_orders(
             self,
             *,
             from_date: datetime.datetime,
             to_date: datetime.datetime,
             units: Iterable[UUID],
             skip: int = 0,
@@ -122,7 +60,47 @@
             raise_for_status(response)
 
             response_data: dict = response.json()
             yield response_data['couriersOrders']
             if response_data['isEndOfListReached']:
                 break
             request_query_params['skip'] += take
+
+    async def get_orders_handover_statistics(
+            self,
+            from_date: datetime.datetime,
+            to_date: datetime.datetime,
+            units: Iterable[UUID],
+            sales_channels: Iterable[SalesChannel] | None = None,
+    ) -> list[raw_models.UnitOrdersHandoverStatistics]:
+        url = '/production/orders-handover-statistics'
+        request_query_params = {
+            'from': from_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'to': to_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'units': concatenate_uuids(units),
+        }
+        if sales_channels is not None:
+            request_query_params['salesChannels'] = ','.join(
+                sales_channel.value.replace('-', '')
+                for sales_channel in sales_channels
+            )
+        with bound_contextvars(
+                url=url,
+                request_query_params=request_query_params,
+        ):
+            logger.info('Request orders handover statistics')
+            response = await self.__http_client.get(
+                url=url,
+                params=request_query_params,
+            )
+            logger.info(
+                'Orders handover statistics response',
+                status_code=response.status_code,
+            )
+            raise_for_status(response)
+
+            response_data = response.json()
+            logger.info(
+                'Decoded orders handover statistics response',
+                response_data=response_data,
+            )
+            return response_data['ordersHandoverStatistics']
```

### Comparing `dodo_is_api-0.6.0/dodo_is_api/connection/base.py` & `dodo_is_api-0.6.1/dodo_is_api/connection/base.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.0/dodo_is_api/connection/http_clients.py` & `dodo_is_api-0.6.1/dodo_is_api/connection/http_clients.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.6.0/dodo_is_api/connection/synchronous.py` & `dodo_is_api-0.6.1/dodo_is_api/connection/synchronous.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import datetime
 from collections.abc import Iterable, Generator
 from uuid import UUID
 
 import httpx
+from structlog.contextvars import bound_contextvars
 
 from .base import concatenate_uuids, raise_for_status
+from ..logger import logger
 from ..models import raw as raw_models
+from ..models.dodo_is_api import SalesChannel
 
 __all__ = ('DodoISAPIConnection',)
 
 
 class DodoISAPIConnection:
     __slots__ = ('__http_client',)
 
@@ -205,7 +208,45 @@
             raise_for_status(response)
 
             response_data: dict = response.json()
             yield response_data['couriersOrders']
             if response_data['isEndOfListReached']:
                 break
             request_query_params['skip'] += take
+
+    def get_orders_handover_statistics(
+            self,
+            from_date: datetime.datetime,
+            to_date: datetime.datetime,
+            units: Iterable[UUID],
+            sales_channels: Iterable[SalesChannel] | None = None,
+    ) -> list[raw_models.UnitOrdersHandoverStatistics]:
+        url = '/production/orders-handover-statistics'
+        request_query_params = {
+            'from': from_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'to': to_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'units': concatenate_uuids(units),
+        }
+        if sales_channels is not None:
+            request_query_params['salesChannels'] = ','.join(
+                sales_channel.value.replace('-', '')
+                for sales_channel in sales_channels
+            )
+
+        with bound_contextvars(
+                url=url,
+                request_query_params=request_query_params,
+        ):
+            logger.info('Request orders handover statistics')
+            response = self.__http_client.get(url, params=request_query_params)
+            logger.info(
+                'Orders handover statistics response',
+                status_code=response.status_code,
+            )
+            raise_for_status(response)
+
+            response_data = response.json()
+            logger.info(
+                'Decoded orders handover statistics response',
+                response_data=response_data,
+            )
+            return response_data['ordersHandoverStatistics']
```

### Comparing `dodo_is_api-0.6.0/dodo_is_api/mappers.py` & `dodo_is_api-0.6.1/dodo_is_api/mappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 __all__ = (
     'map_late_delivery_voucher_dto',
     'map_stop_sale_by_sales_channel_dto',
     'map_stop_sale_by_product_dto',
     'map_stop_sale_by_ingredient_dto',
     'map_unit_delivery_statistics_dto',
     'map_courier_order_dto',
+    'map_unit_orders_handover_statistics',
 )
 
 
 def parse_to_datetime_or_none(value: str | None) -> datetime | None | NoReturn:
     match value:
         case str():
             return datetime.fromisoformat(value)
@@ -115,23 +116,27 @@
         unit_delivery_statistics: raw_models.UnitDeliveryStatisticsTypedDict,
 ) -> models.UnitDeliveryStatistics:
     return models.UnitDeliveryStatistics(
         unit_uuid=UUID(unit_delivery_statistics['unitId']),
         unit_name=unit_delivery_statistics['unitName'],
         delivery_sales=unit_delivery_statistics['deliverySales'],
         delivery_orders_count=unit_delivery_statistics['deliveryOrdersCount'],
-        average_delivery_order_fulfillment_time=unit_delivery_statistics['avgDeliveryOrderFulfillmentTime'],
+        average_delivery_order_fulfillment_time=unit_delivery_statistics[
+            'avgDeliveryOrderFulfillmentTime'],
         average_cooking_time=unit_delivery_statistics['avgCookingTime'],
-        average_heated_shelf_time=unit_delivery_statistics['avgHeatedShelfTime'],
+        average_heated_shelf_time=unit_delivery_statistics[
+            'avgHeatedShelfTime'],
         average_order_trip_time=unit_delivery_statistics['avgOrderTripTime'],
         late_orders_count=unit_delivery_statistics['lateOrdersCount'],
         trips_count=unit_delivery_statistics['tripsCount'],
         trips_duration=unit_delivery_statistics['tripsDuration'],
-        couriers_shifts_duration=unit_delivery_statistics['couriersShiftsDuration'],
-        orders_with_courier_app_count=unit_delivery_statistics['ordersWithCourierAppCount'],
+        couriers_shifts_duration=unit_delivery_statistics[
+            'couriersShiftsDuration'],
+        orders_with_courier_app_count=unit_delivery_statistics[
+            'ordersWithCourierAppCount'],
     )
 
 
 def map_courier_order_dto(
         courier_order: raw_models.CourierOrderTypedDict,
 ) -> models.CourierOrder:
     return models.CourierOrder(
@@ -159,7 +164,27 @@
         problematic_delivery_reason=courier_order['problematicDeliveryReason'],
         trip_orders_count=courier_order['tripOrdersCount'],
         unit_uuid=UUID(courier_order['unitId']),
         unit_name=courier_order['unitName'],
         was_late_delivery_voucher_given=courier_order[
             'wasLateDeliveryVoucherGiven'],
     )
+
+
+def map_unit_orders_handover_statistics(
+        unit_orders_handover_statistics: raw_models.UnitOrdersHandoverStatistics,
+) -> models.UnitOrdersHandoverStatistics:
+    return models.UnitOrdersHandoverStatistics(
+        unit_uuid=UUID(unit_orders_handover_statistics['unitId']),
+        unit_name=unit_orders_handover_statistics['unitName'],
+        average_tracking_pending_time=(
+            unit_orders_handover_statistics['avgTrackingPendingTime']
+        ),
+        average_cooking_time=unit_orders_handover_statistics['avgCookingTime'],
+        average_heated_shelf_time=(
+            unit_orders_handover_statistics['avgHeatedShelfTime']
+        ),
+        average_order_handover_time=(
+            unit_orders_handover_statistics['avgOrderHandoverTime']
+        ),
+        orders_count=unit_orders_handover_statistics['ordersCount']
+    )
```

### Comparing `dodo_is_api-0.6.0/dodo_is_api/models/dodo_is_api.py` & `dodo_is_api-0.6.1/dodo_is_api/models/dodo_is_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     'StopSaleByIngredient',
     'StopSaleBySalesChannel',
     'SalesChannel',
     'ChannelStopType',
     'UnitDeliveryStatistics',
     'CourierOrder',
     'DeliveryTransportName',
+    'UnitOrdersHandoverStatistics',
 )
 
 
 @dataclass(frozen=True, slots=True)
 class LateDeliveryVoucher:
     order_id: UUID
     order_number: str
@@ -108,7 +109,18 @@
     order_number: str
     predicted_delivery_time: int
     problematic_delivery_reason: str
     trip_orders_count: int
     unit_uuid: UUID
     unit_name: str
     was_late_delivery_voucher_given: bool
+
+
+@dataclass(frozen=True, slots=True)
+class UnitOrdersHandoverStatistics:
+    unit_uuid: UUID
+    unit_name: str
+    average_tracking_pending_time: int
+    average_cooking_time: int
+    average_heated_shelf_time: int
+    average_order_handover_time: int
+    orders_count: int
```

### Comparing `dodo_is_api-0.6.0/dodo_is_api/models/raw.py` & `dodo_is_api-0.6.1/dodo_is_api/models/raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 __all__ = (
     'StopSaleTypedDict',
     'StopSaleByIngredientTypedDict',
     'StopSaleBySalesChannelTypedDict',
     'StopSaleByProductTypedDict',
     'UnitDeliveryStatisticsTypedDict',
     'CourierOrderTypedDict',
+    'UnitOrdersHandoverStatistics'
 )
 
 
 class StopSaleTypedDict(TypedDict):
     id: str
     unitId: str
     unitName: str
@@ -65,7 +66,17 @@
     deliveryTransportName: Literal['Vehicle', 'OnFoot', 'Bicycle']
     tripOrdersCount: int
     heatedShelfTime: int
     orderAssemblyAvgTime: int
     isProblematicDelivery: bool
     problematicDeliveryReason: str
     wasLateDeliveryVoucherGiven: bool
+
+
+class UnitOrdersHandoverStatistics(TypedDict):
+    unitId: str
+    unitName: str
+    avgTrackingPendingTime: int
+    avgCookingTime: int
+    avgHeatedShelfTime: int
+    avgOrderHandoverTime: int
+    ordersCount: int
```

### Comparing `dodo_is_api-0.6.0/pyproject.toml` & `dodo_is_api-0.6.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.23.3"
+structlog = "^23.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.20.3"
 pytest-httpx = "^0.21.3"
```

### Comparing `dodo_is_api-0.6.0/setup.py` & `dodo_is_api-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.3,<0.24.0']
+['httpx>=0.23.3,<0.24.0', 'structlog>=23.1.0,<24.0.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': '',
     'long_description': '<div align="center">\n<a href="https://dodo-brands.stoplight.io">\n<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">\n</a>\n</div>\n    \n<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n- Delivery:\n    - [Late delivery vouchers](#get-late-delivery-vouchers-)\n- Production:\n    - [Stop sales](#get-stop-sales-)\n\n---\n\n#### 🛵 Get late delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # it will handle pagination for you\n    for late_delivery_vouchers in dodo_is_api_connection.iter_late_delivery_vouchers(\n            from_date=from_date,\n            to_date=to_date,\n            units=units\n    ):\n        # map to dataclass DTO if you need\n        late_delivery_voucher_dtos = [\n            map_late_delivery_voucher_dto(late_delivery_voucher)\n            for late_delivery_voucher in late_delivery_vouchers\n        ]\n        ...\n```\n\n---\n\n#### 📦 Get stop sales:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # for products - dodo_is_api_connection.get_stop_sales_by_products\n    # for sales channels - dodo_is_api_connection.get_stop_sales_by_sales_channels\n    stop_sales = dodo_is_api_connection.get_stop_sales_by_ingredients(\n        from_date=from_date,\n        to_date=to_date,\n        units=units\n    )\n\n    # map to dataclass DTO if you need\n    # use suitable mapper\n    # in this case, ingredient stop sale mapper is used\n    late_delivery_voucher_dtos = [\n        map_stop_sale_by_ingredient_dto(stop_sale)\n        for stop_sale in stop_sales\n    ]\n    ...\n```\n',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
-\ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0'] setup_kwargs =
-{ 'name': 'dodo-is-api', 'version': '0.6.0', 'description': '',
-'long_description': '
+\ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0',
+'structlog>=23.1.0,<24.0.0'] setup_kwargs = { 'name': 'dodo-is-api', 'version':
+'0.6.1', 'description': '', 'long_description': '
   \n\n[https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]\n\n
 \n \n
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
 \n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-
```

### Comparing `dodo_is_api-0.6.0/PKG-INFO` & `dodo_is_api-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dodo-is-api
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Author: Eldos
 Author-email: eldos.baktybekov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: structlog (>=23.1.0,<24.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 <a href="https://dodo-brands.stoplight.io">
 <img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">
 </a>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: dodo-is-api Version: 0.6.0 Summary: Author: Eldos
+Metadata-Version: 2.1 Name: dodo-is-api Version: 0.6.1 Summary: Author: Eldos
 Author-email: eldos.baktybekov@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Description-
-Content-Type: text/markdown
+Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-
+Dist: structlog (>=23.1.0,<24.0.0) Description-Content-Type: text/markdown
       [https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]
                     ****** ð Dodo IS API Wrapper ******
  [Test_badge] [https://codecov.io/gh/goretsky-integration/dodo-is-api-python-
         wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD] [python]
 --- ### Installation Via pip: ```shell pip install dodo-is-api ``` Via poetry:
 ```shell poetry add dodo-is-api ``` --- #### ð [Changelog](https://
 github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/
```

