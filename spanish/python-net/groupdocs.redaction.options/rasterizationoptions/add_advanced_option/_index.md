---
title: "método add_advanced_option"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Registra una opción de rasterización avanzada para aplicar."
type: docs
url: /es/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registra una opción de rasterización avanzada para aplicar.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.). |

### Ejemplo

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registra una opción de rasterización avanzada para aplicar.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.). |
| parameters | `dict[str, str]` | Parámetros para el efecto dado, como el ángulo de rotación. |

### Ejemplo

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Aplicar efectos incorporados
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Aplicar un efecto con configuraciones personalizadas, p. ej., un borde de 10 unidades
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Ver también
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
