---
title: "add_advanced_option yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Uygulanacak gelişmiş bir rasterleştirme seçeneği kaydeder."
type: docs
url: /tr/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

Uygulanacak gelişmiş bir rasterleştirme seçeneği kaydeder.

```python
def add_advanced_option(self, option_type):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar. |

### Örnek

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

Uygulanacak gelişmiş bir rasterleştirme seçeneği kaydeder.

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | Seçilen efekt türü (gri tonlama, kenarlık vb.) hakkında bilgi sağlar. |
| parameters | `dict[str, str]` | Verilen efekt için parametreler, örneğin dönüş açısı. |

### Örnek

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# Yerleşik efektleri uygula
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# Özel ayarlarla bir efekt uygula, ör. 10 birimlik kenarlık
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### Ayrıca Bakınız
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
