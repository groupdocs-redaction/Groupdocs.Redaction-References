---
title: "__init__ 构造函数"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "使用文件路径初始化新的 Redactor 实例。"
type: docs
url: /zh/python-net/groupdocs.redaction/redactor/__init__/
is_root: false
weight: 10
---


## __init__ {#file_path}

使用文件路径初始化新的 Redactor 实例。

```python
def __init__(self, file_path):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_path | `str` | 文件路径。 |

### 示例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    # 在此执行 redaction 操作
    pass
```

## __init__ {#document}

使用流初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。

```python
def __init__(self, document):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| document | `io.RawIOBase` | 文档的源流。 |

### 示例

```python
from groupdocs.redaction import Redactor

def open_from_stream():
    # 以二进制流打开文档
    with open("./sample.pdf", "rb") as stream:
        # 从流加载文档
        with Redactor(stream) as redactor:
            # 在此执行 redaction
            pass
```

## __init__ {#file_path-load_options}

使用路径为受密码保护的文档初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。

```python
def __init__(self, file_path, load_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_path | `str` | 文件路径。 |
| load_options | `LoadOptions` | 选项，包括密码。 |

### 示例

```python
from groupdocs.redaction import Redactor

# 从文件路径加载受密码保护的文档
with Redactor("protected.docx") as redactor:
    # 在此执行 redaction 操作
    pass
```

## __init__ {#file_path-load_options-settings}

使用路径和设置为受密码保护的文档初始化新的 Redactor 实例。

```python
def __init__(self, file_path, load_options, settings):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_path | `str` | 文件路径。 |
| load_options | `LoadOptions` | 基于文件的选项，包括密码。 |
| settings | `RedactorSettings` | redaction 过程的默认设置。 |

### 示例

```python
from groupdocs.redaction import Redactor

with Redactor("./sample.docx") as redactor:
    info = redactor.get_document_info()
    print(f"File type: {info.file_type}")
    print(f"Number of pages: {info.page_count}")
    print(f"Document size: {info.size} bytes")
```

## __init__ {#document-load_options}

使用流为受密码保护的文档初始化新的 Redactor 实例。

```python
def __init__(self, document, load_options):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| document | `io.RawIOBase` | 源输入流。 |
| load_options | `LoadOptions` | 选项，包括密码。 |

### 示例

```python
from groupdocs.redaction import Redactor, LoadOptions

def open_protected_doc():
    # 将受保护的 PDF 以二进制流打开
    with open(r"C:\sample.pdf", "rb") as stream:
        # 通过 LoadOptions 提供密码
        load_options = LoadOptions("mypassword")
        # 使用流和加载选项初始化 Redactor
        with Redactor(stream, load_options) as redactor:
            # 在此执行 redaction 操作
            pass
```

## __init__ {#document-load_options-settings}

使用流和设置为受密码保护的文档初始化 [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) 的新实例。

```python
def __init__(self, document, load_options, settings):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| document | `io.RawIOBase` | 源输入流。 |
| load_options | `LoadOptions` | 选项，包括密码。 |
| settings | `RedactorSettings` | 编辑过程的默认设置。 |

### 另请参阅
* class [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/)
