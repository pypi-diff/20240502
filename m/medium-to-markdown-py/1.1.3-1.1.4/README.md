# Comparing `tmp/medium_to_markdown_py-1.1.3.tar.gz` & `tmp/medium_to_markdown_py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.1.3.tar", last modified: Mon Apr 29 14:46:13 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.1.4.tar", last modified: Thu May  2 14:55:30 2024, max compression
```

## Comparing `medium_to_markdown_py-1.1.3.tar` & `medium_to_markdown_py-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 14:46:13.110270 medium_to_markdown_py-1.1.3/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.3/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 14:46:13.110209 medium_to_markdown_py-1.1.3/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      670 2024-04-29 13:19:17.000000 medium_to_markdown_py-1.1.3/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 14:46:13.108522 medium_to_markdown_py-1.1.3/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)     8034 2024-04-29 14:45:54.000000 medium_to_markdown_py-1.1.3/medium_to_markdown/Parser.py
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-29 14:46:09.000000 medium_to_markdown_py-1.1.3/medium_to_markdown/__init__.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 14:46:13.109912 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 14:46:13.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-29 14:46:13.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-29 14:46:13.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-29 14:46:13.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-29 14:46:13.000000 medium_to_markdown_py-1.1.3/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-29 14:46:13.110726 medium_to_markdown_py-1.1.3/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-29 14:46:06.000000 medium_to_markdown_py-1.1.3/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.707810 medium_to_markdown_py-1.1.4/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.4/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-02 14:55:30.707745 medium_to_markdown_py-1.1.4/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      670 2024-04-29 13:19:17.000000 medium_to_markdown_py-1.1.4/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.706376 medium_to_markdown_py-1.1.4/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)     8414 2024-05-02 14:54:04.000000 medium_to_markdown_py-1.1.4/medium_to_markdown/Parser.py
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-05-02 14:54:35.000000 medium_to_markdown_py-1.1.4/medium_to_markdown/__init__.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-05-02 14:55:30.707534 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      364 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-05-02 14:55:30.000000 medium_to_markdown_py-1.1.4/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-05-02 14:55:30.708116 medium_to_markdown_py-1.1.4/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-05-02 14:54:42.000000 medium_to_markdown_py-1.1.4/setup.py
```

### Comparing `medium_to_markdown_py-1.1.3/LICENSE` & `medium_to_markdown_py-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.3/README.md` & `medium_to_markdown_py-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.3/medium_to_markdown/Parser.py` & `medium_to_markdown_py-1.1.4/medium_to_markdown/Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,26 @@
         if self.output_filename != "":
             if self.output_filename.endswith(".md"):
                 self.output_filename = self.output_filename[:-3]
                 
             self.output_filename = f"{self.current_date}-{self.output_filename}"
 
 
-    def parse(self,is_save=True):
+    def parse(self,txt_html="",is_save=True):
         """
         Parses the Medium post, saves it as a Markdown file, and returns True if successful, False otherwise.
         Parameters:
+        - txt_html (str): The HTML content of the Medium article. If not provided, the content will be fetched from the URL.
         - is_save (bool): Flag indicating whether to save the output Markdown file. Default is True.
         """
         try:
-            dom = self.get_dom(self.url)
+            if txt_html:
+                dom = BeautifulSoup(txt_html, 'html.parser')
+            else:
+                dom = self.get_dom(self.url)
             self.get_meta(dom)
             
             if self.output_filename == "":
                 self.output_filename = re.sub(r'[<>:"/\\|?*]', '', self.title).replace(" ", "_")
                 output_filename = f"{self.OUTPUT_DIR}/{self.current_date}-{self.output_filename}.md"
             else:
                 output_filename = f"{self.OUTPUT_DIR}/{self.output_filename}.md"
@@ -82,16 +86,18 @@
     def get_dom(self,url):
         response = requests.get(url, verify=self.ssl_verify,headers=self.headers)
         response.raise_for_status()
         return BeautifulSoup(response.text, 'html.parser')
     
     def get_meta(self,dom):
         try:
+            url_tag = dom.find('meta', {'property': 'og:url'})
             title_tag = dom.find('meta', {'name': 'title'})
             author_tag = dom.find('meta', {'name': 'author'})
+            self.url = url_tag['content'] if self.url=="" else self.url
             self.title = title_tag['content'] if title_tag else ''
             self.author = author_tag['content'] if author_tag else ''
             return True
         except Exception as e:
             print(f"An error occurred: {e}")
             return False
```

### Comparing `medium_to_markdown_py-1.1.3/setup.py` & `medium_to_markdown_py-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium_to_markdown_py',
-    version='1.1.3',
+    version='1.1.4',
     description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

