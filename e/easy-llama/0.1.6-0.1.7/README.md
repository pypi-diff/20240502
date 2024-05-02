# Comparing `tmp/easy_llama-0.1.6.tar.gz` & `tmp/easy_llama-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_llama-0.1.6.tar", last modified: Thu May  2 15:12:04 2024, max compression
+gzip compressed data, was "easy_llama-0.1.7.tar", last modified: Thu May  2 16:23:46 2024, max compression
```

## Comparing `easy_llama-0.1.6.tar` & `easy_llama-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.949412 easy_llama-0.1.6/
--rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.6/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 15:12:04.949192 easy_llama-0.1.6/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)    13482 2024-05-01 08:34:07.000000 easy_llama-0.1.6/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.948145 easy_llama-0.1.6/easy_llama/
--rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 15:11:16.000000 easy_llama-0.1.6/easy_llama/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.6/easy_llama/formats.py
--rw-r--r--   0 dylan      (501) staff       (20)    24212 2024-04-30 21:53:32.000000 easy_llama-0.1.6/easy_llama/model.py
--rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.6/easy_llama/samplers.py
--rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.6/easy_llama/thread.py
--rw-r--r--   0 dylan      (501) staff       (20)     4731 2024-04-30 21:53:43.000000 easy_llama-0.1.6/easy_llama/utils.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 15:12:04.948995 easy_llama-0.1.6/easy_llama.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 15:12:04.000000 easy_llama-0.1.6/easy_llama.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 15:12:04.949460 easy_llama-0.1.6/setup.cfg
--rw-r--r--   0 dylan      (501) staff       (20)     1212 2024-05-02 15:11:19.000000 easy_llama-0.1.6/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.868368 easy_llama-0.1.7/
+-rw-r--r--   0 dylan      (501) staff       (20)     1211 2024-04-30 22:20:53.000000 easy_llama-0.1.7/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 16:23:46.868135 easy_llama-0.1.7/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)    13907 2024-05-02 15:43:35.000000 easy_llama-0.1.7/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.867113 easy_llama-0.1.7/easy_llama/
+-rw-r--r--   0 dylan      (501) staff       (20)      241 2024-05-02 15:55:14.000000 easy_llama-0.1.7/easy_llama/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    16378 2024-04-30 21:53:31.000000 easy_llama-0.1.7/easy_llama/formats.py
+-rw-r--r--   0 dylan      (501) staff       (20)    24184 2024-05-02 15:54:29.000000 easy_llama-0.1.7/easy_llama/model.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4053 2024-04-30 21:53:34.000000 easy_llama-0.1.7/easy_llama/samplers.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21726 2024-05-01 06:46:41.000000 easy_llama-0.1.7/easy_llama/thread.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4705 2024-05-02 15:54:04.000000 easy_llama-0.1.7/easy_llama/utils.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-05-02 16:23:46.867951 easy_llama-0.1.7/easy_llama.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     1085 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)      324 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       26 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2024-05-02 16:23:46.000000 easy_llama-0.1.7/easy_llama.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-05-02 16:23:46.868413 easy_llama-0.1.7/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     1267 2024-05-02 15:55:17.000000 easy_llama-0.1.7/setup.py
```

### Comparing `easy_llama-0.1.6/LICENSE` & `easy_llama-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.6/PKG-INFO` & `easy_llama-0.1.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.6
+Version: 0.1.7
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.6/README.md` & `easy_llama-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 >>> import easy_llama as ez
 >>> Mixtral = ez.Model('Mixtral-8x7B-v0.1-q8_0.gguf')
 >>> Mixtral.generate('The sky is')
 ' an inverted bowl that covers the earth with an infinite dome, and the sun, moon and stars are attached to its inside surface. The sun revolves around the earth once a day and the stars revolve around the earth at night.\n\nThis is the basic theory of the geocentric model of the universe. This model was the accepted cosmological view of the world in Ancient Greece, and was adopted by the Roman Catholic Church and was the official view of the Church until 1600.\n\nThe geocentric model was based on the writings of Aristotle and Ptolemy, and the Catholic Church accepted it as an article of faith. The Catholic Church was opposed to any views that contradicted the geocentric model, and threatened with excommunication anyone who held to the heliocentric view.\n\nThe heliocentric model of the universe was first proposed by Aristarchus of Samos in the 3rd Century BC, and was based on the observation that the planets and the moon revolve around the sun. The sun is in the center of the universe and the earth and other planets revolve around it.\n\nThe heliocentric model was not accepted by the Catholic Church, and was not accepted as a scientific theory until the 1600s.'
 >>> 
 ```
 
-easy-llama is designed to be as simple as possible to use, at the expense of some functionality. It is a layer of abstraction over [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), which itself provides the Python bindings for the underlying [llama.cpp](https://github.com/ggerganov/llama.cpp) library.
+easy-llama's purpose is to make use of **on-device large language models (LLMs) as easily as possible**. It is a layer of abstraction over [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), which itself provides the Python bindings for the underlying [llama.cpp](https://github.com/ggerganov/llama.cpp) project.
 
 ## Features
 - [x] Automatic arbitrary context length extension
 	- Just specify your desired context length, and easy-llama will adjust the necessary parameters accordingly
 	- A warning will be displayed if the chosen context length is likely to cause a loss of quality
 - [x] Terminal-based interactive chat
     - `Thread.interact()`  
@@ -31,15 +31,15 @@
 	- Both your message and bot's message are added to Thread
 - [x] Several common prompt formats built-in
   - accessible under `easy_llama.formats`
   - Stanford Alpaca, Mistral Instruct, Mistral Instruct Safe, ChatML, Llama2Chat, Llama3, Command-R, Vicuna LMSYS, Vicuna Common, Dolphin, Guanaco, & more
   - Easily extend, duplicate and modify built-in formats
   - `easy_llama.formats.wrap(prompt)` - Wrap a given prompt in any prompt format for single-turn completion
 - [X] Message-based context length handling
-- [ ] WIP: Retrieve sorted list of candidates for the most likely next token (i.e. logits)
+- [ ] Retrieve sorted list of candidates for the most likely next token (i.e. logits)
 - [X] Support all models supported by llama-cpp-python
 
 ## Examples
 
 #### Programmatic chat
 ```python
 >>> import easy_llama as ez
@@ -56,14 +56,19 @@
 ```python
 >>> import easy_llama as ez
 >>> Llama3 = ez.Model('Meta-Llama-3-8B-Instruct-q8_0.gguf')
 >>> Thread = ez.Thread(Llama3, ez.formats.llama3, ez.samplers.TikTokenSampling)
 >>> Thread.interact()
 ```
 
+<details>
+<summary>Click to expand interactive chat example</summary>
+
+In practice, the prompt and the response are differentiated by color for improved readability.
+
 ```
   > What is HTML?
 
 Hello there! I'm Llama 3, here to help you with any questions you may have.
 
 HTML stands for HyperText Markup Language. It's the standard markup language used to create web pages. In simple terms, HTML is a way to add structure and content to a webpage, making it look and behave as intended.
 
@@ -128,137 +133,148 @@
 You're welcome! It was a pleasure chatting with you and helping you understand the basics of HTML. If you have any more questions or need further clarification, feel free to reach out anytime.  
 
 Have a great day and happy coding (or web-browsing)!
 
   > 
 ```
 
+</details>
+
 ## Installing with pip
 
 In most cases, the best way to install easy-llama is through pip.
 
 Select your backend from the list below to see your installation instructions. If you run into issues with the installation, please see the [llama-cpp-python installation instructions](https://github.com/abetlen/llama-cpp-python?tab=readme-ov-file#installation) for a more detailed guide. If you're still having trouble, feel free to [open an issue](https://github.com/ddh0/easy-llama/issues/new/).
 
 <details>
 <summary>CPU only</summary>
 
 ```
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+pip install --upgrade easy-llama
 ```
 
 </details>
 <details>
 <summary>CUDA (for NVIDIA)</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_CUDA=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_CUDA=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>Metal (for Apple Silicon)</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `brew`. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_METAL=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_METAL=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>ROCm (for AMD)</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_HIPBLAS=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_HIPBLAS=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>Vulkan</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_VULKAN=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_VULKAN=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>CLBlast</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_CLBLAST=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_CLBLAST=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>OpenBLAS</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>Kompute</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
-CMAKE_ARGS="-DLLAMA_KOMPUTE=on" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
+pip uninstall llama-cpp-python -y
+CMAKE_ARGS="-DLLAMA_KOMPUTE=on" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 <details>
 <summary>SYCL</summary>
 
 You will need `cmake` to install easy-llama. It is probably available in your preferred package manager, such as `apt`, `brew`, `yum`, etc. Or you can install it [from source](https://cmake.org/download/).
 
 ```bash
+pip uninstall llama-cpp-python -y
 source /opt/intel/oneapi/setvars.sh
-CMAKE_ARGS="-DLLAMA_SYCL=on -DCMAKE_C_COMPILER=icx -DCMAKE_CXX_COMPILER=icpx" pip install --no-cache-dir --force-reinstall --upgrade llama-cpp-python 
-pip install easy-llama
+CMAKE_ARGS="-DLLAMA_SYCL=on -DCMAKE_C_COMPILER=icx -DCMAKE_CXX_COMPILER=icpx" pip install --no-cache-dir llama-cpp-python 
+pip install --upgrade easy-llama
 ```
 </details>
 
 ## Installing from source
 
 Installation from source is only necessary if you rely on some functionality from llama.cpp that is not yet supported by llama-cpp-python. In most cases, you should prefer installing with pip.
 
 > [!NOTE]
 >
-> You will need to modify the CMAKE_ARGS according to your backend. The arguments shown below are for CUDA support. If you're not using CUDA, select your backend above to see the correct CMAKE_ARGS.
+> You will need to modify the `CMAKE_ARGS` variable according to your backend. The arguments shown below are for CUDA support. If you're not using CUDA, select your backend above to see the correct `CMAKE_ARGS`.
 
 To install easy-llama from source, copy and paste the following commands into your terminal:
 
-<details>
-<summary>Click to expand</summary>
-
 ```bash
+pip uninstall easy-llama llama-cpp-python -y
+rm -rf ./easy-llama
+rm -rf ./llama-cpp-python
 git clone https://github.com/abetlen/llama-cpp-python
 cd ./llama-cpp-python/vendor/
 rm -rf ./llama.cpp
 git clone https://github.com/ggerganov/llama.cpp
 cd -
 git clone https://github.com/ddh0/easy-llama
 CMAKE_ARGS="-DLLAMA_CUDA=on" pip install -e ./llama-cpp-python
 pip install -e ./easy-llama
 ```
-</details>
 
 ## Acknowledgments
 easy-llama stands on the shoulders of giants. Thank you to [Andrei Betlen](https://github.com/abetlen) for [llama-cpp-python](https://github.com/abetlen/llama-cpp-python), and to [Georgi Gerganov](https://github.com/ggerganov) for [llama.cpp](https://github.com/ggerganov/llama.cpp) and [GGML](https://github.com/ggerganov/ggml). Thank you to all who have made contributions to these projects.
 
 ###### DISCLAIMER
 All language models tend to produce writing that is factually inaccurate, stereotypically biased, and fundamentally disconnected from reality.
 
 ###### LICENSE
 > [The Unlicense](LICENSE)
 > 
-> *easy-llama is free and unencumbered software released into the public domain*
+> *easy-llama is free and unencumbered software released into the public domain*
```

### Comparing `easy_llama-0.1.6/easy_llama/formats.py` & `easy_llama-0.1.7/easy_llama/formats.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.6/easy_llama/model.py` & `easy_llama-0.1.7/easy_llama/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # model.py
 # https://github.com/ddh0/easy-llama/
 
 """Submodule containing the Model class to work with language models"""
 
+import sys
+
 from typing     import Generator, Optional, TextIO, Union, List
 from .utils     import GGUFReader, print_warning, print_verbose
 from .samplers  import SamplerSettings, DefaultSampling
 from llama_cpp  import Llama, StoppingCriteriaList
 from os.path    import isdir, exists
 
 from os  import cpu_count as os_cpu_count
-from sys import stdout    as sys_stdout
 
 
 # for typing of Model.stream_print() parameter `file`
 class _SupportsWriteAndFlush(TextIO):
     pass
 
 class ModelUnloadedException(Exception):
@@ -515,15 +516,15 @@
 
     def stream_print(
             self,
             prompt: Union[str, list[int]],
             stops: list[Union[str, int]] = [],
             sampler: SamplerSettings = DefaultSampling,
             end: str = "\n",
-            file: _SupportsWriteAndFlush = sys_stdout,
+            file: _SupportsWriteAndFlush = sys.stdout,
             flush: bool = True
     ) -> str:
         """
         Given a prompt, stream text as it is generated, and return the generated string.
         The returned string does not include the `end` parameter.
 
         `Model.stream_print(...)` is a shorthand for:
```

### Comparing `easy_llama-0.1.6/easy_llama/samplers.py` & `easy_llama-0.1.7/easy_llama/samplers.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.6/easy_llama/thread.py` & `easy_llama-0.1.7/easy_llama/thread.py`

 * *Files identical despite different names*

### Comparing `easy_llama-0.1.6/easy_llama/utils.py` & `easy_llama-0.1.7/easy_llama/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # utils.py
 # https://github.com/ddh0/easy-llama/
 
 """Submodule containing convenience functions and GGUFReader"""
 
+import sys
+
 from time     import strftime
 from enum     import IntEnum
 from struct   import unpack
 from colorama import Fore
 from typing   import Any
 
-from sys import stderr as sys_stderr
-
 
 # color codes used in Thread.interact()
 RESET_ALL = Fore.RESET
 USER_STYLE = RESET_ALL + Fore.GREEN
 BOT_STYLE = RESET_ALL + Fore.CYAN
 DIM_STYLE = RESET_ALL + Fore.LIGHTBLACK_EX
 SPECIAL_STYLE = RESET_ALL + Fore.YELLOW
@@ -136,14 +136,14 @@
 
 # no longer used in this module, but left for others to use
 def get_timestamp_prefix_str() -> str:
     # helpful: https://strftime.net
     return strftime("[%Y, %b %e, %a %l:%M %p] ")
 
 def print_verbose(text: str) -> None:
-    print("easy_llama: verbose:", text, file=sys_stderr, flush=True)
+    print("easy_llama: verbose:", text, file=sys.stderr, flush=True)
 
 def print_info(text: str) -> None:
-    print("easy_llama: info:", text, file=sys_stderr, flush=True)
+    print("easy_llama: info:", text, file=sys.stderr, flush=True)
 
 def print_warning(text: str) -> None:
-    print("easy_llama: warning:", text, file=sys_stderr, flush=True)
+    print("easy_llama: warning:", text, file=sys.stderr, flush=True)
```

### Comparing `easy_llama-0.1.6/easy_llama.egg-info/PKG-INFO` & `easy_llama-0.1.7/easy_llama.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_llama
-Version: 0.1.6
+Version: 0.1.7
 Summary: Text generation in Python, made easy
 Home-page: https://github.com/ddh0/easy-llama/
 Author: Dylan Halladay
 Author-email: dylanhalladay02@icloud.com
 License: The Unlicense
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `easy_llama-0.1.6/setup.py` & `easy_llama-0.1.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+# easy_llama.py
+# https://github.com/ddh0/easy-llama/
+
 from setuptools import setup
 
 setup(
     name='easy_llama',
-    version='0.1.6',
+    version='0.1.7',
     description='Text generation in Python, made easy',
     long_description="""To view the current documentation for easy-llama, visit the project's GitHub repository:\nhttps://github.com/ddh0/easy-llama""",
     url='https://github.com/ddh0/easy-llama/',
     author='Dylan Halladay',
     author_email='dylanhalladay02@icloud.com',
     license='The Unlicense',
     packages=['easy_llama'],
```

