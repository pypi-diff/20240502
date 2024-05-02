# Comparing `tmp/django-chromepdf-1.7.1.tar.gz` & `tmp/django-chromepdf-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-chromepdf-1.7.1.tar", last modified: Tue Feb 20 15:17:00 2024, max compression
+gzip compressed data, was "django-chromepdf-1.7.2.tar", last modified: Thu May  2 12:45:35 2024, max compression
```

## Comparing `django-chromepdf-1.7.1.tar` & `django-chromepdf-1.7.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:17:00.000000 django-chromepdf-1.7.1/
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/chromepdf/
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/chromepdf/chromedrivers/
--rw-r--r--   0 kukwaa    (1078) ims        (100)       93 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/chromedrivers/blank.txt
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/chromepdf/chromesession/
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/chromepdf/chromesession/users/
--rw-r--r--   0 kukwaa    (1078) ims        (100)       83 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/chromesession/users/blank.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)      296 2024-02-20 15:16:33.000000 django-chromepdf-1.7.1/chromepdf/__init__.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)      466 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/__main__.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     2276 2024-02-20 15:16:33.000000 django-chromepdf-1.7.1/chromepdf/conf.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)      141 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/exceptions.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3532 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/maker.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     8853 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/pdfconf.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     4685 2024-02-20 15:16:33.000000 django-chromepdf-1.7.1/chromepdf/run.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     2309 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/shortcuts.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3108 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/sizes.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)     9259 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/chromepdf/webdrivermakers.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)    18435 2024-02-20 15:16:33.000000 django-chromepdf-1.7.1/chromepdf/webdrivers.py
-drwxr-xr-x   0 kukwaa    (1078) ims        (100)        0 2024-02-20 15:17:00.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/
--rw-r--r--   0 kukwaa    (1078) ims        (100)    11180 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/PKG-INFO
--rw-r--r--   0 kukwaa    (1078) ims        (100)      541 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/SOURCES.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)        1 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/dependency_links.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)       15 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/requires.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)       10 2024-02-20 15:16:59.000000 django-chromepdf-1.7.1/django_chromepdf.egg-info/top_level.txt
--rw-r--r--   0 kukwaa    (1078) ims        (100)      121 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/MANIFEST.in
--rw-r--r--   0 kukwaa    (1078) ims        (100)     8494 2024-02-20 15:16:33.000000 django-chromepdf-1.7.1/README.md
--rw-r--r--   0 kukwaa    (1078) ims        (100)     3928 2024-02-20 15:15:22.000000 django-chromepdf-1.7.1/setup.py
--rw-r--r--   0 kukwaa    (1078) ims        (100)    11180 2024-02-20 15:17:00.000000 django-chromepdf-1.7.1/PKG-INFO
--rw-r--r--   0 kukwaa    (1078) ims        (100)       38 2024-02-20 15:17:00.000000 django-chromepdf-1.7.1/setup.cfg
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:35.035726 django-chromepdf-1.7.2/
+-rw-r--r--   0 kukwaa    (1078) users      (100)     1545 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/LICENSE
+-rw-r--r--   0 kukwaa    (1078) users      (100)      121 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/MANIFEST.in
+-rw-r--r--   0 kukwaa    (1078) users      (100)     9845 2024-05-02 12:45:35.034725 django-chromepdf-1.7.2/PKG-INFO
+-rw-r--r--   0 kukwaa    (1078) users      (100)     8494 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/README.md
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:34.999721 django-chromepdf-1.7.2/chromepdf/
+-rw-r--r--   0 kukwaa    (1078) users      (100)      296 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/chromepdf/__init__.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)      466 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/__main__.py
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:35.003706 django-chromepdf-1.7.2/chromepdf/chromedrivers/
+-rw-r--r--   0 kukwaa    (1078) users      (100)       93 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/chromedrivers/blank.txt
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:34.958720 django-chromepdf-1.7.2/chromepdf/chromesession/
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:35.010715 django-chromepdf-1.7.2/chromepdf/chromesession/users/
+-rw-r--r--   0 kukwaa    (1078) users      (100)       83 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/chromesession/users/blank.txt
+-rw-r--r--   0 kukwaa    (1078) users      (100)     2276 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/chromepdf/conf.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)      141 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/exceptions.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     3532 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/maker.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     8853 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/pdfconf.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     4685 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/chromepdf/run.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     2309 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/shortcuts.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     3108 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/sizes.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)     9497 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/chromepdf/webdrivermakers.py
+-rw-r--r--   0 kukwaa    (1078) users      (100)    18435 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/chromepdf/webdrivers.py
+drwxr-xr-x   0 kukwaa    (1078) users      (100)        0 2024-05-02 12:45:35.031736 django-chromepdf-1.7.2/django_chromepdf.egg-info/
+-rw-r--r--   0 kukwaa    (1078) users      (100)     9845 2024-05-02 12:45:34.000000 django-chromepdf-1.7.2/django_chromepdf.egg-info/PKG-INFO
+-rw-r--r--   0 kukwaa    (1078) users      (100)      564 2024-05-02 12:45:34.000000 django-chromepdf-1.7.2/django_chromepdf.egg-info/SOURCES.txt
+-rw-r--r--   0 kukwaa    (1078) users      (100)        1 2024-05-02 12:45:34.000000 django-chromepdf-1.7.2/django_chromepdf.egg-info/dependency_links.txt
+-rw-r--r--   0 kukwaa    (1078) users      (100)       15 2024-05-02 12:45:34.000000 django-chromepdf-1.7.2/django_chromepdf.egg-info/requires.txt
+-rw-r--r--   0 kukwaa    (1078) users      (100)       10 2024-05-02 12:45:34.000000 django-chromepdf-1.7.2/django_chromepdf.egg-info/top_level.txt
+-rw-r--r--   0 kukwaa    (1078) users      (100)     1904 2024-05-02 12:43:04.000000 django-chromepdf-1.7.2/pyproject.toml
+-rw-r--r--   0 kukwaa    (1078) users      (100)       38 2024-05-02 12:45:35.036712 django-chromepdf-1.7.2/setup.cfg
+-rw-r--r--   0 kukwaa    (1078) users      (100)     3928 2024-05-01 14:02:32.000000 django-chromepdf-1.7.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-chromepdf-1.7.1/chromepdf/conf.py` & `django-chromepdf-1.7.2/chromepdf/conf.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/maker.py` & `django-chromepdf-1.7.2/chromepdf/maker.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/pdfconf.py` & `django-chromepdf-1.7.2/chromepdf/pdfconf.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/run.py` & `django-chromepdf-1.7.2/chromepdf/run.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/shortcuts.py` & `django-chromepdf-1.7.2/chromepdf/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/sizes.py` & `django-chromepdf-1.7.2/chromepdf/sizes.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/chromepdf/webdrivermakers.py` & `django-chromepdf-1.7.2/chromepdf/webdrivermakers.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,17 +85,18 @@
         pdf_kwargs = _clean_pdf_kwargs(pdf_kwargs)
 
         # we could put the html here. but data urls in Chrome are limited to 2MB.
         dataurl = "data:text/html;charset=utf-8,"
         self.driver.get(dataurl)
 
         # append our html. theoretically no length limit.
-        html = html.replace('`', r'\`')  # escape the backtick used to indicate a multiline string in javascript
+        html = html.replace('\'', '\\\'')  # We wrap the string in '', so escape all other '
+        html = html.replace('\n', ' \\\n')  # Allow newlines within '', and avoid concatenating words
         # we do NOT need to escape any other chars (quotes, etc), including unicode
-        self.driver.execute_script("document.write(`{}`)".format(html))
+        self.driver.execute_script("document.write('{}')".format(html))
 
         return self._get_pdf_bytes(pdf_kwargs)
 
     def generate_pdf_url(self, url, pdf_kwargs):
         "Return the bytes of a PDF generated from a URL."
 
         warnings.warn("generate_pdf_url() is deprecated, use generate_pdf() instead.", DeprecationWarning)
@@ -177,16 +178,18 @@
         # Go to data url that we will turn into the PDF
         driverurl = self._get_driver_command_url('url')
         data = {'url': "data:text/html;charset=utf-8,"}
         output = get_chromedriver_response(driverurl, data)
 
         # Write the HTML for the PDF
         driverurl = self._get_driver_command_url('execute/sync')
-        html = html.replace('`', r'\`')
-        script = "document.write(`{}`)".format(html)
+
+        html = html.replace('\'', '\\\'')  # We wrap the string in '', so escape all other '
+        html = html.replace('\n', ' \\\n')  # Allow newlines within '', and avoid concatenating words
+        script = "document.write('{}')".format(html)
         data = {"script": script, 'args': []}
         output = get_chromedriver_response(driverurl, data)
 
         return self._get_pdf_bytes(pdf_kwargs)
 
     def generate_pdf_url(self, url, pdf_kwargs):
         "Return the bytes of a PDF generated from a URL."
```

### Comparing `django-chromepdf-1.7.1/chromepdf/webdrivers.py` & `django-chromepdf-1.7.2/chromepdf/webdrivers.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/django_chromepdf.egg-info/PKG-INFO` & `django-chromepdf-1.7.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,186 +1,17 @@
 Metadata-Version: 2.1
 Name: django-chromepdf
-Version: 1.7.1
+Version: 1.7.2
 Summary: A small Python 3 library that uses Selenium and Google Chrome to convert HTML into a PDF.
-Home-page: https://github.com/imsweb/django-chromepdf
-Author: Andrew Kukwa
-Author-email: kukwaa@imsweb.com
+Author-email: Andrew Kukwa <kukwaa@imsweb.com>
+Maintainer-email: Andrew Kukwa <kukwaa@imsweb.com>
 License: BSD
-Project-URL: Source, https://github.com/imsweb/django-chromepdf
-Project-URL: Changelog, https://github.com/imsweb/django-chromepdf/blob/main/CHANGELOG.md
-Description: # ChromePDF
-        
-        ## Overview
-        
-        ChromePDF is a small Python 3 library that uses [Selenium](https://pypi.org/project/selenium/) and Google Chrome to convert HTML into a PDF. This is accomplished by using Chrome's `Page.printToPDF` DevTools command.
-        
-        ChromePDF provides a function that accepts an html string, plus a dict of page parameters, and other settings, and returns the bytes containing a PDF:
-        
-        ```
-        pdf_bytes = generate_pdf(html_string, pdf_kwargs, **kwargs)
-        ```
-        
-        As of version 1.4, ChromePDF can also be run from the command line.
-        
-        ```
-        python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/input.html path/to/output.pdf
-        ```
-        
-        Because it renders via Chrome, it supports a wide range of CSS and HTML tags that should display the same as if you used Chrome to view the HTML itself.
-        
-        ChromePDF can take advantage of [Django](https://pypi.org/project/Django/) settings for configuration, but Django is not a required dependency.
-        
-        Official ChromePDF releases [are available on PyPI](https://pypi.org/project/django-chromepdf/).
-        
-        ## Installation
-        
-        **1. Install ChromePDF via pip.**
-        
-        The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
-        
-        You may view the [Changelog](https://github.com/imsweb/django-chromepdf/blob/main/CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
-        ```
-        pip install django-chromepdf~=1.7.1
-        ```
-        
-        **2. Set the location of your Chrome executable.** This can be done in one of two ways:
-        
-        * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
-        * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
-        
-        ## About Chromedrivers
-        
-        A chromedriver executable is necessary to interface between Selenium and Chrome. ChromePDF will automatically check the version of your Chrome binary and download the required chromedriver [from the Chrome website](https://chromedriver.chromium.org/downloads) if it doesn't exist, into your `site-packages/chromepdf/chromedrivers/` folder. If the Chrome binary ever gets upgraded, ChromePDF will realize this and download the required driver for it.
-        
-        You may disable these automatic downloads in the following way:
-        * In your Django settings, set `CHROMEPDF['CHROMEDRIVER_DOWNLOADS']` to False
-        * OR, pass a `chromedriver_downloads=False` argument to `generate_pdf()`
-        
-        You may also specify a chromedriver path manually. This is recommended if you disable downloads:
-        * In your Django settings, set `CHROMEPDF['CHROMEDRIVER_PATH']` to the full path of the executable (E.G., `r'C:\Users\myuser\...\chromedriver_win32\chromedriver.exe'`)
-        * OR, pass a `chromedriver_path` argument to `generate_pdf()` containing the path.
-        * OR, if both of the above are not set, and you've disabled downloads, and if your chromedriver is in your `PATH` environment variable, then Selenium should be able to find it automatically.
-        
-        ## Example: `generate_pdf()`
-        Note: `generate_pdf()` cannot include external files including CSS. You must include all your CSS within `<style>` tags or as inline styles.
-        
-        ```python
-        # NOTE: This example assumes that you've set Django's settings.CHROMEPDF['CHROME_PATH'] = '(path to your Chrome instance)'
-        from chromepdf import generate_pdf 
-        
-        with open('myfile.html','r') as f:
-            html_string = f.read()
-                     
-        pdf_kwargs = {
-            'paperFormat': 'A4',
-            'marginTop': '2.5cm',
-            'marginLeft': '2cm',
-            'marginRight': '2cm',
-            'marginBottom': '3.5cm',
-            'displayHeaderFooter': True,
-            'headerTemplate': '',
-            'footerTemplate': '''
-                <div style='font-size: 12px; width: 100%; padding: 0; padding-left: 2cm; padding-bottom: 1cm; margin: 0; '>
-                    Page <span class='pageNumber'></span> of <span class='totalPages'></span>
-                </div>
-            ''',
-        }
-        pdf_bytes = generate_pdf(html_string, pdf_kwargs)
-        
-        with open('myfile.pdf', 'wb') as file:
-            file.write(pdf_bytes)
-        ```
-        
-        ## Example: Command-Line Usage
-        ChromePDF can generate PDFs from the command-line. This method will not rely on Django settings. Example syntax:
-        ```
-        # Convert file.html into file.pdf and place in the same directory
-        python -m chromepdf generate-pdf path/to/file.html [kwargs]
-        
-        # Convert file.html and place the output PDF file at a specific path.
-        python -m chromepdf generate-pdf path/to/file.html path/to/output.pdf [kwargs]
-        ```
-        Keyword arguments for command-line usage are almost identical to `generate_pdf()` keyword arguments:
-        ```
-        --chrome-path=path/to/google-chrome
-        --chromedriver-path=path/to/chromedriver
-        --chromedriver-downloads=0 # 0 or 1
-        --chrome-args="--arg1 --arg2" # Always use quotes to avoid misinterpreting as commands. 
-        --pdf-kwargs-json=path/to/file.json # JSON file containing a dict of values to pass to pdf_kwargs
-        ```
-        The recommended usage is to pass a `--chrome-path`, and let ChromePDF handle the chromedriver downloads automatically.
-        ```
-        python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/file.html path/to/output.pdf
-        ```
-        The command will have a return code of zero on success, and nonzero on failure.
-        
-        ## Django Settings
-        
-        You can specify default settings in your Django settings file, if desired, via a `CHROMEPDF` settings. Anything passed via the `pdf_kwargs` argument will override the `PDF_KWARGS` settings.
-        ```python
-        # settings.__init__.py
-        
-        CHROMEPDF = {
-            'CHROME_PATH': r'C:\Program Files (x86)\Google\...\chrome.exe',
-            'CHROME_ARGS': [], # Optional list of command-line argument strings to pass to Chrome when rendering a PDF.
-            'CHROMEDRIVER_PATH': None, # will rely on downloads instead
-            'CHROMEDRIVER_DOWNLOADS': True, # automatically download the correct chromedriver for the chrome path
-            'PDF_KWARGS': {
-                'paperFormat': 'A4',
-                'marginTop': '2.5cm',
-                'marginLeft': '2cm',
-                'marginRight': '2cm',
-                'marginBottom': '3.5cm',
-            }
-        }
-        ```
-        
-        
-        ## PDF_KWARGS Options
-        
-        The `pdf_kwargs` argument to `generate_pdf()` lets you specify all the arguments for Chrome's `Page.printToPDF` API. Its API can be viewed here:
-        
-        [Page.printToPDF API](https://chromedevtools.github.io/devtools-protocol/1-3/Page/#method-printToPDF) (url is funky. If you get a 404, try reloading/refreshing)
-        
-        Some shortcut parameters are provided by `generate_pdf()` for convenience. Here is a list of all the options:
-        
-        Layout:
-        *  **scale**: Scale of the PDF. Default `1`.
-        *  **landscape**: `True` to use landscape mode. Default `False`.
-        
-        Page Dimensions:
-        *  **paperWidth**: Width of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `8.5`
-        *  **paperHeight**: Height of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `11`
-        *  **paperFormat**: A string indicating a paper size format, such as `'letter'` or `'A4'`. Case-insensitive. This will override `paperWidth` and `paperHeight`. Not part of `Page.printToPDF` API.  Provided for convenience.
-        
-        Content:
-        *  **displayHeaderFooter**: `True` to display header and footer. Default `False`.
-        *  **headerTemplate**: HTML containing the header for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values. For example, `<span class='title'></span>` would insert the the title.
-           * date: formatted print date 
-           * title: document title 
-           * url: document location 
-           * pageNumber: current page number 
-           * totalPages: total pages in the document 
-        * **footerTemplate**: HTML containing the footer for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values (same as above)
-        * **printBackground**: `True` to print background graphics. Default `False`.
-        
-        Margins:
-        *  **margin**: Shortcut used to set all four margin values at once. Not part of `Page.printToPDF` API.  Provided for convenience.
-        *  **marginTop**: Top margin. Default: `'1cm'`
-        *  **marginBottom**: Bottom margin. Default: `'1cm'`
-        *  **marginLeft**: Left margin. Default: `'1cm'`
-        *  **marginRight**: Right margin. Default: `'1cm'`
-        
-        Page Ranges:
-        *  **pageRanges**: String indicating page ranges to use. Example: `'1-5, 8, 11-13'`
-        *  **ignoreInvalidPageRanges**: If `True`, will silently ignore invalid 'pageRanges' values. Default `False`.
-        
-        
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/imsweb/django-chromepdf
+Project-URL: repository, https://github.com/imsweb/django-chromepdf
+Project-URL: changelog, https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: OS Independent
@@ -191,7 +22,176 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ChromePDF
+
+## Overview
+
+ChromePDF is a small Python 3 library that uses [Selenium](https://pypi.org/project/selenium/) and Google Chrome to convert HTML into a PDF. This is accomplished by using Chrome's `Page.printToPDF` DevTools command.
+
+ChromePDF provides a function that accepts an html string, plus a dict of page parameters, and other settings, and returns the bytes containing a PDF:
+
+```
+pdf_bytes = generate_pdf(html_string, pdf_kwargs, **kwargs)
+```
+
+As of version 1.4, ChromePDF can also be run from the command line.
+
+```
+python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/input.html path/to/output.pdf
+```
+
+Because it renders via Chrome, it supports a wide range of CSS and HTML tags that should display the same as if you used Chrome to view the HTML itself.
+
+ChromePDF can take advantage of [Django](https://pypi.org/project/Django/) settings for configuration, but Django is not a required dependency.
+
+Official ChromePDF releases [are available on PyPI](https://pypi.org/project/django-chromepdf/).
+
+## Installation
+
+**1. Install ChromePDF via pip.**
+
+The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
+
+You may view the [Changelog](CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
+```
+pip install django-chromepdf~=1.7.2
+```
+
+**2. Set the location of your Chrome executable.** This can be done in one of two ways:
+
+* In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
+* OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
+
+## About Chromedrivers
+
+A chromedriver executable is necessary to interface between Selenium and Chrome. ChromePDF will automatically check the version of your Chrome binary and download the required chromedriver [from the Chrome website](https://chromedriver.chromium.org/downloads) if it doesn't exist, into your `site-packages/chromepdf/chromedrivers/` folder. If the Chrome binary ever gets upgraded, ChromePDF will realize this and download the required driver for it.
+
+You may disable these automatic downloads in the following way:
+* In your Django settings, set `CHROMEPDF['CHROMEDRIVER_DOWNLOADS']` to False
+* OR, pass a `chromedriver_downloads=False` argument to `generate_pdf()`
+
+You may also specify a chromedriver path manually. This is recommended if you disable downloads:
+* In your Django settings, set `CHROMEPDF['CHROMEDRIVER_PATH']` to the full path of the executable (E.G., `r'C:\Users\myuser\...\chromedriver_win32\chromedriver.exe'`)
+* OR, pass a `chromedriver_path` argument to `generate_pdf()` containing the path.
+* OR, if both of the above are not set, and you've disabled downloads, and if your chromedriver is in your `PATH` environment variable, then Selenium should be able to find it automatically.
+
+## Example: `generate_pdf()`
+Note: `generate_pdf()` cannot include external files including CSS. You must include all your CSS within `<style>` tags or as inline styles.
+
+```python
+# NOTE: This example assumes that you've set Django's settings.CHROMEPDF['CHROME_PATH'] = '(path to your Chrome instance)'
+from chromepdf import generate_pdf 
+
+with open('myfile.html','r') as f:
+    html_string = f.read()
+             
+pdf_kwargs = {
+    'paperFormat': 'A4',
+    'marginTop': '2.5cm',
+    'marginLeft': '2cm',
+    'marginRight': '2cm',
+    'marginBottom': '3.5cm',
+    'displayHeaderFooter': True,
+    'headerTemplate': '',
+    'footerTemplate': '''
+        <div style='font-size: 12px; width: 100%; padding: 0; padding-left: 2cm; padding-bottom: 1cm; margin: 0; '>
+            Page <span class='pageNumber'></span> of <span class='totalPages'></span>
+        </div>
+    ''',
+}
+pdf_bytes = generate_pdf(html_string, pdf_kwargs)
+
+with open('myfile.pdf', 'wb') as file:
+    file.write(pdf_bytes)
+```
+
+## Example: Command-Line Usage
+ChromePDF can generate PDFs from the command-line. This method will not rely on Django settings. Example syntax:
+```
+# Convert file.html into file.pdf and place in the same directory
+python -m chromepdf generate-pdf path/to/file.html [kwargs]
+
+# Convert file.html and place the output PDF file at a specific path.
+python -m chromepdf generate-pdf path/to/file.html path/to/output.pdf [kwargs]
+```
+Keyword arguments for command-line usage are almost identical to `generate_pdf()` keyword arguments:
+```
+--chrome-path=path/to/google-chrome
+--chromedriver-path=path/to/chromedriver
+--chromedriver-downloads=0 # 0 or 1
+--chrome-args="--arg1 --arg2" # Always use quotes to avoid misinterpreting as commands. 
+--pdf-kwargs-json=path/to/file.json # JSON file containing a dict of values to pass to pdf_kwargs
+```
+The recommended usage is to pass a `--chrome-path`, and let ChromePDF handle the chromedriver downloads automatically.
+```
+python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/file.html path/to/output.pdf
+```
+The command will have a return code of zero on success, and nonzero on failure.
+
+## Django Settings
+
+You can specify default settings in your Django settings file, if desired, via a `CHROMEPDF` settings. Anything passed via the `pdf_kwargs` argument will override the `PDF_KWARGS` settings.
+```python
+# settings.__init__.py
+
+CHROMEPDF = {
+    'CHROME_PATH': r'C:\Program Files (x86)\Google\...\chrome.exe',
+    'CHROME_ARGS': [], # Optional list of command-line argument strings to pass to Chrome when rendering a PDF.
+    'CHROMEDRIVER_PATH': None, # will rely on downloads instead
+    'CHROMEDRIVER_DOWNLOADS': True, # automatically download the correct chromedriver for the chrome path
+    'PDF_KWARGS': {
+        'paperFormat': 'A4',
+        'marginTop': '2.5cm',
+        'marginLeft': '2cm',
+        'marginRight': '2cm',
+        'marginBottom': '3.5cm',
+    }
+}
+```
+
+
+## PDF_KWARGS Options
+
+The `pdf_kwargs` argument to `generate_pdf()` lets you specify all the arguments for Chrome's `Page.printToPDF` API. Its API can be viewed here:
+
+[Page.printToPDF API](https://chromedevtools.github.io/devtools-protocol/1-3/Page/#method-printToPDF) (url is funky. If you get a 404, try reloading/refreshing)
+
+Some shortcut parameters are provided by `generate_pdf()` for convenience. Here is a list of all the options:
+
+Layout:
+*  **scale**: Scale of the PDF. Default `1`.
+*  **landscape**: `True` to use landscape mode. Default `False`.
+
+Page Dimensions:
+*  **paperWidth**: Width of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `8.5`
+*  **paperHeight**: Height of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `11`
+*  **paperFormat**: A string indicating a paper size format, such as `'letter'` or `'A4'`. Case-insensitive. This will override `paperWidth` and `paperHeight`. Not part of `Page.printToPDF` API.  Provided for convenience.
+
+Content:
+*  **displayHeaderFooter**: `True` to display header and footer. Default `False`.
+*  **headerTemplate**: HTML containing the header for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values. For example, `<span class='title'></span>` would insert the the title.
+   * date: formatted print date 
+   * title: document title 
+   * url: document location 
+   * pageNumber: current page number 
+   * totalPages: total pages in the document 
+* **footerTemplate**: HTML containing the footer for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values (same as above)
+* **printBackground**: `True` to print background graphics. Default `False`.
+
+Margins:
+*  **margin**: Shortcut used to set all four margin values at once. Not part of `Page.printToPDF` API.  Provided for convenience.
+*  **marginTop**: Top margin. Default: `'1cm'`
+*  **marginBottom**: Bottom margin. Default: `'1cm'`
+*  **marginLeft**: Left margin. Default: `'1cm'`
+*  **marginRight**: Right margin. Default: `'1cm'`
+
+Page Ranges:
+*  **pageRanges**: String indicating page ranges to use. Example: `'1-5, 8, 11-13'`
+*  **ignoreInvalidPageRanges**: If `True`, will silently ignore invalid 'pageRanges' values. Default `False`.
+
```

### Comparing `django-chromepdf-1.7.1/README.md` & `django-chromepdf-1.7.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 **1. Install ChromePDF via pip.**
 
 The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
 
 You may view the [Changelog](CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
 ```
-pip install django-chromepdf~=1.7.1
+pip install django-chromepdf~=1.7.2
 ```
 
 **2. Set the location of your Chrome executable.** This can be done in one of two ways:
 
 * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
 * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
```

### Comparing `django-chromepdf-1.7.1/setup.py` & `django-chromepdf-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-chromepdf-1.7.1/PKG-INFO` & `django-chromepdf-1.7.2/django_chromepdf.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,186 +1,17 @@
 Metadata-Version: 2.1
 Name: django-chromepdf
-Version: 1.7.1
+Version: 1.7.2
 Summary: A small Python 3 library that uses Selenium and Google Chrome to convert HTML into a PDF.
-Home-page: https://github.com/imsweb/django-chromepdf
-Author: Andrew Kukwa
-Author-email: kukwaa@imsweb.com
+Author-email: Andrew Kukwa <kukwaa@imsweb.com>
+Maintainer-email: Andrew Kukwa <kukwaa@imsweb.com>
 License: BSD
-Project-URL: Source, https://github.com/imsweb/django-chromepdf
-Project-URL: Changelog, https://github.com/imsweb/django-chromepdf/blob/main/CHANGELOG.md
-Description: # ChromePDF
-        
-        ## Overview
-        
-        ChromePDF is a small Python 3 library that uses [Selenium](https://pypi.org/project/selenium/) and Google Chrome to convert HTML into a PDF. This is accomplished by using Chrome's `Page.printToPDF` DevTools command.
-        
-        ChromePDF provides a function that accepts an html string, plus a dict of page parameters, and other settings, and returns the bytes containing a PDF:
-        
-        ```
-        pdf_bytes = generate_pdf(html_string, pdf_kwargs, **kwargs)
-        ```
-        
-        As of version 1.4, ChromePDF can also be run from the command line.
-        
-        ```
-        python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/input.html path/to/output.pdf
-        ```
-        
-        Because it renders via Chrome, it supports a wide range of CSS and HTML tags that should display the same as if you used Chrome to view the HTML itself.
-        
-        ChromePDF can take advantage of [Django](https://pypi.org/project/Django/) settings for configuration, but Django is not a required dependency.
-        
-        Official ChromePDF releases [are available on PyPI](https://pypi.org/project/django-chromepdf/).
-        
-        ## Installation
-        
-        **1. Install ChromePDF via pip.**
-        
-        The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
-        
-        You may view the [Changelog](https://github.com/imsweb/django-chromepdf/blob/main/CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
-        ```
-        pip install django-chromepdf~=1.7.1
-        ```
-        
-        **2. Set the location of your Chrome executable.** This can be done in one of two ways:
-        
-        * In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
-        * OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
-        
-        ## About Chromedrivers
-        
-        A chromedriver executable is necessary to interface between Selenium and Chrome. ChromePDF will automatically check the version of your Chrome binary and download the required chromedriver [from the Chrome website](https://chromedriver.chromium.org/downloads) if it doesn't exist, into your `site-packages/chromepdf/chromedrivers/` folder. If the Chrome binary ever gets upgraded, ChromePDF will realize this and download the required driver for it.
-        
-        You may disable these automatic downloads in the following way:
-        * In your Django settings, set `CHROMEPDF['CHROMEDRIVER_DOWNLOADS']` to False
-        * OR, pass a `chromedriver_downloads=False` argument to `generate_pdf()`
-        
-        You may also specify a chromedriver path manually. This is recommended if you disable downloads:
-        * In your Django settings, set `CHROMEPDF['CHROMEDRIVER_PATH']` to the full path of the executable (E.G., `r'C:\Users\myuser\...\chromedriver_win32\chromedriver.exe'`)
-        * OR, pass a `chromedriver_path` argument to `generate_pdf()` containing the path.
-        * OR, if both of the above are not set, and you've disabled downloads, and if your chromedriver is in your `PATH` environment variable, then Selenium should be able to find it automatically.
-        
-        ## Example: `generate_pdf()`
-        Note: `generate_pdf()` cannot include external files including CSS. You must include all your CSS within `<style>` tags or as inline styles.
-        
-        ```python
-        # NOTE: This example assumes that you've set Django's settings.CHROMEPDF['CHROME_PATH'] = '(path to your Chrome instance)'
-        from chromepdf import generate_pdf 
-        
-        with open('myfile.html','r') as f:
-            html_string = f.read()
-                     
-        pdf_kwargs = {
-            'paperFormat': 'A4',
-            'marginTop': '2.5cm',
-            'marginLeft': '2cm',
-            'marginRight': '2cm',
-            'marginBottom': '3.5cm',
-            'displayHeaderFooter': True,
-            'headerTemplate': '',
-            'footerTemplate': '''
-                <div style='font-size: 12px; width: 100%; padding: 0; padding-left: 2cm; padding-bottom: 1cm; margin: 0; '>
-                    Page <span class='pageNumber'></span> of <span class='totalPages'></span>
-                </div>
-            ''',
-        }
-        pdf_bytes = generate_pdf(html_string, pdf_kwargs)
-        
-        with open('myfile.pdf', 'wb') as file:
-            file.write(pdf_bytes)
-        ```
-        
-        ## Example: Command-Line Usage
-        ChromePDF can generate PDFs from the command-line. This method will not rely on Django settings. Example syntax:
-        ```
-        # Convert file.html into file.pdf and place in the same directory
-        python -m chromepdf generate-pdf path/to/file.html [kwargs]
-        
-        # Convert file.html and place the output PDF file at a specific path.
-        python -m chromepdf generate-pdf path/to/file.html path/to/output.pdf [kwargs]
-        ```
-        Keyword arguments for command-line usage are almost identical to `generate_pdf()` keyword arguments:
-        ```
-        --chrome-path=path/to/google-chrome
-        --chromedriver-path=path/to/chromedriver
-        --chromedriver-downloads=0 # 0 or 1
-        --chrome-args="--arg1 --arg2" # Always use quotes to avoid misinterpreting as commands. 
-        --pdf-kwargs-json=path/to/file.json # JSON file containing a dict of values to pass to pdf_kwargs
-        ```
-        The recommended usage is to pass a `--chrome-path`, and let ChromePDF handle the chromedriver downloads automatically.
-        ```
-        python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/file.html path/to/output.pdf
-        ```
-        The command will have a return code of zero on success, and nonzero on failure.
-        
-        ## Django Settings
-        
-        You can specify default settings in your Django settings file, if desired, via a `CHROMEPDF` settings. Anything passed via the `pdf_kwargs` argument will override the `PDF_KWARGS` settings.
-        ```python
-        # settings.__init__.py
-        
-        CHROMEPDF = {
-            'CHROME_PATH': r'C:\Program Files (x86)\Google\...\chrome.exe',
-            'CHROME_ARGS': [], # Optional list of command-line argument strings to pass to Chrome when rendering a PDF.
-            'CHROMEDRIVER_PATH': None, # will rely on downloads instead
-            'CHROMEDRIVER_DOWNLOADS': True, # automatically download the correct chromedriver for the chrome path
-            'PDF_KWARGS': {
-                'paperFormat': 'A4',
-                'marginTop': '2.5cm',
-                'marginLeft': '2cm',
-                'marginRight': '2cm',
-                'marginBottom': '3.5cm',
-            }
-        }
-        ```
-        
-        
-        ## PDF_KWARGS Options
-        
-        The `pdf_kwargs` argument to `generate_pdf()` lets you specify all the arguments for Chrome's `Page.printToPDF` API. Its API can be viewed here:
-        
-        [Page.printToPDF API](https://chromedevtools.github.io/devtools-protocol/1-3/Page/#method-printToPDF) (url is funky. If you get a 404, try reloading/refreshing)
-        
-        Some shortcut parameters are provided by `generate_pdf()` for convenience. Here is a list of all the options:
-        
-        Layout:
-        *  **scale**: Scale of the PDF. Default `1`.
-        *  **landscape**: `True` to use landscape mode. Default `False`.
-        
-        Page Dimensions:
-        *  **paperWidth**: Width of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `8.5`
-        *  **paperHeight**: Height of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `11`
-        *  **paperFormat**: A string indicating a paper size format, such as `'letter'` or `'A4'`. Case-insensitive. This will override `paperWidth` and `paperHeight`. Not part of `Page.printToPDF` API.  Provided for convenience.
-        
-        Content:
-        *  **displayHeaderFooter**: `True` to display header and footer. Default `False`.
-        *  **headerTemplate**: HTML containing the header for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values. For example, `<span class='title'></span>` would insert the the title.
-           * date: formatted print date 
-           * title: document title 
-           * url: document location 
-           * pageNumber: current page number 
-           * totalPages: total pages in the document 
-        * **footerTemplate**: HTML containing the footer for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values (same as above)
-        * **printBackground**: `True` to print background graphics. Default `False`.
-        
-        Margins:
-        *  **margin**: Shortcut used to set all four margin values at once. Not part of `Page.printToPDF` API.  Provided for convenience.
-        *  **marginTop**: Top margin. Default: `'1cm'`
-        *  **marginBottom**: Bottom margin. Default: `'1cm'`
-        *  **marginLeft**: Left margin. Default: `'1cm'`
-        *  **marginRight**: Right margin. Default: `'1cm'`
-        
-        Page Ranges:
-        *  **pageRanges**: String indicating page ranges to use. Example: `'1-5, 8, 11-13'`
-        *  **ignoreInvalidPageRanges**: If `True`, will silently ignore invalid 'pageRanges' values. Default `False`.
-        
-        
-Platform: UNKNOWN
+Project-URL: homepage, https://github.com/imsweb/django-chromepdf
+Project-URL: repository, https://github.com/imsweb/django-chromepdf
+Project-URL: changelog, https://github.com/imsweb/django-chromepdf/blob/master/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: OS Independent
@@ -191,7 +22,176 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ChromePDF
+
+## Overview
+
+ChromePDF is a small Python 3 library that uses [Selenium](https://pypi.org/project/selenium/) and Google Chrome to convert HTML into a PDF. This is accomplished by using Chrome's `Page.printToPDF` DevTools command.
+
+ChromePDF provides a function that accepts an html string, plus a dict of page parameters, and other settings, and returns the bytes containing a PDF:
+
+```
+pdf_bytes = generate_pdf(html_string, pdf_kwargs, **kwargs)
+```
+
+As of version 1.4, ChromePDF can also be run from the command line.
+
+```
+python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/input.html path/to/output.pdf
+```
+
+Because it renders via Chrome, it supports a wide range of CSS and HTML tags that should display the same as if you used Chrome to view the HTML itself.
+
+ChromePDF can take advantage of [Django](https://pypi.org/project/Django/) settings for configuration, but Django is not a required dependency.
+
+Official ChromePDF releases [are available on PyPI](https://pypi.org/project/django-chromepdf/).
+
+## Installation
+
+**1. Install ChromePDF via pip.**
+
+The latest version can be installed via PyPI. This will also install Selenium, the only direct dependency (Selenium versions 3 and 4 are supported; 3 will be used if already present, otherwise will install 4). 
+
+You may view the [Changelog](CHANGELOG.md) for a list of all ChromePDF version changes. ChromePDF uses [semantic versioning](https://semver.org/) for its release numbering. You are encouraged to pin your requirements to a Major.Minor version in a manner that will also receive Bugfix updates like so:
+```
+pip install django-chromepdf~=1.7.2
+```
+
+**2. Set the location of your Chrome executable.** This can be done in one of two ways:
+
+* In your Django settings, set `CHROMEPDF['CHROME_PATH']` to the full path of the executable (E.G., `r'C:\Program Files (x86)\Google\...\chrome.exe'`)
+* OR, pass `chrome_path` as a keyword argument to the `generate_pdf()` function.
+
+## About Chromedrivers
+
+A chromedriver executable is necessary to interface between Selenium and Chrome. ChromePDF will automatically check the version of your Chrome binary and download the required chromedriver [from the Chrome website](https://chromedriver.chromium.org/downloads) if it doesn't exist, into your `site-packages/chromepdf/chromedrivers/` folder. If the Chrome binary ever gets upgraded, ChromePDF will realize this and download the required driver for it.
+
+You may disable these automatic downloads in the following way:
+* In your Django settings, set `CHROMEPDF['CHROMEDRIVER_DOWNLOADS']` to False
+* OR, pass a `chromedriver_downloads=False` argument to `generate_pdf()`
+
+You may also specify a chromedriver path manually. This is recommended if you disable downloads:
+* In your Django settings, set `CHROMEPDF['CHROMEDRIVER_PATH']` to the full path of the executable (E.G., `r'C:\Users\myuser\...\chromedriver_win32\chromedriver.exe'`)
+* OR, pass a `chromedriver_path` argument to `generate_pdf()` containing the path.
+* OR, if both of the above are not set, and you've disabled downloads, and if your chromedriver is in your `PATH` environment variable, then Selenium should be able to find it automatically.
+
+## Example: `generate_pdf()`
+Note: `generate_pdf()` cannot include external files including CSS. You must include all your CSS within `<style>` tags or as inline styles.
+
+```python
+# NOTE: This example assumes that you've set Django's settings.CHROMEPDF['CHROME_PATH'] = '(path to your Chrome instance)'
+from chromepdf import generate_pdf 
+
+with open('myfile.html','r') as f:
+    html_string = f.read()
+             
+pdf_kwargs = {
+    'paperFormat': 'A4',
+    'marginTop': '2.5cm',
+    'marginLeft': '2cm',
+    'marginRight': '2cm',
+    'marginBottom': '3.5cm',
+    'displayHeaderFooter': True,
+    'headerTemplate': '',
+    'footerTemplate': '''
+        <div style='font-size: 12px; width: 100%; padding: 0; padding-left: 2cm; padding-bottom: 1cm; margin: 0; '>
+            Page <span class='pageNumber'></span> of <span class='totalPages'></span>
+        </div>
+    ''',
+}
+pdf_bytes = generate_pdf(html_string, pdf_kwargs)
+
+with open('myfile.pdf', 'wb') as file:
+    file.write(pdf_bytes)
+```
+
+## Example: Command-Line Usage
+ChromePDF can generate PDFs from the command-line. This method will not rely on Django settings. Example syntax:
+```
+# Convert file.html into file.pdf and place in the same directory
+python -m chromepdf generate-pdf path/to/file.html [kwargs]
+
+# Convert file.html and place the output PDF file at a specific path.
+python -m chromepdf generate-pdf path/to/file.html path/to/output.pdf [kwargs]
+```
+Keyword arguments for command-line usage are almost identical to `generate_pdf()` keyword arguments:
+```
+--chrome-path=path/to/google-chrome
+--chromedriver-path=path/to/chromedriver
+--chromedriver-downloads=0 # 0 or 1
+--chrome-args="--arg1 --arg2" # Always use quotes to avoid misinterpreting as commands. 
+--pdf-kwargs-json=path/to/file.json # JSON file containing a dict of values to pass to pdf_kwargs
+```
+The recommended usage is to pass a `--chrome-path`, and let ChromePDF handle the chromedriver downloads automatically.
+```
+python -m chromepdf generate-pdf --chrome-path=/usr/bin/google-chrome path/to/file.html path/to/output.pdf
+```
+The command will have a return code of zero on success, and nonzero on failure.
+
+## Django Settings
+
+You can specify default settings in your Django settings file, if desired, via a `CHROMEPDF` settings. Anything passed via the `pdf_kwargs` argument will override the `PDF_KWARGS` settings.
+```python
+# settings.__init__.py
+
+CHROMEPDF = {
+    'CHROME_PATH': r'C:\Program Files (x86)\Google\...\chrome.exe',
+    'CHROME_ARGS': [], # Optional list of command-line argument strings to pass to Chrome when rendering a PDF.
+    'CHROMEDRIVER_PATH': None, # will rely on downloads instead
+    'CHROMEDRIVER_DOWNLOADS': True, # automatically download the correct chromedriver for the chrome path
+    'PDF_KWARGS': {
+        'paperFormat': 'A4',
+        'marginTop': '2.5cm',
+        'marginLeft': '2cm',
+        'marginRight': '2cm',
+        'marginBottom': '3.5cm',
+    }
+}
+```
+
+
+## PDF_KWARGS Options
+
+The `pdf_kwargs` argument to `generate_pdf()` lets you specify all the arguments for Chrome's `Page.printToPDF` API. Its API can be viewed here:
+
+[Page.printToPDF API](https://chromedevtools.github.io/devtools-protocol/1-3/Page/#method-printToPDF) (url is funky. If you get a 404, try reloading/refreshing)
+
+Some shortcut parameters are provided by `generate_pdf()` for convenience. Here is a list of all the options:
+
+Layout:
+*  **scale**: Scale of the PDF. Default `1`.
+*  **landscape**: `True` to use landscape mode. Default `False`.
+
+Page Dimensions:
+*  **paperWidth**: Width of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `8.5`
+*  **paperHeight**: Height of the paper, in inches. Can also use some CSS string values, like `'30cm'`. Default: `11`
+*  **paperFormat**: A string indicating a paper size format, such as `'letter'` or `'A4'`. Case-insensitive. This will override `paperWidth` and `paperHeight`. Not part of `Page.printToPDF` API.  Provided for convenience.
+
+Content:
+*  **displayHeaderFooter**: `True` to display header and footer. Default `False`.
+*  **headerTemplate**: HTML containing the header for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values. For example, `<span class='title'></span>` would insert the the title.
+   * date: formatted print date 
+   * title: document title 
+   * url: document location 
+   * pageNumber: current page number 
+   * totalPages: total pages in the document 
+* **footerTemplate**: HTML containing the footer for all pages. Default is an empty string. You may pass html tags with specific classes in order to insert values (same as above)
+* **printBackground**: `True` to print background graphics. Default `False`.
+
+Margins:
+*  **margin**: Shortcut used to set all four margin values at once. Not part of `Page.printToPDF` API.  Provided for convenience.
+*  **marginTop**: Top margin. Default: `'1cm'`
+*  **marginBottom**: Bottom margin. Default: `'1cm'`
+*  **marginLeft**: Left margin. Default: `'1cm'`
+*  **marginRight**: Right margin. Default: `'1cm'`
+
+Page Ranges:
+*  **pageRanges**: String indicating page ranges to use. Example: `'1-5, 8, 11-13'`
+*  **ignoreInvalidPageRanges**: If `True`, will silently ignore invalid 'pageRanges' values. Default `False`.
+
```

