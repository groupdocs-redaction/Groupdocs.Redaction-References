---
title: "replace_in_column 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "지정된 열 및 워크시트에서 모든 일치를 주어진 교체 문자열로 바꿉니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/icellularformatinstance/replace_in_column/
is_root: false
weight: 1040
---


## replace_in_column {#regular_expression-replacement-column-sheet}

지정된 열 및 워크시트에서 모든 일치를 주어진 교체 문자열로 바꿉니다.

```python
def replace_in_column(self, regular_expression, replacement, column, sheet):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| replacement | `str` | 텍스트 교체. |
| column | `int` | 0부터 시작하는 열 인덱스. |
| sheet | `int` | 0부터 시작하는 워크시트 인덱스. |

**Returns:** Replacement result.

## replace_in_column {#regular_expression-replacement-column}

모든 워크시트의 지정된 열에서 모든 일치를 주어진 교체 문자열로 바꿉니다.

```python
def replace_in_column(self, regular_expression, replacement, column):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | 검색 및 교체를 위한 정규식. |
| replacement | `str` | 텍스트 교체. |
| column | `int` | 0부터 시작하는 열 인덱스. |

**Returns:** Replacement result.

### 또 보기
* class [`ICellularFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/icellularformatinstance/)
