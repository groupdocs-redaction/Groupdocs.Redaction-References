---
title: "add_advanced_option 方法"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "注册要应用的高级光栅化选项。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

注册要应用的高级光栅化选项。

```python
def add_advanced_option(self, option_type):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 提供有关所选效果类型（灰度、边框等）的信息。 |

### 示例

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

注册要应用的高级光栅化选项。

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| 参数 | 类型 | 描述 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 提供有关所选效果类型（灰度、边框等）的信息。 |
| parameters | `dict[str, str]` | 给定效果的参数，例如旋转角度。 |

### 示例

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# 应用内置效果
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# 使用自定义设置应用效果，例如 10 单位的边框
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### 另请参阅
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
