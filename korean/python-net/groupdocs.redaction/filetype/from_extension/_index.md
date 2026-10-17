---
title: "from_extension 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "파일 확장자를 파일 유형에 매핑합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

파일 확장자를 파일 유형에 매핑합니다.

```python
def from_extension(cls, extension):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| extension | `str` | 파일 확장자 (마침표 "." 포함). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| 예외 발생 | 설명 |
| :- | :- |
| `ValueError` | `extension`이 null이거나 빈 문자열일 때. |

### 또 보기
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
