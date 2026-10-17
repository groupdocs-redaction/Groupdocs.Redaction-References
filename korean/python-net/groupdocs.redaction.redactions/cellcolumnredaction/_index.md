---
title: "CellColumnRedaction 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "스프레드시트 문서(CSV, Excel 등)에서 텍스트를 교체하는 텍스트 레드액션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

스프레드시트 문서(CSV, Excel 등)에서 텍스트를 교체하는 텍스트 레드액션을 나타냅니다.

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

CellColumnRedaction 형식은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | 새 CellColumnRedaction을 초기화합니다. |

### 메서드
| 메서드 | 설명 |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | 주어진 포맷 인스턴스에 Redaction을 적용합니다. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### 속성
| 속성 | 설명 |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | Redaction의 설명으로, 이름과 매개변수를 포함합니다. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | 열 및 워크시트 필터입니다. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | 일치시킬 정규식 패턴입니다. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | 텍스트 교체 유형을 지정하는 [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) 인스턴스. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | 그래픽 콘텐츠에서 텍스트를 추출하는 데 사용되는 IOcrConnector 구현. ([`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)에서 상속됨) |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
