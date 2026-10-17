---
title: "PageAreaRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "페이지 영역의 텍스트, 이미지 및 주석에 영향을 주는 복합 텍스트 편집을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/pagearearedaction/
is_root: false
weight: 160
---


## PageAreaRedaction class

페이지 영역의 텍스트, 이미지 및 주석에 영향을 주는 복합 텍스트 편집을 나타냅니다.

자세히 알아보기

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)

PageAreaRedaction 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options) | 새로운 PageAreaRedaction 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/__init__/#regex-options-image_options) | 새로운 PageAreaRedaction을 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [image_options](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/image_options/) | 색상 및 영역 매개변수가 포함된 RegionReplacementOptions 옵션입니다. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 텍스트 교체 유형을 지정하는 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 인스턴스. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | 가리기의 설명으로, 이름과 매개변수를 포함합니다. ([`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)에서 상속됨) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 그래픽 콘텐츠에서 텍스트를 추출하는 데 사용되는 IOcrConnector 구현. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | 매칭에 사용되는 정규식 패턴입니다. ([`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/)에서 상속됨) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import PageAreaRedaction, ReplacementOptions, RegionReplacementOptions
from groupdocs.pydrawing import Color, Size

with Redactor("scan.pdf") as redactor:
    redactor.apply(
        PageAreaRedaction(
            r"\d{3}-\d{2}-\d{4}",
            ReplacementOptions("[SSN]"),
            RegionReplacementOptions(Color.BLACK, Size(120, 20))
        )
    )
    redactor.save()
```

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
