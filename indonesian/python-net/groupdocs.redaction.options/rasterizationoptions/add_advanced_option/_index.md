---
title: "metode add_advanced_option"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mendaftarkan opsi rasterisasi lanjutan untuk diterapkan."
type: docs
url: /id/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Mendaftarkan opsi rasterisasi lanjutan untuk diterapkan.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll). |

### Contoh

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Mendaftarkan opsi rasterisasi lanjutan untuk diterapkan.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Memberikan informasi tentang tipe efek yang dipilih (grayscale, border, dll). |
| parameters | `dict[str, str]` | Parameter untuk efek yang diberikan, seperti sudut rotasi. |

### Contoh

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Terapkan efek bawaan
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Terapkan efek dengan pengaturan khusus, misalnya, border sebesar 10 unit
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Lihat Juga
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
