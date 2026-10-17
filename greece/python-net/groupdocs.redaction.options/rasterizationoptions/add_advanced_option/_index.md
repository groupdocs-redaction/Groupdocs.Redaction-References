---
title: "μέθοδος add_advanced_option"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Καταχωρεί μια προχωρημένη επιλογή rasterization για εφαρμογή."
type: docs
url: /el/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Καταχωρεί μια προχωρημένη επιλογή rasterization για εφαρμογή.

```python
def add_advanced_option(self, option_type):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρι κλίμακα, περίγραμμα κ.ά.). |

### Παράδειγμα

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Καταχωρεί μια προχωρημένη επιλογή rasterization για εφαρμογή.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Παράμετρος | Τύπος | Περιγραφή |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρι κλίμακα, περίγραμμα κ.ά.). |
| parameters | `dict[str, str]` | Παράμετροι για το συγκεκριμένο εφέ, όπως η γωνία περιστροφής. |

### Παράδειγμα

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Εφαρμογή ενσωματωμένων εφέ
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Εφαρμογή εφέ με προσαρμοσμένες ρυθμίσεις, π.χ., ένα περίγραμμα 10 μονάδων
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Δείτε επίσης
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
