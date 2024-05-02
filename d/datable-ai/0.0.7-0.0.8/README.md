# Comparing `tmp/datable_ai-0.0.7.tar.gz` & `tmp/datable_ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.7.tar", max compression
+gzip compressed data, was "datable_ai-0.0.8.tar", max compression
```

## Comparing `datable_ai-0.0.7.tar` & `datable_ai-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-04-30 04:31:28.554459 datable_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0       24 2024-04-30 04:31:28.554459 datable_ai-0.0.7/README.md
--rw-r--r--   0        0        0      137 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/core/llm.py
--rw-r--r--   0        0        0     4017 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/output.py
--rw-r--r--   0        0        0     1736 2024-04-30 04:31:28.554459 datable_ai-0.0.7/datable_ai/structured_output.py
--rw-r--r--   0        0        0      506 2024-04-30 04:31:28.554459 datable_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 datable_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-01 08:28:04.000079 datable_ai-0.0.8/LICENSE
+-rw-r--r--   0        0        0      426 2024-05-01 08:28:04.000079 datable_ai-0.0.8/README.md
+-rw-r--r--   0        0        0      175 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     3643 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/core/llm.py
+-rw-r--r--   0        0        0      169 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/helper.py
+-rw-r--r--   0        0        0     3131 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/ocr.py
+-rw-r--r--   0        0        0     5680 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/output.py
+-rw-r--r--   0        0        0     2526 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/structured_output.py
+-rw-r--r--   0        0        0      665 2024-05-01 08:28:04.004079 datable_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 datable_ai-0.0.8/PKG-INFO
```

### Comparing `datable_ai-0.0.7/LICENSE` & `datable_ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.7/datable_ai/output.py` & `datable_ai-0.0.8/datable_ai/output.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,27 +7,47 @@
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_text_splitters import CharacterTextSplitter
 
 from datable_ai.core.llm import LLM_TYPE, create_llm
 
 
 class Output:
+    """
+    A class for generating output using a language model.
+
+    Args:
+        llm_type (LLM_TYPE): The type of language model to use.
+        prompt_template (str): The prompt template to use for generating output.
+    """
+
     def __init__(
         self,
         llm_type: LLM_TYPE,
         prompt_template: str,
     ) -> None:
         self.llm_type = llm_type
         self.prompt_template = prompt_template
         self.prompt = ChatPromptTemplate.from_template(self.prompt_template)
         self.llm = create_llm(self.llm_type)
         self.encoding_name = self._encoding_name()
         self.max_tokens = self._max_tokens(self.encoding_name)
 
     def invoke(self, **kwargs):
+        """
+        Generates output using the language model.
+
+        Args:
+            **kwargs: Keyword arguments to pass to the prompt template.
+
+        Returns:
+            The generated output.
+
+        Raises:
+            RuntimeError: If an error occurs while generating output.
+        """
         try:
             summarized_kwargs = {}
             for key, value in kwargs.items():
                 num_tokens = self._num_tokens_from_string(value)
                 if num_tokens > self.max_tokens:
                     summarized_value = self._summarize(value)
                     summarized_kwargs[key] = summarized_value["output_text"]
@@ -36,14 +56,26 @@
 
             chain = self.prompt | self.llm | StrOutputParser()
             return chain.invoke(summarized_kwargs)
         except Exception as e:
             raise RuntimeError(f"Error invoking Output: {str(e)}") from e
 
     def _num_tokens_from_string(self, text: str) -> int:
+        """
+        Calculates the number of tokens in a string.
+
+        Args:
+            text (str): The string to calculate the number of tokens for.
+
+        Returns:
+            The number of tokens in the string.
+
+        Raises:
+            RuntimeError: If an error occurs while calculating the number of tokens.
+        """
         try:
             if (
                 self.llm_type == LLM_TYPE.OPENAI
                 or self.llm_type == LLM_TYPE.AZURE_OPENAI
             ):
                 encoding = tiktoken.encoding_for_model(self.encoding_name)
             elif self.llm_type == LLM_TYPE.ANTHROPIC:
@@ -52,37 +84,67 @@
                 encoding = tiktoken.get_encoding("gpt2")
             num_tokens = len(encoding.encode(text))
             return num_tokens
         except Exception as e:
             raise RuntimeError(f"Error calculating number of tokens: {str(e)}") from e
 
     def _summarize(self, long_text: str):
+        """
+        Summarizes a long text into a shorter text.
+
+        Args:
+            long_text (str): The long text to summarize.
+
+        Returns:
+            A dictionary containing the summarized text.
+
+        Raises:
+            RuntimeError: If an error occurs while summarizing the text.
+        """
         try:
             text_splitter = CharacterTextSplitter.from_tiktoken_encoder(
                 chunk_size=1000, chunk_overlap=50
             )
             split_docs = text_splitter.split_text(long_text)
             docs = [Document(page_content=chunk) for chunk in split_docs]
             return load_summarize_chain(
                 self.llm, chain_type="map_reduce", verbose=False
             ).invoke(docs)
         except Exception as e:
             raise RuntimeError(f"Error summarizing text: {str(e)}") from e
 
     def _encoding_name(self):
+        """
+        Returns the encoding name for the language model.
+
+        Returns:
+            The encoding name for the language model.
+
+        Raises:
+            ValueError: If the language model type is unsupported.
+        """
         if self.llm_type == LLM_TYPE.OPENAI:
             return os.environ.get("OPENAI_API_MODEL")
         elif self.llm_type == LLM_TYPE.AZURE_OPENAI:
             return os.environ.get("AZURE_OPENAI_API_MODEL")
         elif self.llm_type == LLM_TYPE.ANTHROPIC:
             return os.environ.get("ANTHROPIC_API_MODEL")
         else:
             raise ValueError(f"Unsupported LLM type: {self.llm_type}")
 
     def _max_tokens(self, model_name: str):
+        """
+        Returns the maximum number of tokens for the specified model.
+
+        Args:
+            model_name (str): The name of the model.
+
+        Returns:
+            The maximum number of tokens for the specified model.
+        """
         model_configs = {
             "openai": {
                 "gpt-4": {"max_tokens": 8000},
                 "gpt-4-32k": {"max_tokens": 32000},
                 "gpt-4-turbo": {"max_tokens": 128000},
                 "gpt-4-turbo-2024-04-09": {},
                 "gpt-4-turbo-preview": {},
```

