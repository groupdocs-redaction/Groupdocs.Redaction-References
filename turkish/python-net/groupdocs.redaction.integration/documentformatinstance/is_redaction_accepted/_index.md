---
title: "is_redaction_accepted yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "IRedactionCallback uygulaması için denetimler yapar ve belirtilmişse onu çağırır."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/
is_root: false
weight: 1030
---


## is_redaction_accepted {#description}

[`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) uygulamasını kontrol eder ve belirtilmişse çağırır.

```python
def is_redaction_accepted(self, description):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| description | `RedactionDescription` | Redaction açıklaması |

**Returns:** bool: True (by default) if redaction is accepted.

### Ayrıca Bakınız
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
