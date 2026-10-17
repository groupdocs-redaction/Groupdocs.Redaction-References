---
title: "add_advanced_option‑Methode"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Registriert eine erweiterte Rasterisierungsoption zum Anwenden."
type: docs
url: /de/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registriert eine erweiterte Rasterisierungsoption zum Anwenden.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Gibt Informationen über den ausgewählten Effekttyp (Graustufen, Rahmen usw.) zurück. |

### Beispiel

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registriert eine erweiterte Rasterisierungsoption zum Anwenden.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parameter | Typ | Beschreibung |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Gibt Informationen über den ausgewählten Effekttyp (Graustufen, Rahmen usw.) zurück. |
| parameters | `dict[str, str]` | Parameter für den angegebenen Effekt, wie z. B. den Rotationswinkel. |

### Beispiel

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Integrierte Effekte anwenden
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Einen Effekt mit benutzerdefinierten Einstellungen anwenden, z. B. einen Rahmen von 10 Einheiten
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Siehe auch
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
