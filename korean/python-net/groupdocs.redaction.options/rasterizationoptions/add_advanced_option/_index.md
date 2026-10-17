---
title: "add_advanced_option 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "적용할 고급 래스터화 옵션을 등록합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

적용할 고급 래스터화 옵션을 등록합니다.

```python
def add_advanced_option(self, option_type):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 선택된 효과 유형(그레이스케일, 테두리 등)에 대한 정보를 제공합니다. |

### 예제

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

적용할 고급 래스터화 옵션을 등록합니다.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 선택된 효과 유형(그레이스케일, 테두리 등)에 대한 정보를 제공합니다. |
| parameters | `dict[str, str]` | 회전 각도와 같은 해당 효과에 대한 매개변수입니다. |

### 예제

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# 내장 효과 적용
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# 사용자 정의 설정으로 효과를 적용합니다. 예: 10 단위의 테두리
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### 또 보기
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
