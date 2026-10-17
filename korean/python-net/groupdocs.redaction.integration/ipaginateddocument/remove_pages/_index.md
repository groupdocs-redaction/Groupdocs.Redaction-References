---
title: "remove_pages 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "시작 위치, 오프셋 및 개수에 따라 하나 또는 여러 페이지를 제거합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/ipaginateddocument/remove_pages/
is_root: false
weight: 1010
---


## remove_pages {#origin-index-count}

시작 위치, 오프셋 및 개수에 따라 하나 또는 여러 페이지를 제거합니다.

```python
def remove_pages(self, origin, index, count):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| origin | `PageSeekOrigin` | 문서의 시작 또는 끝에서 검색 원점 위치를 지정합니다. |
| index | `int` | 시작 위치 인덱스 (0부터 시작). |
| count | `int` | 제거할 페이지 수. |

**Returns:** Pages removal redaction result.

### 또 보기
* class [`IPaginatedDocument`](/redaction/python-net/groupdocs.redaction.integration/ipaginateddocument/)
