---
title: "initialize 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "初始化文档格式处理程序实例。"
type: docs
url: /zh/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

初始化文档格式处理程序实例。

```python
def initialize(self, config, settings):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | 格式配置。 |
| settings | `RedactorSettings` | 编辑过程的默认设置。 |

**Returns:** None.

### 示例

```python
from groupdocs.redaction.integration import DocumentFormatInstance, DocumentFormatConfiguration, RedactorConfiguration

class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        super().__init__()
        self.my_property = None

    def initialize(self, config, settings=None):
        super().initialize(config, settings)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]

# 注册自定义格式
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### 另请参阅
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
