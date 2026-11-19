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
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

with Redactor("./sample.docx") as redactor:
    so = SaveOptions()
    so.rasterization.enabled = True
    so.redacted_file_suffix = "_scan"
    so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
    result_path = redactor.save(so)
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

### Aliases

These names call `add_advanced_option` too, limited to the overloads listed.

| Alias | Accepts |
| :- | :- |
| `add_advanced_option_advanced_rasterization_options` | `add_advanced_option_advanced_rasterization_options(option_type)`<br>`add_advanced_option_advanced_rasterization_options(option_type, parameters)` |

### See Also
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
