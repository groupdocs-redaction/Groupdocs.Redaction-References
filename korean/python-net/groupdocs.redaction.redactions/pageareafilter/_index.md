---
title: "PageAreaFilter 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서 페이지 내에서 편집을 적용할 영역을 설정하는 편집 필터를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/pageareafilter/
is_root: false
weight: 150
---


## PageAreaFilter class

문서 페이지 내에서 편집을 적용할 영역을 설정하는 편집 필터를 나타냅니다.

자세히 알아보기

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

PageAreaFilter 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/__init__/#top_left-size) | 특정 영역을 가리기 위해 새로운 PageAreaFilter를 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [rectangle](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/rectangle/) | 페이지의 사각형(왼쪽 상단 위치와 영역 크기)입니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaFilter
from groupdocs.pydrawing import Point, Size

with Redactor("doc.pdf") as redactor:
    page = redactor.get_document_info().pages[0]
    area_filter = PageAreaFilter(
        Point(0, int(page.height / 2)),
        Size(page.width, int(page.height / 2))
    )
```

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
