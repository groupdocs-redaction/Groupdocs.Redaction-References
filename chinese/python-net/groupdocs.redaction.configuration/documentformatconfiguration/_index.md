---
title: "DocumentFormatConfiguration 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示 DocumentFormatInstance 派生类的类型引用以及用于更快格式检测的受支持文件扩展名列表。"
type: docs
url: /zh/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

表示对 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) 派生类的类型引用，以及用于更快格式检测的受支持文件扩展名列表。

了解更多

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

该 DocumentFormatConfiguration 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | 初始化 DocumentFormatConfiguration 的新实例。 |

### 方法
| 方法 | 描述 |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | 检查给定的文件扩展名是否可以作为 DocumentType 处理。 |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### 属性
| 属性 | 描述 |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | 从 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) 继承的类的类型。 |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | 以逗号分隔的文件扩展名列表（例如 \".pdf\"），不区分大小写。 |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | 用于 [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) 初始化所需的数据。 |

### 示例

```python
from groupdocs.redaction import DocumentFormatConfiguration

# 创建自定义格式配置
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### 另请参阅
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
