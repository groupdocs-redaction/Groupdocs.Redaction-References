---
title: "metodo add_advanced_option"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Registra un'opzione di rasterizzazione avanzata da applicare."
type: docs
url: /it/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Registra un'opzione di rasterizzazione avanzata da applicare.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.). |

### Esempio

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Registra un'opzione di rasterizzazione avanzata da applicare.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.). |
| parameters | `dict[str, str]` | Parametri per l'effetto specificato, come l'angolo di rotazione. |

### Esempio

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Applica effetti incorporati
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Applica un effetto con impostazioni personalizzate, ad es., un bordo di 10 unità
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Vedi anche
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
