# Comparing `tmp/unione-0.3.tar.gz` & `tmp/unione-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unione-0.3.tar", last modified: Wed May  1 10:50:34 2024, max compression
+gzip compressed data, was "unione-0.4.tar", last modified: Thu May  2 08:56:30 2024, max compression
```

## Comparing `unione-0.3.tar` & `unione-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 10:50:34.311270 unione-0.3/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-01 10:50:34.311270 unione-0.3/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-05-01 10:50:34.311270 unione-0.3/setup.cfg
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-05-01 10:50:29.000000 unione-0.3/setup.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 10:50:34.311270 unione-0.3/unilite/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.3/unilite/__init__.py
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)     3642 2024-05-01 05:46:51.000000 unione-0.3/unilite/constants.py
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)   103689 2024-05-01 10:49:31.000000 unione-0.3/unilite/contract_maker.py
-drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-01 10:50:34.311270 unione-0.3/unione.egg-info/
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-01 10:50:34.000000 unione-0.3/unione.egg-info/PKG-INFO
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      224 2024-05-01 10:50:34.000000 unione-0.3/unione.egg-info/SOURCES.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-05-01 10:50:34.000000 unione-0.3/unione.egg-info/dependency_links.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-05-01 10:50:34.000000 unione-0.3/unione.egg-info/requires.txt
--rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-05-01 10:50:34.000000 unione-0.3/unione.egg-info/top_level.txt
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.853366 unione-0.4/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-02 08:56:30.853366 unione-0.4/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       38 2024-05-02 08:56:30.853366 unione-0.4/setup.cfg
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      213 2024-05-02 08:56:12.000000 unione-0.4/setup.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.833366 unione-0.4/unilite/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       35 2024-04-29 13:17:00.000000 unione-0.4/unilite/__init__.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)     3707 2024-05-01 11:25:04.000000 unione-0.4/unilite/constants.py
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)   108670 2024-05-01 11:28:29.000000 unione-0.4/unilite/contract_maker.py
+drwxr-xr-x   0 codeuxi   (1000) codeuxi   (1000)        0 2024-05-02 08:56:30.853366 unione-0.4/unione.egg-info/
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)       68 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/PKG-INFO
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)      224 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/SOURCES.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        1 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/dependency_links.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        5 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/requires.txt
+-rw-r--r--   0 codeuxi   (1000) codeuxi   (1000)        8 2024-05-02 08:56:30.000000 unione-0.4/unione.egg-info/top_level.txt
```

### Comparing `unione-0.3/unilite/constants.py` & `unione-0.4/unilite/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ETH_MAINNET_RPC = 'https://eth.llamarpc.com'
 CONTRACT_ADDRESS = '0x9DAEa35A922492BE23941De2433D3FD88b3e7cAE'
 UNISWAP_V2_FACTORY = '0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f'
 UNISWAP_V2_ROUTER = '0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D'
 UNISWAP_V3_FACTORY = '0x1F98431c8aD98523631AE4a59f267346ea31F984'
 UNISWAP_V3_ROUTER = '0xE592427A0AEce92De3Edee1F18E0157C05861564'
+UNISWAP_V3_QUOTER = '0xb27308f9F90D607463bb33eA1BeBb41C27CE5AB6'
 
 NATIVE = "0x0000000000000000000000000000000000000000"
 EEFI = "0x857FfC55B1Aa61A7fF847C82072790cAE73cd883"
 USDC = "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48"
 OHM = "0x64aa3364F17a4D01c6f1751Fd97C2BD3D7e7f1D5"
 WETH = "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
 GDT = "0xc67B12049c2D0CF6e476BC64c7F82fc6C63cFFc5"
```

### Comparing `unione-0.3/unilite/contract_maker.py` & `unione-0.4/unilite/contract_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -3775,14 +3775,207 @@
                 "type": "address"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     }
 ]
+uniswap_v3_quoter_abi = [
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "_factory",
+                "type": "address"
+            },
+            {
+                "internalType": "address",
+                "name": "_WETH9",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "constructor"
+    },
+    {
+        "inputs": [],
+        "name": "WETH9",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [],
+        "name": "factory",
+        "outputs": [
+            {
+                "internalType": "address",
+                "name": "",
+                "type": "address"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "bytes",
+                "name": "path",
+                "type": "bytes"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amountIn",
+                "type": "uint256"
+            }
+        ],
+        "name": "quoteExactInput",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "amountOut",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "tokenIn",
+                "type": "address"
+            },
+            {
+                "internalType": "address",
+                "name": "tokenOut",
+                "type": "address"
+            },
+            {
+                "internalType": "uint24",
+                "name": "fee",
+                "type": "uint24"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amountIn",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint160",
+                "name": "sqrtPriceLimitX96",
+                "type": "uint160"
+            }
+        ],
+        "name": "quoteExactInputSingle",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "amountOut",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "bytes",
+                "name": "path",
+                "type": "bytes"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amountOut",
+                "type": "uint256"
+            }
+        ],
+        "name": "quoteExactOutput",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "amountIn",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "address",
+                "name": "tokenIn",
+                "type": "address"
+            },
+            {
+                "internalType": "address",
+                "name": "tokenOut",
+                "type": "address"
+            },
+            {
+                "internalType": "uint24",
+                "name": "fee",
+                "type": "uint24"
+            },
+            {
+                "internalType": "uint256",
+                "name": "amountOut",
+                "type": "uint256"
+            },
+            {
+                "internalType": "uint160",
+                "name": "sqrtPriceLimitX96",
+                "type": "uint160"
+            }
+        ],
+        "name": "quoteExactOutputSingle",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "amountIn",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "nonpayable",
+        "type": "function"
+    },
+    {
+        "inputs": [
+            {
+                "internalType": "int256",
+                "name": "amount0Delta",
+                "type": "int256"
+            },
+            {
+                "internalType": "int256",
+                "name": "amount1Delta",
+                "type": "int256"
+            },
+            {
+                "internalType": "bytes",
+                "name": "path",
+                "type": "bytes"
+            }
+        ],
+        "name": "uniswapV3SwapCallback",
+        "outputs": [],
+        "stateMutability": "view",
+        "type": "function"
+    }
+]
 IERC_abi = [
     {
         "constant": True,
         "inputs": [],
         "name": "name",
         "outputs": [
             {
@@ -3997,14 +4190,15 @@
                 "type": "uint256"
             }
         ],
         "name": "Transfer",
         "type": "event"
     }]
 
+
 def get_uniswap_v2_factory():
     return w3.eth.contract(address=constants.UNISWAP_V2_FACTORY, abi=uniswap_v2_factory_abi)
 
 
 def get_uniswap_v2_router():
     return w3.eth.contract(address=constants.UNISWAP_V2_ROUTER, abi=uniswap_v2_router_abi)
 
@@ -4025,7 +4219,11 @@
 def get_uniswap_v3_pool(token0, token1, fee):
     address = get_uniswap_v3_factory().functions.getPool(token0, token1, fee).call()
     return w3.eth.contract(address=address, abi=uniswap_v3_pool_abi)
 
 
 def get_bot_contract():
     return w3.eth.contract(address=constants.CONTRACT_ADDRESS, abi=contract_abi)
+
+
+def get_uniswap_v3_quoter():
+    return w3.eth.contract(address=constants.UNISWAP_V3_QUOTER, abi=uniswap_v3_quoter_abi)
```

