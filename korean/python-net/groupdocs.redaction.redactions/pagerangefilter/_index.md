---
title: "PageRangeFilter 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서 내 페이지 범위를 설정하여 편집을 적용하는 편집 필터를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/pagerangefilter/
is_root: false
weight: 170
---


## PageRangeFilter class

문서 내 페이지 범위를 설정하여 편집을 적용하는 편집 필터를 나타냅니다.

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about redaction filters: [Use PDF redaction filters](https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/)

PageRangeFilter 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/__init__/#origin-index-count) | 새 RemovePageRedaction을 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/count/) | 제거할 페이지 수. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/index/) | 시작 위치 인덱스 (0 기반). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/origin/) | 문서의 시작 또는 끝 중 하나인 탐색 기준 위치. |

### 예제

```python
from groupdocs.redaction.redactions import PageRangeFilter, PageSeekOrigin

# 마지막 페이지와 그 이전 페이지를 대상으로 하는 필터를 정의합니다.
page_filter = PageRangeFilter(PageSeekOrigin.END, 0, 1)

# 필터는 다른 필터와 결합할 수 있습니다, 예: PageAreaFilter,
# 레드랙션을 구성할 때 ReplacementOptions.Filters에 전달됩니다.
```

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
