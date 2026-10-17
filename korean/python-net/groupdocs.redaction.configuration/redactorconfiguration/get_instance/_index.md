---
title: "get_instance 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "내장 형식의 기본 구성을 가진 싱글톤 인스턴스를 반환합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

내장 형식의 기본 구성을 가진 싱글톤 인스턴스를 반환합니다.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### 예제

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# 싱글톤 구성을 얻습니다
config = RedactorConfiguration.get_instance()

# 일반 텍스트 형식에 대한 지원되는 확장자를 확장합니다
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### 또 보기
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
