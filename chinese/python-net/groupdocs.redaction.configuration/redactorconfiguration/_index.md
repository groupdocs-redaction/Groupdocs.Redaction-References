---
title: "RedactorConfiguration 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "提供对受支持格式列表的访问，包括内置格式和自定义用户格式。"
type: docs
url: /zh/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

提供对受支持格式列表的访问，包括内置格式和自定义用户格式。

了解更多：

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

该 RedactorConfiguration 类型公开以下成员：

### 方法
| 方法 | 描述 |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | 查找给定文件扩展名的格式配置。 |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | 返回一个具有内置格式默认配置的单例实例。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | 已识别格式的列表，参见 [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/)。 |

### 示例

```python
# 添加自定义用户格式处理程序
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# 检索内置或自定义的用户格式处理程序
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### 另请参阅
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
