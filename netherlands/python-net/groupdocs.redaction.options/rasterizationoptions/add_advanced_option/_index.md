---
title: "add_advanced_option‑methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Registreert een geavanceerde rasterisatie-optie om toe te passen."
type: docs
url: /nl/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registreert een geavanceerde rasterisatie-optie om toe te passen.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |

### Voorbeeld

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registreert een geavanceerde rasterisatie-optie om toe te passen.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |
| parameters | `dict[str, str]` | Parameters voor het opgegeven effect, zoals rotatiehoek. |

### Voorbeeld

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Toepassen van ingebouwde effecten
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Pas een effect toe met aangepaste instellingen, bijv. een rand van 10 eenheden
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Zie ook
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
