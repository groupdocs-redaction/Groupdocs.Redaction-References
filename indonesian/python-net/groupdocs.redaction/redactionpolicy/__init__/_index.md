---
title: "konstruktor __init__"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Menginisialisasi instance RedactionPolicy baru."
type: docs
url: /id/python-net/groupdocs.redaction/redactionpolicy/__init__/
is_root: false
weight: 10
---


## __init__

Menginisialisasi instance RedactionPolicy baru.

```python
def __init__(self):
    ...
```

### Contoh

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

## __init__ {#redactions}

Menginisialisasi RedactionPolicy baru dengan daftar redaksi tertentu.

```python
def __init__(self, redactions):
    ...
```

| Parameter | Tipe | Deskripsi |
| :- | :- | :- |
| redactions | `list[Redaction]` | Array redactions untuk kebijakan. |

### Contoh

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import ExactPhraseRedaction, RegexRedaction, ReplacementOptions

policy = RedactionPolicy([
    ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
    RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
])
```

### Lihat Juga
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
