---
title: "add_advanced_option-metod"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Registrerar ett avancerat rasteriseringsalternativ att tillämpa."
type: docs
url: /sv/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registrerar ett avancerat rasteriseringsalternativ att tillämpa.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Tillhandahåller information om den valda effekttypen (gråskala, ram, osv.). |

### Exempel

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registrerar ett avancerat rasteriseringsalternativ att tillämpa.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parameter | Typ | Beskrivning |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Tillhandahåller information om den valda effekttypen (gråskala, ram, osv.). |
| parameters | `dict[str, str]` | Parametrar för den givna effekten, såsom rotationsvinkel. |

### Exempel

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Applicera inbyggda effekter
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Applicera en effekt med anpassade inställningar, t.ex. en kant på 10 enheter
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Se även
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
