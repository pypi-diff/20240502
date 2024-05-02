# Comparing `tmp/kilter_protocol-0.4.0.tar.gz` & `tmp/kilter_protocol-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kilter_protocol-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "kilter_protocol-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `kilter_protocol-0.4.0.tar` & `kilter_protocol-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    16726 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/LICENCE.txt
--rw-r--r--   0        0        0     4096 2023-07-20 00:11:32.412260 kilter_protocol-0.4.0/README.md
--rw-r--r--   0        0        0      673 2023-07-30 11:01:43.475151 kilter_protocol-0.4.0/kilter/protocol/__init__.py
--rw-r--r--   0        0        0     5161 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/kilter/protocol/buffer.py
--rw-r--r--   0        0        0     9753 2023-07-30 11:01:43.475151 kilter_protocol-0.4.0/kilter/protocol/core.py
--rw-r--r--   0        0        0     1932 2023-07-19 23:48:56.268122 kilter_protocol-0.4.0/kilter/protocol/exceptions.py
--rw-r--r--   0        0        0    21723 2023-07-30 11:01:43.479151 kilter_protocol-0.4.0/kilter/protocol/messages.py
--rw-r--r--   0        0        0        0 2023-07-13 22:46:35.258757 kilter_protocol-0.4.0/kilter/protocol/py.typed
--rw-r--r--   0        0        0     2639 2023-07-30 11:01:43.479151 kilter_protocol-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5164 1970-01-01 00:00:00.000000 kilter_protocol-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/LICENCE.txt
+-rw-r--r--   0        0        0     4397 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/README.md
+-rw-r--r--   0        0        0      673 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/buffer.py
+-rw-r--r--   0        0        0     9753 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/core.py
+-rw-r--r--   0        0        0     1932 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/exceptions.py
+-rw-r--r--   0        0        0    22888 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/messages.py
+-rw-r--r--   0        0        0        0 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/kilter/protocol/py.typed
+-rw-r--r--   0        0        0     2380 2024-05-01 10:24:13.679304 kilter_protocol-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 kilter_protocol-0.5.0/PKG-INFO
```

### Comparing `kilter_protocol-0.4.0/LICENCE.txt` & `kilter_protocol-0.5.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.4.0/README.md` & `kilter_protocol-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+<!--
+# Disable Gitlab link until hosting is more reliable
 [![gitlab-ico]][gitlab-link]
+-->
+[![github-ico]][github-link]
 [![licence-mpl20]](/LICENCE.txt)
 [![pre-commit-ico]][pre-commit-link]
 [![pipeline-status]][pipeline-report]
 [![coverage status]][coverage report]
 
 
 Kilter Protocol
@@ -56,14 +60,22 @@
   https://img.shields.io/badge/GitLab-code.kodo.org.uk-blue.svg?logo=gitlab
   "GitLab"
 
 [gitlab-link]:
   https://code.kodo.org.uk/kilter/kilter.protocol
   "Kilter Protocol at code.kodo.org.uk"
 
+[github-ico]:
+  https://img.shields.io/badge/GitHub-domsekotill/kilter.protocol-blue.svg?logo=github
+  "GitHub"
+
+[github-link]:
+	https://github.com/domsekotill/kilter.protocol
+	"Kilter Protocol at github.com"
+
 [pre-commit-ico]:
   https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
   "Pre-Commit: enabled"
 
 [pre-commit-link]:
   https://github.com/pre-commit/pre-commit
   "Pre-Commit at GitHub.com"
```

### Comparing `kilter_protocol-0.4.0/kilter/protocol/__init__.py` & `kilter_protocol-0.5.0/kilter/protocol/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 from .core import ResponseMessage as ResponseMessage
 from .exceptions import *
 from .messages import *
 
 if TYPE_CHECKING:
 	from .buffer import FixedSizeBuffer as FixedSizeBuffer
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

### Comparing `kilter_protocol-0.4.0/kilter/protocol/buffer.py` & `kilter_protocol-0.5.0/kilter/protocol/buffer.py`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.4.0/kilter/protocol/core.py` & `kilter_protocol-0.5.0/kilter/protocol/core.py`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.4.0/kilter/protocol/exceptions.py` & `kilter_protocol-0.5.0/kilter/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `kilter_protocol-0.4.0/kilter/protocol/messages.py` & `kilter_protocol-0.5.0/kilter/protocol/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022-2023 Dominik Sekotill <dom.sekotill@kodo.org.uk>
+# Copyright 2022-2024 Dominik Sekotill <dom.sekotill@kodo.org.uk>
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 """
 Classes for representing protocol messages, and packing and unpacking them
@@ -12,14 +12,15 @@
 and unpacking.
 """
 
 from __future__ import annotations
 
 from abc import ABCMeta
 from abc import abstractmethod
+from codecs import decode
 from collections.abc import Collection
 from collections.abc import Iterable
 from collections.abc import Iterator
 from collections.abc import Mapping
 from dataclasses import dataclass
 from dataclasses import field
 from enum import Enum
@@ -245,15 +246,15 @@
 		assert isinstance(ident, int)
 		end = hdr_size + size - 1
 		if buf.filled < end:
 			raise NeedsMore
 		try:
 			msg_class = cls._message_classes[ident]
 		except KeyError:
-			raise UnknownMessage(buf[:end].tobytes())
+			raise UnknownMessage(buf[:end].tobytes()) from None
 		else:
 			with buf[hdr_size:end] as data:
 				return msg_class.from_buffer(data), end
 
 	@classmethod
 	@abstractmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
@@ -297,14 +298,25 @@
 		"""
 		Release any memoryviews a message holds of a buffer from which it was created
 
 		Concrete classes MUST implement this if they store references to memoryviews, or any
 		value that could be a memoryview.
 		"""
 
+	def freeze(self) -> None:
+		"""
+		Similar to `release()`, but memoryviews are replaced with byte object copies
+
+		Users may call this to copy data from a buffer for later reading, for instance if
+		they intend to store messages and process them at a later stage.
+
+		Concrete classes MUST implement this if they store references to memoryviews, or any
+		value that could be a memoryview.
+		"""
+
 
 class NoDataMessage(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with no contents
 	"""
 
 	def __repr__(self) -> str:
@@ -322,15 +334,15 @@
 class BytesMessage(Message):
 	"""
 	Base class implementing `Message` abstract methods for messages with unstructured contents
 	"""
 
 	content: memoryview
 
-	def __init__(self, content: bytes):
+	def __init__(self, content: bytes|memoryview):
 		self.content = memoryview(content).toreadonly()
 
 	def __repr__(self) -> str:
 		content = repr(self.content.tobytes()) if len(self.content) <= 30 else \
 			f"{self.content[:20].tobytes()!r} + {len(self.content)-20} further bytes"
 		return f"{self.__class__.__name__}({content})"
 
@@ -345,14 +357,17 @@
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		buf[:] = self.content
 
 	def release(self) -> None:
 		self.content.release()
 
+	def freeze(self) -> None:
+		self.content = memoryview(self.content.tobytes())
+
 
 # MTA Setup Commands
 
 @dataclass
 class Negotiate(Message, ident=b"O"):
 	"""
 	Message type for MTA and filters to negotiate the features they provide and need
@@ -413,15 +428,15 @@
 	def from_buffer(cls, buf: memoryview) -> Self:
 		stage, *_ = cls._struct.unpack_from(buf)
 		macros = {}
 		with buf[1:] as buf:
 			while len(buf) > 0:
 				key, buf = split_cstring(buf)
 				val, buf = split_cstring(buf)
-				macros[key.tobytes().decode("ascii")] = val.tobytes().decode("ascii")
+				macros[decode(key, "ascii")] = decode(val, "ascii")
 		return cls(stage, macros)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		self._struct.pack_into(buf.get_free(self._struct.size), 0, self.stage)
 		for key, val in self.macros.items():
 			write_cstring(buf, key.encode("ascii"))
 			write_cstring(buf, val.encode("ascii"))
@@ -448,15 +463,15 @@
 	port: int = 0
 
 	_struct = Struct("!H")
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		_hostname, buf = split_cstring(buf)
-		hostname = _hostname.tobytes().decode("idna")
+		hostname = decode(_hostname, "idna")
 		family, buf = Family(buf[0:1].tobytes()), buf[1:]
 		if family == Family.UNKNOWN:
 			return cls(hostname)
 		port, *_ = cls._struct.unpack_from(buf)
 		addr, buf = split_cstring(buf[cls._struct.size:])
 		if family == Family.UNIX:
 			return cls(hostname, Path(addr.tobytes().decode()))
@@ -490,28 +505,28 @@
 	"""
 
 	hostname: str
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		hostname, _ = split_cstring(buf)
-		return cls(hostname.tobytes().decode("idna"))
+		return cls(decode(hostname, "idna"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.hostname.encode("idna"))
 
 
 @dataclass
 class EnvelopeFrom(Message, ident=b"M"):
 	"""
 	An event message reporting a client sent an SMTP "MAIL FROM" command
 	"""
 
-	sender: bytes
-	arguments: list[bytes] = field(default_factory=list)
+	sender: bytes|memoryview
+	arguments: list[bytes|memoryview] = field(default_factory=list)
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		args = cstring_iter(buf)
 		return cls(next(args), [*args])
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
@@ -522,25 +537,33 @@
 	def release(self) -> None:
 		if isinstance(self.sender, memoryview):
 			self.sender.release()
 		for arg in self.arguments:
 			if isinstance(arg, memoryview):
 				arg.release()
 
+	def freeze(self) -> None:
+		if isinstance(self.sender, memoryview):
+			self.sender = self.sender.tobytes()
+		self.arguments[:] = (
+			arg.tobytes() if isinstance(arg, memoryview) else arg
+			for arg in self.arguments
+		)
+
 
 @dataclass
 class EnvelopeRecipient(Message, ident=b"R"):
 	"""
 	An event message reporting a client sent an SMTP "RCPT TO" command
 
 	A client must send at least one "RCPT TO" command, and can send multiple.
 	"""
 
-	recipient: bytes
-	arguments: list[bytes] = field(default_factory=list)
+	recipient: bytes|memoryview
+	arguments: list[bytes|memoryview] = field(default_factory=list)
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		args = cstring_iter(buf)
 		return cls(next(args), [*args])
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
@@ -551,14 +574,22 @@
 	def release(self) -> None:
 		if isinstance(self.recipient, memoryview):
 			self.recipient.release()
 		for arg in self.arguments:
 			if isinstance(arg, memoryview):
 				arg.release()
 
+	def freeze(self) -> None:
+		if isinstance(self.recipient, memoryview):
+			self.recipient = self.recipient.tobytes()
+		self.arguments[:] = (
+			arg.tobytes() if isinstance(arg, memoryview) else arg
+			for arg in self.arguments
+		)
+
 
 class Data(NoDataMessage, ident=b"T"):
 	"""
 	An event message reporting a client sent an SMTP "DATA" command
 
 	This event mainly indicates to a filter that there will be no further SMTP commands
 	sent.
@@ -576,31 +607,35 @@
 @dataclass
 class Header(Message, ident=b"L"):
 	"""
 	Transfers a header name and value from an email to a filter
 	"""
 
 	name: str
-	value: bytes
+	value: bytes|memoryview
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		name, buf = split_cstring(buf)
 		value, buf = split_cstring(buf)
 		assert len(buf) == 0
-		return cls(name.tobytes().decode("ascii"), value)
+		return cls(decode(name, "ascii"), value)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.name.encode("ascii"))
 		write_cstring(buf, self.value)
 
 	def release(self) -> None:
 		if isinstance(self.value, memoryview):
 			self.value.release()
 
+	def freeze(self) -> None:
+		if isinstance(self.value, memoryview):
+			self.value = self.value.tobytes()
+
 
 class EndOfHeaders(NoDataMessage, ident=b"N"):
 	"""
 	A message that indicates the end of an email's headers
 	"""
 
 
@@ -685,15 +720,15 @@
 
 	address: str
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		address, buf = split_cstring(buf)
 		assert len(buf) == 0
-		return cls(address.tobytes().decode("utf-8"))
+		return cls(decode(address, "utf-8"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.address.encode("utf-8"))
 
 
 @dataclass
 class _AddrParCmd(Message):
@@ -708,16 +743,16 @@
 	def from_buffer(cls, buf: memoryview) -> Self:
 		args: memoryview|None = None
 		address, buf = split_cstring(buf)
 		if len(buf) > 0:
 			args, buf = split_cstring(buf)
 		assert len(buf) == 0
 		return cls(
-			address.tobytes().decode("utf-8"),
-			None if args is None else args.tobytes().decode("utf-8"),
+			decode(address, "utf-8"),
+			None if args is None else decode(args, "utf-8"),
 		)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.address.encode("utf-8"))
 		if self.args:
 			write_cstring(buf, self.args.encode("utf-8"))
 
@@ -734,33 +769,37 @@
 class ChangeHeader(Message, ident=b"m"):
 	"""
 	Message from a filter to request a header is modified or removed at a given index
 	"""
 
 	index: int
 	name: str
-	value: bytes
+	value: bytes|memoryview
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		index, *_ = LONG.unpack_from(buf)
 		name, buf = split_cstring(buf[LONG.size:])
 		value, buf = split_cstring(buf)
 		assert len(buf) == 0
-		return cls(index, name.tobytes().decode("ascii"), value)
+		return cls(index, decode(name, "ascii"), value)
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		LONG.pack_into(buf.get_free(LONG.size), 0, self.index)
 		write_cstring(buf, self.name.encode("ascii"))
 		write_cstring(buf, self.value)
 
 	def release(self) -> None:
 		if isinstance(self.value, memoryview):
 			self.value.release()
 
+	def freeze(self) -> None:
+		if isinstance(self.value, memoryview):
+			self.value = self.value.tobytes()
+
 
 class InsertHeader(ChangeHeader, ident=b"i"):
 	"""
 	Message from a filter to request a header is inserted into the message
 	"""
 
 
@@ -808,11 +847,11 @@
 
 	reason: str
 
 	@classmethod
 	def from_buffer(cls, buf: memoryview) -> Self:
 		reason, buf = split_cstring(buf)
 		assert len(buf) == 0
-		return cls(reason.tobytes().decode("utf-8"))
+		return cls(decode(reason, "utf-8"))
 
 	def to_buffer(self, buf: FixedSizeBuffer) -> None:
 		write_cstring(buf, self.reason.encode("utf-8"))
```

### Comparing `kilter_protocol-0.4.0/pyproject.toml` & `kilter_protocol-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
-requires = ["flit_core ~=3.2"]
+requires = ["flit_core ~=3.8"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "kilter.protocol"
 authors = [
 	{name = "Dom Sekotill", email = "dom.sekotill@kodo.org.uk"},
 ]
 license = {file = "LICENCE.txt"}
 readme = "README.md"
 dynamic = ["version", "description"]
 
-# https://github.com/pypa/flit/issues/476
-requires-python = ">=3.10,<4"
+requires-python = "~=3.10"
 
 classifiers = [
 	"Development Status :: 1 - Planning",
 	"Intended Audience :: Telecommunications Industry",
 	"License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
 	"Topic :: Communications :: Email :: Filters",
 ]
@@ -33,50 +32,39 @@
 ]
 coverage = [
 	"coverage[toml]",
 	"kodo.plugins.cover-test-context",
 ]
 
 [project.urls]
-Source = "https://code.kodo.org.uk/kilter/kilter.protocol"
-Issues = "https://code.kodo.org.uk/kilter/kilter.protocol/-/issues"
-Documentation = "http://kilter.doc.kodo.org.uk/kilter.protocol"
+Source = "https://github.com/domsekotill/kilter.protocol"
+Issues = "https://github.com/domsekotill/kilter.protocol/issues"
+Documentation = "https://kilter.kodo.org.uk/kilter.protocol/"
 
 
 [tool.isort]
 force_single_line = true
 
 
 [tool.unimport]
 ignore_init = true
 
 
 [tool.flakeheaven]
 base = "https://code.kodo.org.uk/dom/project-templates/-/raw/main/.flakerules.toml"
-max_line_length = 92
-max_doc_length = 92
-
-[tool.flakeheaven.plugins]
-pycodestyle = ["-E701", "-E226"]
 
 [tool.flakeheaven.exceptions."kilter/protocol/messages.py"]
 flake8-docstrings = ["-D102"]
 
-[tool.flakeheaven.exceptions."tests/"]
-flake8-docstrings = ["-D100"]
-
 [tool.flakeheaven.exceptions."tests/unittest_helpers.py"]
 flake8-docstrings = ["-D10*"]
 
-[tool.flakeheaven.exceptions."doc/*"]
-flake8-docstrings = ["-*"]
-
 
 [tool.mypy]
-python_version = 3.10
+python_version = "3.10"
 strict = true
 warn_unused_configs = true
 warn_unreachable = true
 namespace_packages = true
 explicit_package_bases = true
 allow_redefinition = true
 
@@ -99,24 +87,25 @@
 	"kodo.plugins.cover_test_context",
 ]
 
 [tool.coverage.report]
 precision = 2
 skip_empty = true
 exclude_lines = [
-	"pragma: no-cover",
-	"if .*\\b__name__\\b",
-	"if .*\\bTYPE_CHECKING\\b",
+	"@(abc\\.)abstractmethod",
+	"@overload",
 	"class .*(.*\\bProtocol\\b.*):",
 	"def __repr__",
-	"@overload",
+	"if .*\\bTYPE_CHECKING\\b",
+	"if .*\\b__name__\\b",
+	"pragma: no-cover",
 ]
 partial_branches = [
-	"pragma: no-branch",
 	"if .*\\b__debug__\\b",
+	"pragma: no-branch",
 ]
 
 [tool.coverage.json]
 output = "results/coverage.json"
 show_contexts = true
 
 [tool.coverage.xml]
```

### Comparing `kilter_protocol-0.4.0/PKG-INFO` & `kilter_protocol-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: kilter.protocol
-Version: 0.4.0
+Version: 0.5.0
 Summary: Parsers and state machines for the Sendmail milter communications protocol
 Author-email: Dom Sekotill <dom.sekotill@kodo.org.uk>
-Requires-Python: >=3.10,<4
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Dist: typing-extensions
 Requires-Dist: coverage[toml] ; extra == "coverage"
 Requires-Dist: kodo.plugins.cover-test-context ; extra == "coverage"
 Requires-Dist: sphinx ~=5.0 ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme ; extra == "docs"
-Project-URL: Documentation, http://kilter.doc.kodo.org.uk/kilter.protocol
-Project-URL: Issues, https://code.kodo.org.uk/kilter/kilter.protocol/-/issues
-Project-URL: Source, https://code.kodo.org.uk/kilter/kilter.protocol
+Project-URL: Documentation, https://kilter.kodo.org.uk/kilter.protocol/
+Project-URL: Issues, https://github.com/domsekotill/kilter.protocol/issues
+Project-URL: Source, https://github.com/domsekotill/kilter.protocol
 Provides-Extra: coverage
 Provides-Extra: docs
 
+<!--
+# Disable Gitlab link until hosting is more reliable
 [![gitlab-ico]][gitlab-link]
+-->
+[![github-ico]][github-link]
 [![licence-mpl20]](/LICENCE.txt)
 [![pre-commit-ico]][pre-commit-link]
 [![pipeline-status]][pipeline-report]
 [![coverage status]][coverage report]
 
 
 Kilter Protocol
@@ -79,14 +83,22 @@
   https://img.shields.io/badge/GitLab-code.kodo.org.uk-blue.svg?logo=gitlab
   "GitLab"
 
 [gitlab-link]:
   https://code.kodo.org.uk/kilter/kilter.protocol
   "Kilter Protocol at code.kodo.org.uk"
 
+[github-ico]:
+  https://img.shields.io/badge/GitHub-domsekotill/kilter.protocol-blue.svg?logo=github
+  "GitHub"
+
+[github-link]:
+	https://github.com/domsekotill/kilter.protocol
+	"Kilter Protocol at github.com"
+
 [pre-commit-ico]:
   https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
   "Pre-Commit: enabled"
 
 [pre-commit-link]:
   https://github.com/pre-commit/pre-commit
   "Pre-Commit at GitHub.com"
```

