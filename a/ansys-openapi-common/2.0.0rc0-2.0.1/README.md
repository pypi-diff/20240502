# Comparing `tmp/ansys_openapi_common-2.0.0rc0.tar.gz` & `tmp/ansys_openapi_common-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_openapi_common-2.0.0rc0.tar", max compression
+gzip compressed data, was "ansys_openapi_common-2.0.1.tar", max compression
```

## Comparing `ansys_openapi_common-2.0.0rc0.tar` & `ansys_openapi_common-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      618 2024-03-04 16:13:49.931544 ansys_openapi_common-2.0.0rc0/AUTHORS.md
--rw-r--r--   0        0        0     1088 2024-03-04 16:13:49.931544 ansys_openapi_common-2.0.0rc0/LICENSE
--rw-r--r--   0        0        0     4441 2024-03-04 16:13:49.931544 ansys_openapi_common-2.0.0rc0/README.rst
--rw-r--r--   0        0        0     3766 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      867 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/__init__.py
--rw-r--r--   0        0        0    33299 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_api_client.py
--rw-r--r--   0        0        0       22 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_base/__init__.py
--rw-r--r--   0        0        0     4345 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_base/_types.py
--rw-r--r--   0        0        0     3909 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_exceptions.py
--rw-r--r--   0        0        0      108 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_logger.py
--rw-r--r--   0        0        0    12868 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_oidc.py
--rw-r--r--   0        0        0    19511 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_session.py
--rw-r--r--   0        0        0    14966 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_util.py
--rw-r--r--   0        0        0        0 2024-03-04 16:13:49.935544 ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/py.typed
--rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 ansys_openapi_common-2.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      618 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/AUTHORS.md
+-rw-r--r--   0        0        0     1098 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/LICENSE
+-rw-r--r--   0        0        0     6139 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/README.rst
+-rw-r--r--   0        0        0     3761 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2021 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/__init__.py
+-rw-r--r--   0        0        0    34351 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_api_client.py
+-rw-r--r--   0        0        0     1176 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_base/_types.py
+-rw-r--r--   0        0        0     5063 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_exceptions.py
+-rw-r--r--   0        0        0     1262 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_logger.py
+-rw-r--r--   0        0        0    14146 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_oidc.py
+-rw-r--r--   0        0        0    20665 2024-05-02 15:06:22.749482 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_session.py
+-rw-r--r--   0        0        0    16120 2024-05-02 15:06:22.753483 ansys_openapi_common-2.0.1/src/ansys/openapi/common/_util.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:06:22.753483 ansys_openapi_common-2.0.1/src/ansys/openapi/common/py.typed
+-rw-r--r--   0        0        0     7817 1970-01-01 00:00:00.000000 ansys_openapi_common-2.0.1/PKG-INFO
```

### Comparing `ansys_openapi_common-2.0.0rc0/AUTHORS.md` & `ansys_openapi_common-2.0.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `ansys_openapi_common-2.0.0rc0/LICENSE` & `ansys_openapi_common-2.0.1/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 MIT License
 
-Copyright (c) 2024 ANSYS, Inc. All rights reserved.
+Copyright (c) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `ansys_openapi_common-2.0.0rc0/README.rst` & `ansys_openapi_common-2.0.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,38 @@
+|pyansys| |python| |pypi| |GH-CI| |MIT| |black| |pre-commit-ci|
+
+.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://docs.pyansys.com/
+   :alt: PyAnsys
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-openapi-common?logo=pypi
+   :target: https://pypi.org/project/ansys-openapi-common/
+   :alt: Python
+
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-openapi-common.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-openapi-common
+   :alt: PyPI
+
+.. |GH-CI| image:: https://github.com/pyansys/openapi-common/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/openapi-common/actions/workflows/ci_cd.yml
+   :alt: GH-CI
+
+.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: MIT
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. |pre-commit-ci| image:: https://results.pre-commit.ci/badge/github/ansys/openapi-common/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/openapi-common/main
+   :alt: pre-commit.ci status
+
+
 Overview
 --------
 
 OpenAPI-Common is intended for use with the custom code generation
 template in the `PyAnsys project <https://github.com/pyansys>`_.
 It provides the source code for an authentication-aware
 client for OpenAPI client libraries.
```

### Comparing `ansys_openapi_common-2.0.0rc0/pyproject.toml` & `ansys_openapi_common-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ansys-openapi-common"
 description = "Provides a helper to create sessions for use with Ansys OpenAPI clients."
-version = "2.0.0rc0"
+version = "2.0.1"
 license = "MIT"
 authors = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 maintainers = ["ANSYS, Inc. <pyansys.core@ansys.com>"]
 repository = "https://github.com/pyansys/openapi-common"
 documentation = "https://openapi.docs.pyansys.com"
 readme = "README.rst"
 keywords = [
@@ -39,15 +39,15 @@
 python = "^3.9"
 
 # Packages for core library
 requests = "^2.26"
 requests-negotiate-sspi = { version = "^0.5.2", markers = "sys_platform == 'win32'"}
 requests-ntlm = "^1.1.0"
 pyparsing = "^3.0.8"
-python-dateutil ="^2.6.1"
+python-dateutil ="^2.9"
 
 # Packages for oidc extra
 requests_auth = { version = ">=6,<8", optional = true }
 keyring = { version = ">=22,<25", optional = true }
 
 # Packages for linux-kerberos extra
 requests-kerberos = {version = "^0.13", markers = "sys_platform == 'linux'", optional = true }
```

### Comparing `ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/__init__.py` & `ansys_openapi_common-2.0.1/src/ansys/openapi/common/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 """Provides a helper to create sessions for use with Ansys OpenAPI clients."""
 
 from importlib import metadata as metadata
 
 __version__ = metadata.version("ansys-openapi-common")
 
 from ._api_client import ApiClient
```

### Comparing `ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_api_client.py` & `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import datetime
 from enum import Enum
 import json
 import mimetypes
 import os
 import re
 import tempfile
@@ -19,20 +41,17 @@
     Type,
     Union,
     cast,
 )
 from urllib.parse import quote
 import warnings
 
+from dateutil.parser import parse
 import requests
 
-with warnings.catch_warnings():
-    warnings.simplefilter("ignore", category=DeprecationWarning)
-    from dateutil.parser import parse
-
 from ._base import ApiClientBase, DeserializedType, ModelBase, PrimitiveType, SerializedType, Unset
 from ._exceptions import ApiException, UndefinedObjectWarning
 from ._util import SessionConfiguration, handle_response
 
 
 # noinspection DuplicatedCode
 class ApiClient(ApiClientBase):
```

### Comparing `ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_oidc.py` & `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_oidc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,30 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 from typing import Optional
+import urllib.parse
 
 import keyring
 import requests
 from requests.models import CaseInsensitiveDict
 from requests_auth import InvalidGrantRequest  # type: ignore[import-untyped]
 from requests_auth import OAuth2AuthorizationCodePKCE
 from requests_auth.authentication import OAuth2  # type: ignore[import-untyped]
@@ -235,17 +257,18 @@
         Parameters
         ----------
         url : str
             URL referencing the OpenID identity provider's well-known endpoint.
         """
         logger.info(f"Fetching configuration information from Identity Provider {url}")
         set_session_kwargs(self._initial_session, self._idp_session_configuration)
-        authority_response = self._initial_session.get(
-            f"{url}.well-known/openid-configuration",
-        )
+        if not url.endswith("/"):
+            url += "/"
+        well_known_endpoint = urllib.parse.urljoin(url, ".well-known/openid-configuration")
+        authority_response = self._initial_session.get(well_known_endpoint)
         set_session_kwargs(self._initial_session, self._api_session_configuration)
 
         logger.debug("Received configuration:")
         oidc_configuration = CaseInsensitiveDict(
             authority_response.json()
         )  # type: CaseInsensitiveDict
```

### Comparing `ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_session.py` & `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 import os
 from typing import Any, Mapping, Optional, Tuple, TypeVar, Union
 import warnings
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
```

### Comparing `ansys_openapi_common-2.0.0rc0/src/ansys/openapi/common/_util.py` & `ansys_openapi_common-2.0.1/src/ansys/openapi/common/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+# Copyright (C) 2022 - 2024 ANSYS, Inc. and/or its affiliates.
+# SPDX-License-Identifier: MIT
+#
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from collections import OrderedDict
 import http.cookiejar
 from itertools import chain
 import tempfile
 from typing import Any, Collection, Dict, List, Optional, Tuple, TypedDict, Union, cast
 
 import pyparsing as pp
```

### Comparing `ansys_openapi_common-2.0.0rc0/PKG-INFO` & `ansys_openapi_common-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-openapi-common
-Version: 2.0.0rc0
+Version: 2.0.1
 Summary: Provides a helper to create sessions for use with Ansys OpenAPI clients.
 Home-page: https://github.com/pyansys/openapi-common
 License: MIT
 Keywords: Ansys,OpenAPI
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
@@ -22,24 +22,55 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Provides-Extra: linux-kerberos
 Provides-Extra: oidc
 Requires-Dist: keyring (>=22,<25) ; extra == "oidc"
 Requires-Dist: pyparsing (>=3.0.8,<4.0.0)
-Requires-Dist: python-dateutil (>=2.6.1,<3.0.0)
+Requires-Dist: python-dateutil (>=2.9,<3.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: requests-kerberos (>=0.13,<0.14) ; (sys_platform == "linux") and (extra == "linux-kerberos")
 Requires-Dist: requests-negotiate-sspi (>=0.5.2,<0.6.0) ; sys_platform == "win32"
 Requires-Dist: requests-ntlm (>=1.1.0,<2.0.0)
 Requires-Dist: requests_auth (>=6,<8) ; extra == "oidc"
 Project-URL: Documentation, https://openapi.docs.pyansys.com
 Project-URL: Repository, https://github.com/pyansys/openapi-common
 Description-Content-Type: text/x-rst
 
+|pyansys| |python| |pypi| |GH-CI| |MIT| |black| |pre-commit-ci|
+
+.. |pyansys| image:: https://img.shields.io/badge/Py-Ansys-ffc107.svg?labelColor=black&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAABDklEQVQ4jWNgoDfg5mD8vE7q/3bpVyskbW0sMRUwofHD7Dh5OBkZGBgW7/3W2tZpa2tLQEOyOzeEsfumlK2tbVpaGj4N6jIs1lpsDAwMJ278sveMY2BgCA0NFRISwqkhyQ1q/Nyd3zg4OBgYGNjZ2ePi4rB5loGBhZnhxTLJ/9ulv26Q4uVk1NXV/f///////69du4Zdg78lx//t0v+3S88rFISInD59GqIH2esIJ8G9O2/XVwhjzpw5EAam1xkkBJn/bJX+v1365hxxuCAfH9+3b9/+////48cPuNehNsS7cDEzMTAwMMzb+Q2u4dOnT2vWrMHu9ZtzxP9vl/69RVpCkBlZ3N7enoDXBwEAAA+YYitOilMVAAAAAElFTkSuQmCC
+   :target: https://docs.pyansys.com/
+   :alt: PyAnsys
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/ansys-openapi-common?logo=pypi
+   :target: https://pypi.org/project/ansys-openapi-common/
+   :alt: Python
+
+.. |pypi| image:: https://img.shields.io/pypi/v/ansys-openapi-common.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/ansys-openapi-common
+   :alt: PyPI
+
+.. |GH-CI| image:: https://github.com/pyansys/openapi-common/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/openapi-common/actions/workflows/ci_cd.yml
+   :alt: GH-CI
+
+.. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: MIT
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
+   :target: https://github.com/psf/black
+   :alt: Black
+
+.. |pre-commit-ci| image:: https://results.pre-commit.ci/badge/github/ansys/openapi-common/main.svg
+   :target: https://results.pre-commit.ci/latest/github/ansys/openapi-common/main
+   :alt: pre-commit.ci status
+
+
 Overview
 --------
 
 OpenAPI-Common is intended for use with the custom code generation
 template in the `PyAnsys project <https://github.com/pyansys>`_.
 It provides the source code for an authentication-aware
 client for OpenAPI client libraries.
```

