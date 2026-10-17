---
title: "load metodu"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir XML dosyasından RedactionPolicy yükler."
type: docs
url: /tr/python-net/groupdocs.redaction/redactionpolicy/load/
is_root: false
weight: 1010
---


## load {#file_path}

Bir XML dosyasından RedactionPolicy yükler.

```python
def load(cls, file_path):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_path | `str` | XML dosyasının yolu. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Örnek

```python
from groupdocs.redaction import RedactionPolicy, Redactor

policy = RedactionPolicy.load("RedactionPolicy.xml")

with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

## load {#input}

XML yapılandırması içeren bir akıştan RedactionPolicy örneği yükler.

```python
def load(cls, input):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| input | `io.RawIOBase` | XML yapılandırmasını içeren akış. |

**Returns:** RedactionPolicy: The loaded redaction policy.

### Örnek

```python
from groupdocs.redaction import RedactionPolicy, Redactor

# Politikayı bir XML dosyasından yükle
with open("policy.xml", "rb") as stream:
    policy = RedactionPolicy.load(stream)

# Politikayı bir belgeye uygulayın
with Redactor("document.docx") as redactor:
    redactor.apply(policy=policy)
    redactor.save()
```

### Ayrıca Bakınız
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
