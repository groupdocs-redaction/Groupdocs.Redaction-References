---
title: "redact metodu"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli belge içeriğine özel kırpma uygular."
type: docs
url: /tr/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Belirli belge içeriğine özel kırpma uygular.

Şu anda, bu yalnızca PDF için desteklenmektedir [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Kullanıcılar, AI tabanlı redaksiyon gibi, kendi redaksiyon mantıklarını tanımlayabilir; bu, basit desen tabanlı yöntemlerden daha gelişmiş olabilir.

```python
def redact(self, context):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| context | `CustomRedactionContext` | Redakte edilecek belge içeriğini ve ilgili üst verileri içerir. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Ayrıca Bakınız
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
