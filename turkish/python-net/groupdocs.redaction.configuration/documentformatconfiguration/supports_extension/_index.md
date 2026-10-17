---
title: "supports_extension yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Verilen bir dosya uzantısının DocumentType olarak işlenip işlenemeyeceğini kontrol eder."
type: docs
url: /tr/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/
is_root: false
weight: 1010
---


## supports_extension {#file_extension}

Verilen bir dosya uzantısının DocumentType olarak işlenip işlenemeyeceğini kontrol eder.

```python
def supports_extension(self, file_extension):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_extension | `str` | Dosya uzantısı, format ".ext". |

**Returns:** bool: True if the extension is listed in ExtensionFilter.

### Ayrıca Bakınız
* class [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/)
