---
title: "redact methode"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Past aangepaste redactie toe op specifieke documentinhoud."
type: docs
url: /nl/python-net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
is_root: false
weight: 1010
---


## redact {#context}

Past aangepaste redactie toe op specifieke documentinhoud.

Momenteel wordt dit alleen ondersteund voor PDF [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/).

Gebruikers kunnen hun eigen redactielogica definiëren, zoals AI-gebaseerde redacties, die geavanceerder kunnen zijn dan eenvoudige patroongebaseerde methoden.

```python
def redact(self, context):
    ...
```

| Parameter | Type | Beschrijving |
| :- | :- | :- |
| context | `CustomRedactionContext` | Bevat de documentinhoud die moet worden geredigeerd, samen met gerelateerde metadata. |

**Returns:** CustomRedactionResult: Indicates whether the redaction should be applied and the modified content.

### Zie ook
* class [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/)
