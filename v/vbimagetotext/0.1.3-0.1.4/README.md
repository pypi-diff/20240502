# Comparing `tmp/vbimagetotext-0.1.3.tar.gz` & `tmp/vbimagetotext-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.3.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.4.tar", max compression
```

## Comparing `vbimagetotext-0.1.3.tar` & `vbimagetotext-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.3/README.md
--rw-r--r--   0        0        0      588 2024-05-01 23:24:54.436536 vbimagetotext-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.3/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.3/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.3/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.3/vbimagetotext/copyprompt.py
--rw-r--r--   0        0        0     5109 2024-05-01 23:24:09.689153 vbimagetotext-0.1.3/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.3/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1611 2024-05-01 23:17:13.262619 vbimagetotext-0.1.3/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.3/vbimagetotext/main.py
--rw-r--r--   0        0        0     8960 2024-05-01 23:12:16.544558 vbimagetotext-0.1.3/vbimagetotext/prompts.py
--rw-r--r--   0        0        0      937 2024-05-01 23:24:41.008639 vbimagetotext-0.1.3/vbimagetotext/solution.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.4/README.md
+-rw-r--r--   0        0        0      588 2024-05-01 23:27:10.066746 vbimagetotext-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.4/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.4/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.4/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.4/vbimagetotext/copyprompt.py
+-rw-r--r--   0        0        0     5109 2024-05-01 23:24:09.689153 vbimagetotext-0.1.4/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.4/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1611 2024-05-01 23:17:13.262619 vbimagetotext-0.1.4/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.4/vbimagetotext/main.py
+-rw-r--r--   0        0        0     8967 2024-05-01 23:27:03.556561 vbimagetotext-0.1.4/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0      937 2024-05-01 23:24:41.008639 vbimagetotext-0.1.4/vbimagetotext/solution.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.4/PKG-INFO
```

### Comparing `vbimagetotext-0.1.3/pyproject.toml` & `vbimagetotext-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.3"
+version = "0.1.4"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.3/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.4/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/vbimagetotext/copyprompt.py` & `vbimagetotext-0.1.4/vbimagetotext/copyprompt.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/vbimagetotext/functions.py` & `vbimagetotext-0.1.4/vbimagetotext/functions.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.4/vbimagetotext/geminivision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.4/vbimagetotext/gptvision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/vbimagetotext/prompts.py` & `vbimagetotext-0.1.4/vbimagetotext/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
-prompt_assertion_reason = """
+prompt_assertion_reason = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any assertion-reason type questions, use this code as reference
 \begin{enumerate}
     \item[1. Assertion:] This is an assertion.
     \item[Reason:] This is a reason.
 \end{enumerate}
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
-prompt_mcq = """
+prompt_mcq = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment.
 Use this code as reference for multiple-choice questions
 \begin{enumerate}
     \item This is a question.
         \begin{tasks}(2)
             \task Shorter Option 1
             \task Shorter Option 2
@@ -28,15 +28,15 @@
             \task Longer Option 4\ans
         \end{tasks}
 \end{enumerate}
 
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
-prompt_mcq_solution = """
+prompt_mcq_solution = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment.
 Use this code as reference for multiple-choice questions
 \begin{enumerate}
     \item This is a question.
         \begin{tasks}(2)
             \task Shorter Option 1
             \task Shorter Option 2
@@ -65,20 +65,20 @@
 Try not to use any derived formula if possible, go with fundamentals and basics. Also if possible use align* environment for solutions. You can add descriptive text in between using \intertext{} command. Solve every question and provide the solution as well. Don't separate the question and solution. Solution should be just below the question.
 Try to use the \ans command at the end of the correct option, but check the answer for sure before marking. 
 
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
-prompt_subjective = """
+prompt_subjective = r"""
 Extract Questions from Image and Format in LaTeX
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, put it within the center environment. For horizontal line use \underline{\hspace{2.5 cm}}. Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
-prompt_match = """
+prompt_match = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any match-type or list type questions, please create a table use this code as reference 
 \begin{center}
     \renewcommand{\arraystretch}{2}
     \begin{table}[h]
         \centering
         \begin{tabular}{p{0.25cm}p{8cm}|p{0.25cm}p{5cm}}
         \hline
@@ -92,15 +92,15 @@
         \end{tabular}
     \end{table}
 \end{center}
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
-prompt_comprehension = """
+prompt_comprehension = r"""
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present in any type of question, please create only the TikZ environment with a node "Diagram" only in center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any comprehension type/Paragraph type/Passage type/Question Stem type questions, use this code as reference  
 \begin{center}
     \textsc{Comprehension-II}
 \end{center}
 A uniform wire frame of linear mass density $\lambda$ having three sides each of length $2a$ is kept on a smooth horizontal surface. An impulse $J$ is applied at one end as shown in the figure. $P$ is the midpoint of $AB$. Now answer the following questions. 
 \begin{center}
     \begin{tikzpicture}
@@ -128,15 +128,15 @@
 """
 
 
 prompt_answer = """
 Please analyze the image provided and extract the answers exercisewise in latex format. If possible use enumerate environment for answers. Give me only the document part of the LaTeX file, so that i can include it as a separate file into other document not the whole LaTeX file.
 """
 
-prompt_solution = """
+prompt_solution = r"""
 Following problem in in latex format, Please analyze the following question and if possible solve the problem and provide the solution in LaTeX format as well. Use this code as reference for solution
 \begin{solution}
     \begin{align*}
         \intertext{Momentum of the ball will change only along the normal($x$ direction).}
         \vec{J} &= \vec{p}_f-\vec{p}_i\\
         &= m\vec{v}_f-m\vec{v}_i\\
         &= m\left(\dfrac{3}{4}v_0\hat{i}\right)-m\left(v_0\hat{i}\right)\\
```

### Comparing `vbimagetotext-0.1.3/vbimagetotext/solution.py` & `vbimagetotext-0.1.4/vbimagetotext/solution.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.3/PKG-INFO` & `vbimagetotext-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.3
+Version: 0.1.4
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

