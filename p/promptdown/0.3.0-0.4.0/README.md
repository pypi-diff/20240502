# Comparing `tmp/promptdown-0.3.0.tar.gz` & `tmp/promptdown-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptdown-0.3.0.tar", last modified: Mon Apr 29 01:55:25 2024, max compression
+gzip compressed data, was "promptdown-0.4.0.tar", last modified: Thu May  2 03:25:33 2024, max compression
```

## Comparing `promptdown-0.3.0.tar` & `promptdown-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-29 01:55:14.881076 promptdown-0.3.0/LICENSE
--rw-r--r--   0        0        0     3223 2024-04-29 01:55:14.881076 promptdown-0.3.0/README.md
--rw-r--r--   0        0        0     1074 2024-04-29 01:55:25.985123 promptdown-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-29 01:55:14.881076 promptdown-0.3.0/src/promptdown/__init__.py
--rw-r--r--   0        0        0      124 2024-04-29 01:55:24.577118 promptdown-0.3.0/src/promptdown/__init__.pyi
--rw-r--r--   0        0        0     7357 2024-04-29 01:55:14.881076 promptdown-0.3.0/src/promptdown/promptdown.py
--rw-r--r--   0        0        0      870 2024-04-29 01:55:24.577118 promptdown-0.3.0/src/promptdown/promptdown.pyi
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 promptdown-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-02 03:25:22.183912 promptdown-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4961 2024-05-02 03:25:22.183912 promptdown-0.4.0/README.md
+-rw-r--r--   0        0        0     1074 2024-05-02 03:25:33.131856 promptdown-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-05-02 03:25:22.183912 promptdown-0.4.0/src/promptdown/__init__.py
+-rw-r--r--   0        0        0      124 2024-05-02 03:25:31.899862 promptdown-0.4.0/src/promptdown/__init__.pyi
+-rw-r--r--   0        0        0    10874 2024-05-02 03:25:22.183912 promptdown-0.4.0/src/promptdown/promptdown.py
+-rw-r--r--   0        0        0      993 2024-05-02 03:25:31.899862 promptdown-0.4.0/src/promptdown/promptdown.pyi
+-rw-r--r--   0        0        0     5768 1970-01-01 00:00:00.000000 promptdown-0.4.0/PKG-INFO
```

### Comparing `promptdown-0.3.0/LICENSE` & `promptdown-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptdown-0.3.0/pyproject.toml` & `promptdown-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptdown"
-version = "0.3.0"
+version = "0.4.0"
 description = "A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts"
 authors = [
     { name = "B.T. Franklin", email = "brandon.franklin@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
```

### Comparing `promptdown-0.3.0/src/promptdown/promptdown.py` & `promptdown-0.4.0/src/promptdown/promptdown.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 from __future__ import annotations
 import logging
 from dataclasses import dataclass
-import importlib.resources as pkg_resources
+from importlib import resources
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = None
 
+    def __post_init__(self):
+        """
+        Validate the role to ensure that it does not use the reserved role "System".
+        Raises:
+            ValueError: If the role is set to "System", which is reserved.
+        """
+        if self.role.lower() == "system":
+            raise ValueError(
+                "The role 'System' is reserved and cannot be used for conversation messages."
+            )
+
     def __eq__(self, other: object) -> bool:
+        """
+        Check equality between two Message instances based on role, content, and name.
+
+        Args:
+            other (object): The other object to compare with.
+
+        Returns:
+            bool: True if both objects are Messages and have the same role, content, and name; False otherwise.
+        """
         if isinstance(other, Message):
             return (
                 self.role.lower() == other.role.lower()
                 and self.content == other.content
                 and self.name == other.name
             )
         return False
@@ -25,24 +45,42 @@
 @dataclass
 class StructuredPrompt:
     name: str
     system_message: str
     conversation: list[Message]
 
     def __eq__(self, other: object) -> bool:
+        """
+        Check equality between two StructuredPrompt instances based on name, system_message, and conversation.
+
+        Args:
+            other (object): The other object to compare with.
+
+        Returns:
+            bool: True if both are StructuredPrompts with the same name, system_message, and conversation; False otherwise.
+        """
         if isinstance(other, StructuredPrompt):
             return (
                 self.name == other.name
                 and self.system_message == other.system_message
                 and self.conversation == other.conversation
             )
         return False
 
     @classmethod
     def _parse_conversation(cls, lines: list[str]) -> list[Message]:
+        """
+        Parse the conversation part of a promptdown string into a list of Message objects.
+
+        Args:
+            lines (list[str]): The lines of the conversation section from a promptdown string.
+
+        Returns:
+            list[Message]: A list of Message instances parsed from the given lines.
+        """
         conversation: list[Message] = []
         headers: list[str] = []
 
         # Iterate over each line in the input lines
         for line in lines:
             # Check if the line starts with "|", indicating a conversation row
             if line.startswith("|"):
@@ -76,14 +114,26 @@
                     )
 
         # Return the parsed conversation list
         return conversation
 
     @classmethod
     def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt:
+        """
+        Parse a structured prompt from a raw promptdown string.
+
+        Args:
+            promptdown_string (str): The complete promptdown formatted string to parse.
+
+        Returns:
+            StructuredPrompt: A new instance of StructuredPrompt based on the parsed string.
+
+        Raises:
+            ValueError: If the promptdown string does not contain necessary sections.
+        """
         name: str | None = None
         system_message: str | None = None
         conversation: list[Message] = []
         current_section: str | None = None
         conversation_lines: list[str] = []
 
         lines = promptdown_string.split("\n")
@@ -111,21 +161,24 @@
         conversation = cls._parse_conversation(conversation_lines)
 
         return cls(name=name, system_message=system_message, conversation=conversation)
 
     @classmethod
     def from_promptdown_file(cls, file_path: str) -> StructuredPrompt:
         """
-        Load a promptdown file from a filesystem path.
+        Load and parse a StructuredPrompt from a file containing promptdown-formatted text.
 
         Args:
-        file_path: The path to the promptdown file.
+            file_path (str): The file system path to the promptdown file.
 
         Returns:
-        A StructuredPrompt object loaded from the specified file.
+            StructuredPrompt: A new instance of StructuredPrompt based on the content of the file.
+
+        Raises:
+            FileNotFoundError: If the specified file is not found.
         """
         if not file_path.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
         try:
             with open(file_path, "r") as file:
                 promptdown_string = file.read()
@@ -136,36 +189,46 @@
         return cls.from_promptdown_string(promptdown_string)
 
     @classmethod
     def from_package_resource(
         cls, package: str, resource_name: str
     ) -> StructuredPrompt:
         """
-        Load a promptdown file as a structured prompt from a package resource.
+        Load and parse a StructuredPrompt from a resource within a package.
 
         Args:
-        package: The package name where the resource is located.
-        resource_name: The name of the promptdown resource file.
+            package (str): The name of the package containing the resource.
+            resource_name (str): The name of the resource file to load.
 
         Returns:
-        A StructuredPrompt object loaded from the specified package resource.
+            StructuredPrompt: A new instance of StructuredPrompt based on the resource content.
+
+        Raises:
+            FileNotFoundError: If the resource is not found within the specified package.
         """
         if not resource_name.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
         try:
-            with pkg_resources.open_text(package, resource_name) as file:
+            resource_path = resources.files(package) / resource_name
+            with resource_path.open("r", encoding="utf-8") as file:
                 promptdown_string = file.read()
         except FileNotFoundError:
             _LOGGER.error(f"File {resource_name} not found in package {package}.")
             raise
 
         return cls.from_promptdown_string(promptdown_string)
 
     def to_promptdown_string(self) -> str:
+        """
+        Serialize the StructuredPrompt into a promptdown-formatted string.
+
+        Returns:
+            str: The serialized promptdown-formatted string of the StructuredPrompt.
+        """
         lines: list[str] = []
 
         # Add the name of the prompt
         lines.append(f"# {self.name}")
         lines.append("")
 
         # Add the system message
@@ -197,14 +260,38 @@
                 lines.append(f"| {role} | {name} | {content} |")
             else:
                 lines.append(f"| {role} | {content} |")
 
         return "\n".join(lines)
 
     def to_promptdown_file(self, file_path: str) -> None:
+        """
+        Write the StructuredPrompt to a file in promptdown format.
 
+        Args:
+            file_path (str): The file system path where the promptdown file will be saved.
+        """
         # Check if the file path ends with ".prompt.md"
         if not file_path.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
         with open(file_path, "w") as file:
             file.write(self.to_promptdown_string())
+
+    def apply_template_values(self, template_values: dict[str, str]) -> None:
+        """
+        Apply template values to the placeholders in the prompt content, replacing them with the specified values.
+
+        Args:
+            template_values (dict[str, str]): A dictionary mapping placeholders (without braces) to their replacement values.
+        """
+        for key, value in template_values.items():
+            placeholder = f"{{{{{key}}}}}"  # Define the placeholder once per key
+
+            # Replace placeholders in the system message
+            if placeholder in self.system_message:
+                self.system_message = self.system_message.replace(placeholder, value)
+
+            # Replace placeholders in each message in the conversation
+            for message in self.conversation:
+                if placeholder in message.content:
+                    message.content = message.content.replace(placeholder, value)
```

### Comparing `promptdown-0.3.0/src/promptdown/promptdown.pyi` & `promptdown-0.4.0/src/promptdown/promptdown.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = ...
+    def __post_init__(self) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __init__(self, role, content, name=...) -> None: ...
 
 @dataclass
 class StructuredPrompt:
     name: str
     system_message: str
@@ -18,8 +19,9 @@
     def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt: ...
     @classmethod
     def from_promptdown_file(cls, file_path: str) -> StructuredPrompt: ...
     @classmethod
     def from_package_resource(cls, package: str, resource_name: str) -> StructuredPrompt: ...
     def to_promptdown_string(self) -> str: ...
     def to_promptdown_file(self, file_path: str) -> None: ...
+    def apply_template_values(self, template_values: dict[str, str]) -> None: ...
     def __init__(self, name, system_message, conversation) -> None: ...
```

### Comparing `promptdown-0.3.0/PKG-INFO` & `promptdown-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: promptdown
-Version: 0.3.0
-Summary: A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts
-Author-Email: "B.T. Franklin" <brandon.franklin@gmail.com>
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: File Formats
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Processing :: Markup :: Markdown
-Project-URL: Homepage, https://github.com/btfranklin/promptdown
-Project-URL: Issues, https://github.com/btfranklin/promptdown/issues
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # Promptdown
 
 Promptdown is a Python package that allows you to express structured prompts for language models in a markdown format. It provides a simple and intuitive way to define and manage prompts, making it easier to work with language models in your projects.
 
 ## Installation
 
 ### Using PDM
@@ -66,19 +48,15 @@
 ```python
 from promptdown import StructuredPrompt
 
 structured_prompt = StructuredPrompt.from_promptdown_file('path/to/your_prompt_file.prompt.md')
 print(structured_prompt)
 ```
 
-### Advanced Usage
-
-Promptdown provides several methods for loading and utilizing structured prompts beyond the basic file usage. Here are more advanced ways to integrate Promptdown into your projects:
-
-#### Parsing a Prompt from a String
+### Parsing a Prompt from a String
 
 For scenarios where you have the prompt data as a string (perhaps dynamically generated or retrieved from an external source), you can parse it directly:
 
 ```python
 from promptdown import StructuredPrompt
 
 promptdown_string = """
@@ -98,28 +76,77 @@
 | Assistant | I'd be happy to help. What seems to be the problem? |
 """
 
 structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
 print(structured_prompt)
 ```
 
-#### Loading Prompts from Package Resources
+### Loading Prompts from Package Resources
 
 For applications where prompts are bundled within Python packages, Promptdown can load prompts directly from these resources. This approach is useful for distributing prompts alongside Python libraries or applications:
 
 ```python
 from promptdown import StructuredPrompt
 
-# Replace 'your_package' with the actual package name and 'your_prompt_file.prompt.md' with the resource file name
 structured_prompt = StructuredPrompt.from_package_resource('your_package', 'your_prompt_file.prompt.md')
 print(structured_prompt)
 ```
 
 This method facilitates easy management of prompts within a package, ensuring that they can be versioned, shared, and reused effectively.
 
+### Using Template Strings
+
+Promptdown supports the use of template strings within your prompts, allowing for dynamic customization of both system messages and conversation content. This feature is particularly useful when you need to tailor prompts based on specific contexts or user data.
+
+#### Defining Template Strings
+
+To incorporate template strings in your Promptdown files, use double curly braces `{{variable}}` around placeholders that you intend to replace dynamically. Here is an example of how to use template strings in a prompt:
+
+```markdown
+# My Prompt
+
+## System Message
+
+You are a helpful assistant in {{topic}}.
+
+## Conversation
+
+| Role      | Content                                         |
+|-----------|-------------------------------------------------|
+| User      | Hi, can you help me with {{topic}}?             |
+| Assistant | Of course! What specifically do you need help with in {{topic}}?|
+| User      | I'm having trouble understanding {{concept}}.  |
+| Assistant | No problem! Let's dive into {{concept}} together. |
+```
+
+#### Applying Template Values
+
+Once you have defined a prompt with placeholders, you can replace these placeholders by passing a dictionary of template values to the `apply_template_values` method. Here's how you can apply template values to your prompt:
+
+```python
+from promptdown import StructuredPrompt
+
+# Load your structured prompt from a file or string that contains template placeholders
+structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
+
+# Define the template values to apply
+template_values = {
+    "topic": "Python programming",
+    "concept": "decorators"
+}
+
+# Apply the template values
+structured_prompt.apply_template_values(template_values)
+
+# Output the updated prompt
+print(structured_prompt)
+```
+
+This will replace `{{topic}}` with "Python programming" and `{{concept}}` with "decorators" in the system message and conversation content. Using template strings in Promptdown allows for more flexible and context-sensitive interactions with language models.
+
 ## Contributing
 
 Contributions are welcome! Feel free to open an issue or submit a pull request.
 
 ## License
 
 Promptdown is released under the [MIT License](LICENSE).
```

