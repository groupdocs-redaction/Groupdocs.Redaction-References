---
title: "RegionReplacementOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다."
type: docs
url: /ko/python-net/groupdocs.redaction.redactions/regionreplacementoptions/
is_root: false
weight: 240
---


## RegionReplacementOptions class

이미지 영역 교체를 위한 색상 및 영역 매개변수를 나타냅니다.

자세히 보기:
- More details about image redactions: https://docs.groupdocs.com/redaction/net/image-redactions/

RegionReplacementOptions 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-size) | 새로운 RegionReplacementOptions 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/__init__/#fill_color-font-expected_text) | 주어진 텍스트에 맞는 크기의 RegionReplacementOptions 클래스 새 인스턴스를 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [fill_color](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/fill_color/) | 삭제된 영역을 채우는 데 사용되는 색상입니다. |
| [size](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/size/) | 사각형의 너비와 높이입니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

with Redactor("test.jpg") as redactor:
    # 교체할 영역의 왼쪽 위 위치를 정의합니다.
    point = Point(516, 311)
    # 교체할 영역의 크기를 정의합니다.
    size = Size(170, 35)
    # 대체물로 단색 검은 사각형을 사용합니다.
    repl_opt = RegionReplacementOptions(Color.BLACK, size)
    redaction = ImageAreaRedaction(point, repl_opt)

    result = redactor.apply(redaction)
    if result.status != redactor.RedactionStatus.FAILED:
        redactor.save()
```

### Guides
`RegionReplacementOptions`를 사용하는 작업 가이드:

* [Image redactions](/redaction/python-net/guides/image-redactions/)

### 또 보기
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
