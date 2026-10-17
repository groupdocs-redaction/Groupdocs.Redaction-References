---
title: "find_format 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "주어진 파일 확장자에 대한 형식 구성을 찾습니다."
type: docs
url: /ko/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

주어진 파일 확장자에 대한 형식 구성을 찾습니다.

```python
def find_format(self, file_extension):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_extension | `str` | 파일 확장자, 포맷은 ".ext"입니다. |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### 예제

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# 싱글톤 구성 인스턴스를 얻기
config = RedactorConfiguration.get_instance()

# 주어진 확장자에 대한 포맷 설정을 검색
settings = config.find_format(".txt")
if settings:
    # 처리되는 확장자 목록을 확장하고, 예를 들어 .dump를 추가합니다
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### 또 보기
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
