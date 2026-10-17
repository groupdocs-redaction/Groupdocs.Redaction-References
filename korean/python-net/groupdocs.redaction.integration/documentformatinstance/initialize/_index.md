---
title: "initialize 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서 형식 핸들러 인스턴스를 초기화합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/
is_root: false
weight: 1010
---


## initialize {#config-settings}

문서 형식 핸들러 인스턴스를 초기화합니다.

```python
def initialize(self, config, settings):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| config | `DocumentFormatConfiguration` | 포맷 구성. |
| settings | `RedactorSettings` | 편집 프로세스에 대한 기본 설정. |

**Returns:** None.

### 예제

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

# 사용자 지정 포맷을 등록합니다.
my_config = DocumentFormatConfiguration()
my_config.extension_filter = ".foo"
my_config.document_type = MyCustomHandler
my_config.initialization_data["MyProperty"] = "bar"

redactor_config = RedactorConfiguration.get_instance()
redactor_config.available_formats.append(my_config)
```

### 또 보기
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
