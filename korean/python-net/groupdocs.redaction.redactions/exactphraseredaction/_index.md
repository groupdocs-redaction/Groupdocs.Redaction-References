---
title: "ExactPhraseRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서 텍스트에서 정확한 구문을 기본적으로 대소문자를 구분하지 않고 교체하는 텍스트 레드액션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/exactphraseredaction/
is_root: false
weight: 80
---


## ExactPhraseRedaction class

문서 텍스트에서 정확한 구문을 기본적으로 대소문자를 구분하지 않고 교체하는 텍스트 레드액션을 나타냅니다.

자세히 보기:
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/

ExactPhraseRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-options) | 대소문자 구분 없이 ExactPhraseRedaction의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/__init__/#search_phrase-is_case_sensitive-options) | 새 ExactPhraseRedaction 인스턴스를 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/description/) | 삭제 작업의 설명으로, 삭제 이름과 매개변수를 포함합니다. |
| [is_case_sensitive](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_case_sensitive/) | 검색이 대소문자를 구분하는지 여부를 나타내는 값입니다. |
| [is_right_to_left](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/is_right_to_left/) | 텍스트가 오른쪽에서 왼쪽으로 표시되는지 여부를 나타내는 텍스트 방향 플래그입니다. 기본값은 False입니다. |
| [search_phrase](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/search_phrase/) | 검색 및 교체할 문자열입니다. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 텍스트 교체 유형을 지정하는 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 인스턴스. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 그래픽 콘텐츠에서 텍스트를 추출하는 데 사용되는 IOcrConnector 구현. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

with Redactor("sample.pdf") as redactor:
    # 대소문자 구분 교체
    redactor.apply(ExactPhraseRedaction("John Doe", True, ReplacementOptions("[personal]")))
    redactor.save()
```

### Guides
`ExactPhraseRedaction`을 사용하는 작업 가이드:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
