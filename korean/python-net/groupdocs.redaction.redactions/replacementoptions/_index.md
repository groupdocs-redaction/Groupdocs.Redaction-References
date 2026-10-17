---
title: "ReplacementOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "일치된 텍스트 교체 옵션을 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/replacementoptions/
is_root: false
weight: 260
---


## ReplacementOptions class

일치된 텍스트 교체 옵션을 나타냅니다.

자세히 알아보기

- More details about document text redactions: https://docs.groupdocs.com/redaction/net/text-redactions/
- More details about redaction filters: https://docs.groupdocs.com/redaction/net/use-pdf-redaction-filters/

ReplacementOptions 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#replacement) | 지정된 교체 텍스트를 사용하여 ReplacementOptions의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/__init__/#color) | 색상 사각형을 옵션으로 하여 ReplacementOptions 클래스의 새 인스턴스를 초기화합니다: |

### 속성
| 속성 | 설명 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/action_type/) | 교체 작업: 상자를 그리거나 텍스트를 교체합니다. |
| [box_color](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/box_color/) | `ReplacementType.draw_box` 옵션의 색상 (그 외 경우는 무시됩니다). |
| [custom_redaction](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/custom_redaction/) | 사용자가 자체 삭제 로직을 정의할 수 있도록 하는 사용자 지정 삭제 핸들러. |
| [filters](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/filters/) | 이 삭제와 함께 적용할 필터 배열. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/replacement/) | 텍스트 교체 값. |

### 예제

```python
from groupdocs.redaction.redactions import ReplacementOptions

# 일치하는 텍스트를 "[X]" 자리표시자로 교체합니다
repl_opt = ReplacementOptions("[X]")
```

### Guides
`ReplacementOptions`를 사용하는 작업 가이드:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
