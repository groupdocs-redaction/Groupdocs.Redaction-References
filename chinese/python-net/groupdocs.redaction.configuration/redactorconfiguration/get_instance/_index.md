---
title: "get_instance 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "返回一个具有内置格式默认配置的单例实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

返回一个具有内置格式默认配置的单例实例。

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### 示例

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# 获取单例配置
config = RedactorConfiguration.get_instance()

# 扩展对纯文本格式的支持的扩展名
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### 另请参阅
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
