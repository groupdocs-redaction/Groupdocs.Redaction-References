---
title: "perform_binary_check yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Verilen akışın bu format örneği tarafından desteklenen bir belge içerip içermediğini kontrol eder."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/
is_root: false
weight: 1080
---


## perform_binary_check {#input}

Verilen akışın bu format örneği tarafından desteklenen bir belge içerip içermediğini kontrol eder.

```python
def perform_binary_check(self, input):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| input | `io.RawIOBase` | Belge içerik akışı. |

**Returns:** bool: True if the document can be loaded by this format instance, False otherwise.

### Ayrıca Bakınız
* class [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)
