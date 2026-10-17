---
title: "rasterize yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belgeyi bir akışa PDF olarak kaydeder."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

Belgeyi bir akışa PDF olarak kaydeder.

```python
def rasterize(self, output):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| output | `io.RawIOBase` | Hedef akış. |

## rasterize {#output-options}

Belgeyi bir akışa sayfa aralığı ve uyumluluk seçenekleriyle PDF olarak kaydeder.

```python
def rasterize(self, output, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| output | `io.RawIOBase` | Hedef akış. |
| options | `RasterizationOptions` | PDF dönüştürme seçenekleri. |

### Ayrıca Bakınız
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
