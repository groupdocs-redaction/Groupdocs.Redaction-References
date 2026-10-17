---
title: "redact_annotation yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belge içindeki tüm ek açıklamalardaki eşleşen metni verilen seçeneklerle değiştirir."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/ifixedformatdocument/redact_annotation/
is_root: false
weight: 1030
---


## redact_annotation {#regular_expression-options}

Belge içindeki tüm ek açıklamalardaki eşleşen metni verilen seçeneklerle değiştirir.

```python
def redact_annotation(self, regular_expression, options):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| regular_expression | `System.Text.RegularExpressions.Regex` | Arama ve değiştirme için düzenli ifade. |
| options | `ReplacementOptions` | Değiştirme seçenekleri. |

**Returns:** Replacement result.

### Ayrıca Bakınız
* class [`IFixedFormatDocument`](/redaction/python-net/groupdocs.redaction.integration/ifixedformatdocument/)
