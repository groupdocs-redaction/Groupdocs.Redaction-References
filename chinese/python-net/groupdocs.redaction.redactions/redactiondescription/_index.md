---
title: "RedactionDescription 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "表示在编辑过程中执行的单个更改操作信息。"
type: docs
url: /zh/python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

表示在编辑过程中执行的单个更改操作信息。

了解更多

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

RedactionDescription 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | 初始化 RedactionDescription 类的新实例，不包含替换信息。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | 初始化 RedactionDescription 类的新实例，包含替换信息。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | 初始化带有图像区域替换信息的 RedactionDescription。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | 编辑操作：替换、清理或删除。 |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | 被编辑项的可选详细信息。 |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | 图像区域编辑的替换信息，文本编辑则为 None。 |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | 匹配的文本（如果提供了表达式）。 |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | 文档数据的类型——文本、元数据或注释。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | 替换信息，可能为 None。 |

### 另请参阅
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
