---
title: "redact_annotation yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belge içindeki tüm ek açıklamalardaki eşleşen metni değiştirir."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-replacement}

Belge içindeki tüm ek açıklamalardaki eşleşen metni değiştirir.

```python
def redact_annotation(self, regular_expression, replacement):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| replacement | `str` | Metinsel değiştirme. |

**Returns:** Replacement result.

### Ayrıca Bakınız
* class [`IAnnotatedDocument`](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/)
