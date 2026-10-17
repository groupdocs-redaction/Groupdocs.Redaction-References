---
title: "find_format 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "查找给定文件扩展名的格式配置。"
type: docs
url: /zh/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

查找给定文件扩展名的格式配置。

```python
def find_format(self, file_extension):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| file_extension | `str` | 文件扩展名，格式为 ".ext"。 |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### 示例

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# 获取单例配置实例
config = RedactorConfiguration.get_instance()

# 检索给定扩展名的格式设置
settings = config.find_format(".txt")
if settings:
    # 扩展已处理扩展名的列表，例如，添加 .dump
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### 另请参阅
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
