---
title: "méthode add_advanced_option"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Enregistre une option de rasterisation avancée à appliquer."
type: docs
url: /fr/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Enregistre une option de rasterisation avancée à appliquer.

```python
def add_advanced_option(self, option_type):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.). |

### Exemple

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Enregistre une option de rasterisation avancée à appliquer.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.). |
| parameters | `dict[str, str]` | Paramètres pour l'effet donné, tels que l'angle de rotation. |

### Exemple

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Appliquer les effets intégrés
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Appliquer un effet avec des paramètres personnalisés, p. ex., une bordure de 10 unités
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Voir aussi
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
