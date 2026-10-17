---
title: "save metodu"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Redaksiyon politikasını bir dosyaya kaydeder."
type: docs
url: /tr/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Redaksiyon politikasını bir dosyaya kaydeder.

```python
def save(self, file_path):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_path | `str` | Dosya yolu. |

### Örnek

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Redaksiyon politikasını bir akışa kaydeder.

```python
def save(self, output):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| output | `io.RawIOBase` | Politikayı kaydetmek için hedef akış. |

**Returns:** None.

### Ayrıca Bakınız
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
