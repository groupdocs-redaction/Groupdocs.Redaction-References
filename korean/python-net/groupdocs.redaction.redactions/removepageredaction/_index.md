---
title: "RemovePageRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서에서 페이지(슬라이드, 워크시트 등)를 제거하는 편집을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/removepageredaction/
is_root: false
weight: 250
---


## RemovePageRedaction class

문서에서 페이지(슬라이드, 워크시트 등)를 제거하는 편집을 나타냅니다.

자세히 알아보기
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about removing pages: https://docs.groupdocs.com/redaction/net/remove-page-redaction/

RemovePageRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/__init__/#origin-index-count) | 새 RemovePageRedaction을 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [count](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/count/) | 제거할 페이지 수. |
| [index](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/index/) | 시작 위치 인덱스 (0 기반). |
| [origin](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/origin/) | 문서의 시작 또는 끝 중 하나인 탐색 기준 위치. |
| [description](/redaction/python-net/groupdocs.redaction/redaction/description/) | 레드랙션에 대한 설명으로, 이름과 매개변수를 포함합니다. ([`Redaction`](/redaction/python-net/groupdocs.redaction/redaction/)에서 상속됨) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # 문서 끝에서부터 1페이지를 제거합니다
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    with Redactor("./test.pdf") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(rem_opt)

        # 레다션된 문서를 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        redactor.save(so)
```

### Guides
`RemovePageRedaction`를 사용하는 작업 가이드:

* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
