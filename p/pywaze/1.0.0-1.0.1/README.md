# Comparing `tmp/pywaze-1.0.0.tar.gz` & `tmp/pywaze-1.0.1.tar.gz`

## Comparing `pywaze-1.0.0.tar` & `pywaze-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywaze-1.0.0/.codespell
--rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 pywaze-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pywaze-1.0.0/.python-version
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 pywaze-1.0.0/.ruff.toml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pywaze-1.0.0/.yamllint
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pywaze-1.0.0/mypy.ini
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pywaze-1.0.0/requirements-dev.lock
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pywaze-1.0.0/requirements.lock
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pywaze-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pywaze-1.0.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 pywaze-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pywaze-1.0.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pywaze-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pywaze-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 pywaze-1.0.0/docs/images/bmc-button.svg
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 pywaze-1.0.0/docs/images/paypal-button.svg
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pywaze-1.0.0/src/pywaze/__init__.py
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 pywaze-1.0.0/src/pywaze/route_calculator.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pywaze-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pywaze-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0  1334909 2020-02-02 00:00:00.000000 pywaze-1.0.0/tests/const.py
--rw-r--r--   0        0        0     9057 2020-02-02 00:00:00.000000 pywaze-1.0.0/tests/test_route_calculator.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pywaze-1.0.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywaze-1.0.0/LICENSE
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pywaze-1.0.0/README.md
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pywaze-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pywaze-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywaze-1.0.1/.codespell
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 pywaze-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pywaze-1.0.1/.python-version
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 pywaze-1.0.1/.ruff.toml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pywaze-1.0.1/.yamllint
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pywaze-1.0.1/mypy.ini
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 pywaze-1.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 pywaze-1.0.1/requirements.lock
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pywaze-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 pywaze-1.0.1/.github/release-drafter.yml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 pywaze-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pywaze-1.0.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pywaze-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pywaze-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 pywaze-1.0.1/docs/images/bmc-button.svg
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 pywaze-1.0.1/docs/images/paypal-button.svg
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pywaze-1.0.1/src/pywaze/__init__.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 pywaze-1.0.1/src/pywaze/route_calculator.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pywaze-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 pywaze-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0  1337875 2020-02-02 00:00:00.000000 pywaze-1.0.1/tests/const.py
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 pywaze-1.0.1/tests/test_route_calculator.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pywaze-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywaze-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 pywaze-1.0.1/README.md
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pywaze-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pywaze-1.0.1/PKG-INFO
```

### Comparing `pywaze-1.0.0/.pre-commit-config.yaml` & `pywaze-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/.ruff.toml` & `pywaze-1.0.1/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/requirements-dev.lock` & `pywaze-1.0.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/.github/release-drafter.yml` & `pywaze-1.0.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/.github/workflows/ci.yml` & `pywaze-1.0.1/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,31 @@
     - cron: "0 0 * * *"
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.11.3"]
     steps:
       - uses: actions/checkout@v4
-      - uses: eifinger/setup-rye@v1
+      - uses: eifinger/setup-rye@v2
+        id: setup-rye
         with:
           enable-cache: true
+          cache-prefix: ${{ matrix.python-version }}
       - name: Pin python-version ${{ matrix.python-version }}
+        if: steps.setup-rye.outputs.cache-hit != 'true'
         run: rye pin ${{ matrix.python-version }}
       - name: Install dependencies
+        if: steps.setup-rye.outputs.cache-hit != 'true'
         run: |
           rye sync --no-lock
       - name: Cache pre-commit
-        uses: actions/cache@704facf57e6136b1bc63b828d79edcd491f0ee84  # v3.3.2
+        uses: actions/cache@ab5e6d0c87105b4c9c2047343972218f562e4319  # v4.0.1
         with:
           path: ~/.cache/pre-commit
           key: pre-commit-|${{ matrix.python-version }}|${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Lint
         run: |
           rye run pre-commit run --all-files
       - name: Lint GitHub Actions
```

### Comparing `pywaze-1.0.0/.github/workflows/release.yml` & `pywaze-1.0.1/.github/workflows/release.yml`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - uses: actions/checkout@v4
       - name: Search and replace version
         run: |
           VERSION="${TAG_NAME//v/}"
           sed -i "s/1\.0+versionplaceholder\.1/$VERSION/" pyproject.toml
         env:
           TAG_NAME: ${{ github.event.release.tag_name }}
-      - uses: eifinger/setup-rye@v1
+      - uses: eifinger/setup-rye@v2
         with:
           enable-cache: true
       - name: Build
         run: |
           rye build
       - name: Publish package distributions to PyPI
-        uses: pypa/gh-action-pypi-publish@2f6f737ca5f74c637829c0f5c3acd0e29ea5e8bf
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `pywaze-1.0.0/docs/images/bmc-button.svg` & `pywaze-1.0.1/docs/images/bmc-button.svg`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/docs/images/paypal-button.svg` & `pywaze-1.0.1/docs/images/paypal-button.svg`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/src/pywaze/route_calculator.py` & `pywaze-1.0.1/src/pywaze/route_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Waze route calculator."""
 
 from dataclasses import dataclass
 from typing import Any, Literal, TypedDict
 import httpx
 import re
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class Coords(TypedDict):
     """Coordinates and bounds."""
 
     lat: float
     lon: float
@@ -197,14 +200,15 @@
 
     @staticmethod
     def _check_response(response: httpx.Response) -> Any:
         """Check waze server response."""
         if response.is_success:
             try:
                 response_json = response.json()
+                logger.debug("Response is: %s", response_json)
                 if "error" in response_json:
                     raise WRCError(response_json.get("error"))
                 return response_json
             except ValueError:
                 raise WRCError("empty response")
         raise WRCError(response.text)
 
@@ -290,17 +294,19 @@
                 real_time=real_time,
                 stop_at_bounds=stop_at_bounds,
             )
             result.append(
                 CalcRoutesResponse(
                     distance=distance,
                     duration=duration,
-                    name=route["routeName"],
+                    name=route.get("routeName", ""),
                     street_names=[
-                        name for name in route["streetNames"] if name is not None
+                        name
+                        for name in route.get("streetNames", {})
+                        if name is not None
                     ],
                 )
             )
         return result
 
     async def close(self) -> None:
         """Close the client."""
```

### Comparing `pywaze-1.0.0/tests/conftest.py` & `pywaze-1.0.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,18 @@
         params={"q": "Kaiserstraße 30 55116 Mainz, Germany"},
     ).mock(
         return_value=Response(
             200,
             json=ADDRESS_TO_COORDS_RESPONSE_MAINZ,
         )
     )
+
+
+@pytest.fixture
+def no_route_name_mock(get_route_response: dict[str, Any], respx_mock: MockRouter):
+    """Return the provided json response when calculating routes."""
+    yield respx_mock.get("https://www.waze.com/row-RoutingManager/routingRequest").mock(
+        return_value=Response(
+            200,
+            json=get_route_response,
+        )
+    )
```

### Comparing `pywaze-1.0.0/tests/const.py` & `pywaze-1.0.1/tests/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -30090,7 +30090,99 @@
                 {"x": 8.247291101809203, "y": 50.0840110317197, "z": "NaN"},
                 {"x": 8.247291101809203, "y": 50.0840110317197, "z": "NaN"},
                 {"x": 8.247286829865775, "y": 50.08411891532466, "z": "NaN"},
             ],
         },
     ]
 }
+
+EMPTY_ROUTE_NAME_RESPONSE = {
+    "response": {
+        "results": [
+            {
+                "path": {
+                    "segmentId": 1988980,
+                    "nodeId": 1435615,
+                    "x": 35.21172898702758,
+                    "y": 31.804322521358937,
+                    "direction": True,
+                },
+                "street": 0,
+                "distance": 0,
+                "length": 7,
+                "crossTime": 2,
+                "crossTimeWithoutRealTime": 2,
+                "crossTimeFreeFlow": 2,
+                "knownDirection": True,
+                "penalty": 2,
+                "roadType": 17,
+                "isToll": False,
+                "useHovLane": False,
+                "attributes": 0,
+                "lane": "WHOLE_SEGMENT",
+                "avoidStatus": "OPEN",
+                "isInvalid": False,
+                "isBlocked": False,
+                "speedLimit": 0,
+                "instruction": {"opcode": "APPROACHING_DESTINATION", "arg": 0},
+            }
+        ],
+        "streetNames": [None],
+        "fromlocMetersFromGeom": 15.656917,
+        "fromFraction": 0.42397566690535016,
+        "toFraction": 0.25128010628918573,
+        "sameFromSegment": True,
+        "sameToSegment": True,
+        "wayPoints": [],
+        "tollMeters": 0,
+        "preferedRouteId": -1,
+        "isInvalid": False,
+        "isBlocked": False,
+        "serverUniqueId": "m8176753750470206236",
+        "displayRoute": True,
+        "astarVisited": 3,
+        "astarResult": "UNKNOWN",
+        "isRestricted": False,
+        "avoidStatus": "OPEN",
+        "passesThroughDangerArea": False,
+        "distanceFromSource": 15,
+        "distanceFromTarget": 30,
+        "minPassengers": 0,
+        "hovIndex": -1,
+        "preRefinedRouteIndex": -1,
+        "blockedRouteUid": -1,
+        "alternativeRouteUuid": "7692ded3-3d28-4fdc-8a47-8fb867bca479",
+        "serverTilesVersion": 1714604411000,
+        "rankBeforeReordering": 0,
+        "serverType": "LIVEMAP",
+        "routeType": ["Best"],
+        "routeAttr": [],
+        "astarCost": 4,
+        "uid": 0,
+        "totalRouteTime": 2,
+        "totalRouteTimeWithoutRealtime": 2,
+        "totalRouteTimeFreeFlow": 2,
+        "carbonEmissionsGrams": 0,
+        "creationMechanismSet": ["ASTAR", "HUBCAP_HEURISTIC"],
+        "laneTypes": [],
+        "areas": [],
+        "requiredPermits": [],
+        "etaHistograms": [],
+        "tollPrice": 0.0,
+        "isInvalidForPrivateVehicle": False,
+        "costInfo": {
+            "unbiasedAstarCost": 0,
+            "tollAsSeconds": 0,
+            "keepForReordering": False,
+        },
+        "destinationInformation": {
+            "segment_id": 1988980,
+            "street_id": 3677,
+            "city_id": 800,
+            "country_id": 106,
+            "city_name": "ירושלים",
+            "exit_node_id": 1435240,
+        },
+        "open": True,
+        "totalRouteTimeWithoutMl": 2,
+    }
+}
```

### Comparing `pywaze-1.0.0/tests/test_route_calculator.py` & `pywaze-1.0.1/tests/test_route_calculator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for route_calculator module."""
 import pytest
 from pywaze import route_calculator
 from tests.const import (
+    EMPTY_ROUTE_NAME_RESPONSE,
     GET_ROUTE_RESPONSE_ADDRESSES,
     GET_ROUTE_RESPONSE_COORDS,
     GET_ALL_ROUTES_RESPONSE,
 )
 
 
 @pytest.mark.parametrize(
@@ -203,14 +204,24 @@
                     "Rheinstraße",
                     "L3037 - Rheinstraße",
                     "Wilhelmstraße",
                     "Christian-Zais-Straße",
                 ],
             ],
         ),
+        (
+            "31.804461,35.2115243",
+            "31.80459309184719,35.21160542964936",
+            1,
+            EMPTY_ROUTE_NAME_RESPONSE,
+            [0.03333333333333333],
+            [0.007],
+            [""],
+            [[]],
+        ),
     ),
 )
 @pytest.mark.usefixtures(
     "get_route_mock", "wiesbaden_to_coords_mock", "mainz_to_coords_mock"
 )
 async def test_calc_route_info(
     start: str,
@@ -230,15 +241,16 @@
             assert routes[alternative].distance == expected_route_distances[alternative]
             assert routes[alternative].name == expected_route_names[alternative]
             assert (
                 routes[alternative].street_names == expected_street_names[alternative]
             )
 
 
-async def test_calc_route_info_timeout(timeout_mock):
+@pytest.mark.usefixtures("timeout_mock")
+async def test_calc_route_info_timeout():
     """Test calc_route_info with timeout."""
 
     async with route_calculator.WazeRouteCalculator() as client:
         with pytest.raises(route_calculator.WRCTimeoutError):
             await client.calc_routes(
                 "50.00332659227126,8.262322651915843",
                 "50.08414976707619,8.247836017342934",
```

### Comparing `pywaze-1.0.0/LICENSE` & `pywaze-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaze-1.0.0/README.md` & `pywaze-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 from pywaze import route_calculator
 
 
 async def get_time(start: str, end: str) -> float:
     """Return the travel time home."""
 
     async with route_calculator.WazeRouteCalculator() as client:
-        results = await client.calc_all_routes_info(start, end)
+        results = await client.calc_routes(start, end)
         route_time, _ = list(results.values())[0]
         return route_time
 
 
 start = "50.00332659227126,8.262322651915843"
 end = "50.08414976707619,8.247836017342934"
 
 travel_time = asyncio.run(get_time(start, end))
 
 print(travel_time)
 ```
 
 ---
 
-[<img src="https://raw.githubusercontent.com/eifinger/setup-rye/main/docs/images/bmc-button.svg" width=150 height=40 style="margin: 5px"/>](https://www.buymeacoffee.com/eifinger)
-[<img src="https://raw.githubusercontent.com/eifinger/setup-rye/main/docs/images/paypal-button.svg" width=150 height=40 style="margin: 5px"/>](https://paypal.me/kevinstillhammer)
+[<img src="https://raw.githubusercontent.com/eifinger/pywaze/main/docs/images/bmc-button.svg" width=150 height=40 style="margin: 5px"/>](https://www.buymeacoffee.com/eifinger)
+[<img src="https://raw.githubusercontent.com/eifinger/pywaze/main/docs/images/paypal-button.svg" width=150 height=40 style="margin: 5px"/>](https://paypal.me/kevinstillhammer)
```

### Comparing `pywaze-1.0.0/pyproject.toml` & `pywaze-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywaze"
-version = "1.0.0"
+version = "1.0.1"
 description = "Asynchronous Waze client for calculating routes and travel times."
 authors = [
     { name = "Kevin Stillhammer", email = "kevin.stillhammer@gmail.com" }
 ]
 license = "MIT"
 repository = "http://github.com/eifinger/pywaze"
 dependencies = [
```

### Comparing `pywaze-1.0.0/PKG-INFO` & `pywaze-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pywaze
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous Waze client for calculating routes and travel times.
 Author-email: Kevin Stillhammer <kevin.stillhammer@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: httpx>=0.24.1
 Description-Content-Type: text/markdown
@@ -30,24 +30,24 @@
 from pywaze import route_calculator
 
 
 async def get_time(start: str, end: str) -> float:
     """Return the travel time home."""
 
     async with route_calculator.WazeRouteCalculator() as client:
-        results = await client.calc_all_routes_info(start, end)
+        results = await client.calc_routes(start, end)
         route_time, _ = list(results.values())[0]
         return route_time
 
 
 start = "50.00332659227126,8.262322651915843"
 end = "50.08414976707619,8.247836017342934"
 
 travel_time = asyncio.run(get_time(start, end))
 
 print(travel_time)
 ```
 
 ---
 
-[<img src="https://raw.githubusercontent.com/eifinger/setup-rye/main/docs/images/bmc-button.svg" width=150 height=40 style="margin: 5px"/>](https://www.buymeacoffee.com/eifinger)
-[<img src="https://raw.githubusercontent.com/eifinger/setup-rye/main/docs/images/paypal-button.svg" width=150 height=40 style="margin: 5px"/>](https://paypal.me/kevinstillhammer)
+[<img src="https://raw.githubusercontent.com/eifinger/pywaze/main/docs/images/bmc-button.svg" width=150 height=40 style="margin: 5px"/>](https://www.buymeacoffee.com/eifinger)
+[<img src="https://raw.githubusercontent.com/eifinger/pywaze/main/docs/images/paypal-button.svg" width=150 height=40 style="margin: 5px"/>](https://paypal.me/kevinstillhammer)
```

