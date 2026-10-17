---
title: "IDocumentInfo 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "기본 문서 정보를 가져오는 데 필요한 메서드를 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/idocumentinfo/
is_root: false
weight: 50
---


## IDocumentInfo class

기본 문서 정보를 가져오는 데 필요한 메서드를 제공합니다.

자세히 알아보기: 파일 정보 가져오기 (https://docs.groupdocs.com/redaction/net/get-file-info/).

IDocumentInfo 형식은 다음 멤버를 노출합니다:

### 속성
| 속성 | 설명 |
| :- | :- |
| [file_type](/redaction/python-net/groupdocs.redaction/idocumentinfo/file_type/) | 파일 형식 설명입니다. |
| [page_count](/redaction/python-net/groupdocs.redaction/idocumentinfo/page_count/) | 전체 페이지 수입니다. |
| [pages](/redaction/python-net/groupdocs.redaction/idocumentinfo/pages/) | 페이지 정보를 나타내는 [`PageInfo`](/redaction/python-net/groupdocs.redaction/pageinfo/) 객체 목록입니다. |
| [size](/redaction/python-net/groupdocs.redaction/idocumentinfo/size/) | 문서 크기(바이트)입니다. |

### 예제

```python
from groupdocs.redaction import Redactor

with Redactor("document.pdf") as redactor:
    info = redactor.get_document_info()
    print(info.file_type.file_format, info.page_count, info.size)
    for page in info.pages:
        print(f"Page {page.page_number} size is {page.width}x{page.height}")
```

### 또 보기
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
