---
title: add_advanced_option method
second_title: GroupDocs.Redaction for Python via .NET API References
description: "Registers an advanced rasterization option to apply."
type: docs
url: /python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registers an advanced rasterization option to apply.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Provides information about the selected effect type (grayscale, border, etc.). |

### Example

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registers an advanced rasterization option to apply.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Provides information about the selected effect type (grayscale, border, etc.). |
| parameters | `dict[str, str]` | Parameters for the given effect, such as rotation angle. |

### Example

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Apply built‑in effects
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Apply an effect with custom settings, e.g., a border of 10 units
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### See Also
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
