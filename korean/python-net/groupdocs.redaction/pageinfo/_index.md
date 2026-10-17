---
title: "PageInfo 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "간략한 페이지 정보를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction/pageinfo/
is_root: false
weight: 90
---


## PageInfo class

간략한 페이지 정보를 나타냅니다.

자세히 보기:
- https://docs.groupdocs.com/redaction/net/get-file-info/

PageInfo 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/pageinfo/__init__/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [height](/redaction/python-net/groupdocs.redaction/pageinfo/height/) | 페이지 높이. |
| [page_number](/redaction/python-net/groupdocs.redaction/pageinfo/page_number/) | 페이지 번호. |
| [width](/redaction/python-net/groupdocs.redaction/pageinfo/width/) | 페이지 너비. |

### 예제

```python
from groupdocs.redaction import Redactor

try:
    with Redactor(r"C:\Temp\testfile.doc") as red:
        doc_info = red.get_document_info()
        print(f"Document size: {doc_info.size}")
        print(f"Document format: {doc_info.file_type.file_format}")
        print(f"Document contains {doc_info.page_count} pages")
        for page in doc_info.pages:
            print(f"Page {page.page_number} size is {page.width}x{page.height}")
except GroupDocs.Redaction.Exceptions.PasswordRequiredException:
    print("You are trying to access document which is password protected. Please, set the password.")
except GroupDocs.Redaction.Exceptions.IncorrectPasswordException:
    print("The provided password is not valid.")
```

### 또 보기
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
