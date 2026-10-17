---
title: "from_extension yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Dosya uzantısını dosya türüne eşler."
type: docs
url: /tr/python-net/groupdocs.redaction/filetype/from_extension/
is_root: false
weight: 1040
---


## from_extension {#extension}

Dosya uzantısını dosya türüne eşler.

```python
def from_extension(cls, extension):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| extension | `str` | Dosya uzantısı (nokta \".\" dahil). |

**Returns:** FileType: When file type is supported returns it, otherwise returns default `FileType.unknown` file type.

| Yükseltir | Açıklama |
| :- | :- |
| `ValueError` | `extension` null veya boş bir dize olduğunda. |

### Ayrıca Bakınız
* class [`FileType`](/redaction/python-net/groupdocs.redaction/filetype/)
