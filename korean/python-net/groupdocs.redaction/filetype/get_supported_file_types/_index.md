---
title: "get_supported_file_types 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "지원되는 파일 유형을 검색합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/filetype/get_supported_file_types/
is_root: false
weight: 1060
---


## get_supported_file_types

지원되는 파일 유형을 검색합니다.

```python
def get_supported_file_types(cls):
    ...
```

**Returns:** Iterable[FileType]: Sequence of supported file types.

### 예제

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # 지원 파일 유형 컬렉션 가져오기
    supported_file_types = FileType.get_supported_file_types()

    # 확장자별로 정렬된 파일 유형 열거
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

### 또 보기
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
