# Comparing `tmp/vbimagetotext-0.1.2.tar.gz` & `tmp/vbimagetotext-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbimagetotext-0.1.2.tar", max compression
+gzip compressed data, was "vbimagetotext-0.1.3.tar", max compression
```

## Comparing `vbimagetotext-0.1.2.tar` & `vbimagetotext-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.2/README.md
--rw-r--r--   0        0        0      588 2024-04-26 07:27:24.529673 vbimagetotext-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.2/vbimagetotext/__init__.py
--rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.2/vbimagetotext/__main__.py
--rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.2/vbimagetotext/choice_option.py
--rw-r--r--   0        0        0     3388 2024-04-26 07:17:08.395521 vbimagetotext-0.1.2/vbimagetotext/functions.py
--rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.2/vbimagetotext/geminivision.py
--rw-r--r--   0        0        0     1611 2024-04-18 21:36:33.615000 vbimagetotext-0.1.2/vbimagetotext/gptvision.py
--rw-r--r--   0        0        0      306 2024-04-16 09:07:05.481819 vbimagetotext-0.1.2/vbimagetotext/main.py
--rw-r--r--   0        0        0     7791 2024-04-21 17:36:53.778457 vbimagetotext-0.1.2/vbimagetotext/prompts.py
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717635 vbimagetotext-0.1.3/README.md
+-rw-r--r--   0        0        0      588 2024-05-01 23:24:54.436536 vbimagetotext-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:36:05.717586 vbimagetotext-0.1.3/vbimagetotext/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-16 08:45:08.023791 vbimagetotext-0.1.3/vbimagetotext/__main__.py
+-rw-r--r--   0        0        0     1236 2024-04-16 08:47:47.097235 vbimagetotext-0.1.3/vbimagetotext/choice_option.py
+-rw-r--r--   0        0        0     1518 2024-05-01 23:15:21.290644 vbimagetotext-0.1.3/vbimagetotext/copyprompt.py
+-rw-r--r--   0        0        0     5109 2024-05-01 23:24:09.689153 vbimagetotext-0.1.3/vbimagetotext/functions.py
+-rw-r--r--   0        0        0     2776 2024-04-26 07:27:12.309253 vbimagetotext-0.1.3/vbimagetotext/geminivision.py
+-rw-r--r--   0        0        0     1611 2024-05-01 23:17:13.262619 vbimagetotext-0.1.3/vbimagetotext/gptvision.py
+-rw-r--r--   0        0        0      428 2024-05-01 23:23:16.539392 vbimagetotext-0.1.3/vbimagetotext/main.py
+-rw-r--r--   0        0        0     8960 2024-05-01 23:12:16.544558 vbimagetotext-0.1.3/vbimagetotext/prompts.py
+-rw-r--r--   0        0        0      937 2024-05-01 23:24:41.008639 vbimagetotext-0.1.3/vbimagetotext/solution.py
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 vbimagetotext-0.1.3/PKG-INFO
```

### Comparing `vbimagetotext-0.1.2/pyproject.toml` & `vbimagetotext-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vbimagetotext"
-version = "0.1.2"
+version = "0.1.3"
 description = "A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API"
 authors = ["vaibhavblayer <vaibhavblayer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 click = "^8.1.7"
```

### Comparing `vbimagetotext-0.1.2/vbimagetotext/choice_option.py` & `vbimagetotext-0.1.3/vbimagetotext/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.2/vbimagetotext/geminivision.py` & `vbimagetotext-0.1.3/vbimagetotext/geminivision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.2/vbimagetotext/gptvision.py` & `vbimagetotext-0.1.3/vbimagetotext/gptvision.py`

 * *Files identical despite different names*

### Comparing `vbimagetotext-0.1.2/vbimagetotext/prompts.py` & `vbimagetotext-0.1.3/vbimagetotext/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from rich.console import Console
-
 
 prompt_assertion_reason = """
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any assertion-reason type questions, use this code as reference
 \begin{enumerate}
     \item[1. Assertion:] This is an assertion.
     \item[Reason:] This is a reason.
 \end{enumerate}
@@ -13,48 +11,48 @@
 
 prompt_mcq = """
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment.
 Use this code as reference for multiple-choice questions
 \begin{enumerate}
     \item This is a question.
         \begin{tasks}(2)
-            \task Option 1
-            \task Option 2
-            \task Option 3\ans
-            \task Option 4
+            \task Shorter Option 1
+            \task Shorter Option 2
+            \task Shorter Option 3\ans
+            \task Shorter Option 4
         \end{tasks}
     \item This is another question.
-        \begin{tasks}(2)
-            \task Option 1
-            \task Option 2
-            \task Option 3
-            \task Option 4\ans
+        \begin{tasks}(1)
+            \task Longer Option 1
+            \task Longer Option 2
+            \task Longer Option 3
+            \task Longer Option 4\ans
         \end{tasks}
 \end{enumerate}
 
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 prompt_mcq_solution = """
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, in the center environment. If there are any multiple-choice questions, please put the options in a tasks environment.
 Use this code as reference for multiple-choice questions
 \begin{enumerate}
     \item This is a question.
         \begin{tasks}(2)
-            \task Option 1
-            \task Option 2
-            \task Option 3\ans
-            \task Option 4
+            \task Shorter Option 1
+            \task Shorter Option 2
+            \task Shorter Option 3\ans
+            \task Shorter Option 4
         \end{tasks}
     \item This is another question.
-        \begin{tasks}(2)
-            \task Option 1
-            \task Option 2
-            \task Option 3
-            \task Option 4\ans
+        \begin{tasks}(1)
+            \task Longer Option 1
+            \task Longer Option 2
+            \task Longer Option 3
+            \task Longer Option 4\ans
         \end{tasks}
 \end{enumerate}
 Also if possible solve the problem and provide the solution in LaTeX format as well. Just below each question, use this code as reference for solutions
 \begin{solution}
     \begin{align*}
         \intertext{Momentum of the ball will change only along the normal($x$ direction).}
         \vec{J} &= \vec{p}_f-\vec{p}_i\\
@@ -69,15 +67,15 @@
 
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
 prompt_subjective = """
 Extract Questions from Image and Format in LaTeX
-Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, put it within the center environment. Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
+Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only, put it within the center environment. For horizontal line use \underline{\hspace{2.5 cm}}. Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 prompt_match = """
 Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present, please create only the TikZ environment with a node "Diagram" only. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any match-type or list type questions, please create a table use this code as reference 
 \begin{center}
     \renewcommand{\arraystretch}{2}
     \begin{table}[h]
@@ -95,15 +93,15 @@
     \end{table}
 \end{center}
 Please provide only the enumerated part of the LaTeX file, not the whole LaTeX file.
 """
 
 
 prompt_comprehension = """
-Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present in any type of question, please create only the TikZ environment with a node "Diagram" only in center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any comprehension type or Question Stem type questions, use this code as reference  
+Please analyze the image provided and extract any questions present in the text. Format the questions in LaTeX format. If there are any diagrams present in any type of question, please create only the TikZ environment with a node "Diagram" only in center environment. If there are any multiple-choice questions, please put the options in a tasks environment. If there are any comprehension type/Paragraph type/Passage type/Question Stem type questions, use this code as reference  
 \begin{center}
     \textsc{Comprehension-II}
 \end{center}
 A uniform wire frame of linear mass density $\lambda$ having three sides each of length $2a$ is kept on a smooth horizontal surface. An impulse $J$ is applied at one end as shown in the figure. $P$ is the midpoint of $AB$. Now answer the following questions. 
 \begin{center}
     \begin{tikzpicture}
         \pic[rotate=180] at (0, 0) {frame=3cm};
@@ -130,14 +128,33 @@
 """
 
 
 prompt_answer = """
 Please analyze the image provided and extract the answers exercisewise in latex format. If possible use enumerate environment for answers. Give me only the document part of the LaTeX file, so that i can include it as a separate file into other document not the whole LaTeX file.
 """
 
+prompt_solution = """
+Following problem in in latex format, Please analyze the following question and if possible solve the problem and provide the solution in LaTeX format as well. Use this code as reference for solution
+\begin{solution}
+    \begin{align*}
+        \intertext{Momentum of the ball will change only along the normal($x$ direction).}
+        \vec{J} &= \vec{p}_f-\vec{p}_i\\
+        &= m\vec{v}_f-m\vec{v}_i\\
+        &= m\left(\dfrac{3}{4}v_0\hat{i}\right)-m\left(v_0\hat{i}\right)\\
+        &= -\dfrac{1}{4}mv_0\hat{i}\\
+        &= -\dfrac{5}{4}mv_0\hat{i}
+        \interttext{Option (a) is correct.}
+    \end{align*}
+\end{solution}
+
+Try not to use any derived formula if possible, go with fundamentals and basics. Also if possible use align* environment for solutions. You can add descriptive text in between using \intertext{} command.
+
+Please provide only the solution part of the LaTeX file, not the whole LaTeX file.
+"""
+
 
 def switch_prompt(value):
     if value == "match":
         return prompt_match
     elif value == "mcq":
         return prompt_mcq
     elif value == "mcq_solution":
@@ -146,9 +163,11 @@
         return prompt_subjective
     elif value == "comprension":
         return prompt_comprehension
     elif value == "assertion_reason":
         return prompt_assertion_reason
     elif value == "answer":
         return prompt_answer
+    elif value == "solution":
+        return prompt_solution
     else:
         return value
```

### Comparing `vbimagetotext-0.1.2/PKG-INFO` & `vbimagetotext-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vbimagetotext
-Version: 0.1.2
+Version: 0.1.3
 Summary: A cli tool to convert image to text using openai's GPT-Vision API and google's Gemini Vision API
 Author: vaibhavblayer
 Author-email: vaibhavblayer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
```

