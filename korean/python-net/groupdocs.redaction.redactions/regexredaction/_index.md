---
title: "RegexRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 편집을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/regexredaction/
is_root: false
weight: 230
---


## RegexRedaction class

제공된 정규식을 일치시켜 문서의 텍스트를 검색하고 교체하는 텍스트 편집을 나타냅니다.

자세히 알아보기

- More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
- More details about document text redactions: [Text redactions](https://docs.groupdocs.com/redaction/net/text-redactions/)

RegexRedaction 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#pattern-options) | RegexRedaction의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/__init__/#regex-options) | 새 RegexRedaction 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/description/) | Redaction의 설명으로, 이름과 매개변수를 포함합니다. |
| [regular_expression](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/regular_expression/) | 매칭에 사용되는 정규식 패턴. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 텍스트 교체 유형을 지정하는 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 인스턴스. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 그래픽 콘텐츠에서 텍스트를 추출하는 데 사용되는 IOcrConnector 구현. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

with Redactor("sample.pdf") as redactor:
    # 텍스트로 교체
    redactor.apply(RegexRedaction(r"\d{2}\s*\d{2}[^\d]*\d{6}", ReplacementOptions("[removed]")))
    # 파란색 실선 사각형으로 교체
    redactor.apply(RegexRedaction(r"^\d+[,\.]{1}\d+$", ReplacementOptions(Color.BLUE)))
    redactor.save()
```

### Guides
`RegexRedaction`를 사용하는 작업 가이드:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
